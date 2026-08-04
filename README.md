# ShootProof (shootproof)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
