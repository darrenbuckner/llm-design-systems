---
id: dark-report-fieldbook-049
title: Charcoal Fieldbook
description: A dark long-form research system where a heavy grotesque carries the argument, a six-colour pastel palette carries the data, and hand-drawn annotations break the grid.
tags: [dark, minimal, editorial, publishing, data-visualization, high-contrast, generous-spacing, professional, research-report]
colors: ["#232323", "#F4F4F1", "#FF814D", "#7ED0FE", "#3D3D3C"]
created: 2026-08-28
---

# Charcoal Fieldbook

Charcoal Fieldbook is a dark system for long-form research: industry reports, survey write-ups, ebooks, field studies — anything that has to sustain forty pages of argument and still make a chart legible. A heavy grotesque carries the headings, a soft six-colour pastel palette carries every chart and category, and a hand-drawn annotation layer breaks the grid at chapter boundaries so a rigorous document never reads as a corporate deck. The ground is a single warm charcoal with two barely-separated surfaces above it, and there are no shadows anywhere.

## Color Palette

**Page Surface:** `#232323` — warm charcoal, the ground for every page. Not black, not blue-grey. Everything sits on it directly unless it is one of the two raised surfaces below.

**Neutral Colors:**
- Raised Panel `#262626` — a full-bleed note or letter card. One step up from the ground, distinguishable only by its edge and its size.
- Tile `#2E2E2E` — the selected state of an option tile. The system's brightest surface, and it is still only 1.16:1 against the ground.
- Ink `#F4F4F1` — all headings and body copy. Warm off-white, never `#FFFFFF`. 14.3:1 on the ground.
- Muted `#9A9A98` — eyebrows, captions, attribution roles, axis labels, and the trailing qualifier clause in a definition row. 5.6:1 on the ground and 4.8:1 on the tile, so it clears AA on every surface in the system.
- Hairline `#3D3D3C` — table dividers, chart brackets, section rules. The default separator.
- Panel Border `#4B4B4A` — the 1px edge of a quote panel or a bordered container. One step brighter than a hairline so a container edge reads as deliberate rather than as a divider.

**Primary Colors:**
- Signal Orange `#FF814D` — the single brand accent. The largest data series, inline links, opening and closing quote glyphs, and the "for agents" column marker. 6.4:1 on the ground.

**Data Palette** — six categorical fills, used in this order and never re-ordered to suit a chart:
`#FF814D` orange · `#7ED0FE` sky · `#FFD1E1` pink · `#F6DE90` butter · `#CBB5E9` lilac · `#F4F4F1` chalk

All six are light and read as text-legible against the ground (8.5–11.8:1). A neutral `#6A6A6A` fills the remainder segment in a part-to-whole bar, where the point is what is *not* being counted.

**Tinted Surfaces** — a data colour dissolved into the ground at roughly 12%, used only as the fill of a quadrant or region a data colour already labels:
`#332620` orange · `#252E33` sky · `#332E30` pink · `#323027` butter

**Accent/State Colors:**
- Severity Green `#8FD4A7` (9.1:1), Severity Amber `#F6DE90` (11.8:1), Severity Red `#E86A6A` (5.5:1). The red is lifted from the source's `#E24A4A`, which measured 3.98:1 — safe as a dot, unsafe the moment anyone sets a word in it.
- Inactive Dot `#444443` — the unfilled positions in a severity triad.
- Focus `#FF814D` — 2px outline at 3px offset.

**Handwriting** `#A09A9C` — the annotation layer only. Warm-tinted grey, deliberately quieter than ink and still above 4.5:1 everywhere.

**Inverse:** none. There is no light mode and no inverted band.

## Typography

