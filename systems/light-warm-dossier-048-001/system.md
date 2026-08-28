---
id: light-warm-dossier-048
title: Foolscap Dossier
description: A bone-white print-derived system for personal records, where a high-contrast serif carries every heading and a wide-tracked monospace carries every label.
tags: [light, minimal, warm, serif, monospace, editorial, generous-spacing, high-contrast, portfolio]
colors: ["#FAFAF7", "#1A1A1A", "#183333", "#54504A", "#D9D9D6"]
created: 2026-08-28
---

# Foolscap Dossier

Foolscap Dossier is a bone-white, print-derived system for personal records — profiles, handbooks, changelogs, engagement histories — where a high-contrast serif carries every heading, a wide-tracked monospace carries every label, and nothing else is permitted on the page. There are no cards, no fills, no radii, and no shadows. Structure comes from a two-column record grid, hairline rules, and quantities of vertical space that would read as a mistake in any denser system. A single deep-pine accent marks links and one italic line of positioning; everything else is ink, warm grey, and paper.

## Color Palette

**Page Surface:** `#FAFAF7` — the only background in the system. Warm bone white, never pure white. Every section, every row, and every component sits directly on it; nothing is ever raised, tinted, or boxed.

**Primary Colors:**
- Ink `#1A1A1A` — all serif headings, display type, and entry titles. Near-black, never true black.
- Deep Pine `#183333` — the single accent. Inline links, the italic positioning line under a name, calls to action, and the hover state on any serif heading that is also a link. Desaturated enough to read as ink until it sits beside ink.

**Neutral Colors:**
- Prose `#54504A` — body copy and descriptions. Warm grey, roughly 7.2:1 on the ground.
- Nav Label `#54504A` — the same value, used for monospace labels that are interactive or structural (nav, footer links).
- Meta Label `#89847B` — monospace labels that are annotation rather than navigation: dates, locations, handles, ranges. Roughly 3.6:1, deliberately quiet, and never used for anything a reader must be able to act on.
- Hairline `#D9D9D6` — the only border value in the system. 1px, used for section separators and the footer rule.
- Faint Wash `#F2F1EC` — a one-step-deeper ground, reserved for a swatch chip or an image placeholder. Not a card fill.

**Accent/State Colors:**
- Focus `#183333` — a 2px outline at 3px offset. Same value as the link accent; the system has no separate focus hue.
- Hover `#183333` — ink headings shift to pine on hover. Links stay pine and gain underline weight instead of changing color.
- Success `#2F5D3A`, Warning `#8A6A20`, Error `#8C2F24` — muted, desaturated to sit inside the same warm register. Used as text and hairline color only, never as a fill.

**Inverse:** none. This system has no dark surface, no inverted footer, and no reversed band. Adding one breaks it.

## Typography

**Font Families:**
- **Display & Headings:** Fraunces (variable serif — `wght` 400, `SOFT` 0, `WONK` 0, and `opsz` pinned per level, never left on auto). A high-contrast transitional serif with sharp bracketed serifs and ball terminals. Instrument Serif is an acceptable display-only substitute if only one optical size is needed. Fallback: `'Fraunces', 'Instrument Serif', 'Iowan Old Style', Georgia, serif`.
- **Body:** Figtree (humanist geometric sans, double-story `a`, tall x-height, open apertures). Warm and circular rather than neutral. Fallback: `'Figtree', 'Avenir Next', 'Segoe UI', system-ui, sans-serif`.
- **Labels:** JetBrains Mono, used only in uppercase with wide tracking. Fallback: `'JetBrains Mono', 'IBM Plex Mono', ui-monospace, monospace`.

**Type Scale:**

| Level | Family | Size | Weight | `opsz` | Line height | Tracking |
|---|---|---|---|---|---|---|
| Display | Serif | `clamp(44px, 8vw, 88px)` | 400 | 48 | 1.05 | -0.02em |
| Section heading | Serif | `clamp(38px, 6.5vw, 62px)` | 400 | 40 | 1.08 | -0.015em |
| Positioning line | Serif italic | `clamp(22px, 3.4vw, 32px)` | 400 | 32 | 1.25 | -0.005em |
| Entry title | Serif | `clamp(22px, 3vw, 28px)` | 400 | 20 | 1.2 | -0.01em |
| Body | Sans | 18px | 400 | — | 1.75 | 0 |
| Small body | Sans | 16px | 400 | — | 1.7 | 0 |
| Meta label | Mono | 13px | 500 | — | 1.4 | 0.14em |
| Nav label | Mono | 13px | 500 | — | 1.4 | 0.16em |

**The optical-size ladder.** `opsz` is pinned per level and deliberately runs *below* the rendered pixel size — 48 at 88px, 40 at 62px, 20 at 28px. Left on auto, Fraunces reaches maximum contrast at display sizes and the hairlines go spindly and modern; holding the axis back keeps the sturdier, text-cut serifs that make this read as letterpress rather than as a fashion masthead. This one setting does more for the system's character than any color decision in it.

