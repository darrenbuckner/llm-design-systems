---
id: light-pastel-marquee-055
title: Sherbet Marquee System
description: A high-contrast white-ground event system pairing oversized medium-weight grotesque display type with monospaced uppercase utility labels and wide pastel bands.
tags: [light, bold, playful, colorful, rounded, mobile-first, monospace, marketing, celebration]
colors: ["#FFFFFF", "#000000", "#ECF6D4", "#EBEBFD", "#FEFF56"]
created: 2026-09-06
---

# Sherbet Marquee System

Sherbet Marquee is a high-contrast light system for event, festival, and program marketing: oversized medium-weight grotesque headlines on pure white, monospaced uppercase utility labels, full-round black pill buttons, and wide pastel bands in sherbet greens, lavenders, and creams that segment the page without a single shadow. Everything is flat. Depth comes from tint steps and hairline rules, hierarchy comes from scale, and the whole page reads as printed signage rather than as software.

The system's defining tension is between two voices. Display type is enormous and set at medium weight, never bold, so it reads as confident rather than shouty. Everything functional around it — dates, venue lines, save banners, eyebrow labels — drops into a widely tracked uppercase monospace at 12–13px. The mono is not decoration; it is the system's way of marking anything that is a fact rather than a claim.

## Color Palette

**Page Surface:** `#FFFFFF` — the ground under every section. Never tinted globally; tinting is done by discrete full-width bands.

**Primary Colors:**
- Ink — `#000000` — all display type, body copy, primary button fills, icon strokes. True black, not a softened near-black.
- Accent Blue — `#3787F9` — focus rings, active-state fills, and selection indicators. A non-text signal only; it measures 3.5:1 on white and 3.07:1 on Chip Fill, so it clears the 3:1 bar for graphical indicators and clears nothing else.
- Accent Blue Deep — `#1F5FC4` — the same signal wherever it carries a glyph or a word: menu toggles, close controls, icon strokes. 5.28:1 on Chip Fill, 6.01:1 on white.
- Highlight Yellow — `#FEFF56` — a marker highlight sitting behind a single word ("New", "Now", "Last"). Never a fill for a button or a whole block.

**Neutral Colors:**
- Panel Tint — `#F4F4F4` — grouped list panels and the raised surfaces inside white sections.
- Chip Fill — `#F0F0F0` — pill chips, segmented nav items, and inactive tabs.
- Rule Strong — `#707070` — hairline rules separating rows *inside* a tinted panel. Deliberately mid-gray, not faint.
- Rule Soft — `#D9D9D9` — section separators and accordion rules on the white ground.
- Ink Secondary — `#4A4A4A` — deck copy, subheads under a display line, footer text.
- Ink Tertiary — `#6B6B6B` — captions, disabled labels, swatch metadata.

**Band Colors:** Full-width tinted blocks used to segment a long page. Each is a pastel at roughly 92–96% lightness, so black type sits on it at full contrast.
- Band Mint — `#ECF6D4`
- Band Lavender — `#EBEBFD`
- Band Cream — `#FCF2CF`

**Iridescent Surface:** A single product/feature card takes a four-stop pastel wash running top-left to bottom-right: `#E1FDF1` → `#E5FCEA` → `#F4F3E1` → `#FBEFE1`. Reserved for one card per page.

**Accent/State Colors:**
- Success — `#2E7D4F`
- Warning — `#B26A00`
- Error — `#C62828`
- Focus ring — `#3787F9` at 2px offset 2px
- Disabled — Chip Fill background with Ink Tertiary text

## Typography

**Font Families:**
- **Display & Headings:** Geometric grotesque sans with a tall x-height and tight apertures — `'Archivo', 'Helvetica Neue', Arial, sans-serif`.
- **Body:** The same grotesque at 400, so the page has one voice for reading — `'Archivo', 'Helvetica Neue', Arial, sans-serif`.
- **Utility:** Typewriter-derived monospace for dates, venue lines, eyebrows, and banner text — `'IBM Plex Mono', 'SFMono-Regular', Menlo, monospace`.

**Type Scale:**
| Level | Size | Weight | Line height | Tracking |
|---|---|---|---|---|
| Display XL | `clamp(40px, 11vw, 76px)` | 500 | 1.02 | -0.025em |
| Display L | `clamp(30px, 8vw, 48px)` | 500 | 1.06 | -0.02em |
| Heading M | 24px | 500 | 1.2 | -0.01em |
| Heading S | 19px | 600 | 1.3 | 0 |
| Body L | 18px | 400 | 1.5 | 0 |
| Body | 16px | 400 | 1.55 | 0 |
| Utility Label | 13px | 500 | 1.4 | 0.12em, uppercase |
| Micro | 12px | 500 | 1.4 | 0.08em, uppercase |

