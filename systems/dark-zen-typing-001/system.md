---
id: dark-zen-typing-001
title: Carbon Flow System
tags: [dark, minimal, zen, productivity, focus, monochrome]
colors: ["#3A3A3A", "#4A4A4A", "#FFFFFF", "#F5A623", "#A8A8A8"]
created: 2026-01-13
---

# Carbon Flow System

A deliberately mid-grey focus interface where the ground is neither black nor white, every surface is a translucent white overlay rather than a new color, and one amber numeral is the only chromatic element on the screen. Built around a single enormous figure and a row of round controls beneath it. Suited to typing tests, timers, meditation and breathing apps, focus modes, and any single-task screen that should recede while the user concentrates.

## Color Palette

**Page Surface:** `#3A3A3A` — a mid-grey ground, and the most unusual decision in the system. Pure black is stark and pure white is glaring; a mid-grey at roughly 20% luminance is the value that disappears fastest in a dim room, which is what a focus surface wants. Roughly 80% of any screen.

**Primary Colors:**
- Paper White `#FFFFFF` — the display figure, headings, primary button fill, and icon glyphs. On a mid-grey ground white is bright but not searing, which is why the system can afford to use it for large type.
- Amber `#F5A623` — the single accent, reserved for the live metric: the words-per-minute figure, the countdown, the streak. It marks *the number the user came for* and nothing else.
- Mint `#4CD964` — a success confirmation only. A completed session, a correct word. Never a fill, never a button, never a resting state.

**Neutral Colors:**
- Surface `#4A4A4A` — the raised value, one step above the ground. Used where a panel needs a hard edge rather than a translucent one.
- Muted `#A8A8A8` — supporting copy, tag labels, captions, and inactive controls. The floor for legible text on this ground.
- Indicator `#6A6A6A` — progress tracks, inactive dots, and dividers. Visible but never read as text.

**Overlays — the real surface system:**
Most surfaces are not a color at all but white at low alpha over the ground, so they hold up if the ground value is ever adjusted.
- `rgba(255,255,255,0.1)` — tags, secondary buttons
- `rgba(255,255,255,0.2)` — icon buttons, hovered secondary surfaces
- `rgba(255,255,255,0.3)` — pressed states

**Accent/State Colors:**
- Error `#FF6B6B` — an incorrect entry or a failed state. Text and glyph only.
- Focus Ring `#FFFFFF` at 2px offset 2px.

## Typography

**Display & Headings:** a single neutral system sans across the whole interface. Google Fonts equivalent: `Inter`, weights 400/500. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`. The system uses only two weights; on a low-contrast ground, weight differences read poorly and size carries hierarchy instead.

**Metric numerals:** tabular figures on any live counter, so a number changing from 99 to 100 does not shift the layout.

**Type Scale:**
- Display metric — `clamp(64px, 15vw, 120px)` / 400 / 1.10 / -0.02em, in Amber
- Hero title — `clamp(36px, 8vw, 48px)` / 500 / 1.20 / -0.02em
- Section title — 32px / 400 / 1.30 / -0.01em
- Body — 16px / 400 / 1.60 / 0
- Supporting copy — 16px / 400 / 1.60 / 0, in Muted
- Button — 16px / 500 / 1.00 / 0
- Tag and caption — 14px / 400 / 1.40 / 0, in Muted

**Hierarchy Rules:** The display metric is at least three times the size of anything else on screen — that ratio is the entire hierarchy, and reducing it makes the interface look like a dashboard rather than a focus surface. Section titles run at 400 rather than bold; the only 500 in the system is the hero title and button labels. Nothing is italic or all-caps. `15vw` on the display metric means it genuinely fills a phone screen, which is intended.

## Spacing System

**Base Unit:** 8px.

**Scale:** 8, 16, 24, 32, 48, 64, 96.

**Common Patterns:**
- Page gutter 24px; content measure capped at 720px — narrow, because the screen holds one thing.
- Display metric: 16px below the figure to its label, 48px of clearance above and below the block.
- Icon button row: 24px between buttons, 48px above the row.
- Button padding 16px 32px. Tag padding 8px 16px.
- Section title to its content: 48px — unusually generous, and part of what makes the interface feel unhurried.
- Section to section: 64px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses longhand `padding-top` / `padding-bottom`, never a `padding: 64px 0` shorthand on that element, which would win on source order and zero the gutter.

## Component Styles

### Display Metric

The hero component. A `clamp(64px, 15vw, 120px)` figure at weight 400 in Amber, with a 16px Muted label beneath, centered. It is the only amber element on the screen and the only thing above 48px. Never paired with a second large figure — if two metrics matter equally, neither is the display metric and both drop to section-title size.

### Icon Buttons

**64px circles**, fill `rgba(255,255,255,0.2)`, no border, white 20px glyph, `border-radius: 50%`. Hover: fill `rgba(255,255,255,0.3)`. These are the primary transport controls — start, pause, reset — and their size is deliberate: at 64px they are reachable without looking, which matters on a screen the user is not supposed to be staring at.

### Buttons

**Primary** — fill `#FFFFFF`, label `#3A3A3A` at 16px/500, `border-radius: 25px` (a full pill), padding 16px 32px, no border. The inversion is the point: on a mid-grey ground a white fill is the strongest available signal without introducing a color.

