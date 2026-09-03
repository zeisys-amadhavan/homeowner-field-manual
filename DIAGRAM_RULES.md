# Diagram Rules

## Purpose

Diagrams exist to make the homeowner recognize and understand a real system quickly.

They are not decorative illustrations.

## Primary standard

A useful diagram should answer at least one of these:

- What am I looking at?
- Where is it normally located?
- What are the important parts?
- What connects to what?
- What direction does something move?
- What should I locate or identify in my own house?
- What distinction matters before I complete the paired form?

## Simplification

Remove detail that does not help the page's spread goal.

Prefer a small number of clearly differentiated components over technically exhaustive drawings.

Accuracy must survive simplification.

## Labels

Labels should be:

- short;
- unambiguous;
- visually subordinate to the main illustration;
- connected clearly to the correct component.

Use the established blue annotation system when applicable.

Avoid leader-line tangles and dense clouds of labels.

## Prominence

Only the few elements central to the page should be prominent.

Secondary context should be lighter, smaller, simpler, or otherwise visually subordinate.

## Whole-house / system views

Where a recurring house view is used, maintain the same base geometry so the reader builds spatial familiarity across pages.

System-specific information may be highlighted while unrelated context is ghosted or simplified.

## Endpoint and component symbols

Repeated symbols should have stable meanings across pages.

Do not create a new symbol language for each diagram.

## Text inside diagrams

Use as little prose as possible.

Prefer:

- component names;
- short states;
- arrows;
- numbers;
- small legends.

Long explanation belongs outside the drawing.

## External image-generation prompts

Reusable prompts intended for external image-generation tools are operational assets, not canonical book rules.

Store them under:

`prompts/`

For example:

`prompts/bw-diagram-prompt.md`

A prompt may implement these rules, but the prompt itself is not the source of truth for book design.

## Source artwork and layer assets

Diagram pages are produced from a small number of recurring base views rather than from unrelated one-off drawings. The base view and artwork source for each page are recorded in `toc.csv`.

Principles:

- A recurring house view keeps identical base geometry wherever it is reused, so the reader builds spatial familiarity across pages.
- Spot art is derived from the master view rather than drawn independently, so a zoomed detail and the whole-house view agree with each other.
- A composite overlay page combines system layers that appear separately elsewhere.

### Asset conventions still to be locked

The following are genuinely unowned today and should be recorded in this section once the author decides them. Do not invent them:

- source file organization and naming;
- layer naming and identifier scheme, and how a layer maps to a page code;
- how a layer identifier survives reordering required for correct rendering;
- export format, resolution, and effective PPI;
- minimum printed line weights;
- production color values.

Until they are locked, artwork decisions made per page should be recorded in `toc.csv` rather than assumed to be general rules.

## Source of truth

The required subject, spread goal, diagram-page content, base view, and artwork source for each page are defined in `toc.csv`.