**Hierarchy Rules:**
- Display levels are always weight 500. Weight 700 appears only in button labels, prices, table values, and inline emphasis inside body copy. A bold display line is out of system.
- Display XL is centered and wraps to two or three lines by design; the wrap is part of the composition, so the measure is capped rather than the font shrunk.
- Section headings (Display L) are left-aligned and flush to the gutter. Only hero-level display type is centered.
- Anything that states a fact rather than makes a claim — dates, locations, group sizes, banner copy, eyebrows — is set in the mono at 12–13px uppercase with 0.08–0.12em tracking. Never mix mono into running prose.
- Links inside body copy are underlined and bold, with a trailing `›`. No color change; the underline carries the affordance.
- Numerals in list rows and prices are weight 700 and right-aligned against a left-aligned label.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96, 128.

**Common Patterns:**
- Page gutter: 20px below 768px, 48px at 768–1199px, 64px at 1200px+.
- Section rhythm: 64px vertical padding on mobile, 96px at 768px+, 128px for a hero band.
- Band blocks: 48px internal padding on mobile, 64px at 768px+, with 32px between stacked bands.
- Panel padding: 24px, with 24px vertical padding per list row.
- Button padding: 18px vertical, 40px horizontal (pill).
- Chip padding: 12px vertical, 20px horizontal; 12px gap in the chip rail.
- Gap between a display line and its deck: 24px. Between a deck and the first control: 40px.
- Masthead: 20px above the wordmark row, 16px between it and the mono datestamp line, 20px below, then a 1px Rule Soft.

## Component Styles

### Masthead

Sticky white header on the page ground. A heavy wordmark block sits left, closed by a small solid triangle glyph; one or two circular 48px controls sit right, filled Chip Fill with Accent Blue Deep glyphs. Directly beneath the wordmark, a mono uppercase datestamp line at 13px / 0.12em tracking states the fixed facts of the event — dates, then a pipe, then the location. The whole masthead closes with a 1px Rule Soft, never a shadow. The header owns its own gutter and sets vertical rhythm with `padding-top` / `padding-bottom` longhand.

### Buttons

- **Primary:** Ink fill, `#FFFFFF` label at 17px/700, radius `999px`, padding 18px/40px, full-width on mobile and auto-width at 768px+. Hover drops the fill to `#1F1F1F`; active drops to `#333333`. No shadow, no lift, no scale.
- **Secondary:** `#FFFFFF` fill, 1.5px Ink border, Ink label. Hover fills Panel Tint.
- **Ghost link:** No fill. Bold 16px Ink label, 2px underline offset 4px, trailing `›` with 6px of space. Hover thickens the underline to 3px.
- All buttons are at least 48px tall. Focus is a 2px Accent Blue ring at 2px offset, never a border swap.

### Chip Rail

A row of pills used for in-page section navigation, sitting directly under the masthead with no heading above it. Each chip is Chip Fill, radius `999px`, 15px/500 Ink label, `white-space: nowrap` internally, 48px minimum height, 12px gap. The rail wraps rather than scrolls: `flex-wrap: wrap` plus `min-width: 0` on the container, so a long chip set becomes two lines instead of forcing horizontal overflow. The active chip inverts to Ink fill with a white label. A chip can carry a Highlight Yellow inline marker before its label for new sections.

### Grouped List Panel

The system's signature data container. A Panel Tint block at radius 16px holds a stack of rows. Each row is a flex line, 24px vertical padding, label left in 17px/400 Ink and value right in 17px/700 Ink. Rows are separated by a 1px Rule Strong hairline that is inset 16px from each side and omitted after the last row. There is no header row and no zebra striping — the tint plus the mid-gray rule does all the separation work.

### Band Block

A full-width tinted section carrying a Band color, radius 20px when inset in the page flow and square when truly full-bleed. It is a block-level element at the page's natural width holding its own background, with a nested gutter element inside for content — never negative viewport margins. Content is centered: a Heading M or Display L, a one-line deck in Ink Secondary, then a single primary button. One idea per band, one button per band.

### Feature Card

A single card per page carrying the iridescent four-stop wash, radius 20px, 32px padding. Inside: a Display L title, a 32px/700 price line, a 17px description at Ink Secondary capped at a 34-character measure, then a Heading S label and a bulleted feature list at 17px with 12px between items. On desktop it becomes a 1.1fr / 0.9fr split, the second column holding translucent white tiles (`rgba(255,255,255,0.55)`, radius 16px) that carry a mono micro-label above an oversized 700-weight numeral. This card is the page's only gradient; a second one flattens the effect.

### Accordion

Used for FAQ stacks on the white ground. Each row is a full-width button, 28px vertical padding, question left in 19px/400 Ink capped at a 34-character measure, and a 24px `+` glyph right in Ink that rotates 45° to become `×` when open. Rows are separated by 1px Rule Soft, full width with no inset. Open panels reveal 17px body copy at Ink Secondary with 20px of top spacing. Transition is 180ms ease on the glyph rotation only; the panel height is not animated.

