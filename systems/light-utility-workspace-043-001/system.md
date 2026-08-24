---
id: light-utility-workspace-043
title: Juniper Workspace System
description: A restrained white-ground workspace UI where a single desaturated green carries every action and hairline borders replace shadows entirely.
tags: [light, minimal, professional, cards, modern, sans]
colors: ["#FFFFFF", "#377C70", "#1C1C1C", "#EBEBEB", "#F5C25E"]
created: 2026-08-23
---

# Juniper Workspace System

A document-workspace interface built on near-total white, where a single desaturated juniper green carries every primary action and hairline gray borders do all the structural work that shadows would normally do. Hierarchy comes from weight and ink level, not color or elevation. Suited to file managers, document libraries, admin consoles, and any tool where the user's own content should be the loudest thing on screen.

## Color Palette

**Page Surface:** `#FFFFFF` — the ground for every screen, sidebar, card, panel, and input. There is no second background tone; surfaces are distinguished by border, not fill.

**Primary Colors:**
- Juniper Green `#377C70` — primary button fill, primary CTA fill, brand mark. The only chromatic color in the working interface.
- Juniper Deep `#2D695E` — hover and active state for every green fill. Never used as a resting color.
- Juniper Wash `#EEF4F2` — the tint behind green-accented rows and selected states in green context. Used sparingly, roughly once per screen.

**Neutral Colors:**
- Tint `#EBEBEB` — filled chips, active navigation item, hovered rows, avatar grounds. The workhorse neutral fill.
- Hairline `#D9D9D9` — every border: cards, inputs, panels, dividers, popovers. 1px everywhere except popovers, which take 2px.
- Ink `#1C1C1C` — headings, card titles, button labels on light fills, active navigation label. Near-black, never pure `#000000`.
- Ink Secondary `#3F3F3F` — body copy inside panels and popovers.
- Ink Muted `#707070` — descriptions, section labels, timestamps, inactive navigation labels, icon strokes.
- Ink Faint `#7F7F7F` — the heavier input border and the overflow menu glyphs.

**Accent/State Colors:**
- Badge Amber `#F5C25E` — plan and tier badges only, with `#1C1C1C` ink on top. Never a button, never a background.
- Success `#377C70` — reuses the primary green; the system does not introduce a second green.
- Warning `#B8791F` — inline warnings, text and icon only.
- Error `#B4342A` — destructive confirmation text and invalid input borders.
- Focus Ring `#377C70` at 2px offset 2px — identical on every focusable element.

## Typography

**Display & Headings:** the same sans-serif face as body, differentiated by weight alone.

**Font Families:** A single geometric-humanist sans-serif across the entire system — one family, four weights, no exceptions. Google Fonts equivalent: `Figtree`, weights 400/500/600/700. Fallback chain: `'Figtree', 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`. The system deliberately carries no second face: no serif for display, no alternate sans for UI chrome.

**Type Scale:**
- Page title — 36px / 700 / 1.15 / -0.02em
- Panel headline — 20px / 700 / 1.3 / -0.01em
- Card title — 20px / 700 / 1.35 / -0.01em, truncated to one line with ellipsis
- Body — 17px / 400 / 1.5 / 0
- Navigation label — 17px / 500 / 1.4 / 0
- Button label — 16px / 600 / 1.2 / 0
- Card meta — 16px / 400 / 1.5 / 0, set in Ink Muted
- Section label — 15px / 500 / 1.4 / 0, set in Ink Muted, sentence case
- Chip / timestamp — 14px / 500 / 1.3 / 0

**Hierarchy Rules:** Weight and ink level do all the work — a card title and a card description are two steps apart in weight (700 vs 400) and two steps apart in ink (`#1C1C1C` vs `#707070`) at nearly the same size. Never use color to signal hierarchy; green is reserved for action. Never use all-caps or letterspaced small caps for section labels — they stay sentence case at 15px in muted ink. Card titles truncate rather than wrap; descriptions wrap to two lines then truncate. Nothing is centered except the empty state and the footer.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64.

**Common Patterns:**
- Sidebar width 240px fixed; sidebar item padding 14px 16px; 16px gap between icon and label; 4px vertical gap between items.
- Page gutter 48px desktop, 32px tablet, 20px mobile.
- Header row to first content block: 40px.
- Card interior padding 24px; 16px between the chip row and the title; 12px between title and description; 20px between description and timestamp.
- Card grid gap 24px, four columns at 1200px+, two at 768px, one below.
- Button padding 12px 20px; split-button chevron segment 12px 14px with a 1px hairline divider between segments.
- Input padding 12px 16px with a 40px left inset when a leading icon is present.
- Popover padding 28px; 16px between headline and body; 24px between body and the right-aligned action.

## Component Styles

### Buttons

**Primary** — fill `#377C70`, label `#FFFFFF` at 16px/600, radius 8px, padding 12px 20px, no border, no shadow. Hover: fill `#2D695E`. Active: fill `#2D695E` with no transform. Focus: 2px `#377C70` ring at 2px offset. Disabled: fill `#EBEBEB`, label `#707070`.

**Secondary** — fill `#FFFFFF`, 1px `#D9D9D9` border, label `#1C1C1C`, same radius and padding. Hover: fill `#EBEBEB`, border unchanged. This is the default for utility actions like Upload.

**Split** — a primary or secondary button joined to a 44px chevron segment sharing the same fill and outer radius, separated by a 1px divider (`rgba(255,255,255,0.28)` on green fills, `#D9D9D9` on white). The whole unit shares one border radius; only the outer corners round.

**Ghost** — no fill, no border, label `#707070`. Hover: fill `#EBEBEB`, label `#1C1C1C`. Used for overflow menus and sidebar items.

