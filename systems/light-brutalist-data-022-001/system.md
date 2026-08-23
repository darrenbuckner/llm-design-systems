---
id: light-brutalist-data-022
title: Ironpress System
description: A brutalist, monochrome data dashboard aesthetic built on monospaced typography, sharp geometry, and unapologetic information density.
tags: [light, brutalist, monochrome, data-dense, terminal, minimal]
colors: ["#FFFFFF", "#000000", "#1A1A1A", "#4A4A4A", "#7A7A7A", "#B0B0B0", "#D4D4D4", "#EBEBEB"]
created: 2026-02-20
---

# Ironpress System

A brutalist data interface aesthetic that treats information as the primary design element. Rooted in monospaced typography, sharp rectangular geometry, and a strict grayscale palette, this system strips away all ornament to let raw data command attention. Every pixel serves the numbers. The visual language draws from terminal interfaces and newspaper data tables — authoritative, dense, and uncompromising.

## Color Palette

**Primary Colors:**
- Black: #000000 — Primary text, borders, chart lines, maximum-intensity data points
- White: #FFFFFF — Page background, primary surface

**Neutral/Grayscale Scale:**
- Near Black: #1A1A1A — Heavy emphasis text, darkest heatmap cells
- Dark Gray: #333333 — High-intensity heatmap cells, strong data points
- Medium Dark: #4A4A4A — Secondary text, axis labels, supporting information
- Medium Gray: #7A7A7A — Mid-intensity heatmap cells, tertiary text
- Light Medium: #B0B0B0 — Low-intensity heatmap cells, chart gridlines, dashed rules
- Light Gray: #D4D4D4 — Lightest active heatmap cells, subtle borders
- Near White: #EBEBEB — Empty/zero heatmap cells, chart fill areas, subtle backgrounds

**Functional Colors:**
- Chart Line: #000000 — Primary data line in charts
- Chart Fill: #EBEBEB — Area fill beneath line charts
- Grid Dashed: #B0B0B0 — Horizontal reference lines in charts
- Data Point: #FFFFFF with #000000 stroke — Circle markers on line charts

**Note:** This system deliberately avoids color. There are no success/warning/error states using green/yellow/red. Status is communicated through value density and spatial position, not hue.

## Typography

**Font Families:**
- Primary (and only): Monospaced — appears to be a geometric mono like `Space Mono`, `IBM Plex Mono`, or `JetBrains Mono`. All text uses this single family.
- No secondary font. The system is strictly mono throughout.

**Type Scale:**
- Stat Display: 14-16px, 700 weight, uppercase, letter-spacing 0.05em — used for large metric callouts
- Section Heading: 13-14px, 700 weight, uppercase, letter-spacing 0.08-0.12em, line-height 1.3 — "WEEKLY AVERAGE PACE", "WEEKLY DISTANCE"
- Data Label: 11-12px, 400 weight, uppercase, letter-spacing 0.05em — axis labels, month names, date references
- Metric Value: 12-13px, 700 weight, normal case — inline stats like "5.01 KM • 5:51/KM"
- Caption: 10-11px, 400 weight, uppercase, letter-spacing 0.04em — supplementary notes, date stamps

**Hierarchy Rules:**
- ALL headings and labels are uppercase with generous letter-spacing
- Weight (bold vs regular) is the primary differentiator, not size — the type scale is extremely compressed
- The bullet character `•` serves as an inline separator between data points
- Hierarchy is achieved through spatial grouping and border separation more than typographic scale
- No italic usage observed — emphasis is purely through weight and case

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64

**Common Patterns:**
- Section internal padding: 24px vertical, 24px horizontal
- Space between section title and content: 16-24px
- Heatmap cell size: approximately 14-16px squares
- Heatmap cell gap: 3-4px
- Chart area padding: 16px from borders
- Space between major sections: 0px (sections are separated by borders, not whitespace)
- Inline metric spacing: 8px around `•` separators
- Stat line vertical spacing: 12px between rows

**Key Principle:** Sections are delineated by borders, not by generous whitespace. The system packs data tightly and uses hard lines as structural separators.

## Component Styles

### Heatmap Grid
- Individual cells: ~14-16px squares with 3-4px gap
- Color intensity: 5-6 levels from #EBEBEB (empty/low) through grays to #1A1A1A/#000000 (max)
- Arranged in rows by day-of-week, columns by week
- Month labels above in uppercase mono, 11-12px
- No rounded corners on cells — sharp rectangles
- No hover states visible — static data display

