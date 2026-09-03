# Page and Spread Rules

## Fundamental unit

The fundamental design unit is the **two-page spread**, not the isolated page.

Each spread should make one subject understandable and recordable.

## Absolute left/right rule

- **Left page = even page = FORM**
- **Right page = odd page = GUIDE / DIAGRAM**

Forms always land on the left.

This rule is structural and should not be casually broken.

## Purpose of the pairing

The right page explains what the homeowner is looking at.

The left page records how that subject exists in the homeowner's own house.

The reader should be able to move naturally from:

**understand → inspect → record**

without searching elsewhere in the book.

## Spread goal

Every spread has a specific purpose recorded in the `Spread Goal` field of `toc.csv`.

Design, copy, form fields, and illustration should all serve that goal.

Do not add content merely because space is available.

## Flexibility

Some subjects may require:

- additional guide pages;
- additional forms;
- part opener treatment;
- composite/reference pages.

Any exception must preserve the overall page-parity system so later forms still land on even/left pages.

## Part openers

Each part opens with a spread coded `n00` / `n01`, where `n00` is the even / left page carrying the opener composite and `n01` is the odd / right page, left intentionally blank.

Opener rows are identified by `Part opener` in the `Role` column of `toc.csv`. All other rows are `Spread`.

The opener is the only permitted exception to the normal form-left / guide-right pairing.

An opener row may contain text in the `Form Page Fields` column. On a `Part opener` row, that column does **not** define a normal form page. It defines a small reader interaction embedded on `n00` — for example a checklist, mark-up task, or sketch prompt that works with the opener composite.

`n01` remains intentionally blank.

Do not independently invent opener page numbers or reorder pages outside `toc.csv`.

## Front and back matter

Pages outside the lettered parts — title, copyright, contents, how-to-use, the contractor explainer, index, and closing pages — are governed by `FRONT_BACK_MATTER.md`.

## Cross-spread references

When one spread depends on another, use permanent page codes rather than physical page numbers whenever possible.

## Source of truth

Specific form page, diagram page, page code, spread goal, content assignment, and opener interaction belong exclusively in `toc.csv`.
