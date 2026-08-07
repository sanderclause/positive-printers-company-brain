# Project Status

## Project Name

Positive Printers Knowledge Core

## Current Status

Status: Foundation setup with technical source consolidation complete

The Knowledge Core repository has been created to serve as the business source of truth for Positive Printers.

This repository is separate from the Positive Printers Pricing application.

The current focus is establishing the initial repository architecture, development standards, and source-of-truth boundaries before adding product, marketing, sales, or campaign knowledge.

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

Sprint 0 — Repository Architecture & Business Knowledge Inventory

See:

`20-Sprints/ACTIVE-SPRINT.md`

---

# Current Priorities

1. Establish foundational repository files
2. Define source-of-truth boundaries
3. Map the initial repository structure
4. Identify what belongs in the Knowledge Core versus the Pricing App
5. Avoid duplicating product pricing, product option records, or technical logic
6. Prepare the repository for future business knowledge migration
7. Review and accept the consolidated technical repository before archiving older working copies

---

# Not Yet Started

- Company foundation migration
- Product positioning library
- Product marketing angles
- Industry packages
- Campaign library
- Sales scripts
- Proposal frameworks
- AI agent training material

---

# Next Recommended Action

Review the consolidated technical-repository boundary, then complete Sprint 0 by selecting the first business knowledge area for Sprint 1: Company Foundation, Product Positioning, or Industry Packages.
