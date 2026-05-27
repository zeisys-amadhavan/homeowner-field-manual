# Master Diagram Style Prompt

> Reusable base prompt for generating illustrative diagrams that sit harmoniously on a pale cool gray-blue page background (#DAE2E8 at 75% transparency). Append diagram-specific content (composition, components, labels, data) after this block.

---

## Style

**Ultra-clean illustrative diagram, ready for vector tracing.** Bold, uniform outline strokes on every shape — perfectly sharp edges, complete closed paths, no gaps, broken lines, sketching, hatching, anti-aliasing, gradients, or shadows. Centered, clear, ruthlessly simplified composition with minimal deliberate internal lines.

Inside the outlines, fill with a coordinated 16-color palette — visually rich and pretty, like a printed technical reference. Apply color purposefully, not flood-filled. Dorling Kindersley illustration register: muted but saturated, never neon, never washed out.

---

## Palette

Use only these 16 colors and their natural lighter tints / darker shades for highlights and shadows:

| Hex | Name |
|---|---|
| `#0A0A0A` | near black |
| `#FDFFFE` | white |
| `#FCD74A` | yellow |
| `#F4AD39` | orange |
| `#C59B39` | mustard |
| `#B1AD42` | olive yellow |
| `#79A54E` | sage green |
| `#42934E` | leaf green |
| `#3B876D` | forest teal |
| `#5A297B` | deep purple |
| `#884DC3` | bright purple |
| `#8A5E82` | mauve |
| `#6F4537` | brown |
| `#6F6563` | warm gray |
| `#C1B5B5` | light warm gray |
| `#C9C8CD` | light cool gray |

**Do not use:** the muted slate-blue around `#5078A0` or pure fire-engine red around `#FA0000`.

---

## Background harmony

Render the diagram on a **pure white canvas**, but choose colors knowing the final placement is on a page tinted **#DAE2E8 at 75% transparency** (a pale cool gray-blue). Optimize for visual harmony against that cool page tone:

- **Lean warm.** The page is cool, so the diagram should bring warmth forward. Favor the warm palette members — yellow, orange, mustard, olive, brown, mauve, warm gray — as primary fills. Use cool palette members (forest teal, sage green, deep purple, light cool gray) as accents or secondary supporting colors, never as dominant fills across large areas.
- **Avoid background camouflage.** Light cool gray (`#C9C8CD`) is too close to the page tint and will visually disappear — use it sparingly and never for elements that need to read clearly. Prefer light warm gray (`#C1B5B5`) for neutral fills, gridlines, and subtle structural elements.
- **Maintain contrast.** Every shape needs enough tonal contrast against a slightly cool background. When in doubt, darken the fill or strengthen the outline — pale fills should still have a confident outline in near black or brown.
- **Alarm and emphasis colors.** Since the palette excludes red, treat orange (`#F4AD39`) as the high-emphasis color and yellow (`#FCD74A`) as the medium-emphasis color. For maximum urgency, escalate from yellow → orange → mustard (`#C59B39`) or brown (`#6F4537`) rather than reaching for red.
- **Whites and outlines.** Keep white fills (`#FDFFFE`) only where they actively contribute — they will read as page-color through the placement, which can be desirable for negative space or could weaken a shape that needed solidity. Use near-black (`#0A0A0A`) outlines confidently to anchor every form against the cool background.

The diagram should feel like it belongs on the page — warm, grounded, editorial — not like an unrelated graphic dropped on top.

---

## How to use

Append diagram-specific instructions below this block — composition zones, components, labels, cell values, layout sizing, typography notes, and so on. The style and background-harmony rules above are portable across diagram types (matrix, flowchart, illustration, infographic).
