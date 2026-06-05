# doordash (doordash)

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