**Font Families:**
- **Display & Headings:** Inter Tight, at 800 for chapter titles and 700 for section headings. A tightly-fitted grotesque; the compression is the point, and a normal-width grotesque at the same weight reads flabby at 44px. Fallback: `'Inter Tight', 'Inter', 'Helvetica Neue', Arial, sans-serif`.
- **Body:** Inter at 400 and 600. Same superfamily, normal fit, because tight display metrics hurt a 17px paragraph. Fallback: `'Inter', system-ui, 'Helvetica Neue', Arial, sans-serif`.
- **Annotation:** Architects Daughter — upright, hand-printed, monoline. Used only for the annotation layer, never for a heading, a label, or anything a reader must act on. Fallback: `'Architects Daughter', 'Comic Sans MS', cursive`.

**Type Scale:**

| Level | Family | Size | Weight | Line height | Tracking |
|---|---|---|---|---|---|
| Chapter title | Inter Tight | `clamp(32px, 5.5vw, 46px)` | 800 | 1.12 | -0.025em |
| Section heading | Inter Tight | `clamp(22px, 3vw, 26px)` | 700 | 1.25 | -0.015em |
| Subhead | Inter | 17px | 600 | 1.45 | -0.005em |
| Lede | Inter | `clamp(17px, 2.2vw, 20px)` | 400 | 1.55 | 0 |
| Body | Inter | 17px | 400 | 1.65 | 0 |
| Small / caption | Inter | 14px | 400 | 1.55 | 0 |
| Eyebrow | Inter | 11px | 500 | 1.4 | 0.16em, uppercase |
| Annotation | Architects Daughter | 19px | 400 | 1.5 | 0 |

**Hierarchy Rules:**
- Chapter titles run two or three lines on purpose and break where the sense breaks, not where the box ends. A one-line chapter title is a sign the title is too short for this system.
- There is exactly one 800 weight per page, on the chapter title. Everything below it tops out at 700.
- Eyebrows are uppercase, tracked at 0.16em, muted, and sit 12px above the title they label. They carry a section number, never a sentence.
- The two-tone sentence is a system rule, not an author's flourish: a definition row opens with the term in 600 ink, continues in 400 ink, and closes with the qualifying clause in 400 muted, all inside one paragraph. It replaces the bullet list this content would otherwise become.
- Prose measure caps at 74ch. Chapter titles are allowed to run wider than the prose column.
- Nothing is centered except the annotation layer and the page number.
- The annotation face appears at most twice per page and never inside a paragraph.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 96, 128.

**Common Patterns:**
- Page gutter: `clamp(20px, 4vw, 40px)`, owned by one container class.
- Container max width: 900px, centered. Prose measure 720px inside it.
- Chapter opener: eyebrow, 12px, title, 32px, lede, 64px, annotation rule, 64px, first paragraph.
- Section rhythm: 64px between major sections, 96px around a chapter boundary.
- Chart block: 16px from its heading rule to the first bar, 12px between a bar label and its bar, 20px between bar groups.
- Table cell padding: 16px vertical, 20px horizontal.
- Panel padding: 24px on mobile, 32px on desktop.
- Paragraph spacing: 16px.

## Component Styles

### Chapter Openers

Eyebrow (`CHAPTER 04`), then the 800-weight title, then a lede paragraph one step larger than body. No rule above, no ornament, no drop cap. The opener is followed by the annotation rule and nothing else — the first body paragraph does not start until after it.

### The Annotation Rule

The signature component, and the one thing that stops this system reading as a consulting deck. A 1px `#3D3D3C` line spanning the container, with a short tick at each end canted about 20° off vertical, as if drawn by hand. Below it, centered, one or two lines of the annotation face in `#A09A9C` posing the question the chapter answers.

Rendered as an inline SVG so the ticks stay crisp, or as a flex row of three elements: tick, `flex: 1` rule, tick. It carries 40px of clearance above and 24px below before the annotation text, then 56px before body resumes.

Used once per chapter opener. Twice on a page and the device stops being a marker and becomes decoration.

### Data Bars & Chart Frames

