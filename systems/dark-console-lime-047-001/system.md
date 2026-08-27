---
id: dark-console-lime-047
title: Basalt Console
description: A near-black developer console system built on hairline borders, four barely-separated surface tints, and one electric lime accent.
tags: [dark, developer, dashboard, saas, minimal, cards, onboarding, high-contrast]
colors: ["#04080A", "#0A0D0F", "#D4FE51", "#FCFCFE", "#171B1D"]
created: 2026-08-27
---

# Basalt Console

A near-black console system for developer platforms and account dashboards, built on hairline borders, four barely-separated surface tints, and a single electric lime accent reserved for the one next action on screen. Depth comes entirely from stepping the background one tone deeper; there are no shadows anywhere in the system.

## Color Palette

**Page Surface:** `#04080A` — the ground everywhere, a black carrying a faint blue-green cast. Every other surface is a step up from it.

**Neutral Colors:**
- Rail / sidebar: `#05090B` — one step up, distinguishable from the ground only where they meet a border
- Panel / dialog: `#090C0E` — modals, sheets, the onboarding card
- Card: `#0A0D0F` — feature tiles and content cards resting inside a panel
- Raised / selected: `#131617` — the selected state of an otherwise flat card, and hover on interactive rows
- Field: `#0E1214` — text inputs, search, keyboard chips
- Border hairline: `#171B1D` — the default 1px rule on every card, panel, divider, and quick-link
- Border strong: `#252829` — selected cards, focused fields, and the outline button
- Text primary: `#FCFCFE` — headings, active nav, button labels
- Text secondary: `#A2A3A5` — body copy, descriptions, inactive nav labels
- Text muted: `#808285` — timestamps, group labels, empty-state glyphs, placeholder copy. This is the floor: it clears 4.5:1 against all four surface tints, and anything darker fails on `#131617`.

**Accent Colors:**
- Lime: `#D4FE51` — the primary action, the active nav label, the selected radio. One per view.
- Lime pressed: `#C4EC4C` — the active/pressed state of a lime fill
- Lime tint: `#161C10` — the fill behind an active nav item or a lime badge
- Ink on lime: `#04080A` — the page ground reused as the label color on any lime fill. Never white.

**Accent/State Colors:**
- Info blue: `#2659D6` with tint `#070E1A` and border `#102552` — announcement bars, beta badges, informational callouts. Informational only; it never marks something to click.
- Success: `#56BC77` on tint `#0F1915` — confirmation checks and completed states
- Warning: `#E8B23A` on tint `#1A1509` — budget thresholds and soft limits
- Error: `#E5484D` on tint `#1A0D0E` — failed requests, invalid keys
- Focus ring: `#D4FE51` at 45% opacity, 2px, offset 2px from the element

## Typography

**Font Families:** A single geometric grotesque carries the entire system — near-circular bowls, tall x-height, straight-tailed `y`, angled cuts on `t` and `c`. Google Fonts equivalent: `DM Sans`, with `Outfit` as an acceptable substitute. Stack: `'DM Sans', -apple-system, 'Segoe UI', system-ui, sans-serif`. Monospace appears only in keyboard chips, key fragments, and hex values: `'JetBrains Mono', ui-monospace, 'SF Mono', monospace`.

**Display & Headings:** Sans. The system has no serif at any level.

**Type Scale:**
| Level | Size | Weight | Line-height | Tracking |
|---|---|---|---|---|
| Dialog title | 32px | 700 | 1.15 | -0.02em |
| Page title | 28px | 700 | 1.2 | -0.02em |
| Section heading | 20px | 500 | 1.3 | -0.01em |
| Card title | 17px | 500 | 1.35 | 0 |
| Body | 16px | 400 | 1.5 | 0 |
| Card description | 15px | 400 | 1.75 | 0 |
| Meta / small | 14px | 400 | 1.45 | 0 |
| Nav label | 15px | 500 | 1.2 | 0 |
| Badge | 11px | 500 | 1.1 | 0.02em |
| Mono chip | 12px | 500 | 1 | 0 |

**Hierarchy Rules:** Weight and color do the work; size steps are small and there are only three of them above body. Headings are always `#FCFCFE` at 500 or 700 and never lime — lime marks action, not importance. Descriptive copy inside a card is set at 15px with a deliberately loose 1.75 line-height, which is the single most identifying typographic move in the system. Nothing is centered except a modal's confirmation state. Sentence case everywhere, including badges and buttons; no all-caps labels. Numerals are tabular in any usage or metrics figure.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80.