### Line Charts
- Line stroke: 1.5-2px solid #000000
- Data points: 6-8px circles, white fill (#FFFFFF), 1.5-2px black stroke
- Area fill: #EBEBEB beneath the line to x-axis
- Grid lines: 1px dashed #B0B0B0, horizontal only
- Axis labels: 11px monospaced, uppercase, #4A4A4A
- Y-axis labels: right-aligned, left of chart area
- X-axis labels: centered beneath tick positions
- No legend — chart title serves as the only label

### Bar Charts
- Bar fill: #4A4A4A to #1A1A1A (darker for higher values, or uniform)
- Bar width: fills available space with ~2-3px gaps
- Outline: 1px #000000 stroke on bars
- Same grid line and axis label treatment as line charts
- Area beneath bars may use lighter fill for empty space

### Section Containers
- Border: 1px solid #000000
- Background: #FFFFFF
- Padding: 24px
- No border-radius — sharp 0px corners everywhere
- No shadow — completely flat
- Sections can sit adjacent with shared borders (no gap between)

### Stat Lines / Data Rows
- Layout: Label left, values right, or inline with `•` separators
- All uppercase labels
- Monospaced alignment ensures columns naturally align
- Thin 1px #000000 horizontal rules between major groups
- No zebra striping — plain white rows

### Navigation / Header Area
- Date range displayed in monospaced format: `2025-07-23 → 2026-07-22`
- Pipe character `|` as inline section separator
- All metrics inline, uppercase, mono
- No traditional nav bar — the data IS the interface

## Layout Principles

- **Max content width:** Full viewport or ~1000-1200px for data panels
- **Grid structure:** Flexible columns, sections sized to content needs. Charts sit side-by-side in 2-column layouts on desktop.
- **Responsive behavior:** Sections stack vertically on narrow viewports. Charts scale down but maintain aspect ratio.
- **Alignment:** Strict left alignment. No centered content except within chart areas.
- **Density:** Maximum data per viewport. The system avoids empty space aggressively.
- **Sectioning:** Hard 1px black borders create structure. No padding between adjacent sections.

## Visual Effects

- **Border Radius:** 0px everywhere. No rounded corners on any element. This is non-negotiable for the aesthetic.
- **Shadows:** None. Zero elevation system. Everything is flat.
- **Borders:** 1px solid #000000 — the primary structural element. Borders do all the work that shadows and spacing do in other systems.
- **Backgrounds:** Pure #FFFFFF only. No gradients, no patterns, no textures.
- **Effects:** None. No blur, no glow, no animation. Static and print-like.
- **Decorative elements:** None. The data itself is the decoration.

## Design Tone

This is a system that respects the viewer's intelligence. It's anti-decorative, anti-trendy, and entirely focused on information transfer. The aesthetic sits at the intersection of newspaper data journalism, terminal interfaces, and brutalist web design. It feels authoritative and serious without being corporate — more like a researcher's personal dashboard than a SaaS product. The strict monochrome palette and monospaced typography create a sense of rigor and precision that ornamental design systems can't achieve.

## Usage Notes for AI Implementation

- **Never add border-radius.** The sharp geometry is the single most important visual attribute. Even 2px of rounding destroys the aesthetic.
- **Never add color.** If you need to highlight something, use bold weight or a darker gray — not a hue. The entire system operates on the grayscale axis.
- **Use monospaced fonts exclusively.** Proportional fonts break the visual alignment that makes data grids readable. `Space Mono`, `JetBrains Mono`, or `IBM Plex Mono` are appropriate choices.
- **Uppercase all labels and headings** with letter-spacing of 0.05em or greater.
- **Use borders for structure, not whitespace.** Adjacent sections should share borders or sit directly against each other.
- **Data formatting:** Use the `•` bullet as an inline separator. Display dates in `YYYY-MM-DD` or `MMM DD` format. Times in 24-hour or `HH:MM` format.
- **Charts should be minimal:** No 3D effects, no gradient fills, no decorative gridlines. Black lines, white dots, gray fill. That's it.
- **When building dashboards:** Pack the viewport. White space is wasted space in this system. Every section should contain meaningful data.
- **Print-friendly by default:** This system looks as good printed in black and white as it does on screen. Maintain that quality.