A chart block is bracketed by two 1px `#3D3D3C` rules: one directly under the block heading, one above the source line. Nothing else frames it — no axes, no gridlines, no plot border.

Each bar is a hard rectangle, `border-radius: 2px`, filled from the data palette in order, with its category label in 14px muted **above** the bar and its value in 14px ink immediately to the **right of the bar's end**, never inside the fill. Bars are 34px tall with 12px between the label and the bar.

A part-to-whole bar is a single 40px row of segments in palette order with `#6A6A6A` for the remainder, followed by a legend of 10px colour chips and 14px labels.

The source line sits under the closing rule: a 12px bold wordmark in ink, then 11px muted caption, on one row.

### Severity Dot Triads

A three-dot rating where exactly one dot is filled and the other two are `#444443`. Position encodes level — left is best, right is worst — and the filled dot takes the matching severity colour: green left, amber middle, red right. The word follows in 15px ink.

6px dots, 5px apart, vertically centered against the label. The triad is redundant with its own label by design: colour alone never carries the meaning, so the component survives greyscale printing and colour-blind readers.

### Comparison Tables

No zebra striping, no fills, no outer border. A 1px `#3D3D3C` rule under each row and between each column, and that is the entire structure.

The table lives inside an `overflow-x: auto` wrapper and carries a `min-width` floor of about 520px, so it scrolls within its own bounds on a narrow screen rather than widening the page.

Column headers are a small icon plus a label in the column's own data colour — sky for one side, orange for the other. The row label sits in the left column in 15px ink; each cell holds a severity triad above two or three lines of 15px ink.

### Quote Panels

A 1px `#4B4B4A` border, no fill, `border-radius: 2px`, 24–32px padding. The quote runs at 19px/1.5 ink, opened and closed by an oversized `#FF814D` quotation glyph set inline at 1.4em and raised, not floated into the margin. Attribution follows 16px below: name in 15px ink, role and organisation in 15px muted on the next line.

A portrait variant places a square image flush against the panel's left edge with no radius and no gap, so the image and the border form one object.

### Definition Rows

A 24px line icon in `#FF814D` or muted, then a single paragraph running term-bold, definition-regular, qualifier-muted. 16px gap between icon and text, 20px between rows. No bullets, no cards, no dividers.

This is how the system renders anything that would otherwise be a bulleted list of four to six options, and it is a large part of why the pages read as prose rather than as slides.

### Option Tiles

A selectable tile: 24px line icon centered, then a two-line 13px label. Unselected is transparent with muted-to-ink text; selected fills `#2E2E2E` with ink text and an ink icon. `border-radius: 2px`, no border in either state, 12px padding, 96px minimum tap target width and 44px minimum height.

Grouped four-across under a 15px/600 group heading, collapsing to two-across below 600px. The fill is the only state signal, which is why the tile background must stay `#2E2E2E` and never pick up a colour.

### Raised Note Cards

A full-width `#262626` card with a 1px `#4B4B4A` border and 32–48px padding, holding a personal letter or closing note. The heading uses the annotation face at 24px; the body stays in Inter so the card is still readable at length.

The only place in the system where the annotation face carries more than one line, and the only raised surface that holds body copy.

## Layout Principles

- One centered container at 900px, one class owning the horizontal gutter. Anything sharing that element sets vertical rhythm with `padding-top` / `padding-bottom` longhand so it cannot zero the gutter.
- Single column throughout. The option-tile grid is the one thing that reflows, four-across above 600px and two-across below. The comparison table keeps its columns at every width and scrolls horizontally inside a contained `overflow-x` wrapper with a `min-width` floor — stacking a two-consequence table into single-file rows destroys the side-by-side comparison that is the entire reason the table exists, so the scroll is the correct trade and the wrapper keeps it off the page's own scrollWidth.
- Prose caps at 720px and stays left-aligned inside the 900px container. Charts, tables, and panels take the full container width. That width difference is the page's only rhythm device.
- Charts are full-container width, always. A chart indented to the prose measure looks like an accident.
- Vertical space and hairlines do all the grouping. There are no cards around ordinary content — the raised surfaces are reserved for the two components that name them.
- Page numbers are centered at the foot in 11px muted. They are the only centered non-annotation element.

