---
id: light-warm-editorial-041
title: Vellum Editorial System
description: A warm paper-toned editorial system pairing heavy geometric sans headlines with a reading serif, built for long-form program pages and application flows.
tags: [light, warm, editorial, serif, minimal, long-form, form-heavy]
colors: ["#F0EDE4", "#E4DFD1", "#CC7A5A", "#1A1917"]
created: 2026-08-23
---

# Vellum Editorial System

A warm, paper-inspired system that treats the page as a printed document rather than an app surface. Long measures of serif body copy sit on an unbleached ivory ground, punctuated by heavy geometric sans headlines and a single terracotta accent. Structure comes from tinted panels and hairline rules rather than shadows or cards — the whole surface stays flat, matte, and quiet, which lets dense informational content breathe over very long scroll lengths.

## Color Palette

**Primary Colors:**
- Ink: `#1A1917` — All primary text, filled buttons, icon fills, footer ground
- Terracotta: `#CC7A5A` — Single accent: inline links, required-field markers, emphasis marks

**Neutral Colors:**
- Page Surface: `#F0EDE4` — Base background for the entire document (warm unbleached ivory)
- Surface Tint: `#E9E5D9` — Secondary panels, pull-out callout blocks
- Surface Deep: `#E1DCCC` — Application/form panel, the deepest non-ink ground
- Surface Raised: `#F7F5EF` — Input field fills, chips, elements sitting on tinted panels
- Text Primary: `#1A1917`
- Text Secondary: `#57544D` — Supporting paragraphs, helper text, timestamps
- Text Muted: `#8A867C` — Placeholder text, captions, footer legal
- Border: `#D6D1C1` — Input borders, panel edges, structural containers
- Border Hairline: `#DFDACB` — Section dividers, agenda row separators, list rules

**Accent/State Colors:**
- Success: `#4A7C59`
- Warning: `#B8843F`
- Error: `#B4462F`
- Focus Ring: `#CC7A5A` at 30% opacity, 3px spread

**Inverse:**
- Footer Ground: `#141311`
- Footer Text: `#F0EDE4`
- Footer Muted: `#7C7871`

## Typography

**Font Families:**
- Display/UI: Geometric-grotesque sans, heavy weights only — `Space Grotesk` (fallback: `Poppins`, `system-ui`). Used for all headings, buttons, form labels, chips, and navigation.
- Body: Transitional reading serif — `Source Serif 4` (fallback: `Georgia`, serif). Used for every paragraph, list item, and FAQ answer.

The split is strict: sans is never used for running prose, serif is never used for interface chrome. This is the single most defining characteristic of the system.

**Type Scale:**
- Display: 44px / 700 / 1.05 / -0.02em tracking
- Heading 1: 34px / 700 / 1.12 / -0.015em
- Heading 2: 26px / 700 / 1.2 / -0.01em
- Heading 3: 19px / 700 / 1.3 / -0.005em
- Body Large: 18px / 400 / 1.65 (serif) — lead paragraphs
- Body: 16px / 400 / 1.7 (serif) — default prose
- Label: 14px / 600 / 1.4 (sans) — form labels, agenda times, metadata
- Caption: 13px / 400 / 1.5 — helper text, legal, footer

**Hierarchy Rules:**
- Display and H1 wrap deliberately across 3–4 short lines rather than running full-width; the ragged left-aligned stack is intentional.
- Headings carry negative tracking that decreases as size increases; body serif uses default tracking.
- Bold body emphasis is set in the serif at 600, not switched to sans.
- No heading is ever centered. No heading uses color other than Ink.
- Section headings sit directly above a hairline rule or with 48px of clear space — never both.

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 96, 128

**Common Patterns:**
- Page gutter: 24px mobile, 40px tablet, 64px desktop
- Section spacing (between major blocks): 64px mobile, 96px desktop
- Panel padding: 24px mobile, 32–40px desktop
- Form field vertical rhythm: 20px between fields, 8px between label and input
- List item spacing: 16px between items, 12px gap between icon and text
- Agenda rows: 20px vertical padding, separated by hairline rules
- Paragraph spacing: 16px, with a 66–72 character max measure

## Component Styles

### Buttons
- **Primary:** Ink `#1A1917` fill, `#F0EDE4` text, fully pill-shaped (`border-radius: 999px`), 14px/600 sans, 14px vertical / 24px horizontal padding, trailing arrow glyph set 8px from the label. Hover: fill lightens to `#2E2C28`, arrow translates 3px right over 150ms. Active: fill returns to Ink, no transform.
- **Secondary:** Transparent fill, 1px `#1A1917` border, Ink text, same pill geometry and padding. Hover: fill becomes `rgba(26,25,23,0.06)`.
- **Tertiary/Text:** Ink text with 1px terracotta underline offset 3px. Hover: underline thickens to 2px.
- All buttons maintain a 44px minimum touch height. Buttons never carry shadows or color blends.

