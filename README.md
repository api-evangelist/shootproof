# ShootProof (shootproof)

ShootProof is a SaaS platform for professional photographers that handles client galleries, proofing, digital download rules, watermarking, contracts, invoicing, and print/product e-commerce fulfilled through partner labs. The ShootProof Studio API is a RESTful, hypermedia (HAL-style links) API secured with three-legged OAuth 2.0, published with a downloadable OpenAPI 3.0 document (`oas/studio.json`) at developer.shootproof.com. It exposes a studio's Brands, Events (client galleries) and Albums, Photos, Contacts (clients), Contracts, Orders, Invoices, Price Sheets, and Email automation as linked resources under a single `https://api.shootproof.com/studio` base URL. API access is included free with a ShootProof account; a client ID is issued by ShootProof support on request. A separate legacy REST API also remains documented for older integrations.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/shootproof/refs/heads/main/apis.yml)

## Tags

- Photography
- Client Galleries
- Proofing
- Digital Downloads
- Photo Studio Management
- E-Commerce
- SaaS

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

### ShootProof Studios API

Read and update a photographer's Studio and its Brands - list a studio's brands, get and partially update a brand, manage brand themes and homepage settings, list watermarks, and pull gallery-activity, lab-order, and sales-history summaries for a brand.

- **Human URL:** [https://developer.shootproof.com/reference/studio/brands/](https://developer.shootproof.com/reference/studio/brands/)
- **Base URL:** `https://api.shootproof.com/studio`

#### Tags

- Studios
- Brands
- Account

#### Properties

- [Documentation](https://developer.shootproof.com/guide/)
- [API Reference](https://developer.shootproof.com/reference/studio/brands/)
- [OpenAPI](openapi/shootproof-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### ShootProof Events & Galleries API

Create, list, update, and batch-manage Events (client galleries and shoots) and the Albums nested inside them - event categories and defaults, per-event/album digital download rules, cover photos, QR codes for Volume events, and the client contact attached to an event.

- **Human URL:** [https://developer.shootproof.com/reference/studio/events/](https://developer.shootproof.com/reference/studio/events/)
- **Base URL:** `https://api.shootproof.com/studio`

#### Tags

- Events
- Galleries
- Albums

#### Properties

- [Documentation](https://developer.shootproof.com/guide/)
- [API Reference](https://developer.shootproof.com/reference/studio/events/)
- [OpenAPI](openapi/shootproof-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### ShootProof Photos API

List, retrieve, create, update, and delete the photos inside an event - generate a signed photo upload policy, redirect to a photo's original file, add or remove photos from an album, and create zip-bundle download links for an event or album.

- **Human URL:** [https://developer.shootproof.com/reference/studio/events/](https://developer.shootproof.com/reference/studio/events/)
- **Base URL:** `https://api.shootproof.com/studio`

#### Tags

- Photos
- Uploads
- Digital Downloads

#### Properties

- [Documentation](https://developer.shootproof.com/guide/)
- [API Reference](https://developer.shootproof.com/reference/studio/events/)
- [OpenAPI](openapi/shootproof-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### ShootProof Clients API

Manage the contacts (clients) attached to a brand - create, list, search, update, and delete contacts, look up referral tags and relationships, send a contact an email, and read a contact's recent activity timeline.

- **Human URL:** [https://developer.shootproof.com/reference/studio/contacts/](https://developer.shootproof.com/reference/studio/contacts/)
- **Base URL:** `https://api.shootproof.com/studio`

#### Tags

- Contacts
- Clients
- CRM

#### Properties

- [Documentation](https://developer.shootproof.com/guide/)
- [API Reference](https://developer.shootproof.com/reference/studio/contacts/)
- [OpenAPI](openapi/shootproof-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### ShootProof Orders API

Create and manage print/product orders placed against a brand (beta, per ShootProof's own API tagging) - list and retrieve orders, add/update/remove order items tied to specific photos, email order receipts, generate lab shipment records, and list client payments recorded against an order.

- **Human URL:** [https://developer.shootproof.com/reference/studio/orders/](https://developer.shootproof.com/reference/studio/orders/)
- **Base URL:** `https://api.shootproof.com/studio`

#### Tags

- Orders
- E-Commerce
- Lab Fulfillment

#### Properties

- [Documentation](https://developer.shootproof.com/guide/)
- [API Reference](https://developer.shootproof.com/reference/studio/orders/)
- [OpenAPI](openapi/shootproof-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### ShootProof Contracts API

Create and manage client contracts and reusable contract templates - full CRUD on contracts and templates, updating contract status and associated contacts, and emailing a contract to its contacts for review and e-signature.

- **Human URL:** [https://developer.shootproof.com/reference/studio/contracts/](https://developer.shootproof.com/reference/studio/contracts/)
- **Base URL:** `https://api.shootproof.com/studio`

#### Tags

- Contracts
- E-Sign
- Templates

#### Properties

- [Documentation](https://developer.shootproof.com/guide/)
- [API Reference](https://developer.shootproof.com/reference/studio/contracts/)
- [OpenAPI](openapi/shootproof-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [GitHub Organization](https://github.com/ShootProof)
- [LinkedIn](https://www.linkedin.com/company/shootproof)
- [Website](https://www.shootproof.com)
- [Documentation](https://developer.shootproof.com/)
- [Plans](plans/shootproof-plans-pricing.yml)
- [Rate Limits](rate-limits/shootproof-rate-limits.yml)
- [Fin Ops](finops/shootproof-finops.yml)

## Review

Does ShootProof expose a documented public WebSocket API? **No.** See [review.yml](review.yml) for the full findings - ShootProof's Studio API is a RESTful, hypermedia (HAL-style links) API over HTTPS with three-legged OAuth 2.0, confirmed live against its published OpenAPI 3.0 document (157 paths, 181 schemas). No WebSocket, SSE, or webhook subscription mechanism is documented.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
