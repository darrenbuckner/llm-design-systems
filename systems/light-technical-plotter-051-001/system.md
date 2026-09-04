---
id: light-technical-plotter-051
title: Plotter Spring System
description: A white technical-drawing system built on dashed hairline grids, monospace UI labels, and a single acid-green highlighter accent.
tags: [light, high-contrast, monospace, neon, developer, marketing, illustrated, minimal]
colors: ["#FFFFFF", "#F6F6F4", "#000000", "#1BE670", "#F6C7F2"]
created: 2026-09-03
---

# Plotter Spring System

A stark white infrastructure-marketing system that treats the page like a plotter drawing: dashed hairline rules divide every section and column, every interactive label is set in letterspaced uppercase monospace, and a single acid spring green appears as a highlighter block dragged behind headline text. Nothing is rounded, nothing has a shadow, and the only decoration is technical — isometric line diagrams annotated with mono callouts. Built for developer platforms and infrastructure products that need to read as precise and fast rather than friendly.

## Color Palette

**Page Surface:** `#FFFFFF` — the default ground for every section. The system is white-dominant; roughly two-thirds of vertical space sits on pure white.

**Primary Colors:**
- Ink — `#000000` — all headings, body copy, borders, and primary button fills. True black, never softened to a charcoal.
- Accent Spring — `#1BE670` — the highlighter block behind headline fragments, the announcement bar ground, active carousel dots, status indicators, and diagram fills. It is never a button fill and never carries white text.
- Inverse Ground — `#000000` — the footer band and any full-bleed inverse section.

**Neutral Colors:**
- Alt Surface — `#F6F6F4` — the alternating section ground. Warm by two points of red; it must not read as a cool gray.
- Hairline — `#E4E4E1` — every dashed rule, column divider, and section boundary.
- Border Solid — `#D8D8D4` — solid 1px borders on secondary buttons, eyebrow chips, and carousel controls.
- Text Primary — `#000000` — headings and body prose.
- Text Secondary — `#4A4A48` — supporting paragraphs beneath a heading, and mono labels inside eyebrow chips.
- Text Muted — `#A2A4A3` — footer column labels and metadata. On black this is the only non-white text.

**Accent/State Colors:**
- Success — `#1BE670` — the status pill dot and its border.
- Diagram Tint — `#75F1A9` — mid-fill on isometric geometry.
- Diagram Wash — `#D3FBE3` — the lightest fill on isometric geometry.
- Diagram Secondary — `#F6C7F2` — pale orchid, used only as a counterweight inside illustrations. Never in UI.
- Focus — `#000000` — a 2px solid outline offset 2px. Focus is black, not green.

**Inverse Block (footer):** ground `#000000`, links `#FFFFFF`, column labels `#A2A4A3`, divider `#2A2A2A`, status pill text and 1px border `#1BE670` on a `#0A2417` fill.

## Typography

**Font Families:**
- Display and body — a tight geometric grotesque with slightly rounded terminals and a single-story `g`. Google Fonts equivalent: `Space Grotesk`. Stack: `'Space Grotesk', 'Helvetica Neue', Arial, sans-serif`.
- Interface labels — a plain typewriter monospace. Google Fonts equivalent: `JetBrains Mono`. Stack: `'JetBrains Mono', 'Space Mono', ui-monospace, monospace`.

**Display & Headings:** Space Grotesk. The reading experience is entirely sans; the monospace is a labelling device, never a text face.

**Type Scale:**
- Hero — `clamp(40px, 11vw, 76px)` / 700 / line-height 0.98 / letter-spacing `-0.03em`
- Section Head — `clamp(30px, 8vw, 52px)` / 700 / 1.04 / `-0.025em`
- Subsection — `clamp(22px, 6vw, 34px)` / 700 / 1.12 / `-0.02em`
- Card Title — `18px` / 700 / 1.3 / `-0.01em`
- Body — `16px` / 400 / 1.55 / `0`
- Body Small — `14px` / 400 / 1.5 / `0`
- Mono Label — `12px` / 500 / 1.2 / `0.12em` / uppercase
- Mono Micro — `11px` / 500 / 1.2 / `0.14em` / uppercase

