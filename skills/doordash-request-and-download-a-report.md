---
name: doordash-request-and-download-a-report
description: Request a DoorDash financial or operational report asynchronously and fetch its download link — the data-exchange path for payouts, transactions and order items.
api: DoorDash Reporting API
spec: openapi/_original/doordash-reporting-openapi.yml
generated: '2026-09-17'
method: generated
source: openapi/_original/doordash-reporting-openapi.yml, https://developer.doordash.com/en-US/docs/reporting/overview/release_notes
operations:
  - createReport
  - getReportLink
---

# Request and download a DoorDash report

Base URL `https://openapi.doordash.com/dataexchange/v1`. Same self-signed HS256 JWT bearer.

This is a two-step asynchronous surface — there is no synchronous report read.

## 1. Request

`createReport` — `POST /reports`. Returns **202 Accepted**, not 200. The report is queued, not
produced. Treat the 202 as "the job exists", nothing more.

There is no idempotency key and no cancellation operation: once requested, a report runs. If the
POST times out you cannot tell whether the job was created, so record your own request attempt
before firing it.

## 2. Collect

`getReportLink` — `GET /reports/{report_id}/reportlink`. Returns a link to the finished report.
Poll with backoff rather than tightly — the shared limit of roughly 300 requests per 60 seconds per
access key applies here too, and a 429 costs you more than waiting.

## Know which report version you are reading

Report shapes are versioned independently of the API (`report_version` 2, 3, 4, 5). DoorDash's
policy, stated in the release notes, is that legacy report versions stay supported but receive **no
new fields** — so pinning an old version silently freezes your data model. Current at the last
update (2026-05-21, v0.2.3): `PROMOTION_PERFORMANCE` and `SPONSORED_LISTING_PERFORMANCE` were added;
`is_storefront` landed on `PAYOUT_SUMMARY` v2, `TRANSACTION_DETAIL` v3 and `ORDER_ITEM` v3;
`CONSUMER_FEEDBACK` v5 carries `merchant_emoji_rating` and `merchant_tags`.

Reporting is the only DoorDash API surface with 2026 release-note activity — Drive last published a
release note in January 2023.
