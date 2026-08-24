---
id: light-geometric-kanban-001
title: Bauhaus Board System
description: A playful geometric design system with bold primary colors, hand-drawn textures, and neobrutalist card styling
tags: [light, geometric, playful, neobrutalist, kanban]
colors: ["#F5E6DC", "#E63946", "#1D3557", "#FFDD00", "#FFFFFF"]
created: 2026-01-04
---

# Bauhaus Board System

A distinctive interface aesthetic that combines Bauhaus-inspired geometric shapes with neobrutalist card styling. The system features bold primary colors (red, blue, yellow) as accent elements against warm neutral backgrounds, with thick black borders creating strong visual definition. Hand-drawn textures and playful corner decorations add personality while maintaining functional clarity.

## Color Palette

**Primary Accent Colors:**
- Red: #E63946 — Primary accent, used for column indicators and avatars
- Blue: #1D3557 — Secondary accent, used for badges, avatars, and geometric shapes
- Yellow: #FFDD00 — Tertiary accent, column indicators and decorative elements

**Neutral Colors:**
- Background: #F5E6DC — Warm peachy-cream base background
- Surface/Cards: #FFFFFF — Pure white card backgrounds
- Text Primary: #1A1A1A — Near-black for headings and important text
- Text Secondary: #666666 — Medium gray for body text and descriptions
- Border: #1A1A1A — Bold black borders for cards and UI elements

**State/Semantic Colors:**
- Success/Done: #1D3557 — Blue badge for completed state
- In Progress: #E63946 — Red/coral for active items
- Warning: #FFDD00 — Yellow for attention states

**Tag Colors:**
- Design Tag: #1A1A1A — Black background with white text
- Dev Tag: #1A1A1A — Black background with white text
- Research Tag: #1A1A1A — Black background with white text
- UX Tag: #1A1A1A — Black background with white text
- Content Tag: #1A1A1A — Black background with white text
- Planning Tag: #1A1A1A — Black background with white text

## Typography

**Font Families:**
- Primary: Inter, system-ui, sans-serif — Clean geometric sans-serif
- Headings: Inter or similar geometric sans — Bold, condensed tracking

**Type Scale:**
- Display/Stats: 32px, 700 weight, 1.1 line-height (large numbers in header)
- Column Headers: 18px, 700 weight, 1.2 line-height, uppercase, letter-spacing: 0.05em
- Card Titles: 14px, 600 weight, 1.4 line-height
- Labels/Tags: 11px, 600 weight, 1.2 line-height, uppercase
- Caption/Meta: 12px, 400 weight, 1.3 line-height

**Hierarchy Rules:**
- Column headers use uppercase with generous letter-spacing for scanability
- Card titles use sentence case, medium weight for readability
- Stats use large bold numbers with small uppercase labels beneath
- Tags are always uppercase, compact, high contrast

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64

**Common Patterns:**
- Card internal padding: 16px
- Space between cards: 12px
- Column padding: 16px
- Section gaps: 24px
- Header padding: 24px 32px
- Component margins: 8px

**Card Dimensions:**
- Card width: Fluid within column (approximately 200-240px)
- Column width: Approximately 260px with gaps
- Min card height: Content-driven

## Component Styles

### Column Headers
- Typography: 18px, uppercase, bold, letter-spacing 0.05em
- Count badge: 28px circular, bold number, colored background matching column
- Left border accent: 4px wide, full height, column color
- Background: White with subtle texture/noise
- Border: 2px solid #1A1A1A on sides and bottom

### Task Cards
- Background: #FFFFFF
- Border: 2px solid #1A1A1A
- Border-radius: 0px (sharp corners)
- Padding: 16px
- Shadow: None (relies on borders for definition)
- Corner decorations: Small colored triangles (8px) in corners, using column accent colors
- Hover state: Subtle background shift or border color change

### Tags/Badges
- Background: #1A1A1A
- Text: #FFFFFF
- Padding: 4px 10px
- Border-radius: 4px
- Font: 11px, uppercase, 600 weight
- Letter-spacing: 0.02em

