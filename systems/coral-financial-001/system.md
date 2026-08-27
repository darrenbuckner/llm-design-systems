---
id: coral-financial-001
title: Coral Financial System
tags: [light, minimal, professional, fintech, cards, high-contrast]
colors: ["#F7FAFC", "#FFFFFF", "#000000", "#E53E3E", "#718096"]
created: 2026-01-09
---

# Coral Financial System

A cool, near-monochrome financial interface built on a faintly blue-grey ground, where black carries every primary action and a single coral red is spent only on the moment that needs attention. Rounded but restrained, shadowless, and built to make numbers legible above everything else. Suited to banking dashboards, payment flows, invoicing, expense tools, and any product where a misread figure is the expensive failure.

## Color Palette

**Page Surface:** `#F7FAFC` — a very pale blue-grey, the ground for every screen and also the fill for input fields at rest. That dual role is deliberate: a field reads as a recess cut into the page rather than an object sitting on it.

**Primary Colors:**
- Ink `#000000` — the primary action color and the color of every number. Pure black, not a near-black, because financial figures need maximum definition. Fills the default button.
- Coral `#E53E3E` — the accent, spent at most once per screen: the emphasis button, an alert, or a negative balance. It is never a general-purpose brand wash.
- Coral Deep `#C53030` — hover and active state for every Coral fill. Never a resting color.

**Neutral Colors:**
- Card White `#FFFFFF` — every card, panel, and elevated surface.
- Slate `#2D3748` — headings and card titles. A cool near-black one step softer than Ink, which keeps pure black reserved for numbers and buttons.
- Muted `#718096` — body copy, labels, captions, placeholder text, links, and tag text. Runs cool to match the ground.
- Hairline `#E2E8F0` — the border on every card, input, and divider. One weight, one color.

**Accent/State Colors:**
- Negative `#E53E3E` — reuses Coral for a falling figure or a debit.
- Positive `#2F855A` — a rising figure or a credit. Text and glyph only, never a fill.
- Focus Ring `#000000` at 2px offset 2px — black rather than Coral, so focus never competes with the alert color.
- Disabled — `#E2E8F0` fill with `#718096` label.

## Typography

**Display & Headings:** a single neutral grotesque across the whole interface, differentiated by weight rather than family. Google Fonts equivalent: `Inter`, weights 400/500/600/700. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`.

**Numerals:** a monospaced face for every figure, account number, and transaction ID. Google Fonts equivalent: `JetBrains Mono`, weights 400/500. Fallback: `'JetBrains Mono', 'SF Mono', Monaco, monospace`. This is the system's one typographic split and it is functional rather than decorative — a column of monospaced amounts aligns without tabular-figure tricks and cannot be misread across rows.

**Type Scale:**
- Display figure (mono) — 48px / 500 / 1.10 / -0.02em
- Page title — 32px / 700 / 1.20 / -0.02em
- Section heading — 24px / 600 / 1.30 / -0.01em
- Card title — 18px / 600 / 1.40 / 0
- Table figure (mono) — 16px / 400 / 1.50 / 0
- Body — 16px / 400 / 1.60 / 0, set in Muted
- Button — 16px / 600 / 1.00 / 0
- Label — 14px / 500 / 1.40 / 0, set in Muted
- Caption and link — 14px / 400 / 1.40 / 0, set in Muted

**Hierarchy Rules:** The sans carries language and the mono carries quantity — any figure a user might compare, sum, or transcribe is set in the monospaced face, and prose never is. Headings are Slate, numbers are Ink, and everything explanatory is Muted, so the page has three text tones doing three distinct jobs. Coral never appears in a heading. Nothing is italic or all-caps.

## Spacing System

**Base Unit:** 8px.

**Scale:** 8, 16, 24, 32, 48, 64, 96.

**Common Patterns:**
- Page gutter 24px; content measure capped at 1200px.
- Section to section: 64px.
- Card padding 24px; a card holding a display figure gets 32px.
- Card to card in a grid: 24px.
- Button padding 16px 24px.
- Input padding 16px, 16px between stacked fields, 8px from label to field.
- Table row height 56px with 16px horizontal cell padding.
- Heading to first content block: 24px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses longhand `padding-top` / `padding-bottom`, never a `padding: 64px 0` shorthand on that element, which would win on source order and zero the gutter.

## Component Styles

### Buttons

**Default** — fill `#000000`, label `#FFFFFF` at 16px/600, 8px radius, padding 16px 24px, no border, no shadow. Hover: fill `#2D3748`. This is the standard action; black rather than a brand color is what keeps the interface calm around loud numbers.

**Emphasis** — fill `#E53E3E`, label `#FFFFFF`, otherwise identical. Used at most once per screen for the irreversible or time-sensitive action. Hover: `#C53030`.

