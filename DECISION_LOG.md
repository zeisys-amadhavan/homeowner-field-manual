# Decision Log

This file records major durable project decisions, especially decisions that supersede older project directions.

Keep entries short. Detailed rules belong in their canonical files.

---

## 2026-09-02 — Assigned page codes are permanent

**Decision:** Once a page code is assigned in `toc.csv`, it is permanent across tiers and editions. It is never renumbered, repurposed, or reused. A retired code remains reserved.

**Reason:** Page codes are the stable cross-reference language for homeowners, contractors, artwork, and future editions.

---

## 2026-09-02 — Page codes are part letter + zero-padded sequence

**Decision:** The page-code rule is **part letter + zero-padded sequence**, normally two digits, continuing to three where a part runs past 99.

**Supersedes:** the "two-digit sequence" wording in `PAGE_CODES.md`.

**Reason:** Parts C and F already contain `C100`, `C101`, `F100`–`F103`. Widening the rule preserves existing codes; renumbering would have violated code permanence for cosmetic reasons.

---

## 2026-09-02 — "Part" replaces "section" as the structural term

**Decision:** The book's lettered top-level divisions are **parts**. *Section* is retired for this concept.

**Reason:** `toc.csv` uses Part / Part Name. One term, matching the canonical database, avoids conflicting structural language.

---

## 2026-09-02 — Part X (Extension) defined

**Decision:** Part `X`, **Extension**, is the part holding cross-system rollups, seasonal checklists, and general reference — material belonging to the property as a whole rather than to any single system. Its rollup pages summarize facts owned by system spreads; they do not replace them.

**Reason:** Part `X` existed in `toc.csv` with no definition in any Markdown file, leaving AI tools no basis for deciding what belongs there.

---

## 2026-09-02 — Front and back matter get a canonical owner

**Decision:** `FRONT_BACK_MATTER.md` owns all pages outside the lettered parts.

**Reason:** Title, copyright, limitations, contents, how-to-use, the contractor explainer, index, and closing pages need one explicit owner because `toc.csv` currently contains no front/back-matter rows.

---

## 2026-09-02 — TOC gains a Role column; opener codes normalized

**Decision:** `toc.csv` gains a **Role** column, positioned after `Part Name`, with values `Spread` and `Part opener`. Opener rows carry clean codes `n00` and `n01` in the existing two code columns.

**Supersedes:** the free-text value `00 (opener spread, 01 blank)` previously stored in the `Form Page (even, left)` column on ten rows.

**Reason:** Free text in a code column defeated machine parsing of every page code.

---

## 2026-09-02 — Annotation blue holds; per-system color deferred

**Decision:** Bright blue remains reserved for annotation. No system may be assigned blue, and no per-system palette is introduced on individual pages before a book-wide decision.

**Reason:** A subject-color scheme that colored water blue would collide with the annotation standard and make labels ambiguous.

---

## 2026-09-02 — Commercial decisions excluded from the repository

**Decision:** Pricing, royalties, print-cost modeling, channels, gift or bulk packaging, digital companion products, and series plans are deliberately not recorded in this repository.

**Reason:** Their absence was being read as a gap. It is a boundary. Figures in older material are obsolete and must not be imported.

---

## 2026-09-02 — RENAME.md marked superseded in place

**Decision:** `RENAME.md` keeps its filename and location but opens with a banner listing which specifications are obsolete.

**Reason:** Its strategic reasoning remains useful, but its old trim size, form IDs, page plan, page counts, and commercial figures are not current authority.

---

## 2026-09-02 — Repository becomes modular AI knowledge base

**Decision:** `Instructions_for_AI_Tools.md` is the master entry point for AI tools. Project knowledge is divided into small authoritative modules with minimal duplication.

**Reason:** AI tools should be able to work from the repository without the author repeatedly restating project context.

---

## 2026-09-02 — Flat repository structure preferred

**Decision:** Canonical project Markdown files should remain in the repository root unless a category genuinely benefits from a subdirectory.

**Reason:** Human browsing and updating are easier when core knowledge files remain visible together.

---

## 2026-09-02 — TOC owns page-level definitions

**Decision:** `toc.csv` is the sole canonical source for page codes, page subjects, tiers, spread goals, diagram content, page-specific form fields, base views, and artwork sources.

**Supersedes:** duplicated page plans in older concept documents.

**Reason:** Page definitions should not require synchronized edits in multiple files.

---

## 2026-09-02 — Trim size changed to 8 × 10

**Decision:** The KDP book is designed at **8 × 10 inches, portrait**.

**Supersedes:** all prior 5 × 8 production assumptions.

**Reason:** The recordkeeping forms and visual diagrams require more usable page area while the book should remain easier to handle than a large 8.5 × 11 reference manual.

---

## 2026-09-02 — Prompt assets belong under `prompts/`

**Decision:** Reusable prompts for external generation tools are stored in the lowercase `prompts/` subdirectory.

**Example:** `prompts/bw-diagram-prompt.md`

**Reason:** Prompts are frequently reusable operational assets and are distinct from canonical AI/project instruction files.
