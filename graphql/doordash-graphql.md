# DoorDash GraphQL Schema

## Overview

This conceptual GraphQL schema models the DoorDash platform's core domains: on-demand delivery logistics (Drive API), marketplace order management, menu and catalog operations, and reporting. DoorDash's public APIs are REST-based (documented at [developer.doordash.com](https://developer.doordash.com/)), but this schema represents the underlying resource graph that those APIs expose, structured as GraphQL types for integration, tooling, and documentation purposes.

## Domains Covered

- **Delivery Logistics** — Deliveries, drivers, quotes, tracking events, pickup/dropoff details
- **Merchant & Store Operations** — Businesses, business locations, stores, store hours, special hours
- **Menu & Catalog** — Menus, categories, items, modifiers, modifier groups, pricing, availability
- **Orders** — Orders, order items, order modifiers, fees, payments, payment methods
- **Customer & Address** — Customers, profiles, addresses, geolocation
- **Promotions & Loyalty** — DashPass, promotions, promotion items, vouchers
- **Reviews & Ratings** — Reviews, ratings, driver ratings
- **Webhooks & Scheduling** — Webhooks, webhook events, schedules, preorder details
- **Financial** — Subtotals, taxes, tips, service fees, drive tips, signatures

## Key Types

| Type | Description |
|------|-------------|
| `Business` | A registered business entity using DoorDash Drive |
| `BusinessLocation` | A physical location belonging to a Business |
| `Store` | A merchant store on the DoorDash Marketplace |
| `StoreHours` | Regular operating hours for a Store |
| `SpecialHour` | Override hours for holidays or special events |
| `StoreMenu` | The top-level menu attached to a Store |
| `Menu` | A named menu grouping categories and items |
| `MenuCategory` | A grouping of MenuItems within a Menu |
| `MenuItem` | An individual item available for order |
| `MenuItemDetail` | Extended detail and nutritional info for a MenuItem |
| `MenuModifierGroup` | A group of options (e.g. "Choose a size") |
| `MenuModifier` | A single modifier option within a group |
| `Price` | A monetary value with currency |
| `PriceModifier` | A delta applied to a base Price |
| `Availability` | Time-based availability window for a menu entity |
| `Order` | A completed or in-progress customer order |
| `OrderItem` | A line item within an Order |
| `OrderModifier` | A modifier applied to an OrderItem |
| `OrderFee` | A fee line on an Order (delivery, service, etc.) |
| `Payment` | Payment record associated with an Order |
| `PaymentMethod` | A saved payment method on a Customer account |
| `Card` | Credit/debit card details within a PaymentMethod |
| `Delivery` | A Drive delivery job assigned to a Dasher |
| `DeliveryStatus` | Current status of a Delivery |
| `DeliveryQuote` | A price and time estimate for a potential Delivery |
| `DeliveryWindow` | An estimated time window for delivery arrival |
| `PickupWindow` | An estimated time window for Dasher pickup |
| `Driver` | A DoorDash Dasher fulfilling deliveries |
| `DriverLocation` | Real-time GPS location of a Driver |
| `DriverRating` | Rating and feedback for a Driver |
| `Customer` | A DoorDash end-user placing orders |
| `CustomerProfile` | Extended profile data for a Customer |
| `Address` | A structured postal address |
| `GeoLocation` | Latitude/longitude coordinate pair |
| `Pickup` | Pickup details for a Delivery |
| `Dropoff` | Dropoff details for a Delivery |
| `DropoffDetail` | Additional instructions and contact info for Dropoff |
| `PreorderDetails` | Scheduling details for a future-dated order |
| `DeliveryTracking` | Aggregated tracking state for a Delivery |
| `TrackingEvent` | A single event in the Delivery tracking timeline |
| `Webhook` | A registered webhook endpoint |
| `WebhookEvent` | A fired event payload sent to a Webhook |
| `Schedule` | A recurring availability schedule |
| `DashPass` | A DashPass membership subscription record |
| `Promotion` | A discount or promotional offer |
| `PromotionItem` | An item targeted by a Promotion |
| `Voucher` | A redeemable voucher code |
| `Review` | A customer review of a Store or Driver |
| `Rating` | An aggregate rating score |
| `Merchant` | A business entity on the Marketplace |
| `MerchantProfile` | Extended profile and metadata for a Merchant |
| `Category` | A top-level category tag for Stores |
| `Subtotal` | Order subtotal before fees and tax |
| `Tax` | Tax line on an Order |
| `Tip` | Customer tip on an Order |
| `ServiceFee` | Platform service fee on an Order |
| `DriveTip` | Tip paid directly to the Dasher |
| `Signature` | Proof of delivery signature record |
| `Photo` | A photo associated with proof of delivery or a menu item |

## Schema File

See [`doordash-schema.graphql`](doordash-schema.graphql) for the full type definitions.

## References

- Developer Portal: https://developer.doordash.com/
- Drive API Docs: https://developer.doordash.com/en-US/docs/drive/overview/about_drive/
- Marketplace API Docs: https://developer.doordash.com/en-US/docs/marketplace/overview/about_marketplace/
- GitHub: https://github.com/doordash
- Node.js SDK: https://www.npmjs.com/package/@doordash/sdk
