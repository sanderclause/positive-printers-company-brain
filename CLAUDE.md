# Claude Code Entry Point

Before working in this repository, read these files in order:

1. `README.md`
2. `AI-BOOT.md`
3. `PROJECT-STATUS.md`
4. `REPOSITORY-MAP.md`
5. `DEVELOPMENT-STANDARDS.md`
6. `DECISIONS.md`
7. `20-Sprints/ACTIVE-SPRINT.md`

Follow the active sprint exactly.

## Source-of-truth boundary

This repository owns normalized Positive Printers business knowledge.

The separate `positive-printers-pricing` repository owns prices, product records, product options, database schema, Supabase logic, APIs, imports, integrations, and application implementation.

Reference technical sources when useful; do not copy their technical data into this repository.

## Working rules

- Inspect before creating.
- Prefer extending a canonical file over creating a duplicate.
- Use evidence before recommendation.
- Label assumptions and unresolved claims `needs_validation`.
- Do not move, rename, delete, or reorganize source folders unless the user explicitly approves that action.
- Do not place credentials, client-private data, or raw exports in this repository.
- End each work session with changes made, decisions made, files needing updates, and the next recommended action.

## Current Sprint 1 status

Sprint 1 Company Foundation work is complete and awaiting pull-request review.

Do not repeat the source inventory or recreate `Company-Foundation.md`. Preserve the approved Company Foundation unless the owner requests a revision.

The likely next project is a post-2020 customer and product opportunity analysis, but Sprint 2 has not yet been formally approved.
