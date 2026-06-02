# DoorDash (doordash)
DoorDash is an on-demand local commerce platform whose developer program exposes its logistics and marketplace network through public APIs. The Drive and Drive Classic APIs let businesses request on-demand deliveries fulfilled by DoorDash's Dasher fleet, while the Marketplace, Item Management, and Reporting APIs let merchants and retailers receive orders, synchronize menus and catalogs, and access financial and operational reporting. All APIs use JWT-based authentication and are documented at developer.doordash.com.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Analytics, Catalog, Data, Delivery, Enterprise, Financial, Food Delivery, Inventory, Last Mile, Logistics, Marketplace, Menus, On-Demand, Operations, Orders, Pricing, Reporting, Restaurants, Retail

## Timestamps

- **Created:** 2026-03-20
- **Modified:** 2026-06-02

## APIs

### DoorDash Drive API
The DoorDash Drive API enables businesses to request on-demand deliveries fulfilled by DoorDash's fleet of Dashers. It provides endpoints for checking delivery serviceability, getting delivery quotes, creating and managing deliveries, and tracking delivery status in real time. The API uses JWT-based authentication and is designed for businesses that want to offer delivery from their own ordering experience while leveraging DoorDash's logistics network.

**Human URL:** [https://developer.doordash.com/en-US/docs/drive/overview/about_drive/](https://developer.doordash.com/en-US/docs/drive/overview/about_drive/)

#### Tags:

 - Delivery, Food Delivery, Last Mile, Logistics, On-Demand

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/drive/overview/about_drive/)
- [OpenAPI](openapi/doordash-drive-openapi.yml)
- [AsyncAPI](asyncapi/doordash-drive-webhooks-asyncapi.yml)
- [NaftikoCapability](capabilities/drive-addresses.yaml)
- [NaftikoCapability](capabilities/drive-businesses.yaml)
- [NaftikoCapability](capabilities/drive-deliveries.yaml)
- [NaftikoCapability](capabilities/drive-quotes.yaml)
- [NaftikoCapability](capabilities/drive-stores.yaml)
- [Node.js SDK](https://www.npmjs.com/package/@doordash/sdk)
- [Node.js SDK Example Application](https://github.com/doordash-oss/doordash_sdk_example_application)
- [Node.js Sample](https://github.com/JoshAtDoorDash/DoorDashAPI-Nodejs-Sample)
- [Python Sample](https://github.com/JoshAtDoorDash/DoorDashAPI-Python-Sample)
- [Java Sample](https://github.com/JoshAtDoorDash/DoorDashAPI-Java-Sample)
- [Kotlin Sample](https://github.com/JoshAtDoorDash/DoorDashAPI-Kotlin-Sample)
- [PHP Sample](https://github.com/JoshAtDoorDash/DoorDashAPI-PHP-Sample)
- [C# / .NET Sample](https://github.com/JoshAtDoorDash/DoorDashAPI-CSharp-Dotnet-Sample)

### DoorDash Drive Classic API
The DoorDash Drive Classic API is the legacy version of the Drive API, designed for large enterprises and middleware providers who require extensive configuration and customizability for their delivery integrations. It provides endpoints for managing businesses, stores, and deliveries through DoorDash's logistics platform. The API uses JWT-based Bearer token authentication and operates at the v1 endpoint path.

**Human URL:** [https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/](https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/)

#### Tags:

 - Delivery, Enterprise, Food Delivery, Last Mile, Logistics

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/)
- [OpenAPI](openapi/doordash-drive-classic-openapi.yml)
- [NaftikoCapability](capabilities/drive-classic-businesses.yaml)
- [NaftikoCapability](capabilities/drive-classic-deliveries.yaml)
- [NaftikoCapability](capabilities/drive-classic-stores.yaml)

### DoorDash Marketplace API
The DoorDash Marketplace API allows merchants and third-party providers to integrate directly with the DoorDash marketplace for order management, menu synchronization, and store operations. It supports receiving orders from DoorDash, updating order statuses, and managing menu availability in real time. The API is not generally available and access is granted through a selective partner program where DoorDash evaluates integration quality and business fit.

**Human URL:** [https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/](https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/)

#### Tags:

 - Food Delivery, Marketplace, Orders, Restaurants, Retail

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/)
- [OpenAPI](openapi/doordash-marketplace-openapi.yml)
- [AsyncAPI](asyncapi/doordash-marketplace-webhooks-asyncapi.yml)
- [NaftikoCapability](capabilities/marketplace-items.yaml)
- [NaftikoCapability](capabilities/marketplace-menus.yaml)
- [NaftikoCapability](capabilities/marketplace-orders.yaml)
- [NaftikoCapability](capabilities/marketplace-stores.yaml)

### DoorDash Item Management API
The DoorDash Item Management API enables merchants and integration partners to programmatically manage their item catalogs, inventory levels, pricing, and other product attributes on the DoorDash platform. It provides endpoints for creating, updating, and retrieving item data across stores. This API is particularly useful for retail and grocery partners who need to keep large catalogs synchronized between their own systems and DoorDash's marketplace.

**Human URL:** [https://developer.doordash.com/en-US/api/marketplace_v2/](https://developer.doordash.com/en-US/api/marketplace_v2/)

#### Tags:

 - Catalog, Inventory, Menus, Pricing, Retail

#### Properties

- [Documentation](https://developer.doordash.com/en-US/api/marketplace_v2/)
- [OpenAPI](openapi/doordash-item-management-openapi.yml)
- [NaftikoCapability](capabilities/item-management-catalog.yaml)
- [NaftikoCapability](capabilities/item-management-inventory.yaml)
- [NaftikoCapability](capabilities/item-management-promotions.yaml)

### DoorDash Reporting API
The DoorDash Reporting API provides approved partners with access to standardized financial, operations, and menu reporting data. It offers a POST endpoint for creating report requests and a GET endpoint for retrieving report download links, along with webhook notifications when reports are ready.

**Human URL:** [https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/](https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/)

#### Tags:

 - Analytics, Data, Financial, Operations, Reporting

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/)
- [OpenAPI](openapi/doordash-reporting-openapi.yml)
- [AsyncAPI](asyncapi/doordash-reporting-webhooks-asyncapi.yml)
- [NaftikoCapability](capabilities/reporting-reports.yaml)

## Common Properties

- [DeveloperPortal](https://developer.doordash.com/)
- [Documentation](https://developer.doordash.com/en-US/)
- [Website](https://www.doordash.com/)
- [Blog](https://doordash.engineering/)
- [Login](https://developer.doordash.com/en-US/login)
- [TermsOfService](https://www.doordash.com/terms/)
- [PrivacyPolicy](https://www.doordash.com/privacy/)
- [Support](https://help.doordash.com/)
- [GitHubOrganization](https://github.com/doordash)
- [DoorDash Open Source](https://github.com/doordash-oss)
- [LinkedIn](https://www.linkedin.com/company/doordash)
- [Node.js SDK](https://www.npmjs.com/package/@doordash/sdk)
- [OpenAPI Go Codegen (oapi-codegen-dd)](https://github.com/doordash-oss/oapi-codegen-dd)
- [JSONLD](json-ld/doordash-context.jsonld)
- [JSONSchema](json-schema/doordash-delivery-schema.json)
- [JSONSchema](json-schema/doordash-order-schema.json)
- [JSONSchema](json-schema/doordash-menu-schema.json)
- [JSONSchema](json-schema/doordash-report-schema.json)
- [Vocabulary](vocabulary/doordash-vocabulary.yml)
- [Rules](rules/doordash-spectral-rules.yml)
- [Plans](plans/doordash-plans-pricing.yml)
- [RateLimits](rate-limits/doordash-rate-limits.yml)
- [FinOps](finops/doordash-finops.yml)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [doordash-drive-classic-openapi.yml](openapi/doordash-drive-classic-openapi.yml)
- [doordash-drive-openapi.yml](openapi/doordash-drive-openapi.yml)
- [doordash-item-management-openapi.yml](openapi/doordash-item-management-openapi.yml)
- [doordash-marketplace-openapi.yml](openapi/doordash-marketplace-openapi.yml)
- [doordash-reporting-openapi.yml](openapi/doordash-reporting-openapi.yml)

### AsyncAPI

- [doordash-drive-webhooks-asyncapi.yml](asyncapi/doordash-drive-webhooks-asyncapi.yml)
- [doordash-marketplace-webhooks-asyncapi.yml](asyncapi/doordash-marketplace-webhooks-asyncapi.yml)
- [doordash-reporting-webhooks-asyncapi.yml](asyncapi/doordash-reporting-webhooks-asyncapi.yml)

### JSON Schema

97 JSON Schema files in [`json-schema/`](json-schema/).

### JSON Structure

55 JSON Structure files in [`json-structure/`](json-structure/).

### JSON-LD

- [doordash-context.jsonld](json-ld/doordash-context.jsonld)
- [doordash-drive-classic-context.jsonld](json-ld/doordash-drive-classic-context.jsonld)
- [doordash-drive-context.jsonld](json-ld/doordash-drive-context.jsonld)
- [doordash-drive-webhooks-context.jsonld](json-ld/doordash-drive-webhooks-context.jsonld)
- [doordash-item-management-context.jsonld](json-ld/doordash-item-management-context.jsonld)
- [doordash-marketplace-context.jsonld](json-ld/doordash-marketplace-context.jsonld)
- [doordash-marketplace-webhooks-context.jsonld](json-ld/doordash-marketplace-webhooks-context.jsonld)
- [doordash-reporting-context.jsonld](json-ld/doordash-reporting-context.jsonld)
- [doordash-reporting-webhooks-context.jsonld](json-ld/doordash-reporting-webhooks-context.jsonld)

### Examples

55 example payloads in [`examples/`](examples/).

## Naftiko Capabilities

Self-contained Naftiko capabilities (one per API business surface), each exposing a REST adapter and an MCP adapter.

### DoorDash Drive API

| Capability | Tools | File |
|------------|-------|------|
| DoorDash Drive API — Addresses | 1 | [drive-addresses.yaml](capabilities/drive-addresses.yaml) |
| DoorDash Drive API — Businesses | 4 | [drive-businesses.yaml](capabilities/drive-businesses.yaml) |
| DoorDash Drive API — Deliveries | 5 | [drive-deliveries.yaml](capabilities/drive-deliveries.yaml) |
| DoorDash Drive API — Quotes | 2 | [drive-quotes.yaml](capabilities/drive-quotes.yaml) |
| DoorDash Drive API — Stores | 3 | [drive-stores.yaml](capabilities/drive-stores.yaml) |

### DoorDash Drive Classic API

| Capability | Tools | File |
|------------|-------|------|
| DoorDash Drive Classic API — Businesses | 4 | [drive-classic-businesses.yaml](capabilities/drive-classic-businesses.yaml) |
| DoorDash Drive Classic API — Deliveries | 5 | [drive-classic-deliveries.yaml](capabilities/drive-classic-deliveries.yaml) |
| DoorDash Drive Classic API — Stores | 3 | [drive-classic-stores.yaml](capabilities/drive-classic-stores.yaml) |

### DoorDash Marketplace API

| Capability | Tools | File |
|------------|-------|------|
| DoorDash Marketplace API — Items | 1 | [marketplace-items.yaml](capabilities/marketplace-items.yaml) |
| DoorDash Marketplace API — Menus | 2 | [marketplace-menus.yaml](capabilities/marketplace-menus.yaml) |
| DoorDash Marketplace API — Orders | 1 | [marketplace-orders.yaml](capabilities/marketplace-orders.yaml) |
| DoorDash Marketplace API — Stores | 3 | [marketplace-stores.yaml](capabilities/marketplace-stores.yaml) |

### DoorDash Item Management API

| Capability | Tools | File |
|------------|-------|------|
| DoorDash Item Management API — Catalog | 2 | [item-management-catalog.yaml](capabilities/item-management-catalog.yaml) |
| DoorDash Item Management API — Inventory | 2 | [item-management-inventory.yaml](capabilities/item-management-inventory.yaml) |
| DoorDash Item Management API — Promotions | 2 | [item-management-promotions.yaml](capabilities/item-management-promotions.yaml) |

### DoorDash Reporting API

| Capability | Tools | File |
|------------|-------|------|
| DoorDash Reporting API — Reports | 2 | [reporting-reports.yaml](capabilities/reporting-reports.yaml) |

## Vocabulary

- [DoorDash Vocabulary](vocabulary/doordash-vocabulary.yml) — Unified taxonomy mapping 12 resources, 7 actions, 16 workflows, and 4 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [DoorDash Spectral Ruleset](rules/doordash-spectral-rules.yml) — 36 rules enforcing DoorDash API conventions

## Commercial

- [Plans & Pricing](plans/doordash-plans-pricing.yml) — API Commons Plans 0.1
- [Rate Limits](rate-limits/doordash-rate-limits.yml) — API Commons Rate Limits 0.1
- [FinOps](finops/doordash-finops.yml) — FOCUS-aligned FinOps Framework

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