### Cards & Panels

White fill, 1px `#D9D9D9` border, 10px radius, 24px padding, **no shadow at any state**. Hover: border darkens to `#7F7F7F`, nothing else moves — no lift, no scale, no shadow. Internal order is fixed: a chip row with the overflow glyph pushed right, then a 20px/700 title, then a 16px description in Ink Secondary, then a 16px preview line in Ink Muted, then a 14px timestamp in Ink Muted.

### Popovers & Coachmarks

White fill, **2px** `#D9D9D9` border, 12px radius, 28px padding, and the one place a shadow is permitted: `0 4px 24px rgba(28,28,28,0.10)`. A 12px triangular pointer in the same fill and border color anchors it to its trigger. A 20px close glyph sits top-right in Ink Muted. The action is a single primary button, right-aligned, never a pair.

### Input Fields

White fill, 1px `#7F7F7F` border — deliberately heavier than the `#D9D9D9` used on cards, so inputs read as the most interactive thing in a view. Radius 8px, padding 12px 16px, 17px/400 text. Leading icons sit 16px from the left edge in Ink Muted with a 40px text inset. Placeholder in Ink Muted. Focus: border `#377C70` plus a 2px `#377C70` ring at 2px offset. Invalid: border `#B4342A`, with the message below at 15px in the same color.

### Chips & Badges

**Type chip** — fill `#EBEBEB`, ink `#1C1C1C`, 14px/500, padding 6px 14px, fully rounded pill. Non-interactive.

**Tier badge** — fill `#F5C25E`, ink `#1C1C1C`, 14px/600, padding 6px 14px, fully rounded pill. Reserved for plan and tier only.

**Count badge** — fill `#377C70`, ink `#FFFFFF`, 13px/600, 24px circle, right-aligned in navigation rows.

### Navigation

A fixed 240px white sidebar separated from content by a 1px `#D9D9D9` right border. Rows are 24px icon plus 17px/500 label, 16px gap, 14px 16px padding, 8px radius. Resting label Ink Muted with matching icon stroke. Hover: fill `#EBEBEB`. Active: fill `#EBEBEB` with label and icon promoted to `#1C1C1C` — the fill is the same as hover, so weight of ink is what distinguishes active from hovered. A 1px `#D9D9D9` divider separates the primary group from the account group pinned to the bottom.

### Lists & Dividers

Hairline `#D9D9D9` rules at full container width, never inset, never doubled. Section labels sit 15px/500 in Ink Muted, 16px above the first row, with no rule beneath them.

## Layout Principles

Fixed 240px sidebar plus a fluid content column with a 1440px max width and 48px gutters. Content is grid-first: four card columns above 1200px, two between 768px and 1200px, one below, with a constant 24px gap at every breakpoint. The page header is a single row — title, then primary and secondary actions grouped left, then search pushed hard right — and it collapses to a stacked title / action row / full-width search on mobile. The sidebar becomes an off-canvas drawer below 768px, not a bottom bar. Body copy inside panels is capped at 60 characters; card descriptions are capped by the card, not by measure.

## Visual Effects

Radii: 8px on buttons, inputs, and navigation rows; 10px on cards; 12px on popovers; 999px on chips and badges. Borders are 1px hairline `#D9D9D9` everywhere except inputs (1px `#7F7F7F`) and popovers (2px `#D9D9D9`). The system is functionally shadowless — the only permitted shadow is `0 4px 24px rgba(28,28,28,0.10)` on floating layers (popovers, dropdown menus, modals), and it must never appear on a card, button, or panel that sits in the document flow. Transitions are 120ms ease on background-color, border-color, and color only; nothing translates, scales, or fades. There are no gradients, no glass, no texture, and no illustration.

## Design Tone

Quiet, dense, and utility-first — an interface that gets out of the way of the user's own documents. The near-total absence of color makes the single juniper green read as unmistakably actionable, and the shadowless hairline construction gives it a flat, engineering-drawing calm rather than a soft consumer polish. It feels like a tool that expects to be used every day for years.

## Usage Notes for AI Implementation

1. **Never add shadows to in-flow elements.** Cards, buttons, panels, and inputs are separated by border alone. If two surfaces need distinguishing, add a hairline, not elevation. The moment cards get a shadow this becomes a generic SaaS dashboard.

2. **Green is a marker, not a palette.** Roughly one to three green elements per screenful — the primary button, a count badge, a focus ring. If green starts appearing in headings, links, icons, or backgrounds, the system is broken. Everything else is white, three grays, and near-black.

3. **Inputs get a heavier border than cards.** `#7F7F7F` on inputs against `#D9D9D9` on cards is deliberate, not an inconsistency. It's how the system signals interactivity without color.

4. **Do not introduce a second surface tone.** There is no `#FAFAFA` page background with white cards. The page and the cards are both `#FFFFFF`, and `#EBEBEB` is a fill for chips and hovered rows only — never a large area.

5. **Hierarchy is weight plus ink, at nearly the same size.** A 20px/700 `#1C1C1C` title over a 16px/400 `#707070` description is the core pattern. Resist widening the size gap; the density is the point.

6. **The amber badge is singular.** One tier badge per screen, top-left near the mark. It is never a button, never a background fill, and never joined by a second amber element.

7. **Hover changes color, never position.** No lift, no scale, no shadow bloom. Card hover darkens the border; button hover darkens the fill; row hover adds the `#EBEBEB` tint. 120ms, color properties only.

8. **Keep the sidebar labels muted at rest.** Active state promotes ink to `#1C1C1C` while sharing the same `#EBEBEB` fill as hover — that ink shift is the entire active affordance. Do not add a left accent bar or a green fill.
