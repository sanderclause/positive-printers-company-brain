# Project Status

## Project Name

Positive Printers Knowledge Core

## Current Status

Status: Sprint 1 active — Company Foundation source inventory

The Knowledge Core repository has been created to serve as the business source of truth for Positive Printers.

This repository is separate from the Positive Printers Pricing application.

Sprint 0 established the repository architecture, development standards, and source-of-truth boundaries. Sprint 1 now focuses on building the Company Foundation from existing evidence.

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

Sprint 1 — Company Foundation

See:

`20-Sprints/ACTIVE-SPRINT.md`

---

# Current Priorities

1. Complete a read-only inventory of existing Positive Printers business sources
2. Identify evidence for company identity, positioning, markets, customer types, differentiators, capabilities, and voice
3. Separate confirmed facts, inferences, conflicts, and `needs_validation` items
4. Approve the smallest canonical Company Foundation structure
5. Create normalized Company Foundation content without duplicating the Pricing App
6. Review and accept the consolidated technical repository before archiving older working copies

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

Use Claude Code to complete Sprint 1 Phase 1 as a read-only source inventory. Review its findings and proposed Company Foundation structure before authorizing content creation.
