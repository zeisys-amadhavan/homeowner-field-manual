# Front and Back Matter

This file owns the pages that sit outside the lettered parts of **The Homeowner's Field Manual**.

`toc.csv` owns the lettered parts. It does not currently contain front or back matter rows. Until it does, this file is the authority for what those pages are and what each must accomplish.

## Why these pages matter more here than in an ordinary book

Most books can treat front matter as a formality. This one cannot, for two reasons:

1. **The book has to teach the reader how to use it.** A reader who does not understand the spread structure, the page codes, or the fact that they are meant to write in it will use the book as a reference and never complete it.
2. **The book is shared with strangers.** A photographed page may reach a contractor, inspector, adjuster, or buyer who has never seen the book. The front matter is what makes that page legible to them.

## Required front matter

The following pages are required. Their order below is the intended reading order.

### Title page
Title, subtitle, author.

### Copyright and edition
Copyright, edition identifier, ISBN, printing information.

The edition identifier matters more than usual, because page codes are promised to be stable across editions and a reader comparing two copies needs to know which edition they hold.

### Limitations and safe use
The reader-facing statement of what the book is and is not: not a repair manual, not a code reference, not a substitute for qualified professional inspection or advice, and not specific to any one jurisdiction.

Content posture for this page is owned by `CONTENT_SCOPE_SAFETY.md`. This file owns only the fact that the page exists and where it sits.

Place it early. A limitations page buried in the back does not do its job.

### Contents
The part-level and page-level index.

Entries carry page codes as well as physical page numbers, so a reader can navigate by either.

### How to use this book
The single most important page in the front matter.

It must establish:

- that the book is meant to be written in;
- the spread structure — the right page explains, the left page records;
- that page codes are permanent identifiers, and how to read one;
- that forms should be dated;
- that filled pages should be photographed periodically, because the book is a single physical copy and the only copy of the data it holds;
- that a superseded entry is struck through and dated rather than erased.

### For your contractor
A page addressed to someone who is *not* the owner.

Its job is to let a professional who receives a photographed page understand the system in well under two minutes: what the book is, what a page code means, that the even page is the owner's record of their own house, and that the code in the corner identifies the page precisely.

This page is what makes the contractor protocol work at N=1. It should be written so it still makes sense in isolation, because in practice it will often be photographed and sent along with a form.

### Property identity
The first thing recorded, because everything else in the book describes this one property.

If this is implemented as a normal spread it belongs in `toc.csv` under Part `A` rather than here. Decide once and record it in whichever file owns it — not both.

## Required back matter

### Glossary
Homeowner-facing vocabulary and document terms.

A glossary of trades and terms currently exists as a spread inside Part `X`. If that spread is the glossary, this back-matter entry is redundant and should be dropped rather than duplicated. Resolve before layout.

### Page code index
An index of every page code with its subject and physical page number.

This is the lookup a contractor or a returning reader uses. It is distinct from the contents page: contents is ordered by the book, the index is ordered for lookup.

### Where your documents live
A single page recording where the source documents summarized throughout the book are physically or digitally stored.

The book holds standardized summaries, not the documents themselves. Without this page the summaries point nowhere.

### Continuation and replacement pages
The book's answer to running out of room: what the reader does when a log fills or a system is replaced.

Whether this is satisfied by additional blank forms bound into the back, or by some other means, is **not yet decided.** Do not assume a downloadable companion exists.

### Closing pages
About the author, and any series or edition information.

## Rules that apply to these pages

- Front and back matter follow `WRITING_RULES.md` and `VISUAL_DESIGN_RULES.md` like any other page.
- These pages do not carry part-letter page codes, since they belong to no part. If a coding scheme for them is later needed, define it in `PAGE_CODES.md`.
- Page parity still applies to the book as a whole: front matter must resolve to a page count that leaves every part opener and every form on the correct side. This is a hard layout constraint, not a preference.

## Still to be decided

- Whether front and back matter get rows in `toc.csv`, and if so under what part letter or role.
- Whether property identity is front matter or a Part `A` spread.
- Whether the glossary is back matter or the existing Part `X` spread.
- Final page count for front and back matter, which feeds the unlocked page-count and gutter decisions in `KDP_PRINT_SPEC.md`.
- Whether continuation forms are bound in, and how many.

## Source of truth

This file owns the inventory and purpose of front and back matter.

It does not own content posture (`CONTENT_SCOPE_SAFETY.md`), voice (`WRITING_RULES.md`), visual treatment (`VISUAL_DESIGN_RULES.md`), or the physical format (`KDP_PRINT_SPEC.md`).
