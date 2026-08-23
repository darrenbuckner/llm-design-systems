---
id: light-editorial-neon-023
title: Highlighter Press
description: A bold editorial news aesthetic pairing chunky display type with a signature neon chartreuse accent and monospaced ticker treatments.
tags: [light, editorial, bold, news, neon, financial]
colors: ["#F1F0EC", "#0B0B0B", "#DFFF3C", "#E63946", "#8A8A85"]
created: 2026-04-09
---

# Highlighter Press

A punchy editorial system built for financial news and market commentary. It pairs a heavy, slightly condensed display sans with clean body copy, then punctuates everything with a single high-voltage neon chartreuse and inline monospaced ticker chips. The result reads like a print broadsheet that got a neon highlighter run through it.

## Color Palette

**Primary Colors:**
- Ink Black: `#0B0B0B` — headlines, body text, dark section backgrounds
- Highlighter: `#DFFF3C` — signature accent, CTA backgrounds, brand moments
- Paper: `#F1F0EC` — page background, warm off-white

**Neutral Colors:**
- Surface: `#FAFAF7` — article card background
- Text Primary: `#0B0B0B`
- Text Secondary: `#55554F` — bylines, timestamps, meta
- Text Muted: `#8A8A85`
- Border: `#D8D7D1` — hairlines, dividers
- Dark Surface: `#111111` — nav drawer, footer blocks
- Dark Surface Text: `#FFFFFF`

**Accent/State Colors:**
- Negative (Red): `#E63946` — downticks, loss indicators, boxed negative values
- Positive (Green): `#1F9E5B` — upticks, gains (inferred)
- Link Underline: `#0B0B0B` — always underlined on hover, strong weight

## Typography

**Font Families:**
- Display: A heavy geometric/grotesque sans with slightly condensed proportions and sharp terminals — closest free equivalent: **Archivo Black** or **Space Grotesk 700**
- Body: A clean humanist sans — closest free equivalent: **Inter** or **Söhne** substitute
- Mono: A boxy monospace for tickers — closest free equivalent: **JetBrains Mono** or **IBM Plex Mono**

**Type Scale:**
- Display: 48px / 900 / 1.05 / -0.02em
- Heading 1: 32px / 800 / 1.1 / -0.015em
- Heading 2: 24px / 800 / 1.15 / -0.01em
- Heading 3: 18px / 700 / 1.2
- Body Large: 18px / 400 / 1.55
- Body: 16px / 400 / 1.6
- Meta: 13px / 600 / 1.3 / uppercase for bylines
- Ticker Mono: 13px / 500 / 1 (inline chip treatment)

**Hierarchy Rules:**
Headlines are set extremely heavy (800–900 weight) and tight, body is comfortably loose at 1.55–1.6 line height. Meta info (bylines, timestamps) is uppercase, small, and semibold. Inline tickers break the prose with boxed monospace chips to create visual texture mid-paragraph.

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 96

**Common Patterns:**
- Article card padding: 32px (mobile) / 48px (desktop)
- Paragraph spacing: 20px between blocks
- Section spacing: 64–96px
- Inline chip padding: 4px 8px

## Component Styles

### Buttons
- Primary: Solid `#0B0B0B` background, white text, 0px radius (hard edges), 14px 24px padding, 700 weight, uppercase or sentence case, arrow indicator (`→`)
- Accent: Solid `#DFFF3C` background, black text, same structure
- Ghost: Transparent with 1px `#0B0B0B` border
- No shadows. No rounding. Hover: inverted color pair.

### Cards
- White (`#FAFAF7`) background sitting on paper (`#F1F0EC`) page
- 1px `#D8D7D1` border or no border at all
- 0px radius — hard rectangular edges
- Generous internal padding (32–48px)
- Decorative glyph or mark floating above card top

### Input Fields
- 1px bottom border only (underline style) or full 1px border
- 0px radius, transparent background
- 16px font size, black text
- Focus: border thickens to 2px black

### Ticker Chips (signature component)
- Inline monospaced text: `SYM $000.00 (+/-0.00%)`
- 1px border matching the state color
- 4px 8px padding, 0px radius
- Red `#E63946` border + red text for negative
- Sits inline within prose, breaking the text rhythm

### Navigation
- Full-screen overlay drawer, black (`#111`) background
- Oversized display type list (32–40px), white, left-aligned
- Stacked vertical menu with generous line height
- Close X in top-right corner

## Layout Principles

- Max content width: ~720px for article body
- Single-column, centered, mobile-first
- Generous top/bottom padding on sections
- Hairline dividers (1px `#D8D7D1`) to separate content blocks
- Alignment: strictly left-aligned — no centered body copy
- Asymmetric composition: meta in top-left, timestamp top-right

## Visual Effects

- **Border Radius:** 0px everywhere — hard edges define the aesthetic
- **Shadows:** None. Zero. Flat and print-like.
- **Borders:** 1px hairlines in `#D8D7D1` for structure, thicker 2px black borders for emphasis
- **Backgrounds:** Solid warm paper tone for page, white for content, black for nav/footer, neon chartreuse for brand moments — no gradients, no textures
- **Decorative elements:** Small pixel-art or editorial glyph marks used sparingly as visual punctuation above cards

## Design Tone

Authoritative but irreverent. This system reads like a financial broadsheet that refuses to be boring — it takes the gravity of ink-on-paper typography and shocks it with a highlighter-yellow accent that insists you pay attention. Confident, opinionated, and unapologetically editorial.

## Usage Notes for AI Implementation

- Default to zero border radius on everything. Rounding kills this aesthetic.
- Reserve the chartreuse for brand moments and CTAs — never use it for large body areas except intentional "follow the money" brand blocks
- Ticker chips are the signature move — any numeric value in prose (prices, percentages, stats) can get the boxed mono treatment
- Use uppercase meta labels for bylines, timestamps, categories
- Never use shadows. Flatness is the point.
- Body copy stays black on warm paper — resist the urge to use gray for "softness"
- Pair the heaviest display weight you can find with a neutral humanist body sans
