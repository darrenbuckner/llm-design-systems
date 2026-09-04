---
id: dark-oxide-nocturne-052
title: Oxide Nocturne
description: A near-black grotesque system where a rust-orange italic serif and uppercase monospace labels do all the accent work.
tags: [dark, stark, high-contrast, monospace, serif, marketing, generous-spacing]
colors: ["#030A12", "#12171F", "#CB623A", "#F1F3F6", "#DCDCDE"]
created: 2026-09-04
---

# Oxide Nocturne

A near-black interface built on a single deep blue-black ground, where a rust-orange italic serif cuts across wide grotesque headlines and every label, button, and numeral is set in uppercase monospace. Sharp corners throughout, hairline rules instead of shadows, and roughly one accent per screenful. It is built for a practice that sells judgment rather than volume: long-form prose is treated as a first-class element, the page never brightens, and contrast comes from typeface switching instead of color.

## Color Palette

**Page Surface:** `#030A12` — the single ground for every section. There is no alternating band, no lighter page, no hero gradient. Every screen in the system sits on this one value.

**Primary Colors:**
- Accent Oxide — `#CB623A` — the only chromatic value in the system. Used for the italic serif phrase inside a headline, step numerals, and the small underscore rule beneath an active icon. Never as a button fill.
- Accent Oxide Deep — `#8A4227` — the dot-matrix imagery only. A halftone field of these dots reads as texture rather than as an element.
- Inverse Fill — `#DCDCDE` — the primary button, and nothing else. It is the brightest surface in the system and is spent on exactly one element per screen.

**Neutral Colors:**
- Page Surface — `#030A12` — the ground
- Raised Surface — `#12171F` — quote cards, testimonial panels, any panel that must separate from the ground
- Sunken Surface — `#080E17` — icon wells and inset chips; one step off the ground, never more
- Hairline — `#161D28` — every border, divider, accordion rule, and outlined control at 1px
- Hairline Strong — `#242C39` — hover state for outlined controls only
- Text Primary — `#F1F3F6` — display type, headings, questions, statistics
- Text Body — `#C1C8D0` — long-form prose in a wide measure
- Text Muted — `#8D96A2` — component body copy, eyebrows, captions, attribution
- Text Faint — `#737C89` — copyright, legal links, inactive pagination
- Inverse Ink — `#0B121B` — text on the inverse fill

**Accent/State Colors:**
- Focus — `#CB623A` — a 2px outline at 3px offset, in the accent. Focus is the one place the accent is allowed to appear more than once per screen.
- Success — `#4E9E7A`
- Warning — `#C9903C`
- Error — `#C1503F`

State colors appear in system feedback only and never in marketing layout. If a page needs three colors it has left the system.

## Typography

**Display & Headings:** Wide neutral grotesque sans — Archivo, with Helvetica Neue, Arial, sans-serif as the fallback chain. Set at 400–500 weight and never heavier; size, not weight, carries the hierarchy.

**Accent Face:** High-contrast display serif italic — Instrument Serif Italic, with Georgia and serif as fallbacks. Used exclusively for a phrase set inside a sans headline, always in the accent color, always italic, never for a whole heading and never for body copy.

**Label Face:** Monospace — IBM Plex Mono, with SFMono-Regular, Menlo, monospace as fallbacks. Every eyebrow, button label, step numeral, statistic unit, pagination control, and footer legal line.

**Font Families:** Three faces, three jobs, no overlap. The grotesque states, the serif inflects, the mono labels. A fourth face breaks the system.

