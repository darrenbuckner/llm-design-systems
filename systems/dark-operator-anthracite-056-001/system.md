---
id: dark-operator-anthracite-056
title: Anthracite Operator
description: A pure-black operator landing system with warm charcoal bands, condensed grotesque headlines, monospace readouts, and a five-hue status palette used as signal, never as decoration.
tags: [dark, high-contrast, condensed, monospace, terminal, marketing, data-visualization, cards, forms]
colors: ["#000000", "#272725", "#E1AD3F", "#E03C14", "#F2F1ED"]
created: 2026-09-10
---

# Anthracite Operator

A pure-black landing system for technical consultancies and operator programs: warm charcoal bands, condensed grotesque headlines, monospace diagnostic readouts, and five status hues that act as signals rather than decoration. It reads like a field report written by engineers for executives, with terminal windows standing in for hero imagery.

## Color Palette

**Page Surface:** Pure black `#000000`. The whole page sits on true black; nothing is gradient-washed and nothing is tinted blue.

**Neutral Colors:**
- Card Surface `#161614` — terminal windows, nested readout panels, logo walls. Warm near-black, one step up from the page.
- Band Surface `#272725` — full-width section bands, featured panels, testimonial blocks, form inputs. The warm charcoal that alternates with black to create rhythm.
- Hairline `#33332F` — row dividers inside cards, section rules, borders around cards on black.
- Strong Border `#45443F` — card borders when the card sits on a band, the outlined hamburger button.
- Meter Track `#4A4945` — unfilled portion of progress meters.
- Text Primary `#F2F1ED` — headlines and primary body. Warm off-white, never `#FFFFFF` for type.
- Text Secondary `#B5B4AE` — body paragraphs under headings, feature descriptions.
- Text Muted `#95948E` — monospace eyebrows, input placeholders, footer links, readout keys. 4.9:1 on the band, so it is the dimmest text allowed.
- Signal White `#FFFFFF` — reserved for the primary button fill only.

**Primary Colors:**
- Signal Gold `#E1AD3F` — the one warm action color: nav CTA fill, "active" readout values, featured category labels, footer column headers, testimonial names. Black text on it (10.3:1).
- Vermilion `#E03C14` — the second most-used hue: short dash markers before service labels, "missing / poor / not installed" values, the section rule on a picks band, primary feature tile.

**Accent/State Colors:** Five status hues, each with a fill value and a text-safe ink. Fill values go on tiles, bars, dashes, and dots. Ink values go on text smaller than 18px.
- Vermilion — fill `#E03C14`, ink `#F2603A` (error, missing, blocking)
- Signal Gold — fill and ink `#E1AD3F` (active, attention, featured)
- Indigo — fill `#5B5BD6`, ink `#9294F2` (uneven, in-flight, chart bars, focus ring)
- Sage — fill and ink `#62B06E` (making progress, success)
- Orchid — fill `#CE45AC`, ink `#E27BC9` (metrics, training, secondary category)

Focus: 2px `#9294F2` outline, 2px offset. Error: vermilion ink text plus a 1px `#E03C14` inner edge on the input.

**Art Band:** The contact section sits on a pixel-sorted glitch field built from vermilion `#E03C14`, violet `#7A55CE`, indigo `#5B5DCE`, and bone `#D9D2C4` in horizontal streaks. It is the only place color is used expressively.

## Typography

**Display & Headings:** Barlow Semi Condensed (Google Fonts), a condensed grotesque sans, weight 600. Fallback: "Arial Narrow", "Roboto Condensed", sans-serif. Every headline is set in it and every card headline ends with a period.

**Body:** Geist (Google Fonts), a tight neo-grotesque sans, weight 400, tracking -0.01em. Fallback: Inter, system-ui, sans-serif.

**Mono:** IBM Plex Mono (Google Fonts), weights 400/500/600. Fallback: ui-monospace, "SF Mono", Menlo, monospace. Used for every label, every button, every readout, and the entire footer.

**Type Scale:**
- Hero: `clamp(44px, 8vw, 84px)` / 600 / line-height 0.98 / tracking -0.015em
- Section H2: `clamp(34px, 5.5vw, 56px)` / 600 / 1.02 / -0.01em
- Card H3: `clamp(24px, 3vw, 30px)` / 600 / 1.08
- Feature Title: 19px / 600 / 1.2 (Barlow Semi Condensed)
- Lead: 18px / 400 / 1.5 Geist, Text Secondary
- Body: 16px / 400 / 1.55 Geist
- Readout: 13px / 400 / 1.6 IBM Plex Mono
- Button Label: 12px / 600 / uppercase / tracking 0.14em Mono
- Eyebrow: 11px / 500 / uppercase / tracking 0.16em Mono, Text Muted

