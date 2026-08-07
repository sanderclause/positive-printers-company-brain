# Active Sprint

## Sprint 2 — Website Launch and New Order Workflow

## Sprint Status

Active — read-only launch audit phase

---

# Sprint Objective

Launch the Positive Printers website and begin taking customer orders through a new GoHighLevel-based workflow as quickly and safely as possible.

---

# Owner Priorities

1. Finish and activate the customer-facing website.
2. Establish a working order or quote-intake workflow.
3. Begin moving operational work from Zoho to GoHighLevel.
4. Use recent customer and product data to decide which products should receive initial launch emphasis.
5. Avoid a risky all-at-once migration.

---

# Target Minimum Viable Workflow

Customer-facing website
→ customer selects a product or requests a quote
→ contact and order information enters GoHighLevel
→ staff receives and reviews the request
→ artwork, pricing, and production details are confirmed
→ job proceeds through the agreed production workflow
→ customer receives confirmation and status communication

This does not require every product, historical record, automation, or production stage to be migrated before launch.

---

# Safety Boundary

Zoho remains available as the existing reference and fallback system until:

- The new workflow has been tested with realistic orders
- Required customer and order fields have been mapped
- Staff can reliably find and manage new requests
- Customer confirmations work
- No required information is being lost
- The owner explicitly approves reducing or ending reliance on Zoho

Do not disable, delete, overwrite, or bulk-migrate Zoho data during this phase.

Do not make any live deployment, GoHighLevel configuration, database migration, DNS, or customer-facing change during the initial audit.

---

# Sprint Workflow

## Phase 1 — Read-only launch audit

Inspect, from the current `main` branches, without making any live deployment, GoHighLevel configuration, database migration, DNS, or customer-facing change:

- Positive Printers Company Brain
- `positive-printers-pricing`
- The customer-facing website work
- Catalog Admin
- Existing GoHighLevel integration code
- Existing Zoho imports, exports, mappings, and migration utilities
- Available deployment configuration
- Existing product, pricing, artwork, and order-intake workflows

Determine:

1. Which project is the canonical customer-facing website.
2. What is already built and working.
3. Whether anything is currently deployed and where.
4. What prevents the website from being safely activated.
5. Which parts of the GoHighLevel workflow exist only in code.
6. Which parts have been verified in an actual GoHighLevel account.
7. The current customer order journey from first contact through production.
8. The fields and stages that must move from Zoho to GoHighLevel.
9. Which historical Zoho information should be migrated, referenced, archived, or left in place.
10. The smallest product set that can support a real launch.
11. Which products can use instant pricing and which should begin as quote requests.
12. Required artwork-upload, payment, confirmation, staff-notification, and error-handling steps.
13. The safest pilot-order procedure.
14. Any credentials, environment variables, integrations, or external approvals that are missing.

Credential and environment-variable **names** may be inspected when necessary. Secret values are never displayed, copied, committed, or reported.

## Phase 2 — Implementation planning and execution

Not yet started. Requires Phase 1 findings and explicit owner approval of the implementation plan before any deployment, GoHighLevel configuration, database migration, DNS, or customer-facing change is made.

---

# Product and Customer Data

Post-2020 customer and order data may be used, initially only to help identify:

- Frequently purchased products
- Repeat-order products
- Products still selling recently
- Products suitable for an initial website launch
- Customer-product combinations suitable for early campaigns

Raw customer records, private contact information, order-level exports, or credentials must never be placed in the Company Brain or GitHub. Only aggregated and owner-approved findings may eventually become durable Company Brain knowledge.

---

# Constraints

- Do not disable, delete, overwrite, or bulk-migrate Zoho data during this phase.
- Do not make any live deployment, GoHighLevel configuration, database migration, DNS, or customer-facing change during the initial audit.
- Do not place raw customer records, private contact information, order-level exports, or credentials in the Company Brain or GitHub.
- Never display, copy, commit, or report secret credential values; environment-variable and integration **names** may be referenced.
- Do not treat the presence of integration code as proof that an integration is verified live.
- Preserve the existing Knowledge Core / Pricing App source-of-truth boundary.

---

# Acceptance Criteria

Phase 1 is complete when the following have been presented and separated into Confirmed working / Implemented in code but not verified live / Missing / Needs owner validation / Recommended for the minimum viable launch / Deferred until after launch:

1. Current-state website assessment
2. Current Zoho workflow
3. Current GoHighLevel implementation and verified-live status
4. Proposed minimum viable order workflow
5. Product launch recommendation
6. Zoho-to-GoHighLevel field and stage mapping
7. Deployment and integration blockers
8. Pilot test plan
9. Recommended implementation sequence
10. Exact files or systems that would change during implementation
11. Items requiring owner access, decisions, or approval

---

# Current Recommended Next Action

Complete the Phase 1 read-only launch audit, present the categorized findings and the Sprint 2 implementation plan, and stop for owner approval before any deployment, GoHighLevel configuration, database migration, DNS, or customer-facing change.
