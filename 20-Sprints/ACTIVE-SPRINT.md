# Active Sprint

## Sprint 2 — Website Launch and New Order Workflow

## Sprint Status

Active — Phase 2A: architecture approved, verification and containment planning

---

# Sprint Objective

Launch the Positive Printers website and begin taking customer orders through a new HighLevel-based workflow as quickly and safely as possible.

---

# Owner Priorities

1. Finish and activate the customer-facing website.
2. Establish a working order or quote-intake workflow.
3. Begin moving operational work from Zoho to HighLevel.
4. Use recent customer and product data to decide which products should receive initial launch emphasis.
5. Avoid a risky all-at-once migration.

---

# Approved Operating Architecture

- HighLevel AI Studio is the future public Positive Printers website.
- The unfinished AI Studio website must not accept real customer orders yet.
- Supabase remains the detailed product catalog, configuration, pricing, and historical-data layer.
- HighLevel is the operational system for contacts, opportunities, estimates, approvals, invoices, payments, workflows, and staff reporting.
- Native HighLevel Products, Estimates, Invoices, Workflows, and Dashboards are used wherever they meet the requirement.
- The separate estimate app (the Next.js Pricing App customer calculator) is not expanded into a parallel estimating and invoicing system.
- The existing estimate app is preserved for now and audited only for reusable product-configuration and pricing components.
- If native HighLevel estimating later proves insufficient, the only additional build considered is a focused Print Configurator that sends calculated line items into native HighLevel estimates.
- Business Cards are the first instant-pricing candidate. Other products may begin as quote-request products.
- Artwork handling and payment may remain manual during the first controlled pilot.
- Zoho remains a reference and fallback system until the new workflow is validated.

---

# Dynamic Website Architecture

The AI Studio website displays products dynamically from a safe Supabase-backed catalog endpoint. Product presentation supports: category slug, product slug, product name, short and full descriptions, product images, published/draft status, featured status, sort order, instant-price / configured-estimate / quote-request selling mode, available variants and options, starting-price display where appropriate, and SEO title and description.

Security boundary:

- Never expose a Supabase service-role key, Zoho secret, or HighLevel private token in browser code.
- The public website may use only a properly restricted anonymous Supabase connection with verified row-level security, or a protected backend/Edge Function.
- Vendor costs, markup rules, private notes, and sensitive pricing logic must never be returned to the public browser.

---

# Target Minimum Viable Workflow

Customer visits the AI Studio website
→ browses dynamic Supabase-backed products
→ configures Business Cards (instant price) or requests a quote for another product
→ contact and request information enters HighLevel
→ staff creates or reviews a native HighLevel estimate
→ customer receives and accepts/rejects the estimate
→ accepted estimate converts into a native HighLevel invoice
→ staff tracks progress through the approved HighLevel workflow

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

---

# Sprint Workflow

## Phase 1 — Read-only launch audit

Status: Complete.

Findings covered: canonical-website ambiguity (Next.js app vs. WordPress vs. HighLevel AI Studio), current Next.js app capability and deployment status, current Zoho sales and production workflow, GoHighLevel/HighLevel implementation reviewed stage-by-stage (code vs. verified-live), a data-driven product launch recommendation from post-2020 Opportunities data, a proposed Zoho-to-HighLevel field/stage mapping, deployment and integration blockers, a pilot test plan, and items requiring owner decision.

The owner reviewed the findings and approved the operating architecture recorded above.

## Phase 2A — Verification, containment, and reuse audit

Status: In progress.

1. Record the approved Sprint 2 decisions in the Company Brain.
2. Assess credential exposure (exposed Supabase service-role key, exposed Zoho client secret/refresh token) without displaying secret values; prepare a safe rotation sequence; replace hardcoded credentials in working code with environment-variable references where safe; do not rotate live credentials.
3. Correct the known GoHighLevel documentation overstatement in the canonical pricing repository's `README.md`.
4. Attempt read-only HighLevel verification of existing Products, estimate/invoice templates, pipelines, workflows, dashboards, custom fields, forms, and any prior test contacts/opportunities. Make no changes.
5. Identify genuine native-HighLevel capability gaps against Positive Printers' requirements (Products, Estimates, templates, accept/reject, invoice conversion, payments, pipelines, workflows, dashboards).
6. Audit the existing estimate app read-only; separate its features into natively-covered-by-HighLevel, reusable Supabase pricing/configuration logic, reusable product-selection interface, reusable templates/presets, duplicate functionality to retire, and functionality that may justify a future Print Configurator.
7. Prepare the exact configuration plan for the minimum Business Card pilot workflow (Target Minimum Viable Workflow above).
8. Confirm the safest reversible method to prevent `website.positiveprinters.com` from accepting real orders while development continues, and report the recommended action for owner approval. Do not change the domain, DNS, published state, or website.

## Phase 2B — Implementation

Not yet started. Requires Phase 2A findings and explicit owner approval before any credential rotation, live HighLevel configuration change, website publish/unpublish, DNS change, data migration or deletion, or sending of a real estimate or invoice.

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

- Do not disable, delete, overwrite, or bulk-migrate Zoho data.
- Do not rotate or revoke live credentials.
- Do not change live HighLevel configuration, workflows, pipelines, or templates.
- Do not publish or unpublish the website, or change DNS.
- Do not migrate or delete data.
- Do not send a real estimate or invoice, or test with a real customer.
- Do not place raw customer records, private contact information, order-level exports, credentials, technical schemas, or detailed pricing logic in the Company Brain or GitHub.
- Never display, copy, commit, or report secret credential values; environment-variable and integration **names** may be referenced.
- Do not treat the presence of integration code as proof that an integration is verified live.
- Do not expand the separate estimate app into a parallel estimating and invoicing system.
- Do not recommend a custom estimate app (Print Configurator) merely because one already exists; only if native HighLevel proves insufficient.
- Preserve the existing Knowledge Core / Pricing App source-of-truth boundary.

---

# Acceptance Criteria

Phase 2A is complete when the following have been reported:

1. Files changed and branches used
2. Sprint 2 decisions recorded
3. Credential exposure scope, without revealing secrets
4. Exact credential-rotation sequence
5. Current native HighLevel inventory (or confirmation that live access was unavailable)
6. HighLevel capability gaps
7. Estimate-app components worth reusing
8. Dynamic Supabase product-display architecture
9. Minimum Business Card pilot workflow
10. Exact action required to contain the unfinished public website
11. External changes requiring owner approval

---

# Current Recommended Next Action

Review the Phase 2A findings, approve or adjust the recommended credential-rotation sequence and website-containment action, and authorize Phase 2B implementation scope before any credential rotation, live HighLevel configuration change, website publish/unpublish, DNS change, data migration, or real estimate/invoice send.
