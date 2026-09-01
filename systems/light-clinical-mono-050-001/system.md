---
id: light-clinical-mono-050
title: Lattice Dawn
description: A light, clinical-precision system that pairs monospace UI chrome with a proportional grotesque, warmed by a single dawn gradient.
tags: [light, minimal, modern, monospace, gradient, rounded, forms, marketing, healthcare, clinical]
colors: ["#FFFFFF", "#17151B", "#F6CDA6", "#CBDDF4", "#C9BEE8"]
created: 2026-09-01
---

# Lattice Dawn

Lattice Dawn is a light, clinical-precision system for technical platforms that need to read as human. Monospace carries every label, button, and data tag; a proportional grotesque carries everything you actually read; and a single soft dawn gradient — lavender through peach — is the one warm gesture on an otherwise white, hairline-ruled page. It is built for the domain that has to signal rigor and traceability without feeling cold: infrastructure, health data, developer platforms, anything where a form and a promise of compliance sit on the same screen.

The whole system runs on restraint. There are no shadows, almost no color, and no bold headings — hierarchy comes from size, generous space, and the disciplined split between the two typefaces. When it works, the page feels calm and exact at the same time.

## Color Palette

**Page Surface:** `#FFFFFF` — the default ground for nearly every section. White is the rule; every other surface is an exception used sparingly.

**Primary Colors:**
- Ink `#17151B` — near-black with a faint violet cast, used for all headings, primary body, button fills, and outline borders.
- Button Fill `#141317` — the solid ink pill; a hair deeper than body ink so it reads as a deliberate surface.

**Neutral Colors:**
- Alt Band `#EAECF1` — a cool blue-gray used only as a full-bleed section band (contact, compliance). The single non-white background in the layout.
- Diagram Tint `#DFE1F3` — a soft lavender-white behind the connection diagram's radial dome.
- Secondary Text `#6C6C74` — descriptive body copy on white. Step it one shade darker over tinted grounds to hold AA contrast: `#63636B` on the gray band, `#4D4D54` over the hero gradient.
- Label `#63636B` — the muted color for monospace eyebrow labels; deliberately darker than tertiary so small mono labels clear AA on both white and the band.
- Tertiary Text `#8B8B93` — input placeholders and the decorative diagram node labels only; never for real reading content.
- Hairline Border `#E4E4E8` — 1px rules on chips, inputs, dividers, and cards.

**Accent / Highlight Colors:**
- Highlight Peach `#F6CDA6` — a warm marker background sitting behind a single phrase in a sentence.
- Highlight Periwinkle `#CBDDF4` — the cool counterpart, used for the second highlighted phrase in the same sentence.
- Focus Violet `#6F5DB0` — the only saturated color in the system, reserved for input focus rings.

**Hero Gradient:** first stop `#C9BEE8` (lavender). A soft diagonal wash `linear-gradient(150deg, #CBBFE8 0%, #D6C2D8 32%, #EDC4AA 68%, #FCF9F7 100%)` — lavender to mauve to peach, dissolving to near-white. It appears exactly once, in the hero.

**On-Ink Text:** `#FFFFFF` — text and glyphs on the ink button fill.

## Typography

**Font Families:**
- **Display & Headings:** Hanken Grotesk — a neo-grotesque sans-serif; fallbacks `Inter, system-ui, sans-serif`. Carries all headings and all reading copy. This is the reading experience of the system.
- **Monospace / Chrome:** IBM Plex Mono — carries every piece of UI chrome: eyebrow labels, buttons, toggle pills, source chips, and the wordmark. Fallbacks `"SFMono-Regular", ui-monospace, monospace`.

