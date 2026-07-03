# Positive Printers Knowledge Core

This repository is the business knowledge layer for Positive Printers.

It is the authoritative source of truth for business strategy, product positioning, marketing systems, sales systems, campaigns, industry solutions, AI agent training, and operational knowledge.

The Positive Printers Pricing application is the authoritative source of truth for application behavior, pricing, product records, and technical implementation.

---

# Mission

Build a business knowledge system that helps Positive Printers:

- Sell more effectively
- Market products consistently
- Create industry-specific solutions
- Train AI agents
- Support presentations and proposals
- Develop repeatable business systems
- Extend the pricing application without duplicating it

---

# Source of Truth

## This repository owns

- Company Foundation
- Business Strategy
- Product Positioning
- Marketing Systems
- Sales Systems
- Industry Packages
- Campaign Planning
- AI Agent Training
- Business Processes
- Proposal Frameworks
- Presentation Frameworks

## The Pricing Application owns

Repository:

`positive-printers-pricing`

Including:

- Product pricing
- Product options
- Product catalog records
- Database schema
- Supabase
- APIs
- Next.js application
- Technical implementation
- Pricing calculations
- Import processes

---

# Development Principles

Always inspect existing knowledge before creating new knowledge.

Prefer extending existing documentation over creating duplicate documentation.

Prefer referencing the pricing application instead of copying technical information.

Business knowledge belongs here.

Technical implementation belongs in the pricing application.

---

# Reasoning Order

Always reason in this order:

Business Problem
→ Business System
→ Capability
→ Existing Platform
→ Business Knowledge
→ Solution

---

# Operating Rule

Before adding new knowledge, determine whether the information already exists in:

- the pricing application
- the database
- the product catalog
- the application code

If it already exists there, reference it rather than duplicate it.

This repository explains **why**, **when**, and **how** Positive Printers sells and markets its products.

The pricing application explains **how the software works**.
