---
id: light-warm-sketchnote-054
title: Marigold Sketchnote
description: A hand-drawn sketchnote system — warm cream paper, felt-tip lettering, and a single highlighter-yellow marker doing every bit of emphasis.
tags: [light, warm, playful, friendly, hand-drawn, sketchnote, illustrated, highlighter, rounded, marketing]
colors: ["#F7F3E8", "#FCFBF4", "#F2E64B", "#1C1B19"]
created: 2026-09-05
---

# Marigold Sketchnote

Marigold Sketchnote is a hand-drawn explainer aesthetic: warm cream paper, black felt-tip lettering, hand-outlined boxes, and one highlighter-yellow marker carrying every bit of emphasis. It looks like a sharp friend mapping an idea out on a whiteboard — approachable and energetic, structured but never polished. Everything is monochrome ink on paper with a single warm accent, so the system leans entirely on outline weight, hand-drawn irregularity, and marker highlights rather than color, fills, or shadow. Best for marketing explainers, playbooks, onboarding walkthroughs, workshop decks, and any place a diagram should feel personally drawn rather than machine-generated.

## Color Palette

**Page Surface:** warm cream paper — `#F7F3E8` — the ground for everything; never pure white.
**Raised Surface:** `#FCFBF4` — a near-white warm panel used sparingly when a card must lift off the paper; most cards stay on the page ground and are defined by their outline alone.
**Sunken Tint:** `#EFEAD9` — a slightly deeper paper tone for insets, code-ish blocks, or a footer band.

**Primary Ink:** `#1C1B19` — a warm near-black, the color of a felt-tip pen. All lettering, borders, icons, arrows, and strokes are this one ink.
**Secondary Ink:** `#6B675C` — warm gray for sub-labels, captions, and supporting descriptions under a heading.
**Faint Ink:** `#A8A296` — for dividers, placeholder text, and disabled states.

**Accent — Highlighter Yellow:** `#F2E64B` — the only accent in the system. Used three ways: as a marker swash behind key words, as a solid tab-label chip, and as the hover/active fill for primary controls. Roughly one highlighted element per screenful.
**Accent Deep:** `#E4D42E` — a marginally darker yellow used only for the underside/edge of a pressed control or a swash overlap, never as a second accent.

**State Colors** (kept within the palette so they never introduce a new hue):
**Success:** ink text with a highlighter-yellow check swash — success is shown, not colored.
**Warning:** `#1C1B19` ink on a `#F2E64B` marker band.
**Error:** `#B23A2E` — a muted brick red, the single permitted departure from the two-color rule, reserved exclusively for destructive confirmation and inline validation.
**Focus:** a `#1C1B19` 2.5px hand-drawn outline plus a `#F2E64B` marker underlay; never a blue glow.

## Typography

**Font Families:**
**Display & Headings:** "Shantell Sans" — a variable marker sans-serif (Google Fonts) drawn to look hand-lettered; used bold, frequently uppercase, with generous tracking. Fallback: "Comic Sans MS", "Segoe Print", cursive-adjacent system faces, sans-serif.
**Body & Labels:** "Patrick Hand" — a single-weight neat-print handwriting face (Google Fonts) that stays legible down to 15px where a marker face would not. Fallback: "Comic Sans MS", "Segoe Print", sans-serif.
**Loose Asides:** "Caveat" (Google Fonts) — a fast handwritten script, optional, reserved for the smallest scrawled annotations ("3× faster", margin notes). Never for running text.

**Type Scale** (fluid; display sizes use `clamp()` so a large numeral survives 393px):
- Hero numeral / statement — Shantell Sans 800, `clamp(44px, 9vw, 88px)`, line-height 0.95, tracking 0.5px, usually uppercase.
- H1 section — Shantell Sans 700, `clamp(30px, 5vw, 46px)`, line-height 1.05, uppercase.
- H2 — Shantell Sans 700, `clamp(22px, 3.4vw, 30px)`, line-height 1.1, uppercase.
- Card title / tab-label — Shantell Sans 700, 18–20px, uppercase, tracking 1px.
- Body — Patrick Hand 400, 17px, line-height 1.55, sentence case.
- Small label / caption — Patrick Hand 400, 15px, line-height 1.4, color Secondary Ink.

