# KDP Print Specification

This file owns the physical print-format decisions for **The Homeowner's Field Manual**.

## Locked decisions

- **Platform:** Amazon KDP
- **Format:** paperback
- **Orientation:** portrait
- **Trim size:** **8 × 10 inches**
- **Interior:** full color

The 8 × 10 trim supersedes all earlier 5 × 8 references.

## Design intent of the trim size

The book must provide enough room for:

- handwriting;
- practical form fields;
- tables and inventories;
- full-page explanatory diagrams;
- callouts and legends;
- comfortable two-page spread reading.

At the same time, it should remain substantially more manageable than a large 8.5 × 11 reference manual.

## Canonical layout assumption

All page and spread design work should be created for 8 × 10 portrait unless the author explicitly changes the trim size.

Do not scale layouts from old 5 × 8 concepts without redesigning them for the new proportions.

## Production values still to be locked

The following should be verified against current KDP requirements before final production and then recorded here:

- bleed / no-bleed choice;
- exact inside, outside, top, and bottom margins;
- gutter allowance by final page count;
- paper/interior color option;
- minimum line weights;
- image resolution and effective PPI;
- PDF export standard;
- spine calculation;
- cover dimensions;
- final page-count constraints;
- current print-cost assumptions.

Until these are explicitly locked, do not invent production numbers.

## Source-of-truth rule

Physical production specifications belong here.

Page-level content and page assignments belong in `toc.csv`.
