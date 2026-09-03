# Decision Log

This file records major durable project decisions, especially decisions that supersede older project directions.

Keep entries short. Detailed rules belong in their canonical files.

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

**Decision:** `toc.csv` is the sole canonical source for page codes, page subjects, tiers, spread goals, diagram content, form fields, base views, and artwork sources.

**Supersedes:** duplicated page plans in older concept documents.

**Reason:** Page definitions should not require synchronized edits in multiple files.

---

## 2026-09-02 — Trim size changed to 8 × 10

**Decision:** The KDP book is designed at **8 × 10 inches, portrait**.

**Supersedes:** all prior 5 × 8 production assumptions.

**Reason:** The recordkeeping forms and visual diagrams require more usable page area while the book should remain easier to handle than a large 8.5 × 11 reference manual.

---

## 2026-09-02 — Prompt assets belong under `prompts/`

**Decision:** Reusable prompts for external generation tools are stored in a `prompts/` subdirectory.

**Example:** `prompts/bw-diagram-prompt.md`

**Reason:** Prompts are frequently reusable operational assets and are distinct from canonical AI/project instruction files.
