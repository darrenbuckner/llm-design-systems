---
id: dark-publisher
title: Obsidian Publisher System
description: A pure-black publishing interface where white paper panels invert out of the page and a single arterial red marks every interactive element.
tags: [dark, minimal, publishing, high-contrast, editorial, serif]
colors: ["#000000", "#FFFFFF", "#E53E3E", "#F7F7F7", "#A3A3A3"]
created: 2026-01-13
---

# Obsidian Publisher System

A reading-first publishing interface built on pure black, where blocks of near-white paper invert out of the page to carry forms, pull quotes, and pagination, and a single arterial red marks every interactive element. Everything is rectangular and shadowless: hierarchy comes from inversion and from the contrast between a large serif and a plain sans. Suited to literary magazines, long-form publications, editorial archives, and any reading surface that wants to feel printed rather than rendered.

## Color Palette

**Page Surface:** `#000000` — the ground for the entire interface. Pure black, not a near-black, because the paper panels that sit on it depend on the maximum available step. Roughly 70% of any screen.

**Primary Colors:**
- Paper White `#FFFFFF` — all body and heading type on the black ground, and the fill for a full-bleed inverted section.
- Arterial Red `#E53E3E` — the only chromatic value in the system. Primary buttons, the active pagination cell, link underlines on hover, and the section rule above a kicker. Nothing else.
- Red Deep `#C42F2F` — hover and active state for every red fill. Never a resting color.

**Neutral Colors:**
- Paper `#F7F7F7` — the inverted surface. Input fills, pagination cells, pull-quote blocks, and any panel meant to read as a sheet laid on the page. Type on Paper is always `#000000`.
- Muted `#A3A3A3` — bylines, timestamps, captions, placeholder text, and inactive navigation on the black ground. The one grey permitted on black; anything dimmer fails against pure black at body size.
- Rule `#262626` — hairline dividers and input borders on the black ground. Deliberately dark: on pure black a `#F7F7F7` border reads as a bright line rather than a division.
- Ink Muted `#5C5C5C` — the equivalent of Muted when type sits on a Paper panel.

**Accent/State Colors:**
- Error `#E53E3E` — reuses Arterial Red; the system does not introduce a second red.
- Success `#3E9E5F` — inline text and form confirmation only, never a fill.
- Warning `#C08A2E` — inline text only.
- Focus Ring `#E53E3E` at 2px offset 2px, on both the black ground and the Paper panels.

## Typography

**Display & Headings:** a transitional publishing serif at normal weight, never bold. Google Fonts equivalent: `Source Serif 4`, weights 400/600. Fallback: `'Source Serif 4', Georgia, 'Times New Roman', serif`.

**Body & UI:** a neutral grotesque for navigation, buttons, labels, metadata, and form type. Google Fonts equivalent: `Inter`, weights 400/500/700. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`.

**Type Scale:**
- Masthead (serif) — 48px / 400 / 1.20 / -0.01em
- Section heading (serif) — 36px / 400 / 1.30 / -0.01em
- Article title (serif) — 24px / 400 / 1.35 / 0
- Pull quote (serif) — 28px / 400 / 1.40 / 0
- Navigation (sans) — 18px / 400 / 1.40 / 0
- Body (sans) — 16px / 400 / 1.60 / 0
- Byline and metadata (sans) — 14px / 400 / 1.50 / 0, set in Muted
- Kicker (sans) — 13px / 700 / 1.20 / 0.12em, uppercase, set in Arterial Red
- Button (sans) — 14px / 700 / 1.00 / 0.04em, uppercase

**Hierarchy Rules:** Serif carries every title and quotation; sans carries everything a reader clicks, fills in, or scans. The two never trade jobs, and the serif is never set bold — at 48px on pure black, weight 400 already carries more presence than a bold sans, and bolding it closes the counters. The kicker is the only place red appears in type and the only all-caps display element besides button labels. Body copy is capped at 68 characters; a full-width line of 16px sans on black is materially harder to track than the same line on paper, so the measure runs tighter than a light system would need.

## Spacing System

**Base Unit:** 8px.

**Scale:** 8, 16, 24, 32, 48, 64, 96.

**Common Patterns:**
- Page gutter 24px; reading measure capped at 800px, wide measure at 1120px.
- Section to section: 96px desktop, 64px mobile.
- Masthead to first article: 48px.
- Article row: 24px between title and byline, 48px between rows, with a `#262626` rule at the midpoint.
- Paper panel padding 32px desktop, 24px mobile.
- Button padding 16px 32px. Input padding 16px.
- Pagination cells 44px square with 8px between them.
- Kicker to the heading beneath it: 16px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses `padding-top` and `padding-bottom` longhand, never a `padding: 96px 0` shorthand, because a shorthand on a class sharing that element wins on source order and silently zeroes the gutter.

**Full-bleed without overflow:** a full-width band is a block-level element at the page's natural width carrying its own background, with a nested gutter element holding the content. It is never produced with `margin: 0 -100vw` plus `padding: 0 100vw`. That idiom doubles the document width and forces a horizontal scrollbar at every viewport size, and because `100vw` includes the scrollbar it stays broken even when the maths looks right.

## Component Styles

### Buttons

**Primary** — fill `#E53E3E`, label `#FFFFFF` at 14px/700 uppercase with 0.04em tracking, `border-radius: 2px`, padding 16px 32px, no border, no shadow. Hover: fill `#C42F2F`. Disabled: fill `#262626`, label `#5C5C5C`.

**Secondary** — transparent fill, 1px `#FFFFFF` border, label `#FFFFFF`, same radius and padding. Hover: fill `#FFFFFF`, label `#000000`. The inversion is the hover state; the border does not merely brighten.

