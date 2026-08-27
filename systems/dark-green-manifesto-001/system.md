---
id: dark-green-manifesto-001
title: Forest Principles Design System
tags: [dark, green, minimal, premium, cards, serif]
colors: ["#4A7C66", "#2D5547", "#F5F3EF", "#FFFFFF", "#1A1A1A"]
created: 2026-01-08
---

# Forest Principles Design System

A statement interface built on a vertical forest-green gradient, where warm cream cards rise out of the field like pages set on a table and a numbered badge marks each principle in sequence. A serif masthead over a plain sans body gives it the register of a printed manifesto rather than a product page. Suited to values pages, principles and charters, sustainability reports, mission statements, and any surface whose job is to be read once and remembered.

## Color Palette

**Page Surface:** `#4A7C66` — the top of the page gradient, which runs `linear-gradient(180deg, #4A7C66 0%, #2D5547 100%)`. The field deepens as the reader scrolls, which is the system's one piece of motion and the reason the ground is a gradient rather than a flat green.

**Primary Colors:**
- Forest Light `#4A7C66` — the gradient's upper stop. Also the fill for any element that should read as slightly lifted off the field.
- Forest Deep `#2D5547` — the gradient's lower stop, and the fill for badges and primary buttons. Carries white type at 7.6:1.
- Forest Darkest `#1E3A2F` — hover and pressed state for every Forest Deep fill, plus the footer band where the page needs to terminate.

**Neutral Colors:**
- Cream `#F5F3EF` — the card surface. Every card, panel, and quote block. This is the system's counterweight: warm rather than white, so a card reads as paper laid on the field rather than as a hole cut in it.
- Ink `#1A1A1A` — all type on a Cream card.
- Ink Body `#3D3D3D` — body copy and category labels inside a card.
- Heading White `#FFFFFF` — all type directly on the green field.

**Accent/State Colors:**
- Error `#B3352B` — message text on a Cream card only; the system never shows an error directly on the field.
- Focus Ring `#F5F3EF` on the field, `#2D5547` on a Cream card — the ring inverts with the surface, because a single ring color fails on one of the two.
- Tag fill `rgba(245, 243, 239, 0.15)` — cream at low alpha, the only translucent surface in the system.

**Two type environments.** Every color decision follows from which of the two surfaces you are on: white type on green, ink type on cream. There is no third environment and no element that spans both.

## Typography

**Display & Headings:** a classical serif for the masthead and any statement line set directly on the green field. Google Fonts equivalent: `Source Serif 4`, weights 400/600. Fallback: `'Source Serif 4', Georgia, 'Times New Roman', serif`.

**Body & UI:** a neutral grotesque for card content, buttons, labels, categories, and tags. Google Fonts equivalent: `Inter`, weights 400/500/700. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`.

**Type Scale:**
- Masthead (serif) — 48px / 400 / 1.15 / -0.01em, in Heading White
- Section heading (sans) — 32px / 700 / 1.25 / 0, in Heading White
- Principle title (sans) — 20px / 600 / 1.35 / 0, in Ink
- Card body (sans) — 16px / 400 / 1.60 / 0, in Ink Body
- Subtitle (sans) — 16px / 400 / 1.50 / 0, in Cream at 90% opacity
- Category label (sans) — 14px / 400 / 1.40 / 0, in Ink Body
- Badge numeral (sans) — 16px / 700 / 1.00 / 0, in Heading White
- Button (sans) — 16px / 500 / 1.00 / 0
- Tag (sans) — 14px / 500 / 1.40 / 0, in Cream

**Hierarchy Rules:** The serif appears only on the green field and only for the masthead or a standalone statement — it never sets card content, which is what keeps a page of numbered principles from reading as an essay. Section headings are sans at 700 rather than serif, so the serif stays rare enough to feel like a voice rather than a style. Card titles are 600 and card body is 400; there is no bold inside body copy. Nothing is italic or all-caps.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 20, 24, 28, 32, 48, 64, 96.

**Common Patterns:**
- Page gutter 24px; content measure capped at 880px — this is a reading page, not a dashboard.
- Masthead to first card: 48px. Section to section: 64px.
- Card padding 28px, with a 20px gap between the badge and the card's text column.
- Card to card: 16px — tighter than most systems, so a run of principles reads as one list rather than as separate objects.
- Button padding 12px 24px. Tag padding 6px 16px.
- Card title to its body: 8px. Category label to title: 4px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses longhand `padding-top` / `padding-bottom`, never a `padding: 64px 0` shorthand on that element, which would win on source order and zero the gutter.

## Component Styles

### Principle Cards

The system's signature component. Fill `#F5F3EF`, **12px radius**, 28px padding, `box-shadow: 0 2px 8px rgba(0,0,0,0.1)`, laid out as a flex row: a 40px circular badge, a 20px gap, then the text column. The text column runs category label, title, body.

