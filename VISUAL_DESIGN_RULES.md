# Visual Design Rules

This file owns the recurring visual grammar of the book.

## Design objective

The book should feel like a practical field instrument: clear, systematic, visual, durable, and easy to scan.

Information hierarchy matters more than decoration.

## Page architecture

Design for **8 × 10 inch portrait**.

The spread is the core composition:

- form on the left;
- guide/diagram on the right.

Related pages should visibly read as one system.

## Established visual grammar

Current recurring elements include:

- strong black page/header typography;
- permanent page code displayed prominently;
- disciplined technical annotation;
- clear callout hierarchy;
- blue used as an intentional labeling/annotation signal;
- warnings separated visually from normal explanation;
- substantial working space rather than filling every area with content.

## Typography standard

Typography is standardized across the book. Do not vary font family, style, size, leading, tracking, alignment, or color page by page unless a later project-wide decision explicitly changes this table.

| **Role**                | **Font Type**  | **Font Style** | **Size**  | **Leading** | **Tracking** | **Alignment** | **Color** |
| ----------------------- | -------------- | -------------- | --------- | ----------- | ------------ | ------------- | --------- |
| PAGE TITLE              | Helvetica Neue | Condensed Bold | **28 pt** | Auto        | **−10**      | **Left**      | **#FFFFFF** |
| PAGE CODE (PAGE NUMBER) | Courier New    | Bold           | **28 pt** | Auto        | **−10**      | **Right**     | **#FFFFFF** |
| INSTRUCTIONS            | Courier New    | Regular        | **14 pt** | Auto        | **−10**      | **Left**      | **#000000** |
| SECTION HEADERS         | Helvetica Neue | Bold           | **18 pt** | Auto        | **−10**      | **Left**      | **#FFFFFF** |
| FORM FIELDS             | Helvetica Neue | Regular        | **14 pt** | Auto        | **−10**      | **Left**      | **#5A7AA0** |
| DIAGRAM LABELS          | Helvetica Neue | Regular        | **14 pt** | **12 pt**   | **−10**      | **Center**    | **#2F5FA8** |
| GRID LABELS             | ISOCP EUR      | Regular        | **8 pt**  | Auto        | **−10**      | **Left**      | **#888888** |

### Typography implementation rules

- **Auto leading is the default** except where the table specifies a fixed value.
- **−10 tracking is the default** for all defined typography roles.
- Page titles are left aligned.
- Page codes are right aligned.
- Diagram labels are center aligned.
- These values are production standards, not starting suggestions.

## Annotation blue

Blue is reserved as an intentional labeling language rather than as a general illustration fill.

The standard diagram-label color is **#2F5FA8**.

The standard form-field color is **#5A7AA0**.

When blue is being used as the annotation standard, avoid allowing large diagram elements to compete with it.

### Annotation blue versus system color coding

There is still an unresolved tension between two possible uses of color, and it should be settled deliberately rather than page by page:

1. **Blue as annotation.** Blue means *this is a label*, regardless of subject. This is the current standard.
2. **Color as subject.** Each system owns a hue — so a reader flipping pages recognizes a system by color alone.

These can coexist only if no system is assigned the established annotation-blue range. A scheme that colors water similarly blue would collide with the current standard and make labels ambiguous on exactly the pages where labels matter most.

Until the author decides:

- annotation blue holds;
- do not assign a competing blue to a system;
- do not introduce a per-system palette on individual pages ahead of a book-wide decision.

## Hierarchy rule

A reader should normally perceive, in order:

1. what this page is about;
2. the major visual/system;
3. the important labeled parts;
4. supporting explanation;
5. secondary details.

Do not give minor facts equal visual weight to the main concept.

## Consistency

Repeated components should behave consistently across the book:

- page codes;
- headers;
- callout circles;
- labels;
- warning treatment;
- legends;
- tables;
- form fields;
- cross-references.

Do not redesign these conventions page by page.

## Density

Whitespace is working space.

Avoid filling unused areas merely to make a page look complete.

For form pages, handwriting space is content.

For guide pages, visual breathing room improves comprehension.

## Relationship to other files

- Illustration-specific rules → `DIAGRAM_RULES.md`
- Fillable-page rules → `FORM_RULES.md`
- Page pairing → `PAGE_SPREAD_RULES.md`
- Page assignments → `toc.csv`
