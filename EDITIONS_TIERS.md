# Editions and Tiers

## Current model

The canonical TOC classifies content into three depth tiers:

1. **Basic**
2. **Advanced**
3. **Professional**

The tier assigned to each spread is defined in `toc.csv`.

## Intended progression

### Basic
Helps a homeowner understand, identify, locate, document, and safely operate the ordinary house.

### Advanced
Adds deeper ownership, maintenance, planning, and system-management knowledge for a more engaged homeowner.

### Professional
Adds greater diagnostic, technical, project, or self-sufficiency depth where appropriate.

## Product-line principle

Higher tiers should build on lower tiers rather than force the core book to be rewritten into a different conceptual system.

The preferred long-term model is **append rather than rewrite** wherever feasible.

## Page-code permanence

Assigned page codes are permanent across tiers and editions.

- Existing Basic codes are never renumbered because Advanced or Professional content is added.
- New content receives new unused codes.
- A retired code remains reserved and is not reused for another concept.

See `PAGE_CODES.md` for the canonical coding rules.

## Important limitation

The precise commercial edition strategy, final page counts, and publication packaging are not yet locked in this file.

Do not infer that every tier must necessarily be released as a separate KDP product until the author explicitly confirms that decision.

## Commercial decisions are deliberately out of repository scope

Pricing, royalty assumptions, print-cost modeling, sales channels, bulk or gift-channel packaging, digital companion products, and any future series titles are **not recorded anywhere in this repository at this time.**

This is intentional, not an omission. Treat their absence as a deliberate boundary rather than a gap to be filled, and do not import figures from older project material, which is obsolete.

If a commercial constraint later needs to drive production work — a hard maximum page count being the likeliest case — record it in the canonical file that owns the affected production decision rather than creating a marketing document.

## Interaction with page count

Tier assignment determines how long each edition is, so tier decisions and the unlocked KDP page-count constraints in `KDP_PRINT_SPEC.md` are linked.

Current tier totals live in `toc.csv` and should be counted from it rather than quoted from memory, because they move whenever a tier is reassigned.

## Source of truth

The tier of each existing page/spread belongs exclusively in `toc.csv`.
