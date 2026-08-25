---
id: light-serif-report-044
title: Tidewater Report System
description: A pale aqua research-report layout where a five-step monochromatic teal ladder replaces every border and shadow, and a transitional serif carries all display type.
tags: [light, editorial, professional, serif, minimal, cards]
colors: ["#F5FAFB", "#D1E9EC", "#9DD1D3", "#245860", "#221F20"]
created: 2026-08-24
---

# Tidewater Report System

A long-form research report layout built on a pale aqua ground, where structure comes entirely from a five-step monochromatic teal ladder — no borders, no shadows, no rules anywhere on the page. A transitional serif carries every display line and pull quote while a geometric sans handles all body copy and data labels. Suited to whitepapers, annual reports, survey findings, industry briefs, and any long document that needs to read as considered rather than promotional.

## Color Palette

**Page Surface:** `#F5FAFB` — the ground for every page. A barely-tinted aqua white, not neutral, and never pure `#FFFFFF`. It occupies roughly 60% of any given page.

**Primary Colors:**
- Deep Teal `#245860` — the anchor. Footer band, value cells, and any inverted block. Carries white type at every size.
- Label Teal `#397F80` — chapter eyebrows and small standalone labels above a heading. Used for text only, never as a fill.
- Ink `#221F20` — serif display type and the wordmark. A warm near-black.
- Ink Body `#232526` — all sans body copy and data labels. A hair cooler than display ink; the two are not interchangeable.

**Neutral Colors — the tonal ladder:**
The system's entire structural vocabulary, in order of depth. Each step up the ladder is a container nested inside the one below it.
- Step 1 `#F5FAFB` — page ground
- Step 2 `#E5F3F5` — large content panels (charts, data blocks, callout regions)
- Step 3 `#D1E9EC` — smaller cards seated directly on the page ground (pull quotes, sidebars)
- Step 4 `#9DD1D3` — filled bands inside a Step 2 panel, such as the label half of a data row
- Step 5 `#245860` — the inverted terminus: value cells, the page footer band

Panels sitting on the page take Step 2 or Step 3. Anything inside a Step 2 panel takes Step 4 or Step 5. Never place a Step 3 card on a Step 2 panel — the contrast step is too small to read as separation.

**Accent/State Colors:**
- Spark Periwinkle `#7B88D5` — a four-point star glyph marking machine-generated or model-derived content, at 24px with an 8px companion star. This is the only non-teal chroma in the entire system and appears at most once per page.
- Success `#245860` — reuses Deep Teal; the system introduces no green.
- Warning `#8A5A1E` — inline text only, never a fill.
- Error `#8C2F2A` — inline text only, never a fill.
- Focus Ring `#245860` at 2px offset 2px.

## Typography

**Display & Headings:** a transitional serif with moderate stroke contrast and sturdy bracketed serifs, used for every chapter title, panel title, and pull quote. Google Fonts equivalent: `Newsreader`, weights 400/600. Fallback: `'Newsreader', 'Tiempos Text', Georgia, 'Times New Roman', serif`.

**Body & Data:** a geometric-humanist sans with a high x-height and rounded terminals, used for all running copy, subheads, eyebrows, table labels, and footer type. Google Fonts equivalent: `Plus Jakarta Sans`, weights 400/600/700. Fallback: `'Plus Jakarta Sans', 'Inter', -apple-system, sans-serif`.

**Type Scale:**
- Chapter title (serif) — 44px / 600 / 1.10 / -0.01em
- Panel title (serif) — 30px / 600 / 1.20 / -0.01em
- Pull quote (serif) — 26px / 400 / 1.35 / 0
- Section subhead (sans) — 20px / 700 / 1.35 / 0
- Chapter eyebrow (sans) — 20px / 700 / 1.2 / 0, set in Label Teal
- Attribution name (sans) — 17px / 700 / 1.4 / 0
- Attribution role (sans) — 17px / 400 / 1.4 / 0
- Data value (sans) — 19px / 700 / 1.2 / 0
- Body (sans) — 15px / 400 / 1.7 / 0
- Data row label (sans) — 15px / 700 / 1.4 / 0
- Table column header (sans) — 14px / 700 / 1.4 / 0
- Footer (sans) — 14px / 700 / 1.4 / 0

**Hierarchy Rules:** Serif and sans do not overlap in function — a serif never sets running copy, and a sans never sets a chapter title or a pull quote. This split is the system's most load-bearing rule. Within body copy, emphasis is a weight jump to 700 in the same ink, never a color change and never italic; statistics and lead-in clauses are the usual targets. Section subheads sit directly on the body copy with no rule and no extra tracking. The chapter eyebrow is the only place type is colored teal, and it always sits immediately above a serif title with roughly 8px between them. Nothing is centered except the footer's two anchored ends.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 24, 32, 40, 48, 64, 80.

**Common Patterns:**
- Page gutter 64px; content measure capped at 920px.
- Wordmark to first eyebrow: 80px. Eyebrow to chapter title: 8px. Chapter title to first subhead: 32px.
- Body paragraph spacing 24px; subhead to its first paragraph 12px.
- Two-column split: text column 48%, card column 44%, 80px gap. Both columns top-align to the same baseline.
- Card padding 32px. Large panel padding 24px on data blocks, 32px on prose panels.
- Panel title to column headers 32px; column headers to first data row 12px.
- Data row height 52px, 8px gap between rows.
- Section to section: 64px.
- Footer band 60px tall, full-bleed, 64px inner gutters matching the page.