**Hierarchy Rules:**
- Serif never goes bold. All hierarchy in the serif comes from size and space, and there is no 700 weight anywhere in the system. If a heading needs more presence, it gets larger or gains more space above it.
- Every top-level section heading ends in a period — `Operating.`, `Personal.`, `Get in touch.` The period is part of the system, not punctuation the writer chose.
- Serif for headings and titles, sans for every sentence a reader actually reads, mono for every label. These three roles never trade places. Prose set in the serif turns this into a magazine; labels set in the sans turn it into a generic product page.
- Monospace is uppercase and tracked at all times. There is no lowercase mono anywhere.
- Nothing is centered. Every block is left-aligned to the container or to its own grid column.
- Prose measure caps at 68ch. Display type is allowed to run wider than the prose column.
- The italic serif appears exactly once per page, as the positioning line beneath the display heading, and it is set in the pine accent.

## Spacing System

**Base Unit:** 8px.

**Scale:** 8, 16, 24, 32, 40, 56, 72, 96, 128, 160, 200.

**Common Patterns:**
- Page gutter: `clamp(24px, 5vw, 48px)`, owned by one container class.
- Container max width: 1040px, centered with `margin-inline: auto`.
- Prose measure inside the container: 680px, left-aligned, not centered.
- Section rhythm: 128px between sections on mobile, 200px on desktop. This is the single largest lever in the system and the first thing that gets cut by mistake.
- Hairline rules carry 96px of clearance above and below, minimum.
- Record row vertical gap: 56px between rows, 16px between a row's title and its description.
- Meta label to the content it labels: 12px on mobile where they stack, 40px of column gap on desktop where they sit side by side.
- Paragraph spacing inside prose: 24px.

## Component Styles

### Meta Labels

The mono layer is the system's signage and its most identifiable feature. Uppercase, 13px, 0.14em tracking, `#89847B`, no background, no border, no icon.

Used for: date ranges (`2026 — PRESENT`), location and handle lines (`@HANDLE · CITY, COUNTRY`), section eyebrows (`FROM YEARS OF ADVISING`), and the copyright line. Ranges use an em dash with a space on either side.

A meta label never has a box, never sits on a tint, and never appears in the same visual weight as the thing it labels. If a label starts competing with its content, it is too large or too dark, not the wrong color.

### Section Headings & Rules

Serif, 400 weight, size from the scale, ink, terminal period. Preceded optionally by a mono eyebrow 16px above it. Followed by at least 56px of space before content.

Section separators are a 1px `#D9D9D6` rule at the container's full width, with 96–128px of clearance on both sides. Rules separate major regions only — never rows within a list, never a heading from its own content.

### Record Rows

The structural workhorse. A CSS grid, `grid-template-columns: minmax(160px, 220px) 1fr`, `gap: 40px`, with a mono meta label in the left column and a serif title plus sans description in the right.

```
2026 — PRESENT     Program Name ↗
                   One or two sentences of description in the sans,
                   at 18px, in prose grey.
```

The label sits on the first baseline of its row content (`align-items: baseline`), not at the top edge — top alignment leaves the mono label floating visibly above a 28px serif title.

Rows carry no borders, no dividers, and no background alternation. They are separated by 56px of vertical space and nothing else. Below 768px the grid collapses to one column and the meta label sits directly above the title with a 12px gap.

Both grid children take `min-width: 0` so long titles wrap instead of forcing the track wider than the container.

### Links & Inline Emphasis

Inline links: pine `#183333`, underlined with `text-decoration-thickness: 1px` and `text-underline-offset: 3px`. On hover the thickness goes to 2px and the color does not change. This is the only underline in the system.

Serif titles that are links: ink at rest, pine on hover, no underline, followed by a `↗` glyph at 0.55em sized down and offset up — the glyph marks external destination and is never used decoratively.

Italic is reserved for the positioning line and for titles of works. Bold is not used in prose at all; emphasis is carried by the pine link color or by moving the phrase into a serif heading.

### Calls to Action

There are no filled buttons in this system. A primary action is a mono uppercase label in pine with a trailing `→`:

```
READ THE FULL HANDBOOK  →
```

13px, 0.16em tracking, `#183333`, no border, no fill, no radius, 44px minimum tap height achieved with vertical padding. On hover the arrow translates 4px right over 160ms and nothing else moves. Focus draws a 2px pine outline at 3px offset.

If a genuinely filled button is unavoidable, it is a 1px pine outline with transparent fill and 0 radius — never a solid block.

### Input Fields

Transparent fill, no border on three sides, a 1px `#D9D9D6` bottom rule only. 18px sans, ink, 12px vertical padding, 0 radius. Placeholder in `#89847B`.

Labels sit above the field as mono meta labels, 12px clear. On focus the bottom rule becomes 1px `#183333` and a 2px pine outline is drawn at 3px offset — the rule change alone is not sufficient contrast signal. Error state turns the bottom rule `#8C2F24` and adds a 14px sans message beneath in the same value.

### Portrait & Media Blocks

Images are hard-edged rectangles: `border-radius: 0`, no border, no shadow, no overlay, no caption chrome. A portrait is square and sits at 260–300px on desktop and caps at 200px on mobile — it stacks above the bio rather than going full-bleed, because a full-width square eats an entire mobile screen and the system's restraint is the point. Two-column grid beside its bio text with a 56px gap.

