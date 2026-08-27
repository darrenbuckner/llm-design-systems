---
id: light-tax-service-001
title: Sage Financial System
tags: [light, professional, warm, minimal, cards, trustworthy]
colors: ["#F8F6F3", "#FFFFFF", "#2D5B3F", "#1A1A1A", "#666666"]
created: 2026-01-21
---

# Sage Financial System

A calm, warm-neutral service interface built on a paper-toned ground, where white cards outlined in a single hairline carry every piece of content and one deep forest green marks the path forward. Generously rounded, entirely shadowless, and deliberately unhurried — the system is designed for people making a decision they are slightly anxious about. Suited to tax and accounting services, legal intake, financial advisory, healthcare admin, and any flow where reassurance matters more than energy.

## Color Palette

**Page Surface:** `#F8F6F3` — a warm paper neutral with a faint pink cast, the ground for every screen. It is doing specific work: against `#FFFFFF` cards it produces a visible but very soft edge, which is what lets the system drop shadows entirely. Roughly 55% of any screen.

**Primary Colors:**
- Forest `#2D5B3F` — the single action color. Primary buttons, active states, and the one link per screen that matters. Deep enough to carry white type at 8.9:1.
- Forest Hover `#4A6B56` — hover and active state for every Forest fill. Notice it goes *lighter* rather than darker, which keeps the button feeling like it is lifting toward the user rather than being pressed away.

**Neutral Colors:**
- Card White `#FFFFFF` — every card, panel, and input fill. The only surface that sits on the ground.
- Ink `#1A1A1A` — headings, card titles, input values, and any number the reader needs to trust.
- Ink Secondary `#666666` — body copy, descriptions, captions, placeholder text, and tag labels. This system runs most of its prose in the secondary tone deliberately; full-strength ink is reserved for what the eye should land on.
- Hairline `#E5E5E5` — the border on every card, input, tag, and divider. One weight, one color, no exceptions.

**Accent/State Colors:**
- Leaf `#7FB069` — illustration and iconography only. A lighter, friendlier green used inside process icons and spot drawings. Never a button, never a border, never type.
- Sky `#4A9EE0` — illustration only, as the secondary drawing color alongside Leaf.
- Error `#B3352B` — message text and a 1px border on the offending input.
- Success `#2D5B3F` — reuses Forest; the system introduces no second green for state.
- Focus Ring `#2D5B3F` at 2px offset 2px.

## Typography

**Display & Headings:** the system uses a single humanist sans-serif across the whole interface, differentiated by weight and size rather than by family. Google Fonts equivalent: `Inter`, weights 400/500/600/700. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`. There is no serif anywhere; a serif would push this toward legal-formal, which is exactly the register the warm ground is working against.

**Numerals:** tabular figures wherever amounts, refunds, or deadlines appear, so a column of currency aligns on the decimal.

**Type Scale:**
- Page title — 40px / 600 / 1.20 / -0.02em
- Section heading — 28px / 600 / 1.25 / -0.01em
- Card title — 20px / 600 / 1.35 / 0
- Process title — 18px / 600 / 1.40 / 0
- Lead paragraph — 18px / 400 / 1.60 / 0, set in Ink Secondary
- Body — 16px / 400 / 1.60 / 0, set in Ink Secondary
- Input value — 16px / 400 / 1.40 / 0, set in Ink
- Button — 16px / 600 / 1.00 / 0
- Tag and caption — 14px / 500 / 1.40 / 0, set in Ink Secondary

**Hierarchy Rules:** Weight carries hierarchy and color carries emphasis — headings are 600 in full-strength Ink while everything explanatory is 400 in Ink Secondary, which produces a page where the eye lands on titles and numbers without any color being spent. Nothing is italic, nothing is all-caps, and no heading is ever set in Forest: green means *action*, and coloring a heading green makes the reader look for a button that is not there. Line length is capped at 65 characters.

## Spacing System

**Base Unit:** 8px.

**Scale:** 8, 16, 24, 32, 48, 64, 96.

**Common Patterns:**
- Page gutter 24px; content measure capped at 1120px.
- Section to section: 64px desktop, 48px mobile.
- Card padding 32px; process card padding 32px 24px with centered contents.
- Card to card in a grid: 24px.
- Button padding 16px 48px — unusually wide horizontally, which is what gives the primary action its calm, unhurried proportion.
- Input padding 16px, with 16px between stacked fields and 8px from label to field.
- Tag padding 8px 16px.
- Heading to its first paragraph: 16px. Paragraph to a card grid: 32px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses longhand `padding-top` / `padding-bottom`, never a `padding: 64px 0` shorthand on that element, which would win on source order and zero the gutter.

## Component Styles

### Buttons

**Primary** — fill `#2D5B3F`, label `#FFFFFF` at 16px/600, `border-radius: 32px` (a full pill), padding 16px 48px, no border, no shadow. Hover: fill `#4A6B56`. Disabled: fill `#E5E5E5`, label `#666666`, pill shape retained.