**Type Scale (mobile-first):**
- Display H1 — `clamp(2.5rem, 9vw, 4rem)` / weight 450 / line-height 1.05 / tracking -0.02em
- Section H2 — `clamp(2rem, 7vw, 3rem)` / weight 450 / line-height 1.08 / tracking -0.015em
- Lead / Subhead — `clamp(1.375rem, 4.5vw, 1.75rem)` / weight 600 / line-height 1.3 (this is the sentence that carries the highlight marks)
- Body — `1.1875rem` (19px) / weight 400 / line-height 1.55 / color secondary text
- Eyebrow Label — mono `0.8125rem` (13px) / weight 500 / uppercase / tracking 0.12em
- Chrome (buttons, toggles) — mono `0.875rem` (14px) / weight 500 / uppercase / tracking 0.07em
- Chip — mono `0.9375rem` (15px) / weight 400 / **mixed case** / tracking 0
- Input Label — sans `1rem` / weight 400 / secondary text

**Hierarchy Rules:**
- Headings are never bold. They sit at weight 450 and let size and whitespace do the work. A bold display heading collapses the whole feel into a generic hero.
- The two families split strictly by role: proportional sans for anything you *read*, monospace for anything you *operate or label*. The families never trade places.
- In-sentence emphasis is a highlight mark, never bold, italic, or a color change on the text itself.
- Everything is left-aligned. Nothing is centered except the footer.
- Display headings are set to wrap deliberately across two lines with tight leading; the break is part of the composition.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 96px.

**Common Patterns:**
- Page gutter: 24px mobile, widening to 48–64px on desktop. The gutter is the only thing that changes across breakpoints.
- Section rhythm: 64px between blocks on mobile, 96px on desktop. The system is deliberately airy.
- Button padding: 18px vertical, 32px horizontal (pill).
- Input padding: 18px vertical, 20px horizontal.
- Chip padding: 10px vertical, 16px horizontal; 10px gap between chips, wrapping across rows.
- Eyebrow-to-heading gap: 16px. Heading-to-body gap: 24px.

## Component Styles

### Buttons
Two variants, both pill-shaped (`border-radius: 999px`), both monospace uppercase tracked, no shadow ever.
- **Primary:** fill `#141317`, text `#FFFFFF`, no border. Hover lightens the fill to `#2C2A32` over 160ms. Focus adds a 2px Focus Violet ring at 2px offset.
- **Secondary:** transparent fill, 1.5px Ink border, Ink text. Hover inverts — fill becomes Ink, text becomes white — over 160ms. This invert-on-hover is the system's signature interaction.
- Minimum 44px tap target; real padding puts them well above it.

### Toggle Pills
A two-option audience switch ("primary path" / "secondary path"), rendered as adjacent outline pills. Unselected: transparent fill, 1px Hairline border, Ink mono uppercase label. Selected: Ink fill, white label. Only one is ever selected. Used as a top-of-page router, not a form control.

### Source Chips
Wrapping tags naming data sources or categories. 1px Hairline border, white fill, `border-radius: 8px`, monospace but **mixed case** — they are data values, not chrome labels. They flow in rows and wrap freely. Hover darkens the border to `#C9C9CF` and does nothing else. Never uppercase them; never fill them.

### Inline Highlight Marks
A rounded background (`border-radius: 8px`, padding 2px 10px) sitting behind a single phrase inside the lead sentence. Two colors only: Highlight Peach and Highlight Periwinkle, used as a warm/cool pair. Text stays Ink. This is the entire emphasis mechanism for running copy.

### Input Fields
White fill, 1px Hairline border, `border-radius: 16px`, 18px/20px padding, 19px sans value text. A sans label sits 8px above in secondary text. Focus: border darkens to Ink and a 2px Focus Violet ring appears; transition 150ms. Generous height is deliberate — these read as calm, not dense.

### Section Eyebrows & Nav
Every section opens with a monospace uppercase tracked eyebrow label in the muted Label color (`#63636B`). On the hero the eyebrow is inked instead. The nav is a monospace wordmark (paired with a small starburst glyph) on the left and a circular outline icon button (1px Hairline, fully round) on the right. The eyebrow is the connective tissue that makes the two-typeface split legible.

