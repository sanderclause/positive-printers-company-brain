# AI Boot Guide

Use this file at the start of every Positive Printers Knowledge Core session.

This repository is the business brain for Positive Printers. It is designed to help AI assistants, ChatGPT Projects, Claude Code, and future agents understand how to work on Positive Printers business knowledge without duplicating the Positive Printers Pricing application.

---

# Required Starting Context

Before making recommendations, read these files first:

1. `README.md`
2. `AI-BOOT.md`
3. `PROJECT-STATUS.md`
4. `REPOSITORY-MAP.md`
5. `DEVELOPMENT-STANDARDS.md`
6. `DECISIONS.md`
7. `20-Sprints/ACTIVE-SPRINT.md`

After reading them, summarize:

- Current project status
- Active sprint
- Repository structure
- Source-of-truth boundaries
- Next recommended action

---

# Primary Rule

Do not interview the user from scratch.

This project should evolve from existing business knowledge, existing product knowledge, and the existing Positive Printers Pricing application.

When information is missing, make a reasonable assumption, label it clearly, and recommend the smallest next step needed to verify it.

---

# Source-of-Truth Boundaries

## Knowledge Core owns

- Company foundation
- Business strategy
- Product positioning
- Product use cases
- Marketing systems
- Sales systems
- Industry packages
- Campaign concepts
- AI agent training
- Business processes
- Presentation frameworks
- Proposal frameworks

## Pricing App owns

Repository: `positive-printers-pricing`

- Prices
- Product options
- Product catalog records
- Database schema
- Supabase logic
- API routes
- Next.js implementation
- Pricing calculations
- Technical workflows

---

# Required Reasoning Order

Always reason in this order:

Business Problem
→ Business System
→ Capability
→ Existing Platform
→ Business Knowledge
→ Solution

---

# Working Style

Think like a software architect, not a documentation writer.

Normalize knowledge.

Avoid duplicate concepts.

Prefer extending existing files over creating new files.

Before recommending a new file or folder, inspect the repository map and explain why the existing structure is insufficient.

---

# Session Wrap-Up Requirement

At the end of every development session, provide:

1. What changed
2. Decisions made
3. Repository files that should be updated
4. Exact markdown to paste into those files when updates are needed
5. Next recommended action
