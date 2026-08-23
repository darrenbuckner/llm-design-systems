---
id: dark-terminal-001
title: Ink Terminal
description: A stark black and white terminal-inspired design system with monospace typography and dashed border motifs
tags: [dark, minimal, technical, monospace, brutalist]
colors: ["#000000", "#FFFFFF", "#E07B54", "#4A6CF7", "#E74C3C", "#333333"]
created: 2025-01-08
---

# Ink Terminal

A brutalist, developer-focused design system built on stark black and white contrast with monospace typography throughout. The aesthetic evokes command-line interfaces and technical documentation while maintaining visual sophistication through careful spacing and dashed border patterns.

## Color Palette

**Primary Colors:**
- Background: #000000 — Pure black, used as the dominant surface
- Foreground: #FFFFFF — Pure white, used for all primary text and borders

**Accent Colors:**
- Coral: #E07B54 — Warm accent for icons and highlights
- Blue: #4A6CF7 — Cool accent for secondary icons and interactive elements
- Red: #E74C3C — Error states, warning indicators, attention nodes

**Neutral Colors:**
- Dark Gray: #333333 — Subtle differentiation on dark surfaces
- Mid Gray: #666666 — Secondary text, disabled states
- Light Gray: #999999 — Tertiary information, timestamps

## Typography

**Font Families:**
- Primary: `'IBM Plex Mono', 'Courier New', monospace` — All text uses monospace
- Alternative: `'Space Mono', 'Fira Code', monospace`

**Type Scale:**
- Display: 48px, 700 weight, 1.1 line-height — Major headlines, title slides
- Heading 1: 36px, 700 weight, 1.2 line-height — Section headers
- Heading 2: 28px, 600 weight, 1.3 line-height — Subsection headers
- Heading 3: 22px, 600 weight, 1.4 line-height — Card titles
- Body: 18px, 400 weight, 1.6 line-height — Primary content
- Body Small: 16px, 400 weight, 1.5 line-height — Secondary content
- Caption: 14px, 400 weight, 1.4 line-height — Labels, meta information

**Hierarchy Rules:**
- Headlines often use italics for emphasis
- Highlighted text uses white background with black text (inverted)
- Step indicators use bracketed format: `STEP [1]`
- All caps used sparingly for labels and badges

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 16, 24, 32, 48, 64, 96, 128

**Common Patterns:**
- Container padding: 48px horizontal, 64px vertical
- Section spacing: 64-96px between major sections
- Component padding: 24-32px internal
- List item spacing: 16-24px between items
- Icon spacing: 16px from text
- Dashed border offset: 2px dash, 6px gap

## Component Styles

### Buttons
- Background: transparent or #FFFFFF
- Border: 2px solid #FFFFFF (or dashed)
- Padding: 12px 24px
- Font: 16px monospace, uppercase optional
- Hover: Inverted (white background, black text)
- Border radius: 0px (sharp corners)

### Cards / Containers
- Background: transparent
- Border: 2px dashed #FFFFFF
- Padding: 32px
- Border radius: 8-12px (slight rounding on dashed containers)
- No shadow

### Step Badges
- Background: #FFFFFF
- Text: #000000
- Format: `STEP [N]`
- Padding: 8px 16px
- Font: 14px monospace, bold

### List Items
- Arrow prefix: `→` character
- Checkmark prefix: `✔` for completed items
- X prefix: `X` for errors/mistakes
- Bullet prefix: `•` for standard lists
- Spacing: 16px between items
- Indent: 24px from arrow to text

### Icons
- Style: Simple line icons, white stroke
- Size: 24-48px
- Container: Rounded rectangle with colored fill (#E07B54, #4A6CF7)
- Container radius: 12px
- Container padding: 12px

### Flow Diagrams
- Connector lines: 2px solid white
- Arrow style: Simple chevron `→`
- Node spacing: 48px minimum
- Dashed containers around grouped elements

## Layout Principles

- Max content width: 900px
- Grid structure: Single column primary, occasional 2-column for diagrams
- Alignment: Left-aligned text, centered diagrams
- Vertical rhythm: Consistent 64px section breaks
- Footer placement: Fixed bottom with author/URL pattern

## Visual Effects

**Border Radius:**
- Containers: 8-12px (dashed boxes)
- Buttons: 0px (sharp)
- Icons containers: 12px
- Badges: 0px

**Shadows:**
- None — Pure flat design

**Borders:**
- Primary: 2px dashed #FFFFFF
- Solid variant: 2px solid #FFFFFF
- Dash pattern: 8px dash, 8px gap (approximate)

**Backgrounds:**
- Primary: Solid #000000
- No gradients
- No textures
- Network/node illustrations as decorative elements

## Design Tone

This system projects a technical, no-nonsense aesthetic that speaks directly to developers and automation enthusiasts. The monospace typography and terminal-inspired visuals create an authentic "builder" feel while the stark black and white contrast ensures maximum readability and focus. Dashed borders add visual interest without compromising the minimalist philosophy.

## Usage Notes for AI Implementation

When implementing this design system:

1. **Always use monospace fonts** — This is non-negotiable for maintaining the terminal aesthetic
2. **Embrace white space** — Large margins and padding are essential
3. **Use dashed borders liberally** — They're the signature visual element
4. **Keep backgrounds pure black** — No dark grays for main surfaces
5. **Limit color accents** — Coral and blue should appear sparingly, primarily in icons
6. **Maintain sharp contrast** — No mid-tones for primary text
7. **Use arrow prefixes** — `→` for list items maintains the technical feel
8. **Step indicators** — Use `STEP [N]` format with inverted colors for sequential content
9. **Network diagrams** — Abstract node networks work well as decorative elements
10. **Footer pattern** — Author name left, URL right, simple horizontal layout