## Visual Effects

**Radii:** 2px on bars, tiles, panels, and images. Not 0 and not 8px — a hair of softening that keeps a page of rectangles from reading as brutalist, and it is uniform everywhere.

**Shadows:** none, at any elevation. Separation comes from the 3-value surface ramp (`#232323` / `#262626` / `#2E2E2E`) and from 1px borders. Adding a shadow to a `#262626` card on a `#232323` ground produces a muddy halo and no legibility gain.

**Borders:** 1px only, at two values — `#3D3D3C` for dividers and chart brackets, `#4B4B4A` for container edges. No 2px borders anywhere except the focus ring.

**Background treatment:** flat `#232323`. No gradients, no noise, no vignette. The tinted surfaces are flat fills, not overlays with opacity.

**Transitions:** 150ms `ease` on `background-color`, `color`, and `opacity`. Nothing else animates.

**Focus:** `outline: 2px solid #FF814D; outline-offset: 3px`, never removed.

## Design Tone

Serious and evidence-led, with one hand-drawn seam showing. It reads like a well-produced industry report that someone actually annotated in pencil — the grotesque and the hairline tables do the arguing, the pastel data palette keeps forty pages of charts from turning into a wall of brand orange, and the handwritten line at each chapter boundary admits that the authors are still working the question out. The warmth comes from the charcoal ground and the off-white ink rather than from any decorative element.

## Usage Notes for AI Implementation

1. **Use the data palette in order and never re-order it.** Orange, sky, pink, butter, lilac, chalk. Assigning colours by hue preference chart-to-chart destroys the cross-chart consistency that makes a long report readable, and it is the fastest way to make this look like a template.

2. **Value labels sit outside the bar, never inside it.** The palette is light and the ground is dark, so ink-on-fill fails and fill-coloured text on the ground is the only readable option. A 4% bar has no room for a label inside it anyway, which is exactly the case that breaks a chart built the other way.

3. **Never let colour alone carry meaning in a severity triad.** Position encodes level and the word is always present. Three green dots with no label is not this component.

4. **Keep the surface ramp to three values and never add a fourth.** `#232323` ground, `#262626` raised, `#2E2E2E` tile. The steps are deliberately near-invisible; a designer "fixing" the contrast between them by lightening the panel turns a quiet document into a dashboard.

5. **The annotation face is a seam, not a voice.** Once per chapter opener plus the closing note card. Setting a heading, a chart label, or a button in it reads as whimsy and undoes the credibility the grotesque establishes.

6. **Muted is `#9A9A98`, not `#818180`.** The lower value looks better and measures 4.03:1, which fails AA for the eyebrows, captions, and attribution lines that carry it. Do not darken it back toward the ground for aesthetics.

7. **One 800 weight per page.** The chapter title. If a section heading also needs 800 to feel important, the page has two competing titles and the structure is wrong.

8. **Charts and tables take the full 900px container while prose stays at 720px.** Do not indent a chart to match the paragraph above it. That width step is the only layout rhythm the system has, and matching them flattens the page.

9. **Give table and grid children `min-width: 0`, and size chapter titles with `clamp()`.** A 46px 800-weight grotesque cannot break, so a fixed size overflows a 393px viewport before any media query fires; and a long unbroken cell in a `1fr` track pushes the table wider than its container with no element reporting as overflowing.

10. **One element owns the horizontal gutter.** If a section class sets `padding: 64px 0` shorthand on that same element, it silently zeroes the gutter and content runs to the viewport edge on mobile while the header stays correctly indented. Use vertical longhand on anything sharing the gutter element.
