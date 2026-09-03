# Production Workflow

## Purpose

This workflow keeps page development consistent and prevents project knowledge from being duplicated.

## 1. Start with the TOC

Every page/spread begins with its current row in `toc.csv`.

Confirm:

- part;
- role (`Spread` or `Part opener`);
- form-page code;
- diagram-page code;
- tier;
- item;
- spread goal;
- diagram-page content;
- form fields;
- base view;
- artwork source.

Do not begin from memory when a TOC row exists.

## 2. Define the page outcome

Restate the spread goal in practical terms:

> What should the homeowner understand, inspect, and record after using these two pages?

Everything else should serve this outcome.

## 3. Build the form logic

Review the form fields already specified in `toc.csv`.

Challenge fields that are:

- unlikely to be useful later;
- impossible for an ordinary homeowner to identify;
- duplicated elsewhere;
- too large for realistic handwriting;
- better stored as a source document rather than summarized.

Any page-specific field change should be made in `toc.csv`.

## 4. Build the guide logic

Determine the minimum visual explanation needed for the homeowner to complete the form correctly.

Prefer diagram-first communication.

Write only the supporting text the visual cannot efficiently carry.

## 5. Apply canonical rules

Before finalizing, check the relevant modules:

- `PAGE_SPREAD_RULES.md`
- `WRITING_RULES.md`
- `VISUAL_DESIGN_RULES.md`
- `DIAGRAM_RULES.md`
- `FORM_RULES.md`
- `CONTENT_SCOPE_SAFETY.md`
- `FRONT_BACK_MATTER.md` (only when working on pages outside the lettered parts)

Read only what is relevant to the current task.

## 6. Create or source artwork

Use the artwork approach specified in `toc.csv`.

Reusable external-generation prompts belong under `prompts/`.

Prompts are tools, not project authority.

## 7. Layout review

Review the spread at 8 × 10 size for:

- hierarchy;
- handwriting room;
- label legibility;
- balance between visual and text;
- parity: form left, guide right;
- page-code visibility;
- cross-reference accuracy;
- safety boundaries.

## 8. Content review

Ask:

- Does the guide pass the Aha Test?
- Does the form pass the Spec Sheet Test?
- Can a normal homeowner identify every requested field?
- Is anything duplicated unnecessarily?
- Is the page trying to become a repair manual?
- Would the spread still make sense years later?

## 9. Update project knowledge

If page content changes, update `toc.csv`.

If a durable global rule changes, update the single canonical Markdown file that owns that rule.

If a major prior decision is superseded, add a short entry to `DECISION_LOG.md`.

Do not copy the same change into multiple files.