## Component Styles

### Pull Quote Card

Step 3 fill `#D1E9EC`, 16px radius, 32px padding, no border and no shadow. Contents in fixed order: attribution name at 17px/700, attribution role at 17px/400 directly beneath with no gap beyond line-height, then 24px of space, then the quote in serif at 26px/400 with straight double quotation marks included in the text. The card never carries a decorative quotation glyph, a rule, an avatar, or a logo.

### Data Panel

Step 2 fill `#E5F3F5`, 20px radius, 24px padding, no border and no shadow. A serif panel title at 30px sits top-left, with the Spark Periwinkle glyph optionally pinned top-right on the same baseline block. Beneath the title, a two-part column header row in 14px/700 — descriptor label hard left, measure label hard right.

### Banded Data Rows

The signature component, and **a banded table rather than a proportional bar chart**. Each row is a fixed two-part band, not a bar scaled to its value:

- Left band — Step 4 fill `#9DD1D3`, containing the row label at 15px/700 in Deep Teal, 24px left padding. Its right edge sits at the same x for every row in the table.
- Right band — Step 5 fill `#245860`, fixed width (roughly 27% of the panel's inner width), containing the value at 19px/700 in `#FFFFFF`, right-aligned with 24px right padding.
- Row radius 6px on the outer left corners of the left band and the outer right corners of the right band; the seam between the two bands is square.
- Row height 52px, 8px gap. No hover state — this is print-derived and static.

Values are read from the right column, not from band length. Do not scale the left band to the percentage; doing so breaks the visual rhythm the whole table depends on.

### Section Heading Block

An eyebrow at 20px/700 in Label Teal, 8px of space, then a serif title at 44px/600 in Ink. Used once at the top of a chapter and nowhere else. Mid-document sections use a 20px/700 sans subhead with no eyebrow.

### Footer Band

Full-bleed Deep Teal `#245860`, 60px tall, no radius, flush to the bottom edge. Page number at 14px/700 in `#FFFFFF` hard left; chapter descriptor at 14px/700 in `#FFFFFF` hard right. Nothing sits in the center. This is the only inverted region on the page.

### Inline Emphasis

Weight 700 in the same `#232526` ink. Applied to leading statistics and to the clause that carries a paragraph's claim. Roughly one emphasized run per paragraph; two makes the page read as a sales sheet.

## Layout Principles

Single fixed-width document column at 920px with 64px gutters, on a page that runs to a full-bleed footer band. The page alternates between full-measure prose blocks and a 48/44 two-column split with an 80px gap — never a three-column grid and never an asymmetric offset. Panels are full-measure; cards are half-measure. On tablet the two-column split collapses to stacked full-measure blocks in source order, prose first and card second. On mobile, gutters drop to 24px, card and panel padding drop to 20px, the chapter title drops to 32px, and the pull quote drops to 21px; the banded rows keep both bands side by side but the right band narrows to 84px. The footer band stays full-bleed at every width.

## Visual Effects

There are no borders, no dividers, no rules, and no shadows anywhere in the system — separation is achieved exclusively by stepping the fill one rung up the tonal ladder. Radii: 20px on large panels, 16px on cards, 6px on data row bands, 0 on the footer band. No gradients, no glass, no texture, no photography, and no illustration beyond the single periwinkle spark glyph. Because the system is print-derived it carries almost no interaction surface; where a web adaptation needs one, transitions are 150ms ease on background-color only.

## Design Tone

Measured, evidential, and quietly institutional — a document that expects to be cited rather than skimmed. The near-monochromatic teal ladder gives it a calm, cohesive weight without ever resorting to a border, and the serif display against geometric sans body reads as research rather than marketing. The single periwinkle spark is the only note of levity, and its scarcity is what makes it land.

## Usage Notes for AI Implementation

1. **Borders are forbidden.** If two regions need separating, step one rung up the tonal ladder — `#F5FAFB` to `#E5F3F5`, or `#E5F3F5` to `#9DD1D3`. A single 1px border anywhere collapses this into a generic report template. The same applies to shadows and horizontal rules.

2. **Never nest a Step 3 card on a Step 2 panel.** `#D1E9EC` on `#E5F3F5` is too small a contrast step to read. Cards sit on the page ground; bands sit inside panels. Skipping a rung is fine, going backward is not.

3. **Serif and sans never trade jobs.** Serif for chapter titles, panel titles, and pull quotes. Sans for everything else, including every subhead. If a subhead is set in the serif, the page starts reading as a magazine feature instead of a research document.

4. **The banded table is not a bar chart.** All left bands terminate at the same x, and the value block is a fixed-width right column. Do not width-scale bands to their percentages — the rhythm of three identical-width rows is the point, and scaling them makes an already-labeled figure redundant.

5. **The periwinkle spark is rationed to one per page.** It marks model-derived content and nothing else. A second instance, or the same periwinkle appearing in type, a fill, or an icon set, destroys the monochrome discipline that carries the system.

6. **Teal type appears in exactly one role.** The chapter eyebrow. Body copy, subheads, links, and labels are all `#232526` or `#221F20`. Emphasis is weight, never color.

7. **The page ground is tinted, not white.** `#F5FAFB` against `#FFFFFF` is a small step but it's what keeps the panels from floating. Never substitute pure white for the page, and never place a pure-white surface on it.

8. **Keep the footer band full-bleed and empty in the middle.** Two anchored ends, nothing between them, no radius, flush to the page edge. It is the system's only inverted region and it should stay that way.