**Secondary** — fill `#FFFFFF`, 1px `#E5E5E5` border, label `#1A1A1A`, same pill radius and padding. Hover: border `#2D5B3F`, label `#2D5B3F`, fill unchanged. The hover *adopts* the action color rather than filling with it.

There is no destructive button variant. Destructive actions are a secondary button plus a confirmation step, because a red button on this ground reads as an alarm.

### Cards

Fill `#FFFFFF`, 1px `#E5E5E5` border, **16px radius**, 32px padding, **no shadow**. The generous radius paired with a hairline is the system's signature: it reads soft without floating. Cards never gain a shadow on hover; hover darkens the border to `#D5D5D5` and nothing moves.

### Process Cards

A card variant with centered contents and 32px 24px padding: a 48px illustrated icon drawn in Leaf and Sky at the top, then an 18px/600 title in Ink, then a 16px/400 description in Ink Secondary. Used in rows of three or four to explain a sequence. The icon is the only place illustration color appears.

### Input Fields

Fill `#FFFFFF`, 1px `#E5E5E5` border, **8px radius**, padding 16px, 16px/400 in Ink. Placeholder in Ink Secondary. Focus: border `#2D5B3F` plus a 2px Forest ring at 2px offset. Invalid: 1px `#B3352B` border with the message beneath at 14px in the same red.

Inputs use 8px radius while cards use 16px. The smaller radius is deliberate — it keeps a field reading as a slot to fill rather than as another card.

### Tags

Fill `#FFFFFF`, 1px `#E5E5E5` border, `border-radius: 32px`, padding 8px 16px, 14px/500 in Ink Secondary. Non-interactive at rest. As a filter, the selected state fills `#2D5B3F` with white type.

### Dividers

1px `#E5E5E5` at full container width. Never doubled, never inset, and never placed inside a card — within a card, separation is spacing.

### Illustration

Flat, rounded, two-color line-and-fill drawings in Leaf and Sky over white, with Ink used sparingly for outlines. Illustration appears inside process icons and at most one hero spot per page. It never bleeds off an edge and never sits directly on the page ground — always inside a white card.

## Layout Principles

A single centered column capped at 1120px with a 24px gutter. Content is a vertical stack of full-measure prose blocks and card grids; process cards run three or four across on desktop, two on tablet, and one below 600px. Everything is left-aligned except process cards, which center their contents, and the single hero block, which may center. There is no sidebar and no two-column body — the system is built for linear flows where the reader is being walked through steps. Forms are always full-measure inside a card rather than floating on the ground, which keeps the paper-toned background as pure negative space.

## Visual Effects

No shadows anywhere. Separation comes from the hairline border plus the small tonal step between `#F8F6F3` and `#FFFFFF`. Radii: 16px on cards and process cards, 8px on inputs, 32px (full pill) on buttons and tags. Borders are always 1px `#E5E5E5`. No gradients, no glass, no texture, no blur. Transitions are 200ms ease on background-color, border-color, and color — slightly slower than typical, which suits the unhurried register. Nothing translates, scales, or lifts.

## Design Tone

Calm, warm, and reassuring without being soft-headed. The paper-toned ground and the fully rounded buttons take the institutional edge off what is usually a stressful category, while the single deep green and the disciplined hairline keep it credible rather than cute. It reads like a well-designed letter from someone competent.

## Usage Notes for AI Implementation

1. **The ground is warm, not white.** `#F8F6F3` against `#FFFFFF` cards is what makes a shadowless system legible. Setting the page to white collapses the card edges and forces you to reach for elevation the system does not have.

2. **Green means action, never emphasis.** Forest is for primary buttons, active states, and focus rings. A green heading makes the reader hunt for a control. Emphasis is weight and Ink, not color.

3. **Body copy runs in the secondary tone.** 16px/400 `#666666` for prose, full-strength `#1A1A1A` reserved for headings, card titles, and numbers. Setting all body text to full Ink flattens the page and removes the cue telling the eye where to land.

4. **No shadows, ever.** Cards separate by 1px hairline plus the ground's tonal step. A box-shadow on a 16px-radius white card instantly turns this into a generic SaaS marketing page.

5. **Keep the radius split.** 16px on cards, 8px on inputs, full pill on buttons. Matching input radius to card radius makes fields read as nested cards; matching card radius to the pill makes the whole page look like a toy.

6. **Illustration colors never enter the UI.** Leaf and Sky exist inside drawings and process icons. They are never a button, a border, a tag fill, a chart series, or a text color.

7. **The primary button is wide.** 16px 48px padding is not arbitrary padding — the horizontal generosity is what gives the action its calm proportion. Tightening it to 16px 24px makes the button read as urgent.

8. **Hover goes lighter, not darker.** Forest Hover `#4A6B56` is above the resting fill. Darkening on hover reads as pressure; lightening reads as invitation, which is the register this system wants.

9. **No red buttons.** Destructive actions are a secondary button plus confirmation. Red is reserved for validation messages, because on this warm ground a red fill reads as an emergency.

10. **Forms live inside cards.** An input floating directly on `#F8F6F3` loses its edge, since the field fill and the card fill are the same white. Always nest the form in a card.