### Cards & Panels
- Panels are tinted blocks, not elevated cards: `#E9E5D9` or `#E1DCCC` fill on the `#F0EDE4` page.
- `border-radius: 24px` on large panels; no border and no shadow — separation comes purely from tonal shift.
- Interior padding 24px mobile / 40px desktop.
- A panel heading sits flush at the top-left of the panel with 24px below it before content begins.

### Input Fields
- Fill `#F7F5EF`, 1px `#D6D1C1` border, `border-radius: 8px`, 12px vertical / 14px horizontal padding, 16px serif-free sans input text.
- Labels sit above the field in 14px/600 sans, Ink; required fields append a terracotta asterisk.
- Placeholder text `#8A867C`.
- Focus: border shifts to `#1A1917`, plus a 3px `rgba(204,122,90,0.3)` ring. No border-radius change.
- Selects use the identical box with a chevron glyph inset 14px from the right edge.
- Checkboxes are 18px squares with 4px radius, Ink fill when checked with an ivory tick.

### Chips & Metadata Pills
- `#F7F5EF` fill, 1px `#D6D1C1` border, `border-radius: 999px`, 8px vertical / 14px horizontal padding, 13px/600 sans.
- Used for dates, venue notes, and tag rows. Never colored, never filled with accent.

### Icon Lists
- 20px Ink-filled circle with an ivory tick or numeral inside, 12px gap to the text.
- Text is serif body; list items separated by 16px.
- Used for benefit lists and numbered process steps alike — the circle carries the meaning, not the color.

### Dividers & Agenda Rows
- 1px `#DFDACB` hairline, full container width.
- Agenda pattern: 14px/600 sans timestamp on its own line, 19px/700 sans title beneath, 16px serif description beneath that, closed by a hairline.

### Footer
- Full-bleed `#141311` ground, 64px vertical padding, centered mark and social glyphs at 20px, legal line in 13px `#7C7871`.

## Layout Principles

- Max content width: 680px for prose, 760px for panels — the system is deliberately narrow and single-column even at desktop widths.
- Grid structure: single column throughout; secondary content (agenda, FAQ) uses stacked full-width rows rather than multi-column grids.
- Responsive behavior: nothing reflows into columns on desktop; the measure simply centers and gutters widen. Form fields go full width at every breakpoint.
- Alignment: everything left-aligned, ragged right. Centering appears only in the footer.
- Vertical rhythm is the primary structural tool — the page reads as a continuous document, not a set of modules.

## Visual Effects

- **Border Radius:** 8px (inputs, checkboxes at 4px), 16px (small panels), 24px (large panels), 999px (buttons, chips)
- **Shadows:** None. The system uses zero elevation — tonal contrast replaces depth entirely.
- **Borders:** 1px only, in two weights of warmth — `#D6D1C1` for interactive containers, `#DFDACB` for structural rules. No 2px borders anywhere.
- **Backgrounds:** Flat solid warm tones only. No blends, no textures, no imagery behind text.
- **Transitions:** 150ms ease on color and transform; nothing animates on scroll.

## Design Tone

Editorial, institutional, and confident without being loud — closer to a well-set printed prospectus than a product page. The warm ivory ground and serif body signal patience and substance, while the heavy geometric headlines and single terracotta accent keep it contemporary rather than nostalgic. It expects the reader to actually read, and rewards that with generous measure, quiet contrast, and no visual competition for attention.

## Usage Notes for AI Implementation

- Enforce the sans/serif split rigidly. If prose is set in the sans, the system collapses into a generic startup page.
- Never add shadows. When you need to separate a region, step the background one tone deeper (`#F0EDE4` → `#E9E5D9` → `#E1DCCC`) and round the corners to 24px.
- Use terracotta sparingly — roughly one accent element per screenful. It is a marker, not a brand color to fill with.
- Keep everything single-column. Resist the urge to build two-column desktop layouts; widening gutters is the only desktop adaptation.
- Headlines should break across multiple short lines. Set `max-width` on the h1 rather than letting it run.
- All buttons are pills with a trailing arrow. There is no rectangular button variant.
- For dense informational sections (agenda, FAQ), lean on hairline-separated stacked rows rather than cards.
- Body copy should never exceed a 72-character measure regardless of viewport.
