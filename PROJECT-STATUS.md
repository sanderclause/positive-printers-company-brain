# Project Status

## Project Name

Positive Printers Knowledge Core

## Current Status

Status: Sprint 2 active — read-only launch audit

The Knowledge Core repository has been created to serve as the business source of truth for Positive Printers.

This repository is separate from the Positive Printers Pricing application.

Sprint 0 established the repository architecture, development standards, and source-of-truth boundaries. Sprint 1 built and merged the canonical Company Foundation (`01-Company-Foundation/Company-Foundation.md`), which is now on `main`. Sprint 2 is approved and underway: launching the Positive Printers website and a new GoHighLevel-based order workflow, beginning with a read-only launch audit.

The previously divergent Positive Printers application work has been consolidated into the canonical `positive-printers-pricing` repository. The consolidated technical source preserves the customer calculator, Catalog Admin, Supabase work, pricing data tools, and GoHighLevel integration boundaries without copying that implementation into the Knowledge Core.

---

# Current Business Objective

Create a normalized business knowledge system that helps Positive Printers:

- Organize product positioning
- Improve marketing consistency
- Build industry-specific offers
- Support sales and proposal generation
- Train AI agents
- Connect print products with Positive AI Marketing offers
- Avoid duplicating pricing application data

---

# Related Repositories

## Business Source of Truth

`positive-printers-company-brain`

Purpose:

- Strategy
- Positioning
- Marketing
- Sales systems
- Industry packages
- AI training
- Business processes

## Technical Source of Truth

`positive-printers-pricing`

Purpose:

- Pricing engine
- Product records
- Product options
- Database schema
- Supabase implementation
- APIs
- Next.js application
- Admin tools

Current consolidation review:

- GitHub draft PR: `sanderclause/positive-printers-pricing#1`
- Customer calculator: `/`
- Staff catalog administration: `/admin/*`
- Local raw inputs and private exports: ignored technical-repository material, not Knowledge Core content

---

# Current Sprint

Sprint 2 — Website Launch and New Order Workflow

See:

`20-Sprints/ACTIVE-SPRINT.md`

---

# Current Priorities

1. Complete the Sprint 2 read-only launch audit across the Company Brain, Pricing App, GoHighLevel integration code, and Zoho workflow/migration utilities
2. Determine the canonical customer-facing website and its current deployment status
3. Distinguish GoHighLevel functionality that is implemented in code from functionality verified live in the account
4. Use post-2020 order data to recommend an initial product launch set, without placing raw customer records in the Company Brain or GitHub
5. Present the minimum viable order workflow, Zoho-to-GoHighLevel mapping, and pilot test plan for owner approval
6. Archive older working copies once the consolidated technical repository is fully accepted

Sprint 1 deliverables (complete and merged): read-only source inventory, owner validation, and a canonical Company Foundation created and approved without duplicating the Pricing App.

---

# Not Yet Started

- Product positioning library
- Product marketing angles
- Industry packages
- Campaign library
- Sales scripts
- Proposal frameworks
- AI agent training material

---

# Next Recommended Action

Complete the Sprint 2 Phase 1 read-only launch audit, present the categorized findings and implementation plan, and stop for owner approval before any deployment, GoHighLevel configuration, database migration, DNS, or customer-facing change.
