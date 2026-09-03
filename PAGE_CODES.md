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

A form and its paired guide are always `n` and `n+1`.

The only exception is the part opener, described below.

## Part openers

Each part begins with an opener spread coded `n00` / `n01`.

- `n00` is the even / left page and carries the opener composite.
- `n01` is the odd / right page and is intentionally blank.

Opener rows are marked `Part opener` in the `Role` column of `toc.csv`. On those rows the `Diagram Page Content` column describes the artwork on `n00`.

## Rules

1. A page code identifies one stable page concept.
2. Do not renumber codes casually to make a sequence aesthetically cleaner.
3. Cross-references should prefer page codes over raw physical page numbers.
4. Form and guide pages keep their own codes.
5. When a code is shown on the printed page, it should be easy to find in a photograph.
6. AI tools must inspect the current `toc.csv` before stating what a code means.

## Printed cross-references

When one page depends on another, the reference is printed as the bare page code.

Conventions:

- A guide page may direct the reader to its own form: *Record this on E04.*
- A form may point to a related form or log with a short **See also** line at the foot of the page.
- A form should carry at most a small number of cross-references. If a form needs many, the spread goal is probably too broad.
- Never print a physical page number inside a cross-reference, because pagination changes between editions and codes do not.

## Contractor protocol

The code system allows a homeowner to share a photographed page and identify it precisely.

Example concept:

> "Use E05 to locate each labeled item."

or

> "Use this diagram to complete E04."

The exact wording is page-specific and should be written only when needed.

## Obsolete conventions

Earlier project material used subject-prefix form identifiers such as `E-1`, `ID-3`, `PR-4`, or `NX-1`. That system is **superseded**. Do not revive it, and do not treat it as an alias for the current codes.

## Editions

The long-term objective is for codes to remain stable across editions whenever practical.

Rules governing Basic, Advanced, and Professional content belong in `EDITIONS_TIERS.md`.

## Source of truth

`toc.csv` owns:

- every active code;
- the page subject associated with it;
- its role;
- its tier;
- its form/diagram pairing.

This file defines only the coding rules.