**On Paper** — inside a Paper panel the primary button is unchanged, but the secondary inverts: 1px `#000000` border, `#000000` label, hover fills black with white label.

### Paper Panels

Fill `#F7F7F7`, `border-radius: 2px`, 32px padding, no border and no shadow. All type inside switches to `#000000` with `#5C5C5C` for secondary lines. This is the system's core move — the panel reads as a sheet laid on the page, and it earns that purely through the tonal jump from `#000000` to `#F7F7F7`. Used for forms, pull quotes, and the pagination strip.

### Input Fields

Fill `#F7F7F7`, no border, `border-radius: 2px`, padding 16px, 16px/400 sans in `#000000`. Placeholder in `#5C5C5C`. Focus: 2px `#E53E3E` ring at 2px offset, fill unchanged. On a black ground the light fill is the entire affordance, so inputs never take a border. Invalid: 2px `#E53E3E` inset border with the message beneath at 14px in Arterial Red.

### Pagination

A row of 44px square cells at `border-radius: 2px`. Resting: fill `#F7F7F7`, numeral `#000000` at 16px/500. Active: fill `#E53E3E`, numeral `#FFFFFF`. Hover: fill `#FFFFFF`. The trailing control reads `NEXT PAGE` in 13px/700 uppercase with 0.12em tracking, in Arterial Red, with no box around it.

### Navigation

White 18px/400 sans on the black ground, laid out with 32px between items and no underline at rest. Hover: a 1px `#E53E3E` underline at 4px offset. Current section: label stays white with a persistent red underline. Inactive or secondary items drop to Muted. No pills, no fills, no background change.

### Article Rows

A kicker in Arterial Red, 16px, then a 24px serif title in white, then a 14px byline in Muted. Rows are separated by 48px and a single `#262626` rule. Rows carry no card, no fill, and no hover background — hover underlines the title in Arterial Red and nothing else moves.

### Pull Quotes

A Paper panel at 32px padding containing a 28px serif quote in `#000000`, then a 14px attribution in `#5C5C5C`. No quotation glyph, no left rule, no italics.

### Rules and Dividers

1px `#262626` at full container width on the black ground, `#D8D8D8` inside a Paper panel. Never doubled, never inset, never used directly above or below a Paper panel — the tonal edge of the panel is already the division.

## Layout Principles

A single centered column on a black page. Reading content is capped at 800px; index and listing views may widen to 1120px but keep the same 24px gutter. The page alternates between black reading stretches and full-bleed inverted bands, and that alternation is the only rhythm the layout has — there is no sidebar, no grid of cards, and no two-column body. Full-bleed bands run edge to edge by carrying their own background at the page's natural width, with a nested gutter element holding the content, so no element ever extends past the viewport. On mobile the gutter holds at 24px, section spacing drops to 64px, the masthead drops to 32px, and pagination cells stay 44px so they remain tappable.

## Visual Effects

Radii are 0 to 2px throughout — this is a rectangular system and rounding anything past 2px breaks it. There are no shadows, no gradients, no glass, no texture, and no blur. Elevation is expressed exclusively by inversion: a Paper panel is "above" the page because it is the opposite value, not because it floats. Transitions are 150ms ease on background-color, border-color, and color only. Because the ground is pure black, avoid pure-white large fills adjacent to body text at length; the Paper panels are deliberately `#F7F7F7` rather than `#FFFFFF` to take the glare off a large inverted block.

## Design Tone

Bold, authoritative, and reader-first. The pure-black ground and the large unbolded serif give it the gravity of a printed masthead, while the paper panels breaking out of the page make forms and quotations feel physically set rather than styled. The single red is doing the work of an entire accent palette, which is why it never gets diluted.

## Usage Notes for AI Implementation

1. **Elevation is inversion, never shadow.** A panel is above the page because it is `#F7F7F7` on `#000000`. Adding a box-shadow, a glow, or a lighter grey "card" tone collapses the one structural idea the system has.

2. **Never build a full-bleed band with `margin: 0 -100vw` and `padding: 0 100vw`.** It doubles the document width and forces a horizontal scrollbar at every viewport, and `100vw` includes the scrollbar so the maths never resolves. Use a block-level element carrying its own background with a nested gutter element inside it.

3. **The serif is never bold.** At 48px on pure black, weight 400 already reads heavier than a bold sans. Bolding closes the counters and turns a masthead into a headline.

4. **Borders on black are `#262626`, not `#F7F7F7`.** The palette lists a light neutral, but using it for a hairline puts a bright line across a dark page. `#F7F7F7` is a surface value in this system, never a stroke value.

5. **One red, roughly one red element per screenful.** The primary button, or the active pagination cell, or a kicker. Red never appears in body copy, headings, borders, or backgrounds, and the system never adds a second accent for secondary actions.

6. **Type inside a Paper panel flips completely.** Black body, `#5C5C5C` secondary. Leaving white or Muted type on a Paper panel is the most common way this system breaks, and it is exactly the failure that shipped in the original preview.

7. **Radii stay at 0 to 2px.** Buttons, inputs, panels, and pagination cells are all effectively rectangular. An 8px radius anywhere makes the whole page read as a generic dark dashboard.

8. **Keep the reading measure tight.** 68 characters maximum for body copy. White-on-black loses tracking accuracy faster than black-on-white, so the measure that feels comfortable in a light system is too wide here.

9. **The kicker is the only red type and the only all-caps besides buttons.** Do not letterspace headings, do not set bylines in caps, and do not color a heading red to create emphasis — emphasis is size and the serif/sans split.
