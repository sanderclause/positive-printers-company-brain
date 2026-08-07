# Active Sprint

## Sprint 1 — Company Foundation

## Sprint Status

Active — source inventory phase

---

# Sprint Objective

Create the first normalized Company Foundation for Positive Printers using existing evidence rather than interviewing the owner from scratch.

The result should give future product, marketing, sales, campaign, proposal, and AI-agent work a consistent understanding of the company without duplicating pricing data or application implementation.

---

# Business Problem

Positive Printers business knowledge exists across project folders, documents, images, historical application work, and the owner's working knowledge.

Without a canonical Company Foundation, future agents may infer inconsistent positioning, invent unsupported claims, or repeatedly ask questions that existing materials can answer.

---

# Business System

Positive Printers Knowledge Core

---

# Capability

Normalized company identity, positioning, market focus, operating context, and evidence traceability.

---

# Existing Platforms and Sources

The source inventory may inspect these locations read-only:

- The Positive Printers Knowledge Core
- The canonical `positive-printers-pricing` repository
- `Product Specific Images`
- `Positive Printers File Organization`
- The pre-consolidation Pricing App archive
- The superseded Catalog Admin and Cost Consolidate folders
- Other clearly relevant Positive Printers business documents discovered in the Claude Code project structure

The Pricing App remains authoritative for prices, product records, database structure, Supabase logic, APIs, and technical implementation.

---

# Sprint Workflow

## Phase 1 — Read-only source inventory

Claude Code should:

1. Read all required governance files.
2. Inventory relevant source locations without moving, renaming, deleting, or rewriting files.
3. Identify candidate evidence for company identity, history, mission, values, positioning, markets, customer types, differentiators, capabilities, voice, and operating boundaries.
4. Separate confirmed facts from reasonable inferences and unresolved questions.
5. Identify duplicates, conflicts, stale material, and information that belongs in the Pricing App instead.
6. Report findings and propose the smallest canonical Company Foundation structure.
7. Stop for human approval before creating Company Foundation content.

## Phase 2 — Canonical Company Foundation

After approval, Claude Code should create or update the minimum number of files needed under `01-Company-Foundation/`.

Prefer one strong canonical file over several thin files. Every durable claim should be traceable to a source, an owner confirmation, or a clearly labeled assumption.

## Phase 3 — Validation and normalization

Claude Code should:

1. Check the Company Foundation against repository boundaries and decisions.
2. Remove duplication and unsupported claims.
3. Confirm that no pricing tables, product records, credentials, client-private data, or technical implementation were copied into the Knowledge Core.
4. Present unresolved questions as a short owner-validation list.
5. Update project status and the active sprint only after the approved content is complete.

---

# Constraints

- Do not interview the owner from scratch.
- Do not copy the Positive AI Marketing company brain and rename it.
- Reuse its governance and normalization discipline, not its company-specific content.
- Do not move or delete source material during the inventory.
- Do not duplicate Pricing App data or technical documentation.
- Do not treat filenames, folder placement, or old drafts as proof that a claim is current.
- Mark uncertain information as `needs_validation`.
- Preserve one concept in one canonical location.

---

# Acceptance Criteria

Sprint 1 is complete when:

1. A read-only source inventory has been reviewed and approved.
2. A canonical Company Foundation exists under `01-Company-Foundation/`.
3. Company identity, positioning, market focus, customer types, differentiators, capabilities, voice, and operating boundaries are covered or explicitly marked `needs_validation`.
4. Durable claims are traceable to evidence or owner confirmation.
5. No pricing or technical implementation has been duplicated.
6. Conflicts and unresolved questions are documented concisely.
7. `PROJECT-STATUS.md`, `DECISIONS.md`, and this sprint file accurately reflect completion.

---

# Current Recommended Next Action

Use Claude Code to complete Phase 1 as a read-only audit, present the source inventory and proposed Company Foundation structure, and stop for approval.
