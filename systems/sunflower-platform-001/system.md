---
id: sunflower-platform-001
title: Sunflower Platform System
description: A cream-ground neo-brutalist system where every surface is outlined in heavy black and a single saturated yellow marks the cards that matter.
tags: [light, bold, playful, high-contrast, cards, serif]
colors: ["#F5F5DC", "#FFD700", "#000000", "#FFFFFF", "#2C2C2C"]
created: 2026-01-09
---

# Sunflower Platform System

A high-energy interface built on warm cream, where every surface is outlined in 2–3px of pure black and a single saturated yellow picks out the cards that carry the most weight. A classical serif handles all display and reading type while a plain grotesque handles anything the user operates, and the two never mix. Suited to creative tools, educational platforms, and consumer products that need to feel loud and tactile without becoming hard to read.

## Color Palette

**Page Surface:** `#F5F5DC` — warm cream, the ground for every screen. Not white and not yellow: the cream is what lets both the white cards and the yellow cards read as distinct surfaces laid on top of it. Roughly 60% of any screen.

**Primary Colors:**
- Sunflower `#FFD700` — the accent surface. Fills feature cards, statistic tiles, and the one block per section that should be looked at first. It is a *surface* color, not a text or border color.
- Sunflower Deep `#F7CA00` — hover state for any yellow fill. Never a resting color.
- Ink `#000000` — pure black. All type, every border, every icon. This system is the one place a pure `#000000` is correct rather than lazy: the borders are structural and need maximum definition against cream.

**Neutral Colors:**
- Card White `#FFFFFF` — the default card surface. The neutral counterpart to a Sunflower card; a section normally alternates between the two.
- Ink Secondary `#2C2C2C` — subtitles, captions, helper text, and metadata. The only softening permitted anywhere in the system.

**Accent/State Colors:**
- Focus Ring `#000000` at 3px offset 2px — thicker than most systems because a thin ring disappears against the existing 2px borders.
- Error `#B3261E` — text and a 3px border on the offending field. The field keeps its white fill.
- Success `#1B5E20` — text only, never a fill.
- Disabled — `#F5F5DC` fill, `#2C2C2C` border and label at 50% opacity. The border is never removed; a control without an outline does not read as a control in this system.

**Contrast note:** black on Sunflower is 12.6:1 and black on cream is 18.1:1, so every text pairing clears AAA. White type is never used anywhere — there is no surface in this palette dark enough to carry it.

## Typography

**Display & Headings:** a classical old-style serif for all display type, headings, body copy, and oversized numerals. Google Fonts equivalent: `Crimson Text`, weights 400/600. Fallback: `'Crimson Text', 'Times New Roman', Georgia, serif`.

**UI & Controls:** a neutral grotesque for buttons, tags, inputs, labels, subtitles, and captions. Google Fonts equivalent: `Inter`, weights 400/500/600. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, sans-serif`.

**Type Scale:**
- Display (serif) — `clamp(48px, 8vw, 96px)` / 600 / 1.00 / -0.02em, centered
- Statistic numeral (serif) — `clamp(36px, 6vw, 64px)` / 600 / 1.00 / -0.01em
- Section heading (serif) — `clamp(24px, 4vw, 40px)` / 600 / 1.15 / 0, centered
- Card heading (serif) — `clamp(24px, 4vw, 36px)` / 600 / 1.20 / 0
- Body (serif) — 18px / 400 / 1.55 / 0
- Subtitle (sans) — 18px / 400 / 1.45 / 0, set in Ink Secondary
- Button and tag (sans) — 15px / 500 / 1.00 / 0.01em
- Input (sans) — 16px / 400 / 1.40 / 0
- Caption (sans) — 14px / 400 / 1.40 / 0, set in Ink Secondary

**Hierarchy Rules:** The serif carries meaning and the sans carries mechanics — headings, body, and numerals are serif; anything the user clicks, types into, or filters by is sans. Display type is fluid via `clamp()` rather than stepped at breakpoints, which is what lets a 96px numeral survive a 393px viewport without a media query. Hierarchy is expressed by size, never by color: the system has exactly one text color and one softer variant, so a heading is large rather than colored. Nothing is italic and nothing is set in caps.

## Spacing System

**Base Unit:** 8px.

**Scale:** 8, 16, 24, 32, 48, 64, 96, 128.

**Common Patterns:**
- Page gutter 24px; content measure capped at 1200px.
- Section to section: 64px.
- Section heading to its first card: 32px.
- Card padding 32px on a white card, 24px on a Sunflower card — the yellow cards run tighter because they hold less.
- Card to card in a grid: 24px.
- Button padding 12px 24px. Tag padding 8px 16px. Input padding 12px 16px.
- Input to the next field: 16px. Label to its input: 8px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses `margin-bottom` or longhand padding, never a `padding: 64px 0` shorthand on that same element, which would win on source order and zero the gutter.

## Component Styles

### Buttons

**Primary** — transparent fill, **2px `#000000` border**, `border-radius: 24px` (a true pill), label `#000000` at 15px/500 sans, padding 12px 24px. Hover: fill `#FFD700`, border unchanged. Active: fill `#F7CA00`. The hover *adds* the yellow rather than removing the outline — the border is permanent.