Placeholders use the faint wash `#F2F1EC` with a centered mono label. Never a gradient, never a skeleton shimmer.

### Navigation & Footer

Navigation is one to three mono uppercase words at 13px `#54504A`, aligned to the top right of the container, with no background, no rule beneath, and no active-state marker other than the pine color. There is no logo and no hamburger — at mobile widths the labels simply stay where they are.

The footer is a 1px `#D9D9D6` rule, then a single row: copyright as a mono meta label on the left, a mono link on the right. 48px of padding above the rule, 40px below. Contact blocks above the footer use the record-row grid, with the serif heading in the left column and a right-aligned mono list of channels in the right.

## Layout Principles

- One centered container at 1040px maximum, with a single class owning the horizontal gutter. Anything else setting vertical rhythm on that element uses `padding-top` and `padding-bottom` longhand so it cannot zero the gutter.
- Single column at every width. The only things that become two columns above 768px are the record rows and the portrait-plus-bio block; both collapse cleanly.
- Prose is capped at 680px and stays left-aligned within the wider container. The asymmetry between a 680px paragraph and a 1040px rule is intentional and is a large part of how the page reads.
- Vertical space is the primary structural device. There is no visual grouping mechanism other than proximity — no cards, no panels, no background bands.
- Content is never justified and never centered. The right rag is left alone.
- Desktop adaptation is: wider gutters, larger display type, and the two-column grids engaging. Nothing new appears at desktop that was absent on mobile.

## Visual Effects

**Radii:** 0 on every element without exception — images, inputs, outlines, swatches.

**Shadows:** none, anywhere, at any elevation. The system has no z-axis. If something needs to feel separated, it gets more space or a hairline, never a shadow.

**Borders:** 1px `#D9D9D6` only, and only as full-width horizontal rules or as the bottom edge of an input. No boxes. The one exception is a 1px `#183333` outline on an unavoidable outline button.

**Background treatment:** flat `#FAFAF7`. No gradients, no texture overlays, no noise, no paper grain image.

**Transitions:** 160ms `ease` on `color`, `text-decoration-thickness`, and `transform`. Nothing else animates. No entrance animations, no scroll reveals, no parallax.

**Focus:** `outline: 2px solid #183333; outline-offset: 3px`, never removed and never replaced with a color-only change.

## Design Tone

Quiet, exact, and confident enough to leave most of the page empty. It reads like a well-set printed record — a letterpress CV or the colophon of a small press — where the monospace annotations do the filing and the serif does the speaking. The warmth comes entirely from the bone ground and the grey-brown ink rather than from any decorative element, and the single pine accent is rationed hard enough that it still registers as a signal on the fifth screen.

## Usage Notes for AI Implementation

1. **Never add a card.** The moment content goes inside a bordered or filled container, this system becomes an ordinary light SaaS page. Grouping is done with 56–200px of vertical space and hairline rules at section boundaries only.

2. **Do not compress the section rhythm.** 128px mobile / 200px desktop between sections looks excessive in isolation and is load-bearing in context. Cutting it to a conventional 64px is the single most common way this system is destroyed, and it will still look tidy afterward — which is what makes it hard to notice.

3. **Keep prose in the sans.** Serif is for headings, titles, and the one italic positioning line. Set a paragraph in Fraunces and the page reads as a literary magazine rather than a record.

4. **Pin `opsz` below the pixel size on every serif level.** Left on auto, Fraunces goes maximum-contrast at display sizes and the whole page shifts from letterpress to fashion masthead. This is the single highest-leverage setting in the system and it is invisible until you compare two renders side by side.

5. **Ration the pine.** Roughly one to three accent elements per screenful: inline links, the italic line, a call to action. Using it for a heading color, a background, or a badge collapses the contrast that makes links legible without a box.

6. **Meta labels are annotation, not navigation.** `#89847B` at 3.6:1 is deliberately below the interactive threshold. Anything a user must click or read carefully goes in `#54504A` or darker. Do not "fix" the quiet label color by darkening all mono uniformly.

7. **Every section heading ends in a period.** It is a system rule, not an editorial choice, and dropping it on one heading makes the set look inconsistent rather than restrained.

8. **Give record rows `min-width: 0` on both grid children.** A long serif title in a `1fr` track will otherwise push the grid wider than the container and produce horizontal scroll at 393px with no element reporting as overflowing.

9. **Use `clamp()` for all display sizes, and one element owns the horizontal gutter.** An 88px serif heading cannot break, so a fixed value overflows a 393px viewport before any media query fires. Separately, if a section class sets `padding: 120px 0` shorthand on the gutter element, it silently zeroes the gutter and content runs to the viewport edge on mobile while the header stays correctly indented — use `padding-top` / `padding-bottom` longhand on anything sharing that element.

10. **No dark mode, no inverted band, no footer in reverse.** The system is defined partly by having exactly one surface. A dark footer or a reversed hero is not an extension of it; it is a different system wearing its fonts.