### Node / Connection Diagram
A decorative motif: a soft radial dome in Diagram Tint at the top, with 1px **dashed** Hairline connector lines radiating out to small circular outline nodes, each labeled in monospace uppercase. It illustrates disparate sources converging on one layer. Purely presentational; dashed lines and round nodes are the identifying detail.

### Bands & Dividers
Depth is created with a single full-bleed band in Alt Band `#EAECF1` (used for the contact/compliance zone) and 1px Hairline dividers. No cards with shadows; where a card is needed it is a hairline-bordered white rectangle at `border-radius: 16px`.

## Layout Principles

Single column, left-aligned, mobile-first. A generous max measure (~640px for reading copy, ~960px for the page frame) keeps line length comfortable; on desktop the gutters widen and chip rows and form fields get room to breathe, but no new columns appear and the hero text is never centered. Whitespace is the primary layout tool — sections are separated by 64–96px of air rather than by rules or backgrounds. The full-bleed gray band is the one moment the layout leaves white, and it spans the full viewport width with its content held inside the standard gutter.

## Visual Effects

- **Radii:** pills 999px (buttons, toggles); inputs, cards, and the alt band 16px; chips and highlight marks 8px; icon buttons fully round.
- **Shadows:** none, anywhere. Separation is done with the gray band and hairline borders. This absence is the defining effect.
- **Borders:** 1px Hairline `#E4E4E8` for chips, inputs, dividers, cards; 1.5px Ink for outline buttons; 1px dashed Hairline for diagram connectors.
- **Background treatment:** white by default; one hero gradient; one gray band; one lavender diagram dome. Every color moment is rationed.
- **Transitions:** 150–160ms ease on fills, borders, and focus rings. Nothing animates on load.

## Design Tone

Clinical precision made warm. The monospace chrome signals rigor, traceability, and system-thinking; the proportional grotesque and the single dawn gradient keep it from tipping into a cold terminal aesthetic. The result is airy, confident, and unhurried — a technical product that trusts whitespace and restraint to do the reassuring instead of stock imagery or drop shadows.

## Usage Notes for AI Implementation

1. Never bold the headings. Keep display and section headings at weight ~450; size and whitespace carry the hierarchy. A bold hero heading turns this into a generic startup landing page and loses the whole editorial-technical register.
2. Split the two typefaces strictly by role and never cross them: proportional sans for everything read (headings, body, input values), monospace for everything operated or labeled (eyebrows, buttons, toggles, chips, wordmark). Put body prose in the mono and it becomes a terminal theme; put a button label in the sans and it looks unfinished.
3. In-sentence emphasis is a highlight mark, not bold/italic/color. Use at most two per sentence — they mark the two words the sentence turns on. Three or more and they stop reading as emphasis and become wallpaper.
4. Pair the accent hues; don't stack them. Peach and periwinkle are a warm/cool set, one of each per sentence. Two peach marks or two blue marks in one phrase kills the contrast that makes the device legible.
5. No shadows, ever. Reach for elevation and the flat clinical calm is gone. Separate content with the full-bleed gray band or a 1px hairline instead.
6. The gradient appears exactly once, in the hero. It is the single warm gesture on an otherwise white page; repeating it per section makes it wallpaper and drains the highlight marks of their pop.
7. Every section opens with a monospace uppercase tracked eyebrow label. Drop it and the page reads as two unrelated typefaces rather than one deliberate system — the eyebrow is what teaches the eye the split.
8. Chips are the one monospace element set in mixed case, and they are never filled or uppercased. They are a queryable list of data sources, not buttons; uppercasing "Pathology (WSI)" or filling "Flow cytometry" makes them read as controls and breaks the data-tag metaphor.
9. Controls are large and rounded with real padding — 44px+ targets, ~18px vertical padding, pill or 16px radius. Tighten them into compact dashboard controls and the calm marketing surface reads as an admin panel.
10. Stay single-column and left-aligned; the only desktop adaptation is wider gutters and more room for chip rows and form fields. Do not add columns, do not center the hero text, and do not introduce a second background color beyond the one gray band.