**Emphasis** — as above but with a resting `#FFD700` fill. Used at most once per screen, for the single most important action. Hover: `#F7CA00`.

There is no filled-black button. Black is the outline and the type; a solid black button would out-weigh every card on the page.

### Cards

**White card** — fill `#FFFFFF`, **3px `#000000` border**, 8px radius, 32px padding. The default container for text, forms, and component demonstrations.

**Sunflower card** — fill `#FFD700`, 3px `#000000` border, 8px radius, 24px padding, centered contents. Reserved for statistics, feature callouts, and the one block per section that should be read first.

Card borders are 3px while controls are 2px. That one-pixel difference is what separates a *surface* from a *control*, and it is the system's quietest but most load-bearing rule.

### Statistic Tiles

A Sunflower card containing an oversized serif numeral at `clamp(36px, 6vw, 64px)`, then an 8px gap, then a 14px sans label in `#000000`. Both centered. No icon, no unit superscript, no trend arrow.

### Input Fields

Fill `#FFFFFF`, **2px `#000000` border**, 8px radius, padding 12px 16px, 16px/400 sans in `#000000`. Placeholder in `#2C2C2C`. Focus: border stays black, plus a 3px `#000000` ring at 2px offset — the ring doubles the outline rather than recoloring it. Invalid: 3px `#B3261E` border with the message beneath at 14px in the same red.

### Tags

Transparent fill, 2px `#000000` border, `border-radius: 20px`, padding 8px 16px, 15px/500 sans. Non-interactive at rest. When a tag is a filter, the selected state fills `#FFD700` and the border does not change.

### Color Swatches

A 3px `#000000` border with 8px radius and `overflow: hidden`, so the swatch fill runs to the inside edge of the border with no gap. The label block sits beneath the fill inside the same outlined box, never floating outside it.

### Cursor

The system ships a custom pointer — a white arrow with a black outline — matching the outline-everything logic. It is decorative and must never be the only affordance: every interactive element still carries its own border and hover state.

## Layout Principles

A single centered column capped at 1200px with a 24px gutter, built from stacked sections separated by 64px. Sections are centered — headings and display type sit on the page's center axis — while text inside a white card is left-aligned and text inside a Sunflower card is centered. Card grids run two or three across on desktop and collapse to one column below 600px. Because display type is fluid rather than stepped, the system needs very few breakpoints; the ones it has exist for grid columns and card padding, not for type. Nothing is ever full-bleed: the cream ground always shows around every outlined surface, and that visible margin is what makes the borders read as edges of objects rather than dividers.

## Visual Effects

Borders are the entire visual language: 3px `#000000` on surfaces, 2px on controls, no exceptions. Radii are 8px on cards, swatches, and inputs, and a full pill (20–24px) on buttons and tags. There are no drop shadows, no gradients, no glass, and no blur — depth comes from the outline and from the cream ground showing through between elements. Transitions are 150ms ease on background-color only; borders never animate, and nothing translates, scales, or lifts on hover.

## Design Tone

Bold, playful, and confident, with a retro-modern printed quality. The heavy black outlines and the classical serif give it a tactile, almost analog feeling despite the saturated palette, and the cream ground keeps the yellow from becoming glaring the way it would against white. It reads as a poster that happens to be interactive.

## Usage Notes for AI Implementation

1. **The page ground is cream, not yellow.** `#F5F5DC` is the surface everything sits on. Yellow is a card fill used for emphasis. Making the page yellow removes the contrast that makes the yellow cards mean anything, and it is exactly the error the original spec described.

2. **Every surface and control carries a black border.** 3px on cards, 2px on buttons, inputs, tags, and swatches. A borderless element does not read as part of this system, and removing the outline on hover or focus is the fastest way to break it.

3. **Yellow is a fill, never type and never a border.** Do not set a heading in `#FFD700`, do not use it for a border, and do not tint the ground with it. It has exactly one job.

4. **There is no solid black button.** Black is the outline and the type. A filled-black control would out-weigh every card on the page, which is why the primary button is an outlined pill that only *gains* yellow on hover.

5. **Serif for meaning, sans for mechanics.** Headings, body, and numerals are serif; buttons, tags, inputs, labels, and captions are sans. Setting a button in the serif immediately makes it look like a caption rather than a control.

6. **Keep display type fluid.** `clamp()` on the display, statistic, and heading sizes is why a 96px numeral survives a 393px viewport. Replacing it with fixed sizes plus breakpoints reintroduces horizontal overflow on small screens.

7. **The 3px/2px split is deliberate.** Surfaces are 3px, controls are 2px. Flattening both to the same weight loses the only cue distinguishing a card from a button, since neither has a shadow.

8. **White type is never used.** No surface in this palette is dark enough to carry it. All text is `#000000`, with `#2C2C2C` as the single softer variant for captions and subtitles.

9. **Let the ground show through.** Nothing runs full-bleed and cards never sit flush against each other. The visible cream gap is what makes each outline read as the edge of an object instead of a divider between regions.

10. **Alternate white and Sunflower cards within a section.** A run of three yellow cards flattens into one yellow block and the emphasis disappears. Roughly one Sunflower card per section is the working ratio.
