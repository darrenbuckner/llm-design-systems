---
id: dark-minimal-domain-001
title: Carbon Domain System
tags: [dark, minimal, professional, marketplace, data-heavy, compact]
colors: ["#1a1a1a", "#2a2a2a", "#ff4444", "#00cc66", "#4488ff"]
created: 2026-01-10
---

# Carbon Domain System

A compact, list-first marketplace interface built on a three-step carbon ladder, where every row is a hairline-separated line item and three signal colors do three unambiguous jobs: red acts, green confirms availability, blue prices. Small type, tight spacing, and no decoration — the system is built for scanning hundreds of rows rather than reading a page. Suited to domain marketplaces, inventory tables, server and resource lists, admin consoles, and any surface where density is the feature.

## Color Palette

**Page Surface:** `#1a1a1a` — a near-black carbon ground for the entire interface. Slightly above pure black so that the `#2a2a2a` surface above it remains distinguishable at small sizes, which pure black would not allow at this tight a ladder.

**Neutral Colors — the ladder:**
- Step 0 `#1a1a1a` — page ground
- Step 1 `#2a2a2a` — cards, inputs, tags, and any raised surface
- Step 2 `#333333` — every border and row divider
- Step 3 `#555555` — hover borders and disabled glyphs

Three steps and a hairline is the whole structural vocabulary. Because the ladder is tight, borders do more work here than in most dark systems: a card is `#2a2a2a` *with* a `#333333` border, not one or the other.

**Text Colors:**
- Primary `#ffffff` — domain names, headings, input values, primary button labels.
- Secondary `#cccccc` — body copy, tag labels, secondary button labels.
- Muted `#888888` — metadata, timestamps, placeholder text, table headers.

**Signal Colors — three jobs, no overlap:**
- Action Red `#ff4444` — the primary button fill and nothing else. It is the *buy* color, not an error color.
- Available Green `#00cc66` — the availability status dot. Never a fill, never type.
- Price Blue `#4488ff` — every price figure. Never a button, never a border, never a status.

This three-way split is the system's most distinctive decision. Most interfaces would make red mean error; here red means *act*, and an error is communicated by text plus a red border, never by a red fill.

**Accent/State Colors:**
- Unavailable — the status dot drops to Muted `#888888`. There is no amber or intermediate state.
- Error — a 1px `#ff4444` border on the field and a 12px message in the same red. The button color and the error border share a hue deliberately: nothing else in the interface is red, so the collision never occurs on screen.
- Focus Ring `#4488ff` at 2px offset 2px — blue rather than red, so focus never looks like a call to action.

## Typography

**Display & Headings:** a single neutral system sans across the interface. Google Fonts equivalent: `Inter`, weights 400/500/600. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`.

**Numerals:** tabular figures on every price and count, so a column of prices aligns without manual spacing.

**Type Scale:**
- Page title — 32px / 600 / 1.20 / -0.01em
- Section heading — 24px / 500 / 1.30 / 0
- Row primary (domain name) — 14px / 500 / 1.40 / 0, in Primary
- Row price — 14px / 500 / 1.40 / 0, in Price Blue
- Body — 15px / 400 / 1.50 / 0, in Secondary
- Input — 14px / 400 / 1.40 / 0
- Button — 14px / 500 / 1.00 / 0
- Tag — 12px / 400 / 1.30 / 0, in Secondary
- Metadata — 12px / 400 / 1.40 / 0, in Muted

**Hierarchy Rules:** Body and row type run at 14–15px rather than 16px — this is a density system and the small scale is deliberate, not an oversight. Hierarchy is carried by the two large sizes at the top of a page and then by color: within a row, everything is 14px and the eye separates name from price by white versus blue, not by size or weight. Nothing is italic or all-caps, and there is no bold inside a row — a bolded domain name in a list of two hundred defeats the scan.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64.

**Common Patterns:**
- Page gutter 24px; content measure capped at 1120px.
- Row padding 16px with a 1px `#333333` bottom border; rows are flush, with no gap between them.
- 8px between a status dot and the name it annotates.
- Button padding 8px 16px — compact, matching the row scale.
- Input padding 12px 16px, 16px between stacked fields.
- Card padding 16px. Tag padding 6px 12px.
- Section heading to its list: 32px. Section to section: 48px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses longhand `padding-top` / `padding-bottom`, never a `padding: 48px 0` shorthand on that element, which would win on source order and zero the gutter.

## Component Styles

### List Rows

The system's core component. A flex row at 16px padding with a 1px `#333333` bottom border and **no gap between rows** — they are flush, forming a continuous ruled list. Contents: a 6px status dot, 8px, the name at 14px/500 in Primary taking the remaining width, then the price at 14px/500 in Price Blue pinned right. The final row in a list has no bottom border.