This is the one system in the library that keeps a shadow, and it is doing real work — a cream card on a mid-value green has weak edge contrast, so a soft shadow is what makes it sit *on* the field rather than being cut out of it. The shadow is deliberately small: 2px offset, 8px blur, 10% black. Anything larger reads as a floating modal.

### Badges

A **40px circle**, fill `#2D5547`, white 16px/700 numeral, perfectly centered, `border-radius: 50%`. Badges are always sequential — they number principles, never categorize them. A badge never carries an icon or a letter.

### Buttons

**Primary** — fill `#2D5547`, label `#FFFFFF` at 16px/500, 8px radius, padding 12px 24px, no border. Hover: `#1E3A2F`. On a Cream card this is the default; on the green field it needs the Cream variant below to stay visible.

**Secondary** — transparent fill, **2px** `#2D5547` border, label `#2D5547`, same radius and padding. Hover: fill `#2D5547`, label white. The 2px border is heavier than the system's other strokes because it sits on cream and needs to hold its own against the card's own weight.

**On the field** — fill `#F5F3EF`, label `#2D5547`. A Forest Deep button directly on the green gradient is nearly invisible; on the field the button inverts to cream.

### Tags

Fill `rgba(245, 243, 239, 0.15)`, no border, `border-radius: 20px`, padding 6px 16px, 14px/500 in Cream. Used on the green field only — on a Cream card a tag takes a 1px `#D8D5CE` border and Ink Body type instead.

### Color Swatches

A Cream card at 12px radius with 16px padding and the same 2px/8px shadow, containing the swatch fill and its label. Swatches follow the card construction exactly rather than being bare rectangles.

### Dividers

On a Cream card: 1px `#D8D5CE`. On the field: `rgba(245, 243, 239, 0.2)`. The system never puts a divider between principle cards — the 16px gap is the separation.

## Layout Principles

A single centered column capped at 880px with a 24px gutter, on a fixed vertical gradient that spans the full page height rather than repeating per section. The page is a masthead set directly on the field, followed by a tight stack of principle cards, closed by a footer band in Forest Darkest. Cards are always full-measure and stacked — they are never placed in a two- or three-across grid, because a numbered sequence read left-to-right loses its order. Content is left-aligned throughout except the masthead, which may center. Below 600px the badge and text column stay side by side rather than stacking; a 40px badge above a paragraph breaks the row rhythm that makes the list scannable.

## Visual Effects

The page gradient runs `180deg` from `#4A7C66` to `#2D5547` across the full document height. Radii: 12px on cards and swatches, 20px pill on tags, 8px on buttons, 50% on badges. The only shadow in the system is `0 2px 8px rgba(0,0,0,0.1)` on Cream cards, and it exists because cream-on-green has weak edge contrast. No gradients other than the page field, no glass, no blur, no texture. Transitions are 150ms ease on background-color, border-color, and color.

## Design Tone

Considered, grounded, and quietly institutional. The deepening green field gives the page a sense of descent as you read, and the cream cards sitting on it feel like physical pages rather than interface. The serif masthead over sans principles is what separates it from a marketing page — it reads like something an organization committed to rather than something it is selling.

## Usage Notes for AI Implementation

1. **The ground is a green gradient, not a cream page.** `#4A7C66` to `#2D5547` vertically. `#F5F3EF` is the *card* fill. Inverting the two — cream page with green cards — produces a completely different and much more ordinary system, and it is exactly the error the original spec described.

2. **Two type environments, no third.** White type on the green field, Ink type on a Cream card. Every color decision follows from which surface you are on. An element that tries to span both will fail on one of them.

3. **Keep the card shadow.** This is the one system in the library that legitimately needs one: cream on mid-value green has weak edge contrast. `0 2px 8px rgba(0,0,0,0.1)` and no larger — a bigger shadow turns a page into a floating modal.

4. **Buttons invert on the field.** Forest Deep on green is nearly invisible. A button placed directly on the gradient is cream with Forest Deep type; the green button belongs on cream.

5. **The serif appears only on the field, only for the masthead.** It never sets card titles or body. Section headings are sans at 700. Spending the serif on card content turns a manifesto into an essay.

6. **Badges are sequential numerals.** 40px circles, Forest Deep, white numeral. Never an icon, never a letter, never a category marker. They exist to say *this is principle three of seven*.

7. **Cards stack, never grid.** A numbered sequence in a three-across grid loses its reading order. Full-measure and stacked at every breakpoint.

8. **Card gap is 16px — tighter than it looks like it should be.** The tight spacing is what makes a run of principles read as one list. Opening it to 24px or 32px turns a manifesto into a set of unrelated cards.

9. **Focus rings invert with the surface.** Cream on the field, Forest Deep on a card. A single ring color is invisible on one of the two surfaces.

10. **The badge stays beside the text on mobile.** Stacking a 40px circle above a paragraph breaks the row rhythm the list depends on. Keep the flex row and let the text column narrow instead.
