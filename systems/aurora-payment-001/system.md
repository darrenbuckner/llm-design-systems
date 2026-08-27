---
id: aurora-payment-001
title: Aurora Payment System
tags: [dark, glass, gradient, minimal, modern, payment-ui]
colors: ["#1a1a1a", "#2d3748", "#00E5FF", "#4A90E2", "#ffffff"]
created: 2026-01-21
---

# Aurora Payment System

A dark, atmospheric payment interface built on a diagonal charcoal-to-slate gradient, where translucent blurred panels float over the ground and a single electric cyan carries the amount and every primary action. Light in weight and generous in radius, with the transaction figure treated as the hero of the screen. Suited to checkout flows, wallets, transfer confirmations, and any moment where a person is about to move money and wants the interface to feel calm and expensive.

## Color Palette

**Page Surface:** `#1a1a1a` — the base of the page gradient, which runs `linear-gradient(135deg, #1a1a1a 0%, #2d3748 100%)`. The diagonal is the system's atmosphere: charcoal at the top-left resolving to a cool slate at the bottom-right, so the ground is never flat and the glass panels have something to be translucent *against*.

**Primary Colors:**
- Aurora Cyan `#00E5FF` — the accent. The transaction amount, primary button fill, tag borders, and active states. Electric enough to be the single thing the eye lands on against a desaturated ground.
- Signal Blue `#4A90E2` — the secondary action color, used as a 20%-opacity fill with a solid border and matching text. Always subordinate to cyan; never used for the primary action.
- Muted Cyan `#66D9EF` — a softened cyan for supporting labels beside a cyan figure, so a caption does not compete with the amount it describes.

**Neutral Colors:**
- Slate `#2d3748` — the gradient terminus, and the fill for any element that needs to read as part of the ground rather than floating on it.
- Text Primary `#ffffff` — headings, body copy, button labels on cyan.
- Text Secondary `rgba(255, 255, 255, 0.7)` — supporting copy and metadata. Expressed as an alpha rather than a hex, deliberately, so it sits correctly on both ends of the gradient.
- Glass Stroke `rgba(255, 255, 255, 0.1)` — the 1px border on every translucent panel. It is the only thing giving a glass card an edge.

**Accent/State Colors:**
- Success `#00E5FF` — reuses Aurora Cyan. A completed payment is the system's happy path and it already owns the accent.
- Error `#FF6B6B` — message text and a 1px border on the offending field.
- Focus Ring `#00E5FF` at 2px offset 2px.

## Typography

**Display & Headings:** a single neutral system sans across the whole interface. Google Fonts equivalent: `Inter`, weights 300/400/500/600. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`.

**The 300 weight matters.** The transaction amount is set at weight 300 — lighter than body text — which is what keeps a 72px figure from feeling aggressive. On a dark ground a light weight at large size reads as elegant; the same figure at 600 reads as a bill.

**Type Scale:**
- Amount — `clamp(48px, 8vw, 72px)` / **300** / 1.10 / -0.02em, in Aurora Cyan
- Page title — `clamp(32px, 5vw, 48px)` / 400 / 1.20 / -0.01em
- Section heading — 32px / 400 / 1.30 / 0
- Card title — 20px / 500 / 1.40 / 0
- Body — 16px / 400 / 1.60 / 0, in Text Secondary
- Button — 16px / 500 / 1.00 / 0
- Label and tag — 14px / 500 / 1.40 / 0
- Caption — 14px / 400 / 1.40 / 0, in Text Secondary

**Hierarchy Rules:** Headings run at 400 rather than 600 — the whole system is deliberately light-weight, and hierarchy comes from size and from the cyan rather than from boldness. The amount is the only element permitted to be cyan and large at the same time; a cyan heading next to a cyan figure produces two focal points where there should be one. Nothing is italic or all-caps. Body copy sits in the 70% white rather than pure white, which keeps full white available for the handful of lines that matter.

## Spacing System

**Base Unit:** 8px.

**Scale:** 8, 16, 24, 32, 48, 64, 96.

**Common Patterns:**
- Page gutter 24px; content measure capped at 960px — narrower than a typical dashboard, because payment flows are single-task.
- Hero block padding 64px 24px, centered, 48px below it.
- Glass card padding 32px; card to card 24px.
- Amount block: 24px above and below the figure, so it is never crowded by its own label.
- Button padding 16px 24px with an 8px gap to a leading icon.
- Input padding 16px, 16px between stacked fields.
- Section to section: 48px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses longhand `padding-top` / `padding-bottom`, never a `padding: 48px 0` shorthand on that element, which would win on source order and zero the gutter.

## Component Styles

### Glass Cards

Fill `rgba(26, 26, 26, 0.85)`, `backdrop-filter: blur(10px)`, 1px `rgba(255, 255, 255, 0.1)` border, **16px radius**, 32px padding. This is the system's core component and every part of it is load-bearing: the 85% opacity lets the gradient show through so the card belongs to the page, the blur keeps content behind it from being distracting, and the 10% white stroke is the only thing defining the edge. Remove any one of the three and the card stops reading as glass.

Glass cards require a non-flat backdrop. On a solid fill the blur has nothing to blur and the translucency has nothing to reveal, which is why the page gradient is mandatory rather than decorative.

### Hero Block

A more opaque variant at `rgba(26, 26, 26, 0.9)`, 16px radius, 64px 24px padding, centered contents, no border. Holds the transaction amount and its label. The extra opacity is deliberate — the one place the reader must not be distracted gets the least transparency.

### Buttons

**Primary** — fill `#00E5FF`, label `#1a1a1a` at 16px/500, 8px radius, padding 16px 24px, no border. Dark type on cyan rather than white: cyan is too light to carry white legibly, and the inversion is what makes the button the brightest object on the screen.

