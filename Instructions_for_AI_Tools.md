# Instructions for AI Tools

This file is the master instruction file for **The Homeowner's Field Manual** repository.

Its purpose is to let ChatGPT, Claude, Codex, and other AI tools work on the book consistently without requiring the author to restate the project structure, design rules, writing rules, production constraints, and prior decisions in every conversation.

## 1. Required first step

Before doing substantive work on this project:

1. Connect to this GitHub repository: `zeisys-amadhavan/homeowner-field-manual`.
2. Read this file.
3. Identify the latest commit on the branch being used.
4. Read only the additional authoritative files relevant to the current task.

The first response in each new project chat should begin with:

> I am giving this response based on commit `[commit]`, into git repo on `[DD.MM.YYYY]` at `[hh.mm.ss EST]`.

Do not claim repository access unless it has actually been verified.

## 2. Repository philosophy

This repository is a **modular source of truth for AI-assisted book production**.

Keep information in the smallest sensible authoritative file. Avoid duplicating the same rule or fact across multiple files. A change should normally require editing **one source of truth**, not many copies of the same information.

Keep files in the repository root unless a category genuinely requires many frequently updated files.

Do not reorganize, rename, merge, split, or move the canonical files without explicit author approval. Stable filenames matter because AI tools are instructed to locate project knowledge through them.

## 3. Authority hierarchy

When sources conflict, use this order:

1. The author's explicit instruction in the current conversation.
2. `Instructions_for_AI_Tools.md` for repository behavior and authority rules.
3. `toc.csv` for the current page-by-page structure of the book.
4. The dedicated canonical Markdown file for the subject being discussed.
5. `DECISION_LOG.md` for the history and rationale of major decisions.
6. Older or superseded project material only as historical context.

Never silently revive an obsolete specification because it appears in an older document.

## 4. Canonical files

The intended root-level knowledge structure is:

- `README.md` — short human-readable explanation of the repository.
- `Instructions_for_AI_Tools.md` — this master file.
- `toc.csv` — canonical page-by-page book structure and page assignments.
- `PROJECT_DEFINITION.md` — what the book is, who it is for, its objectives, positioning, and non-goals.
- `KDP_PRINT_SPEC.md` — physical format and Amazon KDP production constraints.
- `PAGE_SPREAD_RULES.md` — page pairing, left/right page logic, opener rules, and spread behavior.
- `WRITING_RULES.md` — voice, reading level, brevity, instructional method, and text standards.
- `VISUAL_DESIGN_RULES.md` — typography, hierarchy, page chrome, color system, spacing, and visual consistency.
- `DIAGRAM_RULES.md` — illustration and diagram conventions.
- `FORM_RULES.md` — rules for homeowner-fillable forms and record pages.
- `PAGE_CODES.md` — permanent page-code and cross-reference conventions.
- `EDITIONS_TIERS.md` — Basic, Advanced, and Professional edition/tier rules.
- `CONTENT_SCOPE_SAFETY.md` — content boundaries, safe-DIY limits, professional handoff, and national applicability.
- `TERMINOLOGY.md` — canonical vocabulary and naming conventions.
- `PRODUCTION_WORKFLOW.md` — workflow from TOC entry through writing, diagrams, forms, review, layout, and print.
- `DECISION_LOG.md` — dated record of major project decisions and superseded choices.

Do not create separate section files merely to restate content already defined in `toc.csv`. Page-level scope belongs in `toc.csv` unless the author explicitly decides otherwise.

## 5. Single-source rule

Each category of information must have one authoritative home.

Examples:

- Page name, code, tier, spread goal, diagram content, form fields, and artwork source → `toc.csv`.
- Trim size, bleed, margins, print assumptions → `KDP_PRINT_SPEC.md`.
- Writing tone and wording constraints → `WRITING_RULES.md`.
- Diagram aesthetics and annotation conventions → `DIAGRAM_RULES.md`.

Other files may point to the authoritative source, but should not duplicate its detailed contents.

## 6. Current hard constraints

Until superseded by an explicit author decision and recorded in the appropriate canonical file:

- The book is **The Homeowner's Field Manual**.
- Production target is **Amazon KDP**.
- Current trim size is **8 × 10 inches, portrait**.
- `toc.csv` is the authoritative current structure of the book.
- Older references to **5 × 8 inches** are obsolete.

## 7. Working with the TOC

Treat `toc.csv` as a database, not as prose documentation.

Do not manually reproduce its full contents in Markdown files. When a page changes, update the corresponding TOC row rather than creating another independent page description elsewhere.

When answering questions about book structure, page codes, page order, tiers, form fields, diagram content, or spread goals, inspect the current `toc.csv` rather than relying on memory.

## 8. Changes and decisions

When the author makes a durable project decision:

1. Determine the single canonical file that owns that decision.
2. Update that file.
3. If the decision materially supersedes an earlier direction, add a short dated entry to `DECISION_LOG.md`.
4. Do not update unrelated files merely to repeat the same decision.

If no existing canonical file is appropriate, recommend a new small module before creating one.

## 9. Historical material

Documents such as the former `RENAME.md` and imported project briefs may contain valuable reasoning but can also contain obsolete specifications.

Use historical material to recover intent and rationale, not as current authority when it conflicts with the hierarchy above.

## 10. Response discipline

For routine project conversation, default to concise responses under 50 words unless the author explicitly asks for more detail, analysis, a draft, a table, or a file.

When uncertain, inspect the repository rather than guessing. If two authoritative sources genuinely conflict, identify the conflict instead of silently choosing one.
