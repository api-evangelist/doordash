---
name: doordash-accept-and-fulfil-a-marketplace-order
description: Confirm an inbound DoorDash Marketplace order, signal readiness, and adjust, cancel or return it — the merchant-side order lifecycle.
api: DoorDash Marketplace API
spec: openapi/_original/doordash-marketplace-openapi.yml
generated: '2026-09-17'
method: generated
source: openapi/_original/doordash-marketplace-openapi.yml
operations:
  - confirmOrder
  - storeConfirmOrderReadyForPickup
  - adjustOrderItems
  - cancelOrder
  - returnOrder
  - getStoreInfo
---

# Accept and fulfil a DoorDash Marketplace order

Base URL `https://openapi.doordash.com/marketplace`. Same self-signed HS256 JWT bearer as the rest
of the platform.

**Access note:** Marketplace APIs are not generally available. Partners apply through the Developer
Portal Integrations tab. Do not plan around this surface until access is granted.

Orders arrive at your webhook endpoint — DoorDash pushes, you do not poll for new orders.

## 1. Confirm

`confirmOrder` — `PATCH /api/v1/orders/{id}`. This is the acknowledgement that the store has
accepted the order.

## 2. Signal progress

`storeConfirmOrderReadyForPickup` — `PATCH /api/v1/orders/{id}/events/{event_type}`. Use it to tell
DoorDash the order is ready so Dasher arrival can be timed against it.

## 3. Amend when the store cannot fulfil exactly

`adjustOrderItems` — `PATCH /api/v1/orders/{id}/adjustment` — cancels, adjusts or substitutes
individual items. When substituting, `substitute_item_ids` cannot be null or empty if
`substitution_preference` is `substitute`, and `substitution_preference` cannot be `contact` when
customer communication is suppressed. Both are documented field errors.

## 4. Reverse

- `cancelOrder` — `PATCH /api/v1/orders/{id}/cancellation`.
- `returnOrder` — `POST /api/v1/orders/{id}/return` (retail only).

Neither publishes a time window. Treat cancellation as best-effort and confirm the resulting order
state rather than assuming the call succeeded semantically.

## No replay protection here

Nothing on the Marketplace surface has an idempotency key — the `external_delivery_id` mechanism is
Drive-only. A timed-out `confirmOrder` or `adjustOrderItems` cannot be blindly retried; read the
order back with `getStoreInfo`-adjacent reads or the order event stream first.

## Errors

Same shared envelope and status semantics as Drive: `{code, message, field_errors[]}`, 409 for a
state conflict, 422 for a logically impossible operation, 429 at roughly 300 requests per minute.