### Utility Banner

A dismissible Band Cream strip pinned above the page footer or inside the menu overlay, radius 12px, 20px/24px padding. Content is mono uppercase 12px at 0.08em tracking across two columns — a static label left, an underlined action right — with a 24px `×` dismiss control. It is the one place where two mono strings sit side by side.

### Input Fields

`#FFFFFF` fill, 1.5px Rule Soft border, radius 12px, 16px/18px padding, 16px/400 Ink text, placeholder at Ink Tertiary. Labels sit above in Utility Label mono. Focus swaps the border to Ink and adds a 2px Accent Blue ring at 2px offset. Error state swaps the border to Error with a 13px message beneath. Minimum height 52px.

## Layout Principles

- Mobile-first and single-column by default. The desktop adaptation is wider gutters, a two-column feature card, and a chip rail that stops scrolling — not a new grid.
- Content max-width is 1080px, centered with `margin-left: auto; margin-right: auto`. Display copy is capped tighter, at a 720px measure, so hero lines break where intended.
- One element owns the horizontal gutter per section. Any class sharing that element sets vertical rhythm with `padding-top` / `padding-bottom` longhand so the shorthand never zeroes the gutter.
- Vertical rhythm carries the structure. There are no vertical rules, no sidebars, and no boxed layouts around body content.
- Alternate white sections and Band blocks down the page. Two adjacent bands of different colors read as a color demo rather than as structure.
- Media is always a rounded rectangle at radius 16px, full-bleed to the gutter, 16:10 on mobile and 16:9 at 768px+.
- Grid and flex children holding long content take `min-width: 0`; specimen text takes `overflow-wrap: anywhere`.

## Visual Effects

- **Radii:** `999px` for buttons and chips; 20px for bands and the feature card; 16px for panels and media; 12px for inputs and the utility banner. Nothing is square except full-bleed bands.
- **Shadows:** None anywhere. Elevation is expressed by stepping the surface one tint deeper — `#FFFFFF` → `#F4F4F4` → a Band color.
- **Borders:** 1px hairlines only, in Rule Strong inside tinted panels and Rule Soft on the white ground. Interactive borders are 1.5px.
- **Backgrounds:** Flat fills throughout. The single iridescent wash is the only gradient in the system.
- **Transitions:** 180ms ease on background-color, border-color, and transform. Nothing longer, nothing bouncing.
- **Motion:** Hover changes fill, never position. No lifts, no scaling, no parallax.

## Design Tone

Confident festival signage translated to a screen — enormous but unbolded display type on pure white, hard black controls, and sherbet-pastel bands that make a long marketing page navigable by color rather than by chrome. It feels institutional and playful at once: the mono utility labels give it the precision of a printed program, while the mint, lavender, and cream blocks keep it from reading as corporate. The absence of shadow is what holds it together; every surface sits flat on the page and earns its separation from tint and hairline alone.

## Usage Notes for AI Implementation

1. Never set display type at weight 700. The medium-weight-at-huge-size relationship is the whole voice; bolding it turns the system into a generic conversion landing page.
2. Keep the mono strictly to facts — dates, locations, quantities, banner strings, eyebrows. The moment a sentence of persuasion appears in mono, the system reads as a developer tool rather than an event program.
3. Add no shadows, ever. If something needs to separate from its surroundings, step the background one tone deeper or add a hairline. A single `box-shadow` breaks the printed-signage read across the whole page.
4. Use one Band color per section and alternate with white. Stacking mint against lavender against cream with no white between them turns structure into a swatch demo.
5. Ship exactly one iridescent surface per page. It is the visual reward for the primary offer; a second one halves the effect of both.
6. The highlight yellow marks one word, never a block. Treat it as a physical highlighter stroke behind a label — not as a button fill, a card background, or a border.
7. Hairlines inside tinted panels are mid-gray (`#707070`), not faint. Softening them to `#E5E5E5` makes the grouped list panel dissolve, which is the most common way this system gets watered down.
8. Blue appears only on interactive chrome, and which blue depends on whether it carries a shape or a symbol: `#3787F9` for rings, fills, and selection indicators, `#1F5FC4` the moment it becomes a glyph or a label. Using the lighter blue on an icon ships a 3.07:1 control. Neither blue is ever used for links, buttons, or headings — links carry their affordance through a bold underline and a trailing chevron.
9. Center only hero-level display type. Every section heading, list row, and body paragraph is left-aligned to the gutter, and centering them flattens the hierarchy into a template.
10. Keep the desktop adaptation to wider gutters, a two-column feature card, and a wrapped chip rail. Introducing a multi-column grid or a sidebar contradicts the single-column vertical rhythm the whole system is built on.