**Hierarchy Rules:**
- Headings are 700 and nothing heavier; there is no 800 or 900 weight anywhere.
- Negative tracking scales with size. Anything above 30px takes at least `-0.02em`; body text takes none.
- Headings wrap deliberately at two or three lines and are never balanced with `text-wrap: balance` — the ragged break is part of the look.
- Every uppercase string in the system is monospace. Every sentence-case string is the grotesque. There are no uppercase grotesque labels.
- Supporting paragraphs sit directly under their heading at `16px` with no eyebrow, no rule, and a `12px` gap.
- Hero and section heads are left-aligned in product sections and centered in the full-width statement sections. Body prose is never centered below 3 lines.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 96, 128.

**Common Patterns:**
- Page gutter — 24px mobile, 40px at 768px, 64px at 1200px+. One element owns it.
- Section padding — 64px top and bottom on mobile, 96px at 768px, 128px at 1200px+, set as `padding-top` / `padding-bottom` longhand so it never collides with the gutter.
- Heading to supporting paragraph — 12px. Paragraph to button row — 24px.
- Between stacked feature blocks — 48px mobile, 64px desktop.
- Button internal padding — 14px vertical, 20px horizontal. Mono label and chevron separated by 10px.
- Eyebrow chip — 6px vertical, 12px horizontal.
- Logo grid cell — 32px vertical padding, cells divided by dashed rules rather than gaps.
- Footer column gap 32px, row gap 12px between links, 24px above each column label.

## Component Styles

### Buttons

Three variants, all with `border-radius: 0`, all labelled in uppercase mono at 12px with `0.12em` tracking, all ending in a `›` chevron separated by 10px.

- **Primary** — fill `#000000`, text `#FFFFFF`, no border. Hover: fill stays black, chevron translates 3px right over 150ms. Full-width on mobile, auto-width from 768px.
- **Secondary** — fill `#FFFFFF`, text `#000000`, 1px solid `#D8D8D4`. Hover: border to `#000000`. Full-width on mobile when paired with a primary, otherwise inline and shrink-wrapped.
- **Compact** — the same as secondary at 11px mono, 10px/14px padding. Used for `LEARN MORE`, `TRY IT`, `DOCS`, `CASE STUDY` — the inline read-more affordance that appears throughout.

Never fill a button with the accent green. Green is a highlight, not a call to action.

### Eyebrow Chip

A section label above a centered statement head: uppercase mono 11px, `0.14em` tracking, `#4A4A48` text, 1px solid `#D8D8D4`, square corners, 6px/12px padding, white fill, `margin-bottom: 24px`. One per section maximum, and only above centered heads.

### Highlighter Block

The system's defining move. A heading is split so that one or two lines sit inside a `#1BE670` block that extends past the text to the right edge of the content column. Implement as an inline-block span with `background: #1BE670`, `padding: 4px 12px 8px`, `box-decoration-break: clone`, black text, no radius. The block wraps to the exact width of its lines — never a full-width bar behind a short line. One per section, maximum one per screenful.

### Dashed Grid Rules

1px dashed `#E4E4E1` at a 4px dash / 4px gap. Three uses:
- **Section boundaries** — a horizontal dashed rule at the top of each product block.
- **Column rules** — vertical dashed lines marking the content column edges, running the full height of a section and visible in the gutter.
- **Cell dividers** — the logo grid and model list use dashed rules instead of gaps or card borders.

Rules are structural, not decorative. If a section has no grid to express, it gets no rules.

### Cards and Panels

There are almost no cards. Content blocks are separated by dashed rules and vertical space, sitting directly on the section ground. When a raised surface is genuinely needed, it is `#FFFFFF` on the `#F6F6F4` ground with a 1px solid `#D8D8D4` border, zero radius, and no shadow. Depth is expressed by stepping the ground, never by elevation.

### List Rows

The model-list pattern: a 28px square black icon tile, a 14px/700 grotesque name, and a right-aligned `TRY IT ›` compact affordance. Rows are 56px tall, divided by 1px dashed `#E4E4E1`, with 12px between icon and name. Hover: row ground to `#F6F6F4`, chevron translates 3px.

### Input Fields

`#FFFFFF` fill, 1px solid `#D8D8D4`, zero radius, 14px/16px padding, 16px grotesque text, placeholder `#A2A4A3`. Labels above the field in uppercase mono 11px `#4A4A48`. Focus: border `#000000` plus a 2px black outline offset 2px. Error: border `#000000` with the message below in 12px mono. There is no red — errors are stated in words.

