# Page Codes

## Purpose

Page codes are the permanent cross-reference language of **The Homeowner's Field Manual**.

They allow homeowners, AI tools, diagrams, forms, contractors, and future editions to refer to a page without depending on changing physical pagination.

## Current convention

The current TOC uses:

**section letter + two-digit sequence**

Examples:

- `A02`
- `E04`
- `E05`
- `F18`

Section letters and page assignments are defined in `toc.csv`.

## Rules

1. A page code identifies one stable page concept.
2. Do not renumber codes casually to make a sequence aesthetically cleaner.
3. Cross-references should prefer page codes over raw physical page numbers.
4. Form and guide pages keep their own codes.
5. When a code is shown on the printed page, it should be easy to find in a photograph.
6. AI tools must inspect the current `toc.csv` before stating what a code means.

## Contractor protocol

The code system allows a homeowner to share a photographed page and identify it precisely.

Example concept:

> “Use E05 to locate each labeled item.”

or

> “Use this diagram to complete E04.”

The exact wording is page-specific and should be written only when needed.

## Editions

The long-term objective is for codes to remain stable across editions whenever practical.

Rules governing Basic, Advanced, and Professional content belong in `EDITIONS_TIERS.md`.

## Source of truth

`toc.csv` owns:

- every active code;
- the page subject associated with it;
- its tier;
- its form/diagram pairing.

This file defines only the coding rules.
