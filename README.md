# DoorDash (doordash)
DoorDash is a leading on-demand delivery platform connecting consumers with local businesses. Their developer platform provides APIs for integrating with DoorDash's logistics network, marketplace order management, item catalog synchronization, and business reporting, enabling merchants and partners to build delivery and commerce experiences powered by DoorDash's fleet of Dashers.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Delivery, Food Delivery, Logistics, Marketplace, On-Demand

## Timestamps

- **Created:** 2026-03-20
- **Modified:** 2026-03-20

## APIs

### DoorDash Drive API
The DoorDash Drive API enables businesses to request on-demand deliveries fulfilled by DoorDash's fleet of Dashers. It provides endpoints for checking delivery serviceability, getting delivery quotes, creating and managing deliveries, and tracking delivery status in real time. The API uses JWT-based authentication and is designed for businesses that want to offer delivery from their own ordering experience while leveraging DoorDash's logistics network.

**Human URL:** [https://developer.doordash.com/en-US/docs/drive/overview/about_drive/](https://developer.doordash.com/en-US/docs/drive/overview/about_drive/)


#### Tags:

 - Delivery, Logistics, Food Delivery, On-Demand, Last Mile

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/drive/overview/about_drive/)
- [OpenAPI](openapi/doordash-drive-openapi.yml)
- [AsyncAPI](asyncapi/doordash-drive-webhooks-asyncapi.yml)

### DoorDash Drive Classic API
The DoorDash Drive Classic API is the legacy version of the Drive API, designed for large enterprises and middleware providers who require extensive configuration and customizability for their delivery integrations. It provides endpoints for managing businesses, stores, and deliveries through DoorDash's logistics platform. The API uses JWT-based Bearer token authentication and operates at the v1 endpoint path. While still supported, DoorDash recommends new integrations use the newer Drive API (v2) instead.

**Human URL:** [https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/](https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/)


#### Tags:

 - Delivery, Logistics, Food Delivery, Enterprise, Last Mile

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/drive_classic/overview/about_drive_classic/)
- [OpenAPI](openapi/doordash-drive-classic-openapi.yml)

### DoorDash Marketplace API
The DoorDash Marketplace API allows merchants and third-party providers to integrate directly with the DoorDash marketplace for order management, menu synchronization, and store operations. It supports receiving orders from DoorDash, updating order statuses, and managing menu availability in real time. The API is not generally available and access is granted through a selective partner program where DoorDash evaluates integration quality and business fit.

**Human URL:** [https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/](https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/)


#### Tags:

 - Marketplace, Orders, Restaurants, Food Delivery, Retail

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/)
- [OpenAPI](openapi/doordash-marketplace-openapi.yml)
- [AsyncAPI](asyncapi/doordash-marketplace-webhooks-asyncapi.yml)

### DoorDash Item Management API
The DoorDash Item Management API enables merchants and integration partners to programmatically manage their item catalogs, inventory levels, pricing, and other product attributes on the DoorDash platform. It provides endpoints for creating, updating, and retrieving item data across stores. This API is particularly useful for retail and grocery partners who need to keep large catalogs synchronized between their own systems and DoorDash's marketplace.

**Human URL:** [https://developer.doordash.com/en-US/api/marketplace_v2/](https://developer.doordash.com/en-US/api/marketplace_v2/)


#### Tags:

 - Menus, Inventory, Pricing, Catalog, Retail

#### Properties

- [Documentation](https://developer.doordash.com/en-US/api/marketplace_v2/)
- [OpenAPI](openapi/doordash-item-management-openapi.yml)

### DoorDash Reporting API
The DoorDash Reporting API provides approved partners with access to standardized financial, operations, and menu reporting data. It offers a POST endpoint for creating report requests and a GET endpoint for retrieving report download links, along with webhook notifications when reports are ready. The API enables merchants to programmatically access business performance data including order volumes, financial summaries, and operational metrics without needing to manually export from the DoorDash merchant portal.

**Human URL:** [https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/](https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/)


#### Tags:

 - Reporting, Analytics, Financial, Operations, Data

#### Properties

- [Documentation](https://developer.doordash.com/en-US/docs/reporting/overview/about_reporting/)
- [OpenAPI](openapi/doordash-reporting-openapi.yml)
- [AsyncAPI](asyncapi/doordash-reporting-webhooks-asyncapi.yml)

## Common Properties

- [Developer Portal](https://developer.doordash.com/)
- [Documentation](https://developer.doordash.com/en-US/docs/getting-started)
- [Website](https://www.doordash.com/)
- [Blog](https://doordash.engineering/)
- [Login](https://developer.doordash.com/en-US/login)
- [TermsOfService](https://www.doordash.com/terms/)
- [PrivacyPolicy](https://www.doordash.com/privacy/)
- [Support](https://help.doordash.com/)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