### Carousel Controls

Two 48px square outline buttons with 1px solid `#D8D8D4` and a black chevron, flanking a centered dot row. Dots are 10px circles, `#D8D8D4` inactive, `#1BE670` with a 2px `#000000` ring when active. Circles are the single exception to the no-radius rule and exist only here.

### Status Pill

Uppercase mono 11px `#1BE670` on `#0A2417`, 1px solid `#1BE670`, square corners, 8px/14px padding, preceded by a 6px `#1BE670` dot. Footer only.

## Layout Principles

Single column at every width below 768px, with buttons going full-width and stacking at 12px. From 768px the logo grid moves to three columns and paired buttons sit inline. From 1200px the gutter widens to 64px and a max content measure of 1200px centers with `margin-left: auto; margin-right: auto` — the max-width element is outside the gutter element and must carry its own auto margins.

Prose measure caps at 62 characters regardless of container width. Full-bleed bands (the announcement bar, the footer) are block-level elements at the page's natural width carrying their own background, with a nested gutter element holding content — never negative-margin tricks.

Alternate section grounds white → `#F6F6F4` → white down the page. Two adjacent sections never share a ground; the dashed rule does the work only where the ground repeats.

## Visual Effects

**Radii:** `0` on everything except carousel dots and status dots, which are `50%`.

**Shadows:** none, at any elevation, in any state. Separation is ground-stepping, dashed rules, and 1px solid borders only.

**Borders:** 1px throughout. Dashed `#E4E4E1` for structure, solid `#D8D8D4` for interactive containers, solid `#000000` on hover and focus.

**Illustration:** isometric line diagrams built from thin black strokes with `#D3FBE3` / `#75F1A9` / `#1BE670` fills stepping from light to saturated, plus `#F6C7F2` as a cool counterweight. Connectors are dashed `#C9C9C6`. Labels sit in tiny white chips with a 1px solid border and 9px uppercase mono text.

**Transitions:** `150ms ease` on color and border. Chevrons translate 3px on hover. No scale, no lift, no fade-in on scroll.

## Design Tone

Precise, industrial, and unsentimental — a technical drawing that happens to be selling something. The dashed grid and monospace labels borrow the vocabulary of CAD and terminal output, while the acid green highlighter injects exactly enough energy to keep the page from reading as documentation. It is confident without being loud: the black-on-white contrast does the shouting, and the accent is rationed to one gesture per screen.

## Usage Notes for AI Implementation

1. Ration the green to one gesture per screenful. It appears as a highlighter block, a status dot, or a diagram fill — never all three in the same viewport. Two green elements competing on one screen collapses the system into a generic startup landing page.
2. Never fill a button with `#1BE670`. Primary actions are black. The moment green becomes a CTA color, the highlighter stops reading as emphasis and becomes brand wallpaper.
3. Every uppercase string is monospace and every sentence-case string is the grotesque. Setting a button label in uppercase Space Grotesk is the single fastest way to make this look like a different system.
4. Keep `border-radius: 0` everywhere except the two dot cases. Softening buttons or inputs to even 4px removes the drafting-table quality the whole system rests on.
5. The dashed rules must mark real structure — column edges, section boundaries, cell dividers. Scattering them as texture makes the page read as busy rather than surveyed, and the grid loses its meaning.
6. Never add a shadow. When a surface needs to separate, step the ground from `#FFFFFF` to `#F6F6F4` or add a 1px solid `#D8D8D4` border. A single `box-shadow` anywhere makes every borderless block look broken by comparison.
7. Do not center body prose longer than three lines. Centered heads with centered supporting sentences are correct for statement sections; centered paragraphs of five lines are not, and the measure cap of 62 characters exists to stop it.
8. Give the gutter to exactly one element and set section rhythm with `padding-top` / `padding-bottom` longhand. A `padding: 96px 0` shorthand on a sibling class wins on source order and silently flushes content to the viewport edge on mobile while the header stays indented.
9. Size hero and section heads with `clamp()` rather than media queries. The display type is tightly tracked and unbreakable, so a fixed 76px numeral overflows a 393px viewport with no element reporting as overflowing; add `overflow-wrap: anywhere` to any type specimen.
10. Errors are stated in words, not in red. The palette carries no error color on purpose — introducing one adds a hue that appears nowhere else and immediately looks foreign against the two-color scheme.
