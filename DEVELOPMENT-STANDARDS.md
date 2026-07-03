# Development Standards

These standards govern how the Positive Printers Knowledge Core should be developed and maintained.

---

# Core Standard

The Knowledge Core should improve business clarity without duplicating the Positive Printers Pricing application.

Before adding knowledge, determine whether the information belongs in:

1. The Knowledge Core
2. The Pricing App
3. The database
4. The product catalog
5. A shared framework

---

# Source-of-Truth Standards

## Business knowledge belongs here

Examples:

- Positioning
- Messaging
- Industry use cases
- Sales scripts
- Campaign ideas
- AI agent training
- Proposal language
- Presentation structure
- Business processes

## Technical and pricing knowledge belongs in the Pricing App

Examples:

- Prices
- Product records
- Product options
- Database tables
- API routes
- Supabase policies
- Next.js implementation
- Import scripts
- Pricing calculations

---

# Knowledge Normalization Standards

Use one concept in one place.

Do not create duplicate versions of the same idea across multiple files.

When two files need the same information, one file should own the concept and the other should reference it.

---

# File Creation Standards

Before creating a new file, answer:

1. Does an existing file already own this concept?
2. Is this a durable knowledge category?
3. Will this file be maintained over time?
4. Is this business knowledge rather than technical implementation?
5. Does this avoid duplicating the Pricing App?

If the answer is unclear, extend an existing file first.

---

# Writing Standards

Use clear markdown.

Prefer direct language.

Use headings that reflect business systems and capabilities.

Avoid vague documentation.

Every file should make the business easier to operate, sell, market, or train.

---

# Reasoning Standard

Always reason in this order:

Business Problem
→ Business System
→ Capability
→ Existing Platform
→ Business Knowledge
→ Solution

---

# Session Wrap-Up Standard

Every development session should end with:

1. What changed
2. Decisions made
3. Repository files that should be updated
4. Exact markdown to paste into those files when updates are needed
5. Next recommended action

---

# Change Control

Durable architecture decisions belong in `DECISIONS.md`.

Current progress belongs in `PROJECT-STATUS.md`.

Current work belongs in `20-Sprints/ACTIVE-SPRINT.md`.

Repository structure belongs in `REPOSITORY-MAP.md`.
