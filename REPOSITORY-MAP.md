# Repository Map

This file defines the intended structure of the Positive Printers Knowledge Core.

The repository should stay focused on business knowledge and should not duplicate the Positive Printers Pricing application.

---

# Root Files

## `README.md`

Defines the mission, source-of-truth rules, and operating principles for the Knowledge Core.

## `AI-BOOT.md`

Starting guide for AI assistants and future agents. Every new development session should begin by reading this file and the other foundational files.

## `PROJECT-STATUS.md`

Tracks the current state of the Knowledge Core, current priorities, and next recommended action.

## `REPOSITORY-MAP.md`

Defines the folder structure and purpose of each major area.

## `DEVELOPMENT-STANDARDS.md`

Defines how knowledge should be created, updated, normalized, and maintained.

## `DECISIONS.md`

Records durable architectural and business-system decisions.

---

# Sprint Management

## `20-Sprints/`

Tracks active and future development work.

### `20-Sprints/ACTIVE-SPRINT.md`

Defines the current sprint objective, scope, constraints, and acceptance criteria.

---

# Planned Business Knowledge Areas

These folders should be created only when needed. Do not create empty folders for decoration.

## `01-Company-Foundation/`

Purpose:

- Company positioning
- Brand identity
- Mission
- Values
- Voice
- Market focus
- Customer types

## `02-Products/`

Purpose:

- Product positioning
- Product use cases
- Customer-facing product explanations
- Cross-sells
- Upsells
- Product marketing notes

Important:

Do not duplicate pricing tables, product option records, or application product data from `positive-printers-pricing`.

## `03-Marketing/`

Purpose:

- Marketing angles
- Ad concepts
- Email concepts
- Website copy direction
- Seasonal promotions
- Local business campaigns

## `04-Sales/`

Purpose:

- Sales scripts
- Discovery questions
- Objection handling
- Offer presentation
- Proposal language

## `05-Industry-Packages/`

Purpose:

- Dentist packages
- Restaurant packages
- Contractor packages
- Chiropractor packages
- Real estate packages
- Local service business packages

## `06-Campaigns/`

Purpose:

- Product-specific campaigns
- Industry campaigns
- Seasonal campaigns
- AI + print campaign concepts

## `07-AI-Agents/`

Purpose:

- Agent instructions
- AI training material
- Prompt frameworks
- Business assistant behavior

## `99-Archive/`

Purpose:

- Deprecated knowledge
- Superseded drafts
- Historical notes

---

# Architecture Rule

Create new folders only when a real knowledge category is ready to be maintained.

Prefer fewer, stronger files over many thin files.

Extend existing files whenever possible.