**Common Patterns:**
- Page gutter: 20px mobile, 32px tablet, 48px desktop
- Sidebar width: 280px fixed on desktop, collapsing to a top bar below 900px
- Dialog padding: 32px mobile, 48px desktop
- Card padding: 20px mobile, 24px desktop
- Grid gap between sibling cards: 16px
- Gap between a card title and its description: 16px
- Gap between section heading and its grid: 20px
- Vertical rhythm between sections: 48px
- Nav item: 10px vertical, 12px horizontal, 4px between items
- Icon-to-label gap: 12px

Spacing is generous vertically and tight horizontally. Cards sit close together in the grid and breathe internally.

## Component Styles

### Buttons

**Primary:** `#D4FE51` fill, `#04080A` label at 16px/500, 10px radius, 14px vertical and 28px horizontal padding, no border, no shadow. Hover lifts to `#DDFF6E`; active drops to `#C4EC4C`. Full-width on mobile, auto-width and right-aligned in a dialog footer.

**Secondary:** transparent fill, 1px `#171B1D` border, `#FCFCFE` label, same geometry as primary. Hover fills `#0E1214` and moves the border to `#252829`. Optional 18px leading outline icon.

**Ghost:** no fill, no border, `#A2A3A5` label. Hover moves the label to `#FCFCFE`. Used for dismissals and tertiary links.

All buttons keep a 44px minimum height and animate `background-color`, `border-color`, and `color` over 150ms ease.

### Cards & Panels

A panel is `#090C0E` on a 1px `#171B1D` border at 16px radius, holding the page's primary content. A card is `#0A0D0F` at 12px radius with the same hairline border, and nests inside a panel or sits directly on the ground. Neither ever takes a shadow. Hover on an interactive card moves the fill to `#131617` and the border to `#252829` — that pairing is the entire hover language of the system.

Card composition, top to bottom: a 20px outline icon in `#FCFCFE`, 20px gap, a 17px/500 title, 16px gap, a 15px description at 1.75 line-height in `#A2A3A5`.

### Selectable Option Cards

A radio choice rendered as a full card: 12px radius, 24px padding, an optional 40px circular icon tile at `#131617` on the left, title and description stacked in the middle, and a 20px radio control pinned top-right.

Unselected is `#0A0D0F` on `#171B1D` with a 2px `#3A3D3F` ring for the radio. Selected raises the fill to `#131617`, the border to `#252829`, and fills the radio with a 2px `#D4FE51` ring around a 8px `#D4FE51` dot. Both changes fire together — the tint alone is too subtle to read as a selection, and the radio alone gets missed on a wide card.

### Input Fields & Search

`#0E1214` fill, 1px `#171B1D` border, 10px radius, 12px vertical and 16px horizontal padding, 16px text in `#FCFCFE`, placeholder in `#808285`. A leading 18px outline icon sits 16px from the left edge with 12px to the text. Focus moves the border to `#252829` and adds the lime focus ring; the fill does not change.

A search field may carry a trailing keyboard chip: `#0E1214` fill, 1px `#212426` border, 6px radius, 4px by 8px padding, 12px mono in `#808285`.

### Sidebar Navigation

A 280px rail at `#05090B` with a 1px `#171B1D` right border. Items are 8px-radius rows with a 20px outline icon and a 15px/500 label in `#A2A3A5`. Hover moves the label to `#FCFCFE` with no fill. The active item takes a `#161C10` fill with both icon and label in `#D4FE51` — no left indicator bar, no bold weight change.

Group labels above a section are 11px/500 in `#808285` with 0.06em tracking, uppercase, and 24px of space above them. A workspace switcher sits at the top of the rail as a full-width `#0A0D0F` row with a trailing chevron.

### Badges & Chips

11px/500 sentence-case labels in a 6px-radius pill with 3px by 8px padding. Three variants: info (`#070E1A` fill, `#102552` border, `#5B87F0` label), accent (`#161C10` fill, no border, `#D4FE51` label), and neutral (`#131617` fill, no border, `#A2A3A5` label). Badges never carry an icon and never wrap.

### Banners & Callouts

A full-width announcement strip sits above the header at `#070E1A` with a 1px `#102552` bottom border, 14px centered text in `#FCFCFE`, an inline link underlined in `#5B87F0`, and a ghost dismiss button at the right edge. An in-page callout uses the same fill and border at 12px radius with 20px padding, a 15px/500 title, and a 15px description in `#A2A3A5`.

