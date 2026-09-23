---
name: doordash-sync-a-catalog-and-availability
description: Push menus, items, per-store inventory and pricing into DoorDash and flip item or store availability — the catalog write path, which has no undo.
api: DoorDash Item Management API + Marketplace API
spec: openapi/_original/doordash-item-management-openapi.yml
generated: '2026-09-17'
method: generated
source: openapi/_original/doordash-item-management-openapi.yml, openapi/_original/doordash-marketplace-openapi.yml
operations:
  - batchAddItems
  - batchUpdateItems
  - batchAddStoreItem
  - batchUpdateStoreItem
  - updateItemsInBusiness
  - createPromotion
  - updatePromotions
  - menuCreate
  - menuUpdate
  - getStoreMenu
  - getStoreMenuInfo
  - itemActivation
  - itemOptionActivation
  - updateStoreStatus
  - getItemAvailability
---

# Sync a catalog and availability into DoorDash

Two surfaces, two base paths, two identifiers for the same store:

- Item Management — `https://openapi.doordash.com/marketplace/api/v2`, keyed on `store_location_id`.
- Marketplace — `https://openapi.doordash.com/marketplace/api/v1`, keyed on `merchant_supplied_id`.

## 1. Read what is live before writing

- `getStoreMenu` — `GET /api/v1/stores/{merchant_supplied_id}/store_menu`.
- `getStoreMenuInfo` — `GET /api/v1/stores/{merchant_supplied_id}/menu_details`.
- `getItemAvailability` — `GET /api/v1/stores/{merchant_supplied_id}/item/availability`.

**Do this every time.** Catalog writes are last-write-wins upserts with no reversal operation and no
version history. Reading first is the only way to be able to roll back.

## 2. Catalog level

- `batchAddItems` — `POST /api/v2/items`
- `batchUpdateItems` — `PATCH /api/v2/items`
- `updateItemsInBusiness` — `PATCH /api/v2/businesses/{business_id}/items` for inventory and pricing
  across every store in a business.

Modifier nesting is fixed, not recursive: Extra → NestedExtra → NestedL2Extra. A menu deeper than
three levels of modifiers does not fit the schema.

## 3. Store level

- `batchAddStoreItem` — `POST /api/v2/stores/{store_location_id}/items`
- `batchUpdateStoreItem` — `PATCH /api/v2/stores/{store_location_id}/items`
- `createPromotion` / `updatePromotions` — `/api/v2/promotions/stores/{store_location_id}`

## 4. Menus

`menuCreate` — `POST /api/v1/menus`; `menuUpdate` — `PATCH /api/v1/menus/{id}`. DoorDash changed the
menu creation flow in July 2023 specifically to stop duplicate menus being created for a store, so
create once and update thereafter.

## 5. Availability flips

- `itemActivation` — `PUT /api/v1/stores/{merchant_supplied_id}/items/status`
- `itemOptionActivation` — `PUT /api/v1/stores/{merchant_supplied_id}/item_options/status`
- `updateStoreStatus` — `PUT /api/v1/stores/{location_id}/status`

These are the calls an agent reaches for during a live outage. They take effect against a live
consumer storefront immediately.

## Item errors come back per item

Batch writes return item-level errors keyed on `merchant_supplied_id` — `{merchant_supplied_id,
code, message}`. Partial failure is normal; reconcile per item rather than treating the batch as
atomic. Documented examples include `The following external ids were not found: [...]` and
`Item: 123456 is suspended and not available`.

## No replay protection

No idempotency key exists on any catalog write. A timed-out batch must be verified by reading back,
not retried blindly.