**Secondary** — fill `rgba(74, 144, 226, 0.2)`, 1px `#4A90E2` border, label `#4A90E2`, same radius and padding. A tinted-glass button rather than a solid one, so it belongs to the same material family as the cards.

Both take an optional 20px leading icon with an 8px gap. There is no ghost or text-only button — on a gradient ground a borderless control disappears.

### Tags

Fill `rgba(0, 229, 255, 0.2)`, 1px `#00E5FF` border, `border-radius: 24px`, padding 8px 16px, 14px/500 in Aurora Cyan. The tinted-fill-plus-solid-border construction is the same one the secondary button uses, in the accent hue.

### Input Fields

Fill `rgba(255, 255, 255, 0.06)`, 1px `rgba(255, 255, 255, 0.15)` border, 8px radius, padding 16px, 16px in Text Primary. Placeholder in Text Secondary. Focus: border `#00E5FF` plus a 2px cyan ring at 2px offset. Fields are translucent like everything else — a solid input on a glass card breaks the material.

### Amount Display

A label at 14px in Text Secondary, then the figure at `clamp(48px, 8vw, 72px)` weight 300 in Aurora Cyan, then an optional 14px supporting line in Muted Cyan. Always centered, always inside the hero block, always the largest thing on the screen. Currency symbols are set at the same weight, never superscripted.

### Dividers

1px `rgba(255, 255, 255, 0.1)` — the same value as the glass stroke, so a divider inside a card reads as part of the same construction.

## Layout Principles

A single centered column capped at 960px with a 24px gutter, on a fixed diagonal gradient that does not scroll with the content. The page is a hero block followed by a stack of glass cards; card grids run two across on desktop and collapse to one column below 700px. Everything inside the hero centers; everything inside a glass card is left-aligned except a confirmation state. Because the ground is a gradient, no element is ever full-bleed — the visible margin around each card is what lets the gradient read as atmosphere rather than as a backdrop image.

## Visual Effects

The defining effect is `backdrop-filter: blur(10px)` on translucent panels, and it is the only blur in the system. Radii: 16px on cards and the hero, 8px on buttons and inputs, 24px pill on tags. Borders are always 1px white at 10–15% opacity. There are no drop shadows — depth is translucency and blur, not elevation, and a shadow under a glass card makes it look like a sticker instead of a pane. Transitions are 200ms ease on background-color, border-color, and opacity.

**Fallback:** where `backdrop-filter` is unsupported, glass cards fall back to a solid `#1f2430` at full opacity, keeping the border and radius. The layout must not depend on seeing the gradient through a card.

## Design Tone

Calm, premium, and slightly futuristic. The gradient and the blurred panes give it the feeling of a heads-up display rather than a form, and the light-weight cyan figure makes an amount of money feel like information rather than a demand. It is designed for the two seconds before someone confirms a transaction.

## Usage Notes for AI Implementation

1. **The gradient is mandatory, not decorative.** `linear-gradient(135deg, #1a1a1a, #2d3748)` is what glass cards are translucent against. On a flat fill the blur has nothing to blur and every card collapses into a slightly-different-grey rectangle.

2. **Glass is three properties together.** `rgba(26,26,26,0.85)` + `backdrop-filter: blur(10px)` + a 1px 10%-white border. Dropping the border removes the edge, dropping the blur removes the material, dropping the alpha removes the point.

3. **The amount is weight 300.** Lighter than body text. A 72px figure at 600 reads as a bill; at 300 it reads as a balance. This is the single most characteristic decision in the system.

4. **Cyan is the amount and the primary action — nothing else large.** A cyan heading beside a cyan figure creates two focal points. Cyan may appear small (tag borders, focus rings) but only once at display size.

5. **The primary button carries dark type.** `#1a1a1a` on `#00E5FF`. White on cyan fails; inverting is what makes the button the brightest thing on screen.

6. **No shadows.** Depth is translucency and blur. A drop shadow under a glass card turns a pane into a sticker.

7. **Secondary actions are tinted glass, not solid.** `rgba(74,144,226,0.2)` with a solid `#4A90E2` border. A solid secondary button breaks the material logic that every other surface follows.

8. **Body copy is 70% white, not pure white.** Full white is reserved for headings and the few lines that matter. Setting all copy to `#ffffff` on this ground is both harsh and flattening.

9. **Nothing is full-bleed.** The gradient must show around every card. A card running edge to edge turns the atmosphere into a background image.

10. **Always ship the no-blur fallback.** `backdrop-filter` is the system's whole identity and also its most fragile dependency — a solid `#1f2430` fallback keeps the layout intact where it is unsupported.
