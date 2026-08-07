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