**Secondary** — fill `rgba(255,255,255,0.1)`, label `#FFFFFF`, same pill radius and padding, no border. Hover lifts the fill to `0.2`.

There is no amber button. Amber marks the metric; making it a button would put the accent on the control rather than on the number.

### Tags

Fill `rgba(255,255,255,0.1)`, no border, `border-radius: 20px`, padding 8px 16px, 14px in Muted. The quietest element in the system.

### Progress Indicators

A 4px track in Indicator `#6A6A6A` with a white fill, fully rounded. Where progress is stepwise, use 8px dots — Indicator for pending, white for complete, Amber for current. The current-step amber is the one exception to amber being reserved for the display metric, and it exists because a progress row *is* the metric in stepwise flows.

### Input Fields

Fill `rgba(255,255,255,0.1)`, no border, 8px radius, padding 16px, 16px in Paper White. Placeholder in Muted. Focus: fill lifts to `rgba(255,255,255,0.2)` plus a 2px white ring at 2px offset. Typing surfaces never take a hard border — the fill change is the entire affordance.

### Color Cards

An 80px swatch at 16px radius with the name and hex centered beneath. Swatches are the only place a raw color value appears at size.

## Layout Principles

A single centered column capped at 720px with a 24px gutter, vertically centered in the viewport for the primary focus screen. The composition is always the same three-part stack: display metric, supporting label, control row. Supporting content — settings, history, results — lives below the fold and never competes with the metric above it. Nothing is ever placed to the side of the display metric; the system has no two-column layout at any breakpoint. Below 600px the metric's `15vw` already handles scaling, so the only mobile change is the gutter and the control row gap dropping to 16px.

## Visual Effects

No shadows anywhere — on a mid-grey ground a shadow is nearly invisible in one direction and muddy in the other. Elevation is white alpha: 10% for resting surfaces, 20% for controls, 30% for pressed. Radii: 50% on icon buttons, 25px pill on buttons, 20px on tags, 16px on swatches and cards, 8px on inputs. No gradients, no glass, no blur, no texture. Transitions are 200ms ease on background-color and opacity — slower than typical, matching the unhurried register. Nothing translates or scales.

## Design Tone

Quiet, spacious, and unhurried. The mid-grey ground is doing something a black interface cannot: it recedes without feeling like a void, so a single amber number and a row of soft white circles can hold the entire screen. It is designed to be looked *through* rather than at.

## Usage Notes for AI Implementation

1. **The ground is mid-grey, not black.** `#3A3A3A` is chosen so the screen recedes in a dim room without the harshness of pure black or the glare of white. Darkening it to `#1a1a1a` makes every white overlay in the system too contrasty, and the whole surface vocabulary stops working.

2. **Surfaces are white alpha, not new greys.** 10% resting, 20% controls, 30% pressed. Replacing these with opaque hex values means the surfaces stop tracking the ground if it is ever adjusted, and the layered translucency that gives the interface its softness disappears.

3. **Amber marks the metric and nothing else.** One amber element per screen: the live number. Not a button, not a heading, not a border. The single exception is the current step in a progress row, because that row *is* the metric.

4. **The display metric is at least 3× everything else.** That ratio is the whole hierarchy. Shrinking it to fit more on screen turns a focus surface into a dashboard.

5. **Icon buttons are 64px circles.** Not 40px, not squared off. The size is an affordance for a user who is not looking directly at the controls.

6. **The primary button is white with dark type.** On a mid-grey ground, inverting to white is the strongest signal available without spending the accent. There is no amber button in this system.

7. **Only two font weights.** 400 and 500. On a low-contrast ground weight differences read poorly; size carries hierarchy instead. Introducing a 700 makes headings look smudged rather than strong.

8. **No shadows.** On mid-grey they are invisible in one direction and muddy in the other. Depth is white alpha, full stop.

9. **Never two large figures.** If two metrics matter equally, neither is the display metric and both drop to section-title size. The composition depends on there being exactly one thing to look at.

10. **Inputs have no border.** The alpha fill is the entire affordance, and it lifts from 10% to 20% on focus. Adding a hard border reintroduces the visual noise the system exists to remove.