**Type Scale:**
- Display — `clamp(44px, 11vw, 92px)` / 500 / line-height 0.98 / letter-spacing `-0.03em`
- Heading 1 — `clamp(34px, 8vw, 60px)` / 500 / 1.04 / `-0.025em`
- Heading 2 — `clamp(28px, 6.5vw, 40px)` / 400 / 1.1 / `-0.02em`
- Heading 3 — `22px` / 400 / 1.25 / `-0.01em`
- Body Large — `19px` / 400 / 1.62 / `0`
- Body — `17px` / 400 / 1.65 / `0`
- Small — `15px` / 400 / 1.6 / `0`
- Eyebrow — `12px` / 400 / 1 / `0.24em` / uppercase / mono
- Button Label — `13px` / 500 / 1 / `0.16em` / uppercase / mono
- Numeral — `13px` / 400 / 1 / `0.2em` / mono / accent

**Hierarchy Rules:**
- Every section opens with a mono uppercase eyebrow, then the heading. The eyebrow is the section marker; a section without one reads as a fragment.
- Exactly one phrase per heading may switch to the accent serif italic. Two switches in one heading destroys the effect.
- The accent phrase is a grammatical unit — a clause, an apposition, a predicate. Never a single adjective and never a proper noun.
- Display type wraps hard and early. Two or three lines with tight leading is the intended texture; a display headline that runs to one long line is set too small.
- Body prose caps at 62 characters. Marketing paragraphs are allowed to be genuinely long — four or five sentences — because the system's argument is that reading is the point.
- Nothing is centered except a closing call-to-action block and the footer.
- Numerals in statistics are `#F1F3F6`; the words around them drop to `#8D96A2`, so the figure reads first.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 96, 128, 160.

**Common Patterns:**
- Page gutter — 24px mobile, 40px tablet, 64px desktop. One element owns it.
- Section rhythm — 96px mobile, 160px desktop, top and bottom, set with longhand `padding-top` / `padding-bottom` so it cannot collide with the gutter.
- Eyebrow to heading — 24px. Heading to body — 32px.
- Paragraph stack — 24px between paragraphs in a prose block.
- Card padding — 32px mobile, 40px desktop.
- Accordion row — 32px vertical padding, 24px between the question and the toggle glyph.
- Step rail — 48px between the rail and the step content, 80px between consecutive steps.
- Button pair — 16px vertical gap when stacked, 16px horizontal when inline.
- Content max-width — 1160px for full sections, 680px for prose blocks, both centered with `margin-left: auto; margin-right: auto`.

The system's generosity is vertical. Horizontal padding stays modest so long lines can breathe; vertical space is where the money is spent.

## Component Styles

### Buttons

**Primary** — fill `#DCDCDE`, text `#0B121B`, `border-radius: 0`, padding `20px 32px`, mono uppercase 13px at `0.16em` tracking. On hover the fill goes to `#FFFFFF` and the corner brackets tighten inward by 3px. On active, `translateY(1px)`. There is one primary button per screen; a second one halves the value of the first.

**Secondary** — transparent fill, 1px `#161D28` border, text `#8D96A2`, same geometry and label treatment as primary. On hover the border lifts to `#242C39` and the text to `#F1F3F6`. The fill stays transparent at every state.

**Text link** — `#F1F3F6` with a 1px `#161D28` underline offset 4px. On hover the underline takes the accent.

All three are minimum 52px tall. Labels never sentence-case and never lose their tracking.

### Corner Bracket Marker

The signature detail. A primary button is wrapped by four 14px L-shaped brackets, 1px `#DCDCDE`, sitting 8px outside each corner of the control. They are drawn on a wrapper element rather than the button so the button's own box stays square and its hit area stays clean.

Use it on the primary call to action and on nothing else. It reads as a target mark, which is the entire point; applying it to three buttons converts a mark into a border style. On hover the four brackets ease inward 3px over 200ms, which is the only motion in the system that changes an element's geometry.

### Section Eyebrow and Step Numeral

Both are mono, uppercase, letter-spaced. The eyebrow is `#8D96A2` at `0.24em` and sits 24px above its heading with no rule, no icon, and no bullet. The step numeral is `#CB623A` at `0.2em`, zero-padded to two digits, and sits directly above its step heading.

The numerals are the only place the accent appears as standalone text rather than inside a sentence. That is deliberate: it gives the accent a structural job as well as a rhetorical one.