**Hierarchy Rules:**
- Three families, three jobs. Condensed sans speaks, Geist explains, mono labels and operates. Never set a paragraph in mono or a label in Geist.
- Headlines break by meaning, not width. Force line breaks so each line is a phrase ("Your best builders are already moving faster. / We help you with everyone else.").
- Emphasis inside headlines is a second sentence, not a color change.
- Nothing is centered except the preview footer. Every block is left-aligned, including the testimonial.
- All uppercase text is mono. Sans is always sentence case. The single exception is the logo wordmark, set in Barlow 700 uppercase at 20px with +0.02em tracking.

## Spacing System

**Base Unit:** 4px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 96, 128

**Common Patterns:**
- Page gutter: 20px mobile, 32px at 768px, 48px at 1200px. Max content width 1200px.
- Section rhythm: 96px top and bottom on mobile, 112px at 768px, 128px at 1200px. Bands carry the same rhythm internally.
- Card padding: 20px mobile, 28px desktop. Readout rows: 10px vertical, 0 horizontal, hairline between.
- Eyebrow to headline: 16px. Headline to lead: 20px. Lead to actions: 32px.
- Feature list: 40px between items, 16px between tile and title column.
- Form: 8px label to field, 20px between fields, 8px between option rows.

## Component Styles

### Buttons & Links
- **Primary:** `#FFFFFF` fill, `#000000` mono label, uppercase, 12px, 600, tracking 0.14em. Padding 14px 24px, min-height 48px, radius 2px, trailing `→` separated by 12px. Hover: fill `#E1AD3F`, arrow translates 3px right over 160ms. Focus: indigo ring.
- **Accent (nav CTA):** Signal Gold fill, black label, same geometry at min-height 40px. Hover: fill `#F2F1ED`.
- **Text Link:** no fill, Text Primary mono label with `→`, underline appears on hover at 2px offset in the current ink.
- **Bracket Link:** mono label wrapped in `[ ]`, brackets colored with the card's category hue, label in Text Primary. Hover: label takes the category hue.
- **Outlined Square:** 40×40, 1px Strong Border, transparent, radius 2px. Used for the menu toggle and `+` option markers.

### Navigation & Footer
- **Utility Bar:** 32px tall, black, 11px mono uppercase in Text Muted. A 6px vermilion dot precedes the path-style locator on the left; a cohort or status notice sits on the right separated by `·`.
- **Nav:** 64px tall, black, a 26px off-white square logo mark plus an uppercase Barlow 700 wordmark left, gold CTA and outlined menu square right. No border beneath; the hero starts on the same black.
- **Footer:** black, entirely mono. A one-line mono tagline in Text Secondary, then two-column link groups (four on desktop) with Signal Gold uppercase headers and Text Muted links at 13px. External links carry a trailing `↗`. Legal row at the bottom in 11px muted mono.

### Terminal Window Cards
The system's hero image. Card Surface fill, 1px Hairline border on black (Strong Border on a band), radius 6px, no shadow.
- **Title bar:** 36px tall, three 8px dots (vermilion, gold, gold at 60%), then a mono path such as `~/lab.run/diagnostic` in Text Muted. Hairline below.
- **Readout rows:** mono 13px key in Text Secondary on the left, status value right-aligned in its status ink, hairline between rows. Values are one word, lowercase.
- **Prompt line:** `$` in Signal Gold, command in Text Primary, argument in Text Muted. Checklist lines use `[ ]` in gold followed by a mono key and a Geist description.
- Nested panels inside a terminal card use the page black `#000000` as their fill with a Hairline border, inverting the step.

### Meters & Charts
- **Maturity meter:** header row with mono eyebrow left and a mono count right (`3 PILLARS`). Each meter is a label row (key left, status word right in ink, both 11px uppercase mono) over a 4px bar: Meter Track base, status-fill portion, square ends.
- **Bar chart:** 10 to 12 indigo `#5B5BD6` bars on black, 4px gaps, no axes, no gridlines, no labels on bars. Heights trend upward. A mono caption row above states what is measured and the window.
- Charts never use more than one hue. Meters use one hue per row.

### Section Bands & Eyebrows
- **Band:** full-width block in Band Surface `#272725` with a nested gutter container. Bands alternate with black; never stack two bands.
- **Eyebrow rule:** mono eyebrow followed by a 1px line that runs to the container edge (flex: 1). Hairline on black, vermilion on a picks band.
- **Operator roster:** rows inside a band, each with a 44px circular avatar outlined in Strong Border, a condensed name at 20px, and a mono uppercase role line in Text Muted. Hairlines between rows.

### Feature List
Vertical list of capability items. Each item is a 28×28 square tile (radius 2px) filled with one status hue and a black glyph, beside a Barlow title at 19px and a Geist description in Text Secondary. Hues rotate in a fixed order: vermilion, gold, indigo, sage, orchid, then vermilion again. Two columns at 768px, three at 1200px.