### Count Badges (Column Headers)
- Size: 28px × 28px
- Shape: Circle or rounded rectangle
- Background: Column accent color (red, yellow, blue)
- Text: White or black depending on contrast
- Font: 14px, 700 weight

### Avatar Badges
- Size: 28px × 28px
- Shape: Circle
- Background: Varied accent colors
- Text: White initials, 12px, 600 weight
- Position: Bottom-right of card

### Add Task Button
- Style: Dashed border, 2px
- Border color: #CCCCCC
- Text: #999999, 14px
- Padding: 12px 16px
- Full width within column
- Hover: Border and text darken

### Stats Display (Header)
- Large number: 32px, 700 weight, #1A1A1A
- Label: 11px, uppercase, #888888, letter-spacing 0.05em
- Layout: Stacked vertically, centered

### Geometric Shapes (Logo/Decoration)
- Circle: #E63946 (red)
- Square: #1D3557 (blue)
- Triangle: #FFDD00 (yellow)
- Size: 12-16px
- Arrangement: Horizontal row with 4px gaps

## Layout Principles

**Grid Structure:**
- 4-column kanban layout
- Column width: Fluid, approximately 25% each with gaps
- Gap between columns: 16-24px
- Horizontal scroll on overflow

**Container:**
- Max content width: 1200px suggested
- Container padding: 24px on sides
- Centered layout

**Alignment:**
- Left-aligned text within cards
- Centered stats in header
- Column headers left-aligned with count badge right-aligned

**Responsive Behavior:**
- Columns stack or scroll horizontally on mobile
- Cards maintain minimum width of 200px
- Header stats may wrap or condense

## Visual Effects

**Border Radius:**
- Cards: 0px (sharp neobrutalist corners)
- Tags: 4px (subtle rounding)
- Avatars/Badges: 50% (circular)
- Count badges: 50% or 4px

**Shadows:**
- None — System relies on bold borders instead of shadows
- Creates flat, graphic aesthetic

**Borders:**
- Primary border: 2px solid #1A1A1A
- Column accent borders: 4px solid [accent color]
- Card borders: 2px solid #1A1A1A
- Dashed borders: 2px dashed #CCCCCC for empty states

**Backgrounds:**
- Main: Warm cream #F5E6DC with subtle paper texture/noise
- Cards: Pure white #FFFFFF
- Optional: Very subtle grain/noise overlay on background

**Decorative Elements:**
- Corner triangles on cards (8px, accent colors)
- Geometric shapes in logo (circle, square, triangle)
- Paper-like texture on background

## Design Tone

This system embodies a **playful neobrutalist** aesthetic with clear Bauhaus influences. The bold primary color palette (red, blue, yellow) against warm neutral backgrounds creates an approachable yet distinctive look. The lack of shadows combined with thick black borders gives it a graphic, almost print-like quality. The system feels creative and energetic while remaining highly functional for task management — it's serious work tools dressed in kindergarten colors.

## Usage Notes for AI Implementation

**When to use this system:**
- Project management and task tracking interfaces
- Creative team collaboration tools
- Kanban boards and workflow visualizations
- Design tool interfaces
- Playful productivity applications

**Key implementation details:**
1. Always use sharp corners (0px border-radius) on cards — this is essential to the neobrutalist aesthetic
2. Rely on 2px black borders for definition, not shadows
3. Use the three primary accents (red, blue, yellow) sparingly as highlights
4. Maintain warm cream background, not pure white or cool gray
5. Tags should always be black with white text, uppercase
6. Include subtle corner triangle decorations on cards for personality
7. Header should feature geometric shape logo (circle, square, triangle)
8. Stats should use large bold numbers with small uppercase labels

**Color application rules:**
- Red (#E63946): First/urgent column indicators, priority items
- Yellow (#FFDD00): Middle/active column indicators, warnings
- Blue (#1D3557): Final/completed column indicators, informational
- Black (#1A1A1A): All borders, tags, primary text
- Warm cream (#F5E6DC): Page background only
- White (#FFFFFF): Card surfaces, input backgrounds

**Typography emphasis:**
- Use uppercase sparingly — only for column headers, tags, and stat labels
- Card titles should be sentence case for readability
- Generous letter-spacing on uppercase text (0.03-0.05em)