### Cards and Quote Panels

Fill `#12171F`, 1px `#161D28` border, `border-radius: 0`, padding 40px, no shadow at any elevation. Quote panels carry a pixel-block quotation glyph in the top-right corner at `#242C39`, 32px, which is decoration and is `aria-hidden`.

The attribution row sits at the card's bottom edge with 32px of clearance: a 44px circular avatar, then the name in `#F1F3F6` at 16px, then a middot, then the affiliation in `#8D96A2`. The avatar is the only circle in the entire system, and it is circular because a square photograph of a face reads as a mugshot.

Cards never lift on hover. If a card is interactive, its border goes to `#242C39` and nothing else moves.

### Accordion Rows

A stack of full-width rows separated by 1px `#161D28` rules, with a rule above the first and below the last. Each row is 32px vertical padding, the question in 22px grotesque `#F1F3F6`, and a `+` glyph in `#8D96A2` pinned right, rotating 45 degrees to an `×` on open over 200ms.

The open panel reveals body copy at 17px `#C1C8D0` with 24px of clearance below the question and 32px below the panel. The row itself takes no background change on open — the rule structure carries the state, not a fill. The entire row is the trigger, not just the glyph.

### Numbered Step Rail

A vertical 1px `#161D28` line runs the full height of the step list, inset 40px from the gutter. Each step hangs a 44px icon well on the rail: fill `#080E17`, 1px `#161D28` border, sharp corners, holding a pixel-grid glyph in `#8D96A2` with a 2px `#CB623A` underscore at its base.

Step content sits 48px right of the rail: numeral, then a 34px heading, then body copy at `#8D96A2`. Consecutive steps are separated by 80px and a 1px hairline that stops short of the rail rather than crossing it.

On mobile the rail stays. It is the element that makes the sequence legible, and collapsing it to a plain list loses the only structure the section has.

### Navigation Bar

Sticky, `#030A12` at `backdrop-filter: blur(12px)`, 1px `#161D28` bottom border, 80px tall, gutter-aligned. The wordmark sits left in the grotesque at 28px. The menu control is a 56px square with a 1px `#161D28` border, sharp corners, holding a two-line hamburger in `#F1F3F6`.

The bar has no shadow and gains none on scroll — the hairline is the whole separation. Nav is deliberately hidden behind the menu control at every breakpoint, including desktop, so the headline gets the full width.

### Carousel Controls

Pagination is square, not round. Inactive: a 10px square in `#737C89`. Active: a 40px × 10px bar in `#F1F3F6`. Transition is a 240ms width change, not a fade.

Previous and next are 72px squares with a 1px `#161D28` border, sharp corners, holding a chevron in `#8D96A2`. They sit at the outer edges of the pagination row with 24px of gap. Disabled state drops border and glyph to `#12171F` and `#737C89` and keeps the box, so the row's rhythm does not shift.

### Footer

A hairline top rule in `#161D28`, 64px of padding, the wordmark at 28px left, and a single 56px bordered square for a social link at the right. Beneath, the copyright and legal links in mono uppercase `#737C89` at 12px with `0.18em` tracking, left-aligned, 24px apart.

## Layout Principles

Single column by default at every width. The desktop adaptation is wider gutters and a larger type scale, not a new grid — the only places a second column appears are the step rail and the card carousel.

Content max-width is 1160px. Prose blocks inside that are capped at 680px and left-aligned within the container rather than centered, so paragraphs share a left edge with the headings above them.

Sections are separated by vertical space, not by background changes. There is exactly one surface color for the page and one for panels; a system that reaches for a third band has stopped being this system.

Full-bleed dot-matrix imagery sits behind content at low opacity as a block-level element carrying its own background, with a nested gutter element holding the content. It is never positioned with negative viewport margins.

The closing call-to-action is the single centered block on the page, and it earns that by being the only place the reader is asked to act.

