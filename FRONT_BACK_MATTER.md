# Front and Back Matter

This file owns the pages that sit outside the lettered parts of **The Homeowner's Field Manual**.

`toc.csv` owns the lettered parts. It does not currently contain front or back matter rows. Until that changes, this file is the authority for the working front/back-matter inventory and the purpose of each page.

## Why these pages matter more here than in an ordinary book

Most books can treat front matter as a formality. This one cannot, for two reasons:

1. **The book has to teach the reader how to use it.** A reader who does not understand the spread structure, page codes, or the fact that they are meant to write in it will use the book as a reference and never complete it.
2. **The book is shared with strangers.** A photographed page may reach a contractor, inspector, adjuster, or buyer who has never seen the book. The front matter makes that page legible to them.

## Current front-matter plan

The following pages are part of the current working plan. Their exact physical pagination is not yet locked.

### Title page
Title, subtitle, author.

### Copyright and edition
Copyright, edition identifier, ISBN, printing information.

The edition identifier matters more than usual because page codes are permanent across editions and a reader comparing two copies needs to know which edition they hold.

### Limitations and safe use
The reader-facing statement of what the book is and is not: not a repair manual, not a code reference, not a substitute for qualified professional inspection or advice, and not specific to any one jurisdiction.

Content posture for this page is owned by `CONTENT_SCOPE_SAFETY.md`.

Place it early. A limitations page buried in the back does not do its job.

### Contents
The part-level and page-level contents.

Entries should carry page codes as well as physical page numbers so a reader can navigate by either.

### How to use this book
The most important instructional page in the front matter.

It should establish:

- that the book is meant to be written in;
- the spread structure — the right page explains, the left page records;
- that page codes are permanent identifiers and how to read one;
- that normal forms carry a `Last updated` date;
- that filled pages should be photographed periodically because the book is a single physical copy;
- that a superseded entry is struck through and dated rather than erased.

### For your contractor
A page addressed to someone who is *not* the owner.

Its job is to let a professional who receives a photographed page understand the system quickly: what the book is, what a page code means, that the even page is the owner's record of their own house, and that the code in the corner identifies the page precisely.

It should still make sense in isolation because it may itself be photographed and shared.

## Front-matter placement still open

### Property identity
The first property-specific record should identify the house to which the entire manual belongs.

It is **not yet decided** whether Property Identity belongs in front matter or as a normal Part `A` spread.

Once decided, record it in exactly one authoritative place. Do not duplicate it here and in `toc.csv`.

## Current back-matter plan

### Page code index
A lookup of page codes with their subjects and physical page numbers.

This is distinct from the contents page: contents follows book order; the index is optimized for lookup.

### Where your documents live
A single reference page recording where the source documents summarized throughout the book are physically or digitally stored.

The book holds standardized summaries, not the documents themselves.

### Closing pages
About the author and any edition information that belongs at the end of the book.

## Back-matter items still open

### Continuation and replacement pages
The book needs a defined method for what happens when a log fills or a system is replaced.

Whether that means bound continuation forms, another printed mechanism, or something else is **not yet decided**.

Do not assume a downloadable companion exists.

### Glossary placement
A glossary already exists in the canonical TOC as Part `X`, spread `X24` / `X25`.

Therefore, **do not add a second glossary to back matter** unless the author explicitly decides to move or duplicate that function and updates `toc.csv` accordingly.

## Rules that apply to these pages

- Front and back matter follow `WRITING_RULES.md` and `VISUAL_DESIGN_RULES.md`.
- These pages currently do not carry part-letter page codes because they belong to no part. If a coding scheme is later needed, define it in `PAGE_CODES.md`.
- Page parity still applies to the book as a whole: front matter must resolve to a page count that leaves every part opener and every normal form on the correct side.

## Still to be decided

- Whether front and back matter eventually receive rows in `toc.csv`.
- Whether Property Identity is front matter or a Part `A` spread.
- Final front/back-matter page count, which affects gutter and pagination decisions in `KDP_PRINT_SPEC.md`.
- The continuation/replacement mechanism.

## Source of truth

This file owns the working inventory, placement status, and purpose of front and back matter.

It does not own content posture (`CONTENT_SCOPE_SAFETY.md`), voice (`WRITING_RULES.md`), visual treatment (`VISUAL_DESIGN_RULES.md`), or physical format (`KDP_PRINT_SPEC.md`).