**Quiet** — fill `#FFFFFF`, 1px `#E2E8F0` border, label `#000000`. Hover: fill `#F7FAFC`. The default for anything reversible.

### Cards

Fill `#FFFFFF`, 1px `#E2E8F0` border, 8px radius, 24px padding, **no shadow**. Separation is the hairline plus the tonal step from `#F7FAFC`. Hover on an interactive card darkens the border to `#CBD5E0`; nothing lifts.

### Figure Blocks

A card containing a 14px/500 Muted label, then a 48px monospaced figure in Ink, then an optional 14px delta line in Positive or Negative with a leading arrow glyph. The figure is always the largest thing in the card and never shares a line with anything else.

### Input Fields

Fill `#F7FAFC` — the page ground — with 1px `#E2E8F0` border, 8px radius, padding 16px, 16px/400 in Ink. Placeholder in Muted. Focus: border `#000000` plus a 2px black ring at 2px offset, and the fill lifts to `#FFFFFF`. That fill change on focus is the system's clearest affordance: the recess becomes a surface while you type. Invalid: 1px `#E53E3E` border with the message beneath at 14px in Coral.

### Form Groups

A label at 14px/500 Muted, 8px, the field, then an optional 14px helper line in Muted. Groups stack with 16px between them. Labels are never placed inside the field as a substitute for a placeholder.

### Tables

No outer border — the containing card provides it. Rows are 56px with a 1px `#E2E8F0` bottom rule, no zebra striping. Header cells are 14px/500 Muted; body cells are 16px, with any numeric column in the monospaced face and right-aligned. The final row has no rule beneath it.

### Tags

Fill `#F7FAFC`, no border, 8px radius, padding 8px 16px, 14px/500 in Muted. Deliberately the quietest component in the system — tags label, they do not attract.

### Links

14px/400 in Muted with no underline at rest. Hover: color shifts to `#000000` and an underline appears. Links are never Coral.

## Layout Principles

A single centered column capped at 1200px with a 24px gutter, built from stacked sections. Card grids run two to four across on desktop depending on density and collapse to one column below 600px. Figure blocks are always in a grid of equal-width cards so the numbers align across the row. Tables are always inside a card and never run edge to edge. Everything is left-aligned; nothing centers, because centered figures are harder to scan down a column. There is no sidebar in the core layout — the system assumes a top bar and a single content well.

## Visual Effects

No shadows anywhere. Radii are a uniform 8px on cards, buttons, inputs, and tags — this system does not vary radius by component, which is part of why it reads as neutral infrastructure. Borders are always 1px `#E2E8F0`. No gradients, no glass, no texture, no blur. Transitions are 150ms ease on background-color, border-color, and color only.

## Design Tone

Quiet, precise, and slightly cool. Black doing the work a brand color usually does keeps the interface from competing with its own data, and the monospaced figures give it the exactness a financial product needs without any visual flourish. The single coral is the only raised voice in the room, which is why it lands.

## Usage Notes for AI Implementation

1. **Every figure is monospaced.** Amounts, balances, account numbers, transaction IDs, dates in numeric form. Prose is never monospaced. This is the system's core rule — a proportional column of currency is the failure mode it exists to prevent.

2. **Black is the action color; coral is the exception.** The default button is black. Coral appears at most once per screen, for the irreversible or urgent action. Making coral the general button color removes the only signal the system has.

3. **Three text tones, three jobs.** Ink `#000000` for numbers and button labels, Slate `#2D3748` for headings, Muted `#718096` for everything explanatory. Collapsing these into one color removes the scan hierarchy entirely.

4. **Inputs are the ground color, not white.** `#F7FAFC` fill makes a field read as a recess. On focus the fill lifts to `#FFFFFF` — keep that transition; it is the clearest interaction feedback in the system.

5. **No shadows and one radius.** 8px everywhere, hairline borders, zero elevation. Varying radius by component or adding a shadow to figure cards makes the page look like a consumer app rather than infrastructure.

6. **Numeric columns right-align.** Always, in tables and in any list of amounts. Left-aligned currency defeats the point of the monospaced face.

7. **Coral is never a heading, a link, or a tag.** It is a fill for one button, or a text color for a negative figure and a validation message. Nothing else.

8. **No zebra striping in tables.** Rows separate with a 1px bottom rule. Alternating fills fight the card fill and make the monospaced column harder to track, not easier.

9. **Focus rings are black, not coral.** Focus must never look like an error or an alert, and coral is already carrying that meaning.

10. **Positive green is text only.** `#2F855A` colors a rising figure or a credit. It is never a fill, a button, or a badge background — the system has exactly one chromatic fill and it is coral.
