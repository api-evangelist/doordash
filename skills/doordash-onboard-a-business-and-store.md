---
name: doordash-onboard-a-business-and-store
description: Create the Drive merchant hierarchy — a business and its stores — under caller-supplied external identifiers, so deliveries can name a pickup location.
api: DoorDash Drive API
spec: openapi/_original/doordash-drive-openapi.yml
generated: '2026-09-17'
method: generated
source: openapi/_original/doordash-drive-openapi.yml
operations:
  - CreateBusiness
  - ListBusiness
  - GetBusiness
  - UpdateBusiness
  - CreateStore
  - ListStore
  - GetStore
  - UpdateStore
---

# Onboard a business and its stores on DoorDash Drive

These live on `/developer/v1`, not `/drive/v2` — a common mistake, since they are documented inside
the Drive reference.

## 1. Create the business

`CreateBusiness` — `POST /developer/v1/businesses`. You supply `external_business_id`; DoorDash
stores the business under your identifier.

Check first with `ListBusiness` (`GET /developer/v1/businesses`) or `GetBusiness`
(`GET /developer/v1/businesses/{external_business_id}`) — there is no idempotency key on this
surface, so a blind retry of a create is not safe.

## 2. Create each store

`CreateStore` — `POST /developer/v1/businesses/{external_business_id}/stores`, with your
`external_store_id`. Read back with `ListStore` or `GetStore`.

## 3. Keep them current

`UpdateBusiness` and `UpdateStore` are `PATCH`. Both are last-write-wins with **no reversal
operation** — there is no undo, no restore and no version history. If you need to be able to roll
back, keep the previous payload yourself before you write.

## Wiring it to deliveries

A Drive delivery names its pickup location through `pickup_external_business_id` and
`pickup_external_store_id`. A missing `pickup_external_business_id` is a documented field error.

## Watch the identifier split

The same physical store is keyed differently per product: `external_store_id` on Drive,
`merchant_supplied_id` on Marketplace, `store_location_id` on Item Management. If you integrate more
than one, you own the mapping — DoorDash does not reconcile them for you.