Rows have no fill at rest. Hover fills `#2a2a2a`; there is no border change and nothing moves. Rows are never striped — the hairline is the separation.

### Status Dots

**6px circles**, `border-radius: 50%`, Available Green for available and Muted for taken. Deliberately tiny: at 6px a dot is a glyph rather than a badge, which is what allows it to appear on every row without the list turning into a field of lights.

### Buttons

**Primary** — fill `#ff4444`, label `#ffffff` at 14px/500, 6px radius, padding 8px 16px, no border. Hover: `opacity: 0.85`. Red here means *act*, not *danger*.

**Secondary** — transparent fill, 1px `#333333` border, label `#cccccc`, same radius and padding. Hover: border `#555555`, label `#ffffff`.

Both are compact by design; a 16px 32px button next to a 16px-padded row breaks the density.

### Input Fields

Fill `#2a2a2a`, 1px `#333333` border, 6px radius, padding 12px 16px, 14px in Primary. Placeholder in Muted. Focus: border `#4488ff` plus a 2px blue ring at 2px offset. Invalid: 1px `#ff4444` border with a 12px message beneath in the same red.

### Cards

Fill `#2a2a2a`, 1px `#333333` border, 8px radius, 16px padding, no shadow. Cards hold lists and forms; they are containers rather than content objects, and they never carry a hover state of their own.

### Tags

Fill `#2a2a2a`, 1px `#333333` border, 6px radius, padding 6px 12px, 12px in Secondary. Note the border — on this tight ladder a fill alone at `#2a2a2a` is barely distinguishable from a card, so tags take the same hairline every other surface does.

### Search and Filter Bar

A full-measure input with an optional row of tags beneath acting as active filters. A selected filter tag fills `#333333` and its label lifts to Primary. Filters never use a signal color — red, green, and blue are spoken for.

## Layout Principles

A single centered column capped at 1120px with a 24px gutter. The page is a heading, a search bar, then one or more full-measure lists inside cards. Lists are never placed in a two-column layout — a scanning column that requires horizontal eye movement defeats the purpose. Rows keep the name left and the price right at every breakpoint; below 600px the name column truncates with an ellipsis rather than wrapping, because a two-line row destroys the vertical rhythm the list depends on. Padding and type sizes do not change on mobile — the system is already compact and shrinking it further would break the 44px minimum touch target on row actions.

## Visual Effects

No shadows anywhere — the ladder plus the hairline is the entire depth model. Radii are uniform and small: 8px on cards, 6px on buttons, inputs, and tags, 50% on status dots. Borders are always 1px `#333333`, moving to `#555555` on hover. No gradients, no glass, no blur, no texture. Transitions are 200ms ease on opacity and background-color only. Nothing translates, scales, or lifts.

## Design Tone

Utilitarian and quietly confident. It looks like a tool built by someone who uses it daily — dense, unfussy, and completely uninterested in impressing you. The three signal colors doing three fixed jobs give it an internal logic that becomes invisible once learned, which is the goal for an interface someone opens fifty times a day.

## Usage Notes for AI Implementation

1. **Red means act, not error.** `#ff4444` is the primary button fill. Errors are communicated by a red border plus a message, never by a red fill. Treating red as a danger color removes the system's only call-to-action color.

2. **Three signals, three fixed jobs.** Red acts, green confirms availability, blue prices. None of them ever crosses into another role, and no fourth signal color is added. A green button or a blue badge breaks the logic immediately.

3. **Rows are flush and hairline-separated.** 16px padding, 1px `#333333` bottom border, no gap, no fill at rest, no striping. Adding a gap between rows turns a scannable list into a stack of cards and roughly halves the number of rows on screen.

4. **The small type scale is deliberate.** 14–15px for rows and body. This is a density system; bumping it to 16px to feel more comfortable defeats its only real advantage.

5. **Status dots are 6px.** At that size a dot is a glyph, not a badge, which is what lets it appear on every row without the list becoming a light show.

6. **Borders carry the ladder.** With only `#1a1a1a` and `#2a2a2a` as surfaces, the `#333333` hairline is what makes a card a card. Dropping borders and relying on fill alone flattens the interface at this contrast range.

7. **No bold inside a row.** Everything in a row is 14px/500 and the eye separates name from price by color. A bolded name in a list of two hundred defeats the scan.

8. **Focus rings are blue.** Red is the action color and would make a focused field look like a button. Blue is already the neutral informational hue here.

9. **Names truncate, never wrap.** A two-line row destroys the vertical rhythm the whole list depends on. Use an ellipsis and a title attribute.

10. **Do not shrink for mobile.** The system is already compact. Padding and type stay fixed across breakpoints; the only change is the name column narrowing. Shrinking further breaks the 44px minimum touch target on row actions.
