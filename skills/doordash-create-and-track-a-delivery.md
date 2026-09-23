---
name: doordash-create-and-track-a-delivery
description: Quote, commit, track and (while it is still possible) cancel an on-demand DoorDash Drive delivery, using the caller-supplied external_delivery_id as the replay key.
api: DoorDash Drive API
spec: openapi/_original/doordash-drive-openapi.yml
generated: '2026-09-17'
method: generated
source: openapi/_original/doordash-drive-openapi.yml, https://developer.doordash.com/en-US/docs/drive/reference/errors
operations:
  - CheckServiceability
  - GetAddressAutoComplete
  - DeliveryQuote
  - DeliveryQuoteAccept
  - CreateDelivery
  - GetDelivery
  - UpdateDelivery
  - CancelDelivery
---

# Create and track a DoorDash Drive delivery

Base URL `https://openapi.doordash.com`. Every call carries `Authorization: Bearer <JWT>` where the
JWT is one you sign yourself (HS256, `aud=doordash`, `iss=developer_id`, `kid=key_id`, `exp` at most
1800 seconds past `iat`). Mint a fresh one per session; a 401 here almost always means expired.

**Pick the external_delivery_id first.** You supply it, DoorDash does not. It is the primary key of
the delivery *and* the replay key, so generate it before the first write and reuse it for every
retry of that same delivery.

## 1. Confirm the job is possible before spending money

- `CheckServiceability` — `POST /drive/v2/serviceability`. Creates nothing.
- `GetAddressAutoComplete` — `POST /drive/v2/address/auto_complete` to resolve a partial dropoff
  address. `dropoff_phone_number` must be E.164 or the later create returns 400.

## 2. Price it

`DeliveryQuote` — `POST /drive/v2/quotes` with your `external_delivery_id`, pickup and dropoff
details. This returns a fee and does **not** dispatch anything.

## 3. Commit

Either:

- `DeliveryQuoteAccept` — `POST /drive/v2/quotes/{external_delivery_id}/accept`, optionally with a
  tip; or
- `CreateDelivery` — `POST /drive/v2/deliveries` to skip the quote and create in one call.

**This is the step that spends money.** A delivery under 5 miles is billed at a $9.75 base rate,
plus $0.75/mile beyond 5 miles up to 15 miles, charged at creation.

If the call times out, retry with the **same** `external_delivery_id`: identical data returns the
existing delivery. A 409 means you reused that id with *different* data — change the id, do not
retry.

## 4. Track

`GetDelivery` — `GET /drive/v2/deliveries/{external_delivery_id}`. Statuses progress
`created → confirmed → enroute_to_pickup → arrived_at_pickup → picked_up → enroute_to_dropoff →
arrived_at_dropoff → delivered`, with `cancelled` as a terminal branch. A delivery can re-enter
`created` if a Dasher unassigns before pickup.

Prefer webhooks over polling: configure one HTTPS endpoint per environment in the Developer Portal,
protected with Basic Auth or OAuth. DoorDash sends each event up to 3 times and retries on anything
other than 200 OK. It does **not** sign payloads, so your endpoint's own authentication is the only
thing establishing authenticity.

## 5. Amend or reverse

- `UpdateDelivery` — `PATCH /drive/v2/deliveries/{external_delivery_id}` to change addresses or times.
- `CancelDelivery` — `PUT /drive/v2/deliveries/{external_delivery_id}/cancel`.

**Know the window before you commit:** deliveries cannot be cancelled once a Dasher is assigned.
After that DoorDash creates a *return* delivery instead, billed at 60% of the original fee.
Cancelling an inactive delivery returns 409.

## Errors and retries

The envelope is `{code, message, field_errors[]}` — branch on `code`, never on `message` (DoorDash
states it is for debugging only). Do not retry 400, 403, 404, 409 or 422. Retry 429 after at least
one second and 5xx with exponential backoff and jitter — 3 attempts, 1s to 5s. The limit is roughly
300 requests per 60 seconds per access key, and there are no rate-limit response headers to read, so
count your own calls.

## Rehearse first

Sandbox is self-serve and free, separated by which access key signs the JWT (the base URL is the
same). Use the Developer Portal Delivery Simulator to advance a test delivery through its states and
fire the matching webhooks. Test deliveries are auto-cancelled after one hour.