### Empty States

Inside a card at its normal size: a 40px bar-chart or document glyph in `#808285` above a 17px/400 sentence in `#A2A3A5`, both centered, with 56px minimum vertical padding. The sentence names the metric and the window — "No requests this week" — and there is no illustration, no call to action, and no border change.

### Quick-Link Rows

A card whose content is a 36px `#0A0D0F` icon tile at 10px radius, a 17px/500 title, a 15px description at 1.5, and a 20px chevron in `#808285` pinned to the right edge and vertically centered. Hover moves the card fill to `#131617` and the chevron to `#FCFCFE`. These tile in a three-column grid on desktop and stack on mobile.

## Layout Principles

The desktop shell is a fixed 280px rail plus a fluid content column capped at 1440px, with the content column carrying the page gutter. Below 900px the rail unpins into a full-width top bar: the workspace switcher spans the width and the nav items wrap into rows of chips, with no drawer and no hamburger.

Content grids are three-up on desktop, two-up between 700px and 1100px, and one-up below. A grid never partially fills a row with an orphan card — three items or six, not four.

Dialogs are centered with a 720px maximum width and 48px of internal padding, and their action row is right-aligned with the primary button last. Progress through a multi-step dialog is shown as a row of 8px dots below the card, the active one lime and the rest `#252829`.

Everything is left-aligned. Content sits at the top of its container and does not vertically center except inside an empty state or a confirmation dialog.

## Visual Effects

**Radii:** 6px badges and keyboard chips, 8px nav rows, 10px buttons, fields, and icon tiles, 12px cards and callouts, 16px panels and dialogs, full round only on radios and avatars.

**Shadows:** none. There is no elevation system. A surface that needs to read as raised steps one tint deeper — `#04080A` to `#0A0D0F` to `#131617` — and gains a border. This is the system's defining constraint.

**Borders:** exactly 1px, `#171B1D` at rest and `#252829` on selection or focus. Border weight never increases; a heavier structure is expressed by moving to a stronger tint, not a thicker rule.

**Icons:** 20px outline glyphs at 1.5px stroke, never filled, always `#FCFCFE` or `#A2A3A5` — the sole exception is the lime pair in an active nav row.

**Transitions:** 150ms ease on `background-color`, `border-color`, and `color`. Nothing moves, scales, or translates on hover. No blur, no glow, no gradient anywhere in the system.

## Design Tone

Instrument-panel calm — a near-black surface where structure is drawn in hairlines rather than shadows, and a single electric lime tells you the one thing to do next. It reads as a tool for people who already know what they are doing: dense enough to be efficient, quiet enough to sit open all day, and confident enough that the accent appears once per screen and means it.

## Usage Notes for AI Implementation

1. One lime element per view. It marks the single next action — the primary button, the active nav row, the selected option — and a second one destroys the hierarchy the whole palette exists to create.
2. Never add a shadow. Depth is a tint step: `#04080A` → `#0A0D0F` → `#131617`. Adding elevation makes this a generic dark theme, and the flatness is the point.
3. Lime fills always carry `#04080A` ink. White on `#D4FE51` fails contrast and looks unfinished; the ground color reused as ink is what makes the accent feel native.
4. Keep the ground at `#04080A`. Lightening it toward `#111111` or `#1A1A1A` collapses the four surface tints into indistinguishable grays and the entire structure disappears.
5. Card descriptions run at 15px with 1.75 line-height. Tightening that to 1.5 to fit more copy is the fastest way to make this read like every other SaaS dashboard.
6. Blue is informational and never actionable. Announcement bars, beta badges, and callouts use it; nothing the user clicks to proceed does.
7. Hover is a two-property change — fill to `#131617`, border to `#252829` — applied together. Changing one alone reads as a rendering glitch rather than a state.
8. Selection needs both signals. A selected option card raises its tint *and* lights its control. Either one alone gets missed at a glance.
9. Empty states stay inside the card at full size with a muted glyph and a plain sentence naming the metric and window. No illustration, no "get started" button, no border treatment.
10. Icons stay outline at 1.5px stroke and stay monochrome. Colored or filled icons are the wrong register for this system entirely.
11. Everything is sentence case, including badges and buttons. All-caps labels read as a different, louder product.
12. On mobile the rail unpins into a wrapping top bar rather than a drawer overlay, grids go single-column, and the primary button goes full-width. Nothing else about the system adapts.