**Hierarchy Rules:** Display and labels are ALL CAPS marker; descriptions are sentence-case neat-print — the case switch does as much hierarchy work as size. Emphasis is never a CSS underline: it is a hand-drawn swash beneath the word or a marker highlight behind it. Numbers and stats get the largest treatment on any given surface — the payoff figure is the loudest thing on the page. Body text is always left-aligned and never justified; centering is reserved for single-line labels and stat callouts. Headings sit close to the content they title, with the air placed above the heading, not below it.

## Spacing System

**Base Unit:** 4px. The scale is 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 96.

**Scale usage:** 4–8px for icon-to-label gaps, 12–16px for inside-card padding at the tight end, 20–28px for comfortable card padding, 32–48px between cards in a flow, 64–96px between major page sections.

**Common Patterns:** Cards carry 22–28px of internal padding so the hand-drawn border never crowds the text. Related boxes in a flow sit 32–40px apart with a hand-drawn arrow bridging the gap. Tab-labels overlap the top edge of their card by roughly 14px so they read as stuck-on, not floating. The page gutter is 20px on mobile and opens to a centered max measure of ~1100px on desktop; widening the gutter is the primary desktop adaptation.

## Component Styles

### Buttons
Hand-drawn rounded rectangles with a 2.5px Primary Ink border and an irregular multi-value border-radius so no two corners match. **Primary:** highlighter-yellow fill (`#F2E64B`), ink border, ink label, uppercase Shantell Sans; on hover it nudges up 1px and rotates ~-1deg with a faster transition; on active it presses down and the fill deepens to Accent Deep. **Secondary:** transparent (paper) fill, ink border and label; on hover the fill floods to highlighter yellow. **Text button:** ink label with a hand-drawn swash underline that thickens on hover. Minimum tap target 44px. Never add a drop shadow — the lift is rotation and a 1px translate, not elevation.

### Cards & Panels
The workhorse container: paper ground (or Raised Surface when it must lift), a 2.5px ink border, and an irregular border-radius (e.g. `255px 15px 225px 15px / 15px 225px 15px 255px`) that reads as a drawn box rather than a CSS rectangle. Each card may carry a small deliberate rotation of -1.5deg to 2deg so a row of them looks placed by hand. No fills beyond paper/raised, no shadows. A card titled by a **tab-label** has a highlighter-yellow chip overlapping its top-left corner.

### Marker Highlights & Underlines
The signature move. A **highlight** is a skewed highlighter-yellow band sitting behind inline text, built with a slightly angled linear-gradient so its ends are uneven and it bleeds a hair past the words — a marker stroke, not a rectangle. A **swash underline** is a hand-drawn wavy SVG line tucked under a word, ink-colored, used to mark a key term without highlighting the whole phrase. Both are for one or two phrases per screen; more and the emphasis stops meaning anything.

### Chips & Tab Labels
Small uppercase Shantell Sans labels on a solid highlighter-yellow chip with a 2px ink border and a tiny rotation. Used as day/step markers (MONDAY, STEP 1), category tags, and card titles. As a card's tab-label it overlaps the card's top edge; as a standalone chip it sits inline with 8px gaps.

### Hand-Drawn Icons
Monochrome ink line icons at 2px stroke weight with rounded caps and joins, drawn slightly loose. Always ink, never filled and never colored — a filled or yellow icon competes with the one accent. Sized 24–40px, paired left of a label with an 8–12px gap.

### Arrows & Connectors
Hand-drawn SVG arrows in Primary Ink bridge boxes in a flow — a gently curved shaft with an open arrowhead, never a straight CSS border-triangle. Used horizontally between columns on desktop and rotated to vertical between stacked cards on mobile. An "OR" connector is a small ink-outlined pill dropped on the line between two alternatives.

### Stat Callouts
The payoff block: a hero numeral in Shantell Sans 800 (often with a marker highlight behind it), a short uppercase label beneath, optionally inside its own hand-drawn card. This is the loudest element on any surface it appears in and there is only ever one per view.

### Input Fields
Extrapolated for form use: a hand-drawn box with a 2.5px ink underline (or full irregular border), Patrick Hand text at 17px, placeholder in Faint Ink. Focus draws a full 2.5px ink outline with a highlighter-yellow marker underlay behind the field. Labels sit above in uppercase Shantell Sans. Error state swaps the underline to muted brick red with a short hand-scrawled message beneath.

