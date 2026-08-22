# doordash (doordash)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

DoorDash is an on-demand local commerce platform whose developer program exposes its logistics and marketplace network through public APIs. The Drive and Drive Classic APIs let businesses request on-demand deliveries fulfilled by DoorDash's Dasher fleet, while the Marketplace, Item Management, and Reporting APIs let merchants and retailers receive orders, synchronize menus and catalogs, and access financial and operational reporting. All APIs use JWT-based authentication and are documented at developer.doordash.com.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/apis.yml)

## Timestamps

- **Modified:** 2026-06-02

## APIs

### DoorDash Drive API

The DoorDash Drive API enables businesses to request on-demand deliveries fulfilled by DoorDash's fleet of Dashers. It provides endpoints for checking delivery serviceability, getting delivery quotes, creating and managing deliveries, and tracking delivery status in real time. The API uses JWT-based authentication and is designed for businesses that want to offer delivery from their own ordering experience while leveraging DoorDash's logistics network.

- **Human URL:** [https://developer.doordash.com/en-US/docs/drive/overview/about_drive/](https://developer.doordash.com/en-US/docs/drive/overview/about_drive/)
- **Base URL:** `https://openapi.doordash.com/drive/v2`

#### Tags

- Delivery
- Food Delivery
- Last Mile
- Logistics
- On-Demand

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/drive/overview/about_drive/)
- [OpenAPI](openapi/doordash-drive-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/doordash-drive.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/doordash-drive.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/doordash-drive-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [SDK](https://www.npmjs.com/package/@doordash/sdk)
- [Code Examples](https://github.com/doordash-oss/doordash_sdk_example_application)
- [Code Examples](https://github.com/JoshAtDoorDash/DoorDashAPI-Nodejs-Sample)
- [Code Examples](https://github.com/JoshAtDoorDash/DoorDashAPI-Python-Sample)
- [Code Examples](https://github.com/JoshAtDoorDash/DoorDashAPI-Java-Sample)
- [Code Examples](https://github.com/JoshAtDoorDash/DoorDashAPI-Kotlin-Sample)
- [Code Examples](https://github.com/JoshAtDoorDash/DoorDashAPI-PHP-Sample)
- [Code Examples](https://github.com/JoshAtDoorDash/DoorDashAPI-CSharp-Dotnet-Sample)

### DoorDash Drive Classic API

The DoorDash Drive Classic API is the legacy version of the Drive API, designed for large enterprises and middleware providers who require extensive configuration and customizability for their delivery integrations. It provides endpoints for managing businesses, stores, and deliveries through DoorDash's logistics platform. The API uses JWT-based Bearer token authentication and operates at the v1 endpoint path.

- **Human URL:** [https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/](https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/)
- **Base URL:** `https://openapi.doordash.com/drive/v1`

#### Tags

- Delivery
- Enterprise
- Food Delivery
- Last Mile
- Logistics

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/)
- [OpenAPI](openapi/doordash-drive-classic-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/doordash-drive-classic.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/doordash-drive-classic.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DoorDash Marketplace API

The DoorDash Marketplace API allows merchants and third-party providers to integrate directly with the DoorDash marketplace for order management, menu synchronization, and store operations. It supports receiving orders from DoorDash, updating order statuses, and managing menu availability in real time. The API is not generally available and access is granted through a selective partner program where DoorDash evaluates integration quality and business fit.

- **Human URL:** [https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/](https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/)
- **Base URL:** `https://openapi.doordash.com/marketplace`

#### Tags

- Food Delivery
- Marketplace
- Orders
- Restaurants
- Retail

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/)
- [OpenAPI](openapi/doordash-marketplace-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/doordash-marketplace.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/doordash-marketplace.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/doordash-marketplace-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### DoorDash Item Management API

The DoorDash Item Management API enables merchants and integration partners to programmatically manage their item catalogs, inventory levels, pricing, and other product attributes on the DoorDash platform. It provides endpoints for creating, updating, and retrieving item data across stores. This API is particularly useful for retail and grocery partners who need to keep large catalogs synchronized between their own systems and DoorDash's marketplace.

- **Human URL:** [https://developer.doordash.com/en-US/api/marketplace_v2/](https://developer.doordash.com/en-US/api/marketplace_v2/)
- **Base URL:** `https://openapi.doordash.com/marketplace`

#### Tags

- Catalog
- Inventory
- Menus
- Pricing
- Retail

#### Properties

- [Documentation](https://developer.doordash.com/en-US/api/marketplace_v2/)
- [OpenAPI](openapi/doordash-item-management-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/doordash-item-management.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/doordash-item-management.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### DoorDash Reporting API

The DoorDash Reporting API provides approved partners with access to standardized financial, operations, and menu reporting data. It offers a POST endpoint for creating report requests and a GET endpoint for retrieving report download links, along with webhook notifications when reports are ready.

- **Human URL:** [https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/](https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/)
- **Base URL:** `https://openapi.doordash.com/dataexchange/v1`

#### Tags

- Analytics
- Data
- Financial
- Operations
- Reporting

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/)
- [OpenAPI](openapi/doordash-reporting-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/doordash-reporting.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/doordash-reporting.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/doordash-reporting-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

## Common Properties

- [Developer Portal](https://developer.doordash.com/)
- [Documentation](https://developer.doordash.com/en-US/)
- [Website](https://www.doordash.com/)
- [Blog](https://doordash.engineering/)
- [Login](https://developer.doordash.com/en-US/login)
- [Terms of Service](https://www.doordash.com/terms/)
- [Privacy Policy](https://www.doordash.com/privacy/)
- [Support](https://help.doordash.com/)
- [GitHub Organization](https://github.com/doordash)
- [GitHub Organization](https://github.com/doordash-oss)
- [LinkedIn](https://www.linkedin.com/company/doordash)
- [SDK](https://www.npmjs.com/package/@doordash/sdk)
- [Tools](https://github.com/doordash-oss/oapi-codegen-dd)
- [JSON-LD](json-ld/doordash-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/doordash-delivery-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/doordash-order-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/doordash-menu-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/doordash-report-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Vocabulary](vocabulary/doordash-vocabulary.yml)
- [Rules](rules/doordash-spectral-rules.yml)
- [Plans](plans/doordash-plans-pricing.yml)
- [Rate Limits](rate-limits/doordash-rate-limits.yml)
- [Fin Ops](finops/doordash-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
