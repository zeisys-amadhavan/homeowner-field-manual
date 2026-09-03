# Page Codes

## Purpose

Page codes are the permanent cross-reference language of **The Homeowner's Field Manual**.

They allow homeowners, AI tools, diagrams, forms, contractors, and future editions to refer to a page without depending on changing physical pagination.

## Current convention

A page code is:

**part letter + zero-padded sequence number**

The sequence is normally two digits. Where a part runs past 99 it continues at three digits without changing the rule.

Examples:

- `A02`
- `E04`
- `F18`
- `C100`
- `F102`

Part letters and page assignments are defined in `toc.csv`.

## Parity

The sequence number carries the page parity:

- **even number = left page = form**
- **odd number = right page = guide / diagram**

A normal form and its paired guide are always `n` and `n+1`.

The only exception is the part opener, described below.

## Part openers

Each part begins with an opener spread coded `n00` / `n01`.

- `n00` is the even / left page and carries the opener composite.
- `n01` is the odd / right page and is intentionally blank.

Opener rows are marked `Part opener` in the `Role` column of `toc.csv`.

On those rows:

- the `Diagram Page Content` column describes the primary artwork on `n00`;
- the `Form Page Fields` column, when populated, describes a small reader interaction embedded on `n00`, not a normal form;
- `n01` remains blank.

## Permanence

Once a page code is assigned in `toc.csv`, it is **permanent**.

- Do not renumber an assigned code.
- Do not shift existing codes merely to make room for new content.
- Do not reuse a retired code for a different concept.
- If a page is retired, its code remains reserved.
- The rule applies across editions and tiers.

New content receives a new unused code.

## Printed cross-references

When one page depends on another, the reference is printed as the bare page code.

Conventions:

- A guide page may direct the reader to its own form: *Record this on E04.*
- A form may point to a related form or log with a short **See also** line at the foot of the page.
- A form should carry at most a small number of cross-references. If a form needs many, the spread goal is probably too broad.
- Never print a physical page number inside a cross-reference, because pagination can change while page codes do not.

## Contractor protocol

The code system allows a homeowner to share a photographed page and identify it precisely.

Example concept:

> "Use E05 to locate each labeled item."

or

> "Use this diagram to complete E04."

The exact wording is page-specific and should be written only when needed.

## Obsolete conventions

Earlier project material used subject-prefix form identifiers such as `E-1`, `ID-3`, `PR-4`, or `NX-1`. That system is **superseded**.

Do not revive it, and do not treat it as an alias for the current codes.

## Editions

Assigned codes remain permanent across editions.

Higher tiers or later editions may add new codes, but they do not renumber, recycle, or repurpose existing codes.

Rules governing Basic, Advanced, and Professional content belong in `EDITIONS_TIERS.md`.

## Source of truth

`toc.csv` owns:

- every active code;
- the page subject associated with it;
- its role;
- its tier;
- its form/diagram pairing.

This file defines the coding rules.