## Layout Principles

The organizing metaphor is a board, not a grid. Content is arranged as outlined boxes connected by hand-drawn arrows, read left-to-right and top-to-bottom, with generous whitespace of bare paper between clusters. Everything is left-aligned inside its box. On desktop, related steps sit side by side as columns with horizontal connectors and a centered ~1100px measure; on mobile the columns stack into a single column and the connectors rotate to vertical. Deliberate small rotations keep rows from looking mechanically aligned. Depth is created entirely by outline weight and the yellow accent — there are no layers, z-planes, or shadows to manage. The one desktop adaptation that matters is opening the gutter and letting columns sit beside each other; the mobile stack is the honest source of truth for reading order.

## Visual Effects

**Radii:** never a single clean value. Containers use irregular multi-value border-radius so corners differ; buttons and chips use gentler but still-uneven radii. A perfect 8px rounded rectangle is the fastest way to lose the aesthetic.
**Borders:** 2.5px Primary Ink is the default weight; 2px on smaller chips. The border is the structure — it does the job a shadow would do elsewhere.
**Shadows:** none, anywhere. Flat ink on flat paper. Elevation is expressed by outline and, on interaction, by a 1px translate plus a small rotation.
**Rotation:** the texture of the whole system. Cards, chips, and labels carry -3deg to 3deg of hand-placed tilt; 0deg across the board reads as a broken hand-drawn theme, and more than ~3deg reads as a ransom note.
**Marker treatment:** highlights are skewed gradients with uneven ends; swash underlines are wavy SVG paths. Both intentionally imperfect.
**Transitions:** quick and slightly springy — 120–180ms, `cubic-bezier(.34,1.56,.64,1)` on hover lifts so controls feel drawn-and-bouncy rather than smoothly animated.

## Design Tone

Warm, hand-made, and confident without polish — a smart friend explaining something on a whiteboard rather than a brand presenting to you. The single highlighter-yellow accent against black ink on cream paper makes it feel energetic and human, and the deliberate imperfection (drawn borders, small rotations, marker swashes) signals that a person made this on purpose. It reads as approachable and trustworthy precisely because it isn't slick.

## Usage Notes for AI Implementation

1. One accent only. Yellow, ink, and paper are the entire palette; brick red is permitted solely for destructive/error states. Add a second accent color and the sketchnote collapses into a generic startup deck. Budget roughly one highlighted element per screenful — the marker is a pointer, not a fill.
2. Emphasis is never a CSS `text-decoration: underline`. A straight underline reads as a hyperlink and kills the hand-drawn illusion. Emphasis is a marker highlight behind the text or a hand-drawn swash under the word.
3. No drop shadows, ever. Depth is the 2.5px ink outline on paper. The moment a card gains a box-shadow it becomes a material-design card wearing a costume; step nothing, shadow nothing — the border carries it.
4. Borders must look drawn. Use an irregular multi-value `border-radius` (corners that don't match) or a rough SVG rect, not a clean uniform radius. A perfect rounded rectangle is the single fastest way to lose the whole system.
5. Keep to the two hand fonts. If body text switches to a geometric or system sans "for readability," the page instantly reads as a corporate site that pasted in a marker header. Legibility comes from Patrick Hand at 15px or larger, not from abandoning the hand.
6. Uppercase display, sentence-case body. Section titles, labels, and stat labels are ALL CAPS marker; descriptions and running text are neat sentence case. Inverting this flattens the hierarchy the system depends on.
7. Tilt on purpose, a little. Give cards, chips, and labels -3deg to 3deg of rotation and vary it; a grid at exactly 0deg looks like a failed hand-drawn theme, and anything past ~3deg looks chaotic. The imperfection is the design, but it is controlled.
8. Highlight like a marker, not a button. The yellow swash sits behind text, skews slightly, and bleeds a hair past the words with uneven ends. A solid rectangle flush to a text box reads as a filled button and breaks the effect.
9. Tab-labels belong to their card. A yellow title chip overlaps the top edge of the card it names; floating it free in space breaks the "sticky note on the box" read that ties label to content.
10. Icons stay ink-only line drawings. 2px rounded-cap strokes, monochrome, never filled and never colored. A filled or yellow icon competes with the one accent and looks imported from a different set — redraw it as an outline instead.