### Offering Cards & Service Stack
- **Service stack:** one bordered container holding stacked rows with hairlines between. Each row opens with a 16×2px vermilion dash and a mono uppercase phase label, then a Card H3 ending in a period, then one line of Geist.
- **Offering card:** black card on a band, radius 6px, 1px Hairline border, padding 28px. Mono category label in its hue (for example `AI ENGINEERING` in gold, `TRANSFORMATION` in vermilion ink, `TRAINING` in orchid ink), Card H3, Geist paragraph, optional embedded terminal, bracket link at the foot. On desktop these sit in a 2×2 grid with 1px gaps showing the Strong Border color through.

### Testimonials
- **Lead quote:** Band Surface panel, quote set in Section H2 scale at Barlow 600, no quotation marks. Attribution in a black chip: gold mono uppercase name, muted mono role beneath.
- **Supporting quotes:** black rows beneath the lead, hairline-separated, 16px Geist in Text Primary, attribution in 11px vermilion ink mono uppercase.

### Form Panel
- **Container:** black panel with 1px Hairline border, radius 6px, padding 24px, sitting on the art band with 20px of art showing around it on mobile.
- **Labels:** 11px mono uppercase, Text Muted, 8px above the field.
- **Inputs, selects, textarea:** Band Surface fill, no border at rest, radius 4px, 48px min-height, 14px 16px padding, Geist 16px. Hover: 1px Strong Border inner edge. Focus: 2px indigo ring, fill unchanged.
- **Option rows:** full-width Band Surface rows with a Geist label left and a 24×24 outlined `+` square right. Selected: square fills Signal Gold with a black check, row gains a 1px gold inner edge.
- **Submit:** Primary button, right-aligned, label `SEND →`.

## Layout Principles

- Mobile is a single column at full gutter width. The screenshot's rhythm is the reference: black hero, card, black, band, black, band.
- At 1200px the hero splits 7/5 with the headline left and the terminal card right, top-aligned. Every other section keeps a left-aligned heading block above a grid.
- Grids use 1px gaps filled with a border color rather than whitespace gutters (Strong Border on a band, Hairline on black), so card groups read as a single instrument panel.
- Maximum measure for Geist paragraphs is 60ch. Headlines may run wider but break on phrases.
- Bands are full-bleed; cards inside them respect the 1200px container.
- The art band is the only section without a solid ground and is used once, directly before the footer.

## Visual Effects

- **Radii:** 2px buttons and tiles, 4px inputs, 6px cards and terminal windows, 50% avatars. Nothing rounder.
- **Shadows:** none. Elevation is expressed by stepping the ground (black to `#161614` to `#272725`) and by hairlines.
- **Borders:** 1px only. Hairline on black, Strong Border on a band.
- **Texture:** the pixel-sort art band only: a seeded low-resolution canvas of horizontal streaks, scaled up with pixelated rendering, over a hard-stop gradient fallback in the same four colors. No noise overlays elsewhere.
- **Motion:** 160ms ease-out for hovers, 3px arrow nudge on buttons, meters fill left to right over 600ms on first view. No parallax, no fades on scroll.

## Design Tone

Operator-grade and plainspoken: pure black, warm charcoal, and condensed headlines that sound like a field lead talking to an executive. Terminal readouts and status colors carry the credibility, so the page feels like a diagnostic already in progress rather than a pitch.

## Usage Notes for AI Implementation

1. The page ground is `#000000`, not a near-black. Swapping it for `#0B0B0F` or any blue-black turns this into a generic dark SaaS page and flattens the three-step ground system.
2. Charcoal `#272725` is warm. A neutral `#262626` or cool `#1F2937` loses the anthracite character; keep the slight yellow cast in every gray.
3. Status hues are signals. Each one must mean something where it appears (a readout value, a meter, a category). Never tint a background, a heading, or a button with indigo, sage, or orchid.
4. Use the ink variants for any status text under 18px. The indigo and orchid fills fall below 4.5:1 on the card surface and become unreadable as small text.
5. All uppercase text except the logo wordmark is IBM Plex Mono, all mixed-case prose is Geist, all headlines are Barlow Semi Condensed. Putting body copy in mono makes it a developer tool; putting headlines in Geist makes it a startup template.
6. The terminal window replaces the hero image. Do not add photography, 3D renders, or illustration to the hero; if the page needs a visual, build another readout.
7. No shadows and no radius above 6px. Soft rounded cards with drop shadows are the most common way this system gets misapplied.
8. Card headlines end with a period ("Find the constraint."). Dropping the period removes the declarative voice that separates this from marketing copy.
9. Gold is the only action color. The primary button is white, the nav CTA is gold, and nothing else is a filled button. A second gold element per screenful dilutes it.
10. Never stack two charcoal bands. The black-band-black alternation is the section system; two bands in a row read as one oversized card.
