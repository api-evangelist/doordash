# Doordash

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

DoorDash is an on-demand local commerce platform whose developer program exposes its logistics and marketplace network through thirteen publicly documented REST APIs. Drive, Drive (classic) and Parcel let businesses request deliveries fulfilled by DoorDash's Dasher fleet, with Refunds, Redelivery and Dasher Feedback attached to that surface. Marketplace, Marketplace (legacy) and Item Management let merchants and retailers receive orders and synchronize menus, catalogs, inventory and promotions, while Storefront powers white-label online ordering, Reporting delivers financial and operational data exchange, and the Ads API sells sponsored placement on the marketplace. Every API authenticates with a short-lived HS256 JSON Web Token the caller signs itself, and DoorDash serves each OpenAPI definition as plain YAML from developer.doordash.com.

**Areas:** Delivery · Logistics · Last Mile Delivery · On-Demand · Food Delivery · Local Commerce · Marketplace · Restaurant · Grocery · Retail · Fulfillment · Webhook

## Doordash on APIs.io

Everything profiled for Doordash is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/doordash/](https://apis.io/providers/doordash/)** — or go straight to one of the APIs or properties below.

### APIs (49)

- [doordash Addresses API](https://apis.io/apis/doordash/doordash-addresses-api/) — Get address auto-completion suggestions based on partial input.
- [doordash Businesses API](https://apis.io/apis/doordash/doordash-businesses-api/) — Manage business entities that represent legal entities or owners.
- [doordash Catalog API](https://apis.io/apis/doordash/doordash-catalog-api/) — Manage the item catalog including adding new items and updating existing item information such as names, descriptions, images, and attributes.
- [doordash Deliveries API](https://apis.io/apis/doordash/doordash-deliveries-api/) — Create, retrieve, update, cancel, and estimate deliveries using the classic API endpoints.
- [doordash Inventory API](https://apis.io/apis/doordash/doordash-inventory-api/) — Manage store-level inventory, pricing, and other in-store attributes for items on the DoorDash platform.
- [doordash Items API](https://apis.io/apis/doordash/doordash-items-api/) — Manage item availability and 86ing (marking items as unavailable) in real time.
- [doordash Menus API](https://apis.io/apis/doordash/doordash-menus-api/) — Create, update, and manage menus for stores on the DoorDash marketplace.
- [doordash Orders API](https://apis.io/apis/doordash/doordash-orders-api/) — Receive, confirm, update, and manage orders placed through the DoorDash marketplace.
- [doordash Promotions API](https://apis.io/apis/doordash/doordash-promotions-api/) — Manage item-level promotions at the store level, including adding and updating promotional pricing.
- [doordash Quotes API](https://apis.io/apis/doordash/doordash-quotes-api/) — Validate delivery serviceability and get pricing quotes before creating a delivery.
- [doordash Reports API](https://apis.io/apis/doordash/doordash-reports-api/) — Create report requests and retrieve report download links for financial, operations, menu, and feedback data.
- [doordash Stores API](https://apis.io/apis/doordash/doordash-stores-api/) — Manage store locations associated with businesses.
- [Doordash Ad Groups API](https://apis.io/apis/doordash/doordash-ad-groups-api/) — The Ad Groups API from Doordash — 2 operation(s) for ad groups.
- [Doordash Address API](https://apis.io/apis/doordash/doordash-address-api/) — The Address API from Doordash — 5 operation(s) for address.
- [Doordash App API](https://apis.io/apis/doordash/doordash-app-api/) — Endpoints for mobile app related information
- [Doordash Assets API](https://apis.io/apis/doordash/doordash-assets-api/) — The Assets API from Doordash — 3 operation(s) for assets.
- [Doordash Audit API](https://apis.io/apis/doordash/doordash-audit-api/) — The Audit API from Doordash — 1 operation(s) for audit.
- [Doordash Business & Store API](https://apis.io/apis/doordash/doordash-business-store-api/) — The Business & Store API from Doordash — 9 operation(s) for business & store.
- [Doordash Campaigns API](https://apis.io/apis/doordash/doordash-campaigns-api/) — The Campaigns API from Doordash — 3 operation(s) for campaigns.
- [Doordash Checkout Management Endpoints API](https://apis.io/apis/doordash/doordash-checkoutmanagementendpoints-api/) — Endpoints for managing checkout and transactions
- [Doordash Creatives (SB) API](https://apis.io/apis/doordash/doordash-creatives-sb-api/) — For Sponsored Brand campaigns only.
- [Doordash Dasher Feedback API](https://apis.io/apis/doordash/doordash-dasherfeedback-api/) — The DasherFeedback API from Doordash — 2 operation(s) for dasherfeedback.
- [Doordash Dataexchange API](https://apis.io/apis/doordash/doordash-dataexchange-api/) — The Dataexchange API from Doordash — 2 operation(s) for dataexchange.
- [Doordash Delivery API](https://apis.io/apis/doordash/doordash-delivery-api/) — The Delivery API from Doordash — 12 operation(s) for delivery.
- [Doordash Drive Redelivery API](https://apis.io/apis/doordash/doordash-drive-redelivery-api/) — The drive-redelivery API from Doordash — 1 operation(s) for drive-redelivery.
- [Doordash Https: API](https://apis.io/apis/doordash/doordash-https-api/) — The Https: API from Doordash — 2 operation(s) for https:.
- [Doordash Inventory Management Endpoints API](https://apis.io/apis/doordash/doordash-inventorymanagementendpoints-api/) — Endpoints to manage inventory/pricing and other item attributes specific to this store
- [Doordash Item Management Endpoints API](https://apis.io/apis/doordash/doordash-itemmanagementendpoints-api/) — Endpoints for item management
- [Doordash Job Management Endpoints API](https://apis.io/apis/doordash/doordash-jobmanagementendpoints-api/) — Endpoints to create jobs to support pull request flows.
- [Doordash JWT API](https://apis.io/apis/doordash/doordash-jwt-api/) — Endpoints for JWT resources
- [Doordash Keywords (SP) API](https://apis.io/apis/doordash/doordash-keywords-sp-api/) — For Sponsored Products campaigns only.
- [Doordash Loyalty API](https://apis.io/apis/doordash/doordash-loyalty-api/) — Endpoints for loyalty related resources
- [Doordash Menu API](https://apis.io/apis/doordash/doordash-menu-api/) — The Menu API from Doordash — 1 operation(s) for menu.
- [Doordash Menu Endpoints API](https://apis.io/apis/doordash/doordash-menu-endpoints-api/) — Endpoints for updating and creating menus
- [Doordash Menu Item API](https://apis.io/apis/doordash/doordash-menu-item-api/) — The Menu Item API from Doordash — 1 operation(s) for menu item.
- [Doordash Menu V2 API](https://apis.io/apis/doordash/doordash-menu-v2-api/) — The Menu V2 API from Doordash — 1 operation(s) for menu v2.
- [Doordash Merchants (Retailers) API](https://apis.io/apis/doordash/doordash-merchants-retailers-api/) — To retrieve business IDs available for merchant targeting.
- [Doordash New Verticals Self Serve Integration Endpoints API](https://apis.io/apis/doordash/doordash-newverticalsselfserveintegrationendpoints-api/) — Endpoints for new verticals self-serve integration onboarding
- [Doordash Order API](https://apis.io/apis/doordash/doordash-order-api/) — Endpoints for order resources
- [Doordash Order Endpoints API](https://apis.io/apis/doordash/doordash-order-endpoints-api/) — Endpoints for retrieving and confirming success of orders
- [Doordash Product Ads API](https://apis.io/apis/doordash/doordash-product-ads-api/) — The Product Ads API from Doordash — 1 operation(s) for product ads.
- [Doordash Promotion Management Endpoints API](https://apis.io/apis/doordash/doordash-promotionmanagementendpoints-api/) — Endpoints for promotion management
- [Doordash Refunds API](https://apis.io/apis/doordash/doordash-refunds-api/) — The Refunds API from Doordash — 1 operation(s) for refunds.
- [Doordash Report API](https://apis.io/apis/doordash/doordash-report-api/) — The Report API from Doordash — 3 operation(s) for report.
- [Doordash Resources API](https://apis.io/apis/doordash/doordash-resources-api/) — To retrieve brands and categories available for behavioral targeting.
- [Doordash Search API](https://apis.io/apis/doordash/doordash-search-api/) — Endpoints for store searches
- [Doordash Store Endpoints API](https://apis.io/apis/doordash/doordash-store-endpoints-api/) — Endpoints for store based operations
- [Doordash Store Management Endpoints API](https://apis.io/apis/doordash/doordash-storemanagementendpoints-api/) — Endpoints for managing stores
- [Doordash Targeting API](https://apis.io/apis/doordash/doordash-targeting-api/) — The Targeting API from Doordash — 1 operation(s) for targeting.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (3)

Event-driven and webhook contracts.

- [DoorDash Drive Delivery Webhooks](https://apis.io/asyncapis/doordash/doordash-drive-webhooks-asyncapi/)
- [DoorDash Marketplace Webhooks](https://apis.io/asyncapis/doordash/doordash-marketplace-webhooks-asyncapi/)
- [DoorDash Reporting Webhooks](https://apis.io/asyncapis/doordash/doordash-reporting-webhooks-asyncapi/)

#### Event channels (6)

Individual events and webhooks the provider emits.

- [/deliveries](https://apis.io/channels/doordash/deliveries/)
- [/menus](https://apis.io/channels/doordash/menus/)
- [/onboarding](https://apis.io/channels/doordash/onboarding/)
- [/orders](https://apis.io/channels/doordash/orders/)
- [/reports](https://apis.io/channels/doordash/reports/)
- [/webhook](https://apis.io/channels/doordash/webhook/)

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/doordash/](https://apis.io/graphqls/doordash/doordash-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [MCP candidate - DoorDash publishes no MCP server](https://apis.io/servers/doordash/mcp-candidate---doordash-publishes-no-mcp-server/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Doordash Agentic Access](https://apis.io/agentic-access/doordash/doordash-agentic-access/)

#### JSON Schema (59)

The data models the API reads and writes.

- [AcceptQuoteRequest](https://apis.io/schemas/doordash/doordash-accept-quote-request/)
- [AddressSuggestion](https://apis.io/schemas/doordash/doordash-address-suggestion/)
- [Business](https://apis.io/schemas/doordash/doordash-business/)
- [BusinessRequest](https://apis.io/schemas/doordash/doordash-business-request/)
- [CancelledItem](https://apis.io/schemas/doordash/doordash-cancelled-item/)
- [CatalogItem](https://apis.io/schemas/doordash/doordash-catalog-item/)
- [CatalogItemsRequest](https://apis.io/schemas/doordash/doordash-catalog-items-request/)
- [CatalogItemsResponse](https://apis.io/schemas/doordash/doordash-catalog-items-response/)
- [CheckoutAuditSignal](https://apis.io/schemas/doordash/doordash-checkout-audit-signal/)
- [ClassicDelivery](https://apis.io/schemas/doordash/doordash-classic-delivery/)
- [ClassicDeliveryRequest](https://apis.io/schemas/doordash/doordash-classic-delivery-request/)
- [ClassicDeliveryUpdateRequest](https://apis.io/schemas/doordash/doordash-classic-delivery-update-request/)
- [Customer](https://apis.io/schemas/doordash/doordash-customer/)
- [Delivery](https://apis.io/schemas/doordash/doordash-delivery/)
- [DeliveryItem](https://apis.io/schemas/doordash/doordash-delivery-item/)
- [DeliveryRequest](https://apis.io/schemas/doordash/doordash-delivery-request/)
- [DeliveryUpdateRequest](https://apis.io/schemas/doordash/doordash-delivery-update-request/)
- [DeliveryWebhookPayload](https://apis.io/schemas/doordash/doordash-delivery-webhook-payload/)
- [Error](https://apis.io/schemas/doordash/doordash-error/)
- [Estimate](https://apis.io/schemas/doordash/doordash-estimate/)
- [EstimateRequest](https://apis.io/schemas/doordash/doordash-estimate-request/)
- [ItemOption](https://apis.io/schemas/doordash/doordash-item-option/)
- [ItemStatusUpdate](https://apis.io/schemas/doordash/doordash-item-status-update/)
- [ItemError](https://apis.io/schemas/doordash/doordash-itemerror/)
- [Location](https://apis.io/schemas/doordash/doordash-location/)
- …and 34 more published on APIs.io

#### JSON Structure (55)

Data models expressed in JSON Structure.

- [Doordash Accept Quote Request Structure](https://apis.io/json-structure/doordash/doordash-accept-quote-request-structure/)
- [Doordash Address Suggestion Structure](https://apis.io/json-structure/doordash/doordash-address-suggestion-structure/)
- [Doordash Business Request Structure](https://apis.io/json-structure/doordash/doordash-business-request-structure/)
- [Doordash Business Structure](https://apis.io/json-structure/doordash/doordash-business-structure/)
- [Doordash Cancelled Item Structure](https://apis.io/json-structure/doordash/doordash-cancelled-item-structure/)
- [Doordash Catalog Item Structure](https://apis.io/json-structure/doordash/doordash-catalog-item-structure/)
- [Doordash Catalog Items Request Structure](https://apis.io/json-structure/doordash/doordash-catalog-items-request-structure/)
- [Doordash Catalog Items Response Structure](https://apis.io/json-structure/doordash/doordash-catalog-items-response-structure/)
- [Doordash Checkout Audit Signal Structure](https://apis.io/json-structure/doordash/doordash-checkout-audit-signal-structure/)
- [Doordash Classic Delivery Request Structure](https://apis.io/json-structure/doordash/doordash-classic-delivery-request-structure/)
- [Doordash Classic Delivery Structure](https://apis.io/json-structure/doordash/doordash-classic-delivery-structure/)
- [Doordash Classic Delivery Update Request Structure](https://apis.io/json-structure/doordash/doordash-classic-delivery-update-request-structure/)
- [Doordash Customer Structure](https://apis.io/json-structure/doordash/doordash-customer-structure/)
- [Doordash Delivery Item Structure](https://apis.io/json-structure/doordash/doordash-delivery-item-structure/)
- [Doordash Delivery Request Structure](https://apis.io/json-structure/doordash/doordash-delivery-request-structure/)
- [Doordash Delivery Structure](https://apis.io/json-structure/doordash/doordash-delivery-structure/)
- [Doordash Delivery Update Request Structure](https://apis.io/json-structure/doordash/doordash-delivery-update-request-structure/)
- [Doordash Delivery Webhook Payload Structure](https://apis.io/json-structure/doordash/doordash-delivery-webhook-payload-structure/)
- [Doordash Estimate Request Structure](https://apis.io/json-structure/doordash/doordash-estimate-request-structure/)
- [Doordash Estimate Structure](https://apis.io/json-structure/doordash/doordash-estimate-structure/)
- [Doordash Item Option Structure](https://apis.io/json-structure/doordash/doordash-item-option-structure/)
- [Doordash Item Status Update Structure](https://apis.io/json-structure/doordash/doordash-item-status-update-structure/)
- [Doordash Location Structure](https://apis.io/json-structure/doordash/doordash-location-structure/)
- [Doordash Marketplace Delivery Webhook Payload Structure](https://apis.io/json-structure/doordash/doordash-marketplace-delivery-webhook-payload-structure/)
- [Doordash Menu Category Structure](https://apis.io/json-structure/doordash/doordash-menu-category-structure/)
- …and 30 more published on APIs.io

#### JSON-LD (9)

Linked-data contexts for the provider's vocabulary.

- [Doordash Context](https://apis.io/jsonld/doordash/doordash-context/)
- [Doordash Drive Classic Context](https://apis.io/jsonld/doordash/doordash-drive-classic-context/)
- [Doordash Drive Context](https://apis.io/jsonld/doordash/doordash-drive-context/)
- [Doordash Drive Webhooks Context](https://apis.io/jsonld/doordash/doordash-drive-webhooks-context/)
- [Doordash Item Management Context](https://apis.io/jsonld/doordash/doordash-item-management-context/)
- [Doordash Marketplace Context](https://apis.io/jsonld/doordash/doordash-marketplace-context/)
- [Doordash Marketplace Webhooks Context](https://apis.io/jsonld/doordash/doordash-marketplace-webhooks-context/)
- [Doordash Reporting Context](https://apis.io/jsonld/doordash/doordash-reporting-context/)
- [Doordash Reporting Webhooks Context](https://apis.io/jsonld/doordash/doordash-reporting-webhooks-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Doordash Vocabulary](https://apis.io/vocabularies/doordash/doordash-vocabulary/)

#### Examples (55)

Example requests and responses.

- [Doordash Accept Quote Request Example](https://apis.io/examples/doordash/doordash-accept-quote-request-example/)
- [Doordash Address Suggestion Example](https://apis.io/examples/doordash/doordash-address-suggestion-example/)
- [Doordash Business Example](https://apis.io/examples/doordash/doordash-business-example/)
- [Doordash Business Request Example](https://apis.io/examples/doordash/doordash-business-request-example/)
- [Doordash Cancelled Item Example](https://apis.io/examples/doordash/doordash-cancelled-item-example/)
- [Doordash Catalog Item Example](https://apis.io/examples/doordash/doordash-catalog-item-example/)
- [Doordash Catalog Items Request Example](https://apis.io/examples/doordash/doordash-catalog-items-request-example/)
- [Doordash Catalog Items Response Example](https://apis.io/examples/doordash/doordash-catalog-items-response-example/)
- [Doordash Checkout Audit Signal Example](https://apis.io/examples/doordash/doordash-checkout-audit-signal-example/)
- [Doordash Classic Delivery Example](https://apis.io/examples/doordash/doordash-classic-delivery-example/)
- [Doordash Classic Delivery Request Example](https://apis.io/examples/doordash/doordash-classic-delivery-request-example/)
- [Doordash Classic Delivery Update Request Example](https://apis.io/examples/doordash/doordash-classic-delivery-update-request-example/)
- [Doordash Customer Example](https://apis.io/examples/doordash/doordash-customer-example/)
- [Doordash Delivery Example](https://apis.io/examples/doordash/doordash-delivery-example/)
- [Doordash Delivery Item Example](https://apis.io/examples/doordash/doordash-delivery-item-example/)
- [Doordash Delivery Request Example](https://apis.io/examples/doordash/doordash-delivery-request-example/)
- [Doordash Delivery Update Request Example](https://apis.io/examples/doordash/doordash-delivery-update-request-example/)
- [Doordash Delivery Webhook Payload Example](https://apis.io/examples/doordash/doordash-delivery-webhook-payload-example/)
- [Doordash Estimate Example](https://apis.io/examples/doordash/doordash-estimate-example/)
- [Doordash Estimate Request Example](https://apis.io/examples/doordash/doordash-estimate-request-example/)
- [Doordash Item Option Example](https://apis.io/examples/doordash/doordash-item-option-example/)
- [Doordash Item Status Update Example](https://apis.io/examples/doordash/doordash-item-status-update-example/)
- [Doordash Location Example](https://apis.io/examples/doordash/doordash-location-example/)
- [Doordash Marketplace Delivery Webhook Payload Example](https://apis.io/examples/doordash/doordash-marketplace-delivery-webhook-payload-example/)
- [Doordash Menu Category Example](https://apis.io/examples/doordash/doordash-menu-category-example/)
- …and 30 more published on APIs.io

#### Collections (29)

Postman and Open Collection request collections.

- [DoorDash Drive Classic Addresses API](https://apis.io/collections/doordash/open-doordash-addresses-api/)
- [DoorDash Drive Classic Addresses Businesses API](https://apis.io/collections/doordash/open-doordash-businesses-api/)
- [DoorDash Drive Classic Addresses Catalog API](https://apis.io/collections/doordash/open-doordash-catalog-api/)
- [DoorDash Drive Classic Addresses Deliveries API](https://apis.io/collections/doordash/open-doordash-deliveries-api/)
- [DoorDash Drive API](https://apis.io/collections/doordash/open-doordash-drive/)
- [DoorDash Drive Classic API](https://apis.io/collections/doordash/open-doordash-drive-classic/)
- [DoorDash Drive Classic Addresses Inventory API](https://apis.io/collections/doordash/open-doordash-inventory-api/)
- [DoorDash Item Management API](https://apis.io/collections/doordash/open-doordash-item-management/)
- [DoorDash Drive Classic Addresses Items API](https://apis.io/collections/doordash/open-doordash-items-api/)
- [DoorDash Marketplace API](https://apis.io/collections/doordash/open-doordash-marketplace/)
- [DoorDash Drive Classic Addresses Menus API](https://apis.io/collections/doordash/open-doordash-menus-api/)
- [DoorDash Drive Classic Addresses Orders API](https://apis.io/collections/doordash/open-doordash-orders-api/)
- [DoorDash Drive Classic Addresses Promotions API](https://apis.io/collections/doordash/open-doordash-promotions-api/)
- [DoorDash Drive Classic Addresses Quotes API](https://apis.io/collections/doordash/open-doordash-quotes-api/)
- [DoorDash Reporting API](https://apis.io/collections/doordash/open-doordash-reporting/)
- [DoorDash Drive Classic Addresses Reports API](https://apis.io/collections/doordash/open-doordash-reports-api/)
- [DoorDash Drive Classic Addresses Stores API](https://apis.io/collections/doordash/open-doordash-stores-api/)
- [DoorDash Drive Classic Addresses API](https://apis.io/collections/doordash/postman-doordash-addresses-api/)
- [DoorDash Drive Classic Addresses Businesses API](https://apis.io/collections/doordash/postman-doordash-businesses-api/)
- [DoorDash Drive Classic Addresses Catalog API](https://apis.io/collections/doordash/postman-doordash-catalog-api/)
- [DoorDash Drive Classic Addresses Deliveries API](https://apis.io/collections/doordash/postman-doordash-deliveries-api/)
- [DoorDash Drive Classic Addresses Inventory API](https://apis.io/collections/doordash/postman-doordash-inventory-api/)
- [DoorDash Drive Classic Addresses Items API](https://apis.io/collections/doordash/postman-doordash-items-api/)
- [DoorDash Drive Classic Addresses Menus API](https://apis.io/collections/doordash/postman-doordash-menus-api/)
- [DoorDash Drive Classic Addresses Orders API](https://apis.io/collections/doordash/postman-doordash-orders-api/)
- …and 4 more published on APIs.io

#### Overlays (62)

OpenAPI overlays, including conversational phrasing for each operation.

- [Doordash Ad Groups Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-ad-groups-api-phrasing-overlay/)
- [Doordash Address Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-address-api-phrasing-overlay/)
- [Doordash Addresses Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-addresses-api-phrasing-overlay/)
- [Doordash Ads Overlay](https://apis.io/overlays/doordash/doordash-ads-overlay/)
- [Doordash App Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-app-api-phrasing-overlay/)
- [Doordash Assets Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-assets-api-phrasing-overlay/)
- [Doordash Audit Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-audit-api-phrasing-overlay/)
- [Doordash Business Store Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-business-store-api-phrasing-overlay/)
- [Doordash Businesses Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-businesses-api-phrasing-overlay/)
- [Doordash Campaigns Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-campaigns-api-phrasing-overlay/)
- [Doordash Catalog Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-catalog-api-phrasing-overlay/)
- [Doordash Checkoutmanagementendpoints Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-checkoutmanagementendpoints-api-phrasing-overlay/)
- [Doordash Creatives Sb Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-creatives-sb-api-phrasing-overlay/)
- [Doordash Dasherfeedback Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-dasherfeedback-api-phrasing-overlay/)
- [Doordash Dataexchange Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-dataexchange-api-phrasing-overlay/)
- [Doordash Deliveries Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-deliveries-api-phrasing-overlay/)
- [Doordash Delivery Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-delivery-api-phrasing-overlay/)
- [Doordash Drive Classic Overlay](https://apis.io/overlays/doordash/doordash-drive-classic-overlay/)
- [Doordash Drive Dasher Feedback Overlay](https://apis.io/overlays/doordash/doordash-drive-dasher-feedback-overlay/)
- [Doordash Drive Overlay](https://apis.io/overlays/doordash/doordash-drive-overlay/)
- [Doordash Drive Redelivery Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-drive-redelivery-api-phrasing-overlay/)
- [Doordash Drive Redelivery Overlay](https://apis.io/overlays/doordash/doordash-drive-redelivery-overlay/)
- [Doordash Drive Refunds Overlay](https://apis.io/overlays/doordash/doordash-drive-refunds-overlay/)
- [Doordash External Checkout Overlay](https://apis.io/overlays/doordash/doordash-external-checkout-overlay/)
- [Doordash Https Api Phrasing Overlay](https://apis.io/overlays/doordash/doordash-https-api-phrasing-overlay/)
- …and 37 more published on APIs.io

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [Doordash — asyncapi rules](https://apis.io/rules/doordash/doordash-asyncapi-spectral-rules/)
- [Doordash — jsonschema rules](https://apis.io/rules/doordash/doordash-jsonschema-spectral-rules/)
- [Doordash API Rules](https://apis.io/rules/doordash/doordash-spectral-rules/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Doordash Authentication](https://apis.io/security/doordash/doordash-authentication/)
- [Doordash Domain Security](https://apis.io/security/doordash/doordash-domain-security/)
- [Doordash Trust Center](https://apis.io/security/doordash/doordash-trust-center/)
- [Doordash Vulnerability Disclosure](https://apis.io/security/doordash/doordash-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Doordash Plans Pricing](https://apis.io/plans/doordash/doordash-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Doordash Rate Limits](https://apis.io/rate-limits/doordash/doordash-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Doordash Finops](https://apis.io/finops/doordash/doordash-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.doordash.com/)
- [Documentation](https://developer.doordash.com/en-US/)
- [Getting started](https://developer.doordash.com/en-US/docs/drive/tutorials/get_started/)
- [API reference](https://developer.doordash.com/en-US/api/drive)
- [Pricing](https://developer.doordash.com/en-US/docs/drive/overview/pricing_payment)
- [Sign up](https://developer.doordash.com/portal)
- [Support](https://help.doordash.com/)
- [Changelog](https://developer.doordash.com/en-US/docs/reporting/overview/release_notes)
- [Blog](https://doordash.engineering/)
- [Security](https://hackerone.com/doordash)
- [Compliance](https://trust.doordash.com/)
- [Terms of service](https://www.doordash.com/terms/)
- [Privacy policy](https://www.doordash.com/privacy/)
- [GitHub](https://github.com/doordash)
- [Status](https://www.doordashstatus.com)

## API Evangelist rating

**Kin Score 76.2** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 69.1 |
| Contract governance | 31.8 |
| Operational transparency | 73.7 |
| Developer ergonomics | 74.4 |
| Access clarity | 92.1 |

**Agent readiness 35.5** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | verified |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | — |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/doordash/](https://apis.io/providers/doordash/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Doordash: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/doordash/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