## Visual Effects

**Radii:** `0` everywhere except the avatar, which is `border-radius: 50%`. This is the system's most load-bearing constraint. Every button, card, input, icon well, menu control, and pagination dot is a sharp rectangle.

**Shadows:** None. Not on cards, not on the sticky nav, not on hover. Separation comes from the `#161D28` hairline and from stepping to `#12171F`. If something needs to feel raised, step the surface, do not float it.

**Borders:** 1px `#161D28` universally. `#242C39` is a hover state and never a resting border. Nothing in the system uses a 2px border except the focus ring.

**Background treatment:** A dot-matrix halftone field in `#8A4227`, sized 4–6px per dot, at 12–20% opacity, bleeding off the section edge. It is texture, not illustration: it should be readable as a shape at arm's length and as noise up close. One instance per page, in the hero or the closing block, not both.

**Transitions:** 200ms `cubic-bezier(0.4, 0, 0.2, 1)` for color, border, and opacity. 240ms for the pagination width change. Nothing else animates. No scroll-triggered reveals, no parallax on the halftone field.

## Design Tone

Composed, technical, and quietly expensive. The near-black ground and complete absence of shadow give the system a flat, printed quality, while the rust italic serif cutting through a grotesque headline supplies the single moment of voice — a system that argues in prose and then punctuates. The monospace labeling makes every button and eyebrow read as an instrument reading rather than as marketing copy, which is what keeps the long paragraphs from feeling like a brochure.

## Usage Notes for AI Implementation

1. **Never round a corner.** Every rectangle in this system is sharp; the avatar is the sole exception and it is round because a square face photograph reads as an ID card. A 4px radius applied "for softness" converts this into a generic dark SaaS template in a single edit.
2. **One accent phrase per heading, and it must be a clause.** The italic serif works because it reads as an aside inside a sentence. Applying it to a single adjective ("*powerful* results") or to an entire heading collapses the effect and makes the page look like it has two competing display faces.
3. **Never fill anything with the accent.** `#CB623A` is ink, never a surface. An orange button, an orange card, or an orange band destroys the ratio the system depends on — roughly one accent element per screenful, sized to be found rather than avoided.
4. **The eyebrow is structural, not decorative.** Every section starts with a mono uppercase label. Dropping it because a section "is obviously the FAQ" removes the only wayfinding the page has, since there are no background changes to mark section boundaries.
5. **Do not add shadows to create depth.** Step the surface from `#030A12` to `#12171F` instead. A `box-shadow` on a card here is immediately visible as foreign, because nothing else on the page casts one and the ground is dark enough that a shadow reads as a grey halo.
6. **Set prose long and set it wide.** Body paragraphs of four or five sentences at 62 characters are correct. Breaking them into three-line chunks with more whitespace is the standard instinct and it is wrong here — the system's entire argument is that the reader will read, and short marketing fragments make the long-form sections look like a mistake.
7. **Keep the corner brackets on exactly one control.** They are a target mark on the primary call to action. Applied to a secondary button, a card, or an input, they stop being a mark and become a border treatment, and the primary button loses the only thing that distinguished it.
8. **Give the gutter to one element and use longhand vertical padding on its siblings.** A `padding: 96px 0` shorthand on a section class that shares an element with the gutter class wins on source order and flushes content to the viewport edge on mobile, while the nav stays correctly indented — so the page reads as inconsistently aligned rather than obviously broken.
9. **Clamp the display sizes.** A fixed 92px headline overflows a 393px viewport, and the grotesque at 500 weight with `-0.03em` tracking does not break mid-word. Use `clamp()` on every level above 22px and add `overflow-wrap: anywhere` to any type specimen.
10. **The halftone field appears once per page.** It is background texture at 12–20% opacity, built as a block-level band with a nested gutter element. Two instances on one page turn a restrained surface into a patterned one, and negative-viewport-margin full-bleed doubles the document width and forces a horizontal scrollbar at every size.
