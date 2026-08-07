# Decisions

This file records durable decisions for the Positive Printers Knowledge Core.

---

# Decision 001 — Separate Business Brain from Pricing App

## Decision

Positive Printers will use two separate GitHub repositories:

1. `positive-printers-company-brain`
2. `positive-printers-pricing`

## Rationale

The company brain and the software platform have different responsibilities.

The company brain should organize business knowledge, positioning, marketing, sales systems, industry packages, campaigns, and AI training.

The pricing app should remain the technical source of truth for pricing, product records, product options, database schema, Supabase, APIs, and application code.

## Impact

This prevents the Knowledge Core from becoming a duplicate pricing catalog or technical documentation mirror.

---

# Decision 002 — Knowledge Core Name

## Decision

The business repository will be referred to as:

Positive Printers Knowledge Core

## Rationale

This keeps the naming pattern consistent with PAiMOS Knowledge Core while making clear that this repository is the business source of truth.

---

# Decision 003 — No Duplicate Pricing Data

## Decision

The Knowledge Core will not store product pricing tables, product option records, or pricing calculations.

## Rationale

Pricing and product option data already belong in the Positive Printers Pricing application and database.

The Knowledge Core may reference the Pricing App but should not copy its data.

---

# Decision 004 — Business Knowledge First

## Decision

The Knowledge Core will prioritize business knowledge that helps Positive Printers sell, market, package, explain, and operationalize products.

## Rationale

The repository should make the business more consistent and scalable, not simply create documentation for documentation's sake.

---

# Decision 005 — Sprint 0 Before Knowledge Migration

## Decision

The first sprint is Repository Architecture & Business Knowledge Inventory.

## Rationale

Before importing or creating new knowledge, the repository needs clear structure, source-of-truth rules, and development standards.

---

# Decision 006 — One Canonical Technical Repository

## Decision

The GitHub repository `sanderclause/positive-printers-pricing` is the canonical technical source of truth for the Positive Printers pricing platform.

The consolidated application preserves two distinct surfaces in that repository:

1. `/` — customer-facing product selection and instant pricing
2. `/admin/*` — staff-only catalog, pricing, asset, and migration administration

GoHighLevel is the intended customer and job-operations platform, and related integration functionality exists in the consolidated application. Its current live operational status must be verified separately.

## Rationale

The technical work had diverged across separate Codex, Claude Code, Desktop, and Dropbox working copies while GitHub still contained only the initial scaffold.

One canonical technical repository prevents future version ambiguity while preserving the established boundary between the Knowledge Core and application implementation.

## Impact

- The Knowledge Core continues to own business strategy and normalized business knowledge.
- The pricing repository owns application code, pricing data, catalog records, Supabase implementation, imports, and integrations.
- Older working copies remain archives until the consolidated repository is reviewed and accepted.
- Raw inputs, credentials, reports, and private exports remain local-only and are not committed.


---

# Decision 007 — Sprint 1 Begins With Company Foundation

## Decision

Sprint 1 will establish the Positive Printers Company Foundation before building product positioning, industry packages, marketing systems, sales systems, campaigns, or AI-agent training.

## Rationale

Those downstream knowledge areas need a consistent understanding of the company, its market, customers, differentiators, capabilities, voice, and operating boundaries.

Starting with a read-only source inventory allows existing evidence to answer as much as possible before requesting owner validation.

## Impact

- Claude Code will be the primary implementation environment for Sprint 1.
- Codex may support architecture, review, source-of-truth decisions, and cross-repository verification.
- No Company Foundation content will be created until the source inventory and proposed structure receive human approval.

---

# Decision 008 — Sprint 2 Priorities: Website Launch and New Order Workflow

## Decision

Website launch and a new customer order workflow are the immediate priorities for Positive Printers.

GoHighLevel is the intended platform for the new customer order and job-operations workflow.

Zoho remains the fallback and reference system during validation of the new workflow.

No full migration of Zoho data or shutdown of Zoho is approved at this time.

## Rationale

The owner has approved Sprint 2 with the business objective of launching the Positive Printers website and beginning to take customer orders through a new GoHighLevel-based workflow as quickly and safely as possible, while avoiding a risky all-at-once migration.

A minimum viable order workflow, validated with realistic orders and owner approval, is safer than migrating every product, historical record, automation, or production stage before launch.

## Impact

- Sprint 2 begins with a read-only launch audit; no deployment, GoHighLevel configuration, database migration, DNS, or customer-facing change is authorized until the owner approves the resulting implementation plan.
- Zoho data must not be disabled, deleted, overwritten, or bulk-migrated during this phase.
- Reducing or ending reliance on Zoho requires explicit owner approval, conditioned on the new workflow being tested, fields mapped, staff able to manage requests, customer confirmations working, and no required information being lost.
- Raw customer records, private contact information, order-level exports, and credentials must not be placed in the Company Brain or GitHub; only aggregated and owner-approved findings may become durable Company Brain knowledge.
