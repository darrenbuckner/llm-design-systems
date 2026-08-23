---
id: dark-transit-purple-001
title: Amethyst Dispatch System
description: A dark, gradient-rich mobile interface with purple-to-violet accents, lavender CTAs, and magenta highlights — built for real-time service selection and map-driven workflows.
tags: dark, gradient, modern, mobile-first, glass, cards
colors: ["#1A1025", "#2A2038", "#7B61FF", "#C850C0", "#B8A0FF", "#FFFFFF"]
created: 2026-02-23
---

# Amethyst Dispatch System

A dark-mode mobile interface defined by deep purple-black backgrounds, a purple-to-violet gradient header, magenta accent lines, and soft lavender call-to-action buttons. The system uses card-based selection with glowing purple borders for active states, bottom-sheet interaction patterns, and a tab bar navigation. Designed for real-time service apps where users choose options, view maps, and confirm actions quickly.

## Color Palette

**Primary Colors:**
- Primary Purple: #7B61FF — Interactive elements, active tab indicators, icons, search icon
- Magenta Accent: #C850C0 — Route lines, highlight badges, lightning bolt icons, promotional sparkle elements
- Lavender CTA: #B8A0FF — Primary action buttons (large, full-width), soft and inviting

**Background Colors:**
- Deep Background: #1A1025 — Main app background, darkest layer
- Surface Dark: #2A2038 — Card backgrounds, bottom sheets, elevated surfaces
- Surface Elevated: #342A45 — Search input fields, chip/pill buttons, slightly raised elements
- Header Gradient Start: #3D1F5C — Top of gradient header area
- Header Gradient End: #1A1025 — Fades into main background

**Text Colors:**
- Text Primary: #FFFFFF — Headings, prices, primary labels
- Text Secondary: #A09AAF — Subtitles, timestamps, secondary info ("in 5 min")
- Text Muted: #6B6578 — Placeholder text, disabled states
- Text on CTA: #1A1025 — Dark text on lavender buttons for contrast

**Semantic Colors:**
- Success/Promo: #34D399 — Promotional badges, discount indicators, green tags
- Info Blue: #4A9EFF — Map route origin marker, informational elements
- Selection Glow: rgba(123, 97, 255, 0.3) — Glow border on selected cards
- Divider: #3A2F4A — Subtle separators between list items

**Map Colors:**
- Map Base: #1A1A2E — Dark map tile background
- Route Primary: #E040A0 — Main route line (bright magenta-pink)
- Route Secondary: #7B61FF — Alternative route or pickup indicator

## Typography

**Font Families:**
- Primary: SF Pro Display / Inter (system sans-serif, clean geometric)
- Monospace: SF Mono (for numeric data like prices, times)

**Type Scale:**
- Display/Greeting: 28px, weight 700, line-height 1.2 — "Seize the day, [Name]"
- Heading 1: 20px, weight 700, line-height 1.3 — Section headers ("Earn as you ride")
- Heading 2: 17px, weight 600, line-height 1.4 — Card titles ("Extra Comfort", "Priority Pickup")
- Body: 15px, weight 400, line-height 1.5 — Descriptions, details
- Body Bold: 15px, weight 600, line-height 1.5 — Prices, emphasis
- Caption: 13px, weight 400, line-height 1.4 — Timestamps, secondary labels ("in 5 min", "Add shortcut")
- Tab Label: 11px, weight 500, line-height 1.2 — Bottom tab bar labels

**Hierarchy Rules:**
- Prices are always bold (600-700 weight), right-aligned in list rows
- Section headers use sentence case with no uppercase transforms
- Greeting text is the largest element, creates personal connection
- Promotional text uses the green accent color at caption size

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 48, 64

**Common Patterns:**
- Screen edge padding: 20px (mobile safe area)
- Card internal padding: 16px
- Section spacing: 32px between major sections
- List item padding: 16px vertical, 20px horizontal
- Bottom sheet top padding: 24px
- Tab bar height: 56px with 8px icon-to-label gap
- Search input padding: 16px vertical, 20px horizontal
- Chip/pill button padding: 10px 16px
- Between list items: 0px (separated by dividers, not gaps)

## Component Styles

### Primary CTA Button
- Background: #B8A0FF (lavender)
- Text: #1A1025, 17px, weight 600
- Border radius: 28px (fully rounded pill)
- Padding: 18px 32px
- Full width within container margins
- No shadow, no border
- Hover/pressed: slight opacity decrease to 0.9
- Fixed to bottom of screen with safe area padding

### Chip/Pill Buttons (Action Row)
- Background: #342A45
- Text: #FFFFFF, 14px, weight 500
- Border: 1px solid #4A3D5C
- Border radius: 24px (fully rounded)
- Padding: 10px 16px
- Icon + text layout, 8px gap
- Horizontal scrollable row

### Selection Card (Active State)
- Background: #2A2038
- Border: 2px solid #7B61FF
- Box shadow: 0 0 20px rgba(123, 97, 255, 0.25) — purple glow
- Border radius: 16px
- Internal layout: image left, text right, stacked vertically
- Contains sub-banner at bottom with icon + text (e.g., guarantee badge)

### List Row (Inactive Option)
- Background: transparent
- No border
- Padding: 16px 20px
- Layout: thumbnail (56px) left, title + subtitle stacked, price right-aligned
- Divider: 1px solid #3A2F4A below each row
- Tap state: background briefly flashes #342A45

### Search Input
- Background: #342A45
- Border: 1px solid #4A3D5C
- Border radius: 12px
- Padding: 16px 20px
- Placeholder text: #6B6578, 15px
- Search icon: #7B61FF, 20px, left-aligned
- No shadow

### Tab Bar (Bottom Navigation)
- Background: #1A1025
- Border top: 1px solid #3A2F4A
- Height: 56px + safe area inset
- Icons: 24px, default #6B6578, active #7B61FF
- Labels: 11px, default #6B6578, active #7B61FF
- 4 tabs evenly distributed
- Active indicator: color change only (no underline or dot)

### Info Badge / Promotional Tag
- Background: transparent
- Text: #34D399, 13px, weight 500
- Icon: green diamond/tag, 14px
- Inline with text, 6px gap

### Bottom Sheet
- Background: #1A1025
- Border radius: 16px 16px 0 0 (top corners only)
- Drag handle: 36px wide, 4px tall, #4A3D5C, centered, 12px from top
- Shadow: 0 -4px 24px rgba(0, 0, 0, 0.4)
- Slides up from bottom, overlay on map

### Map Overlay UI
- Arrival pill: background #2A2038 with 80% opacity, border-radius 12px, padding 8px 16px
- Back arrow: 40px circle, background #2A2038, icon #FFFFFF
- Route info bar: background #2A2038 with blur backdrop, full width, padding 12px 20px

## Layout Principles

- **Screen structure:** Map top half, bottom sheet bottom half (draggable)
- **Max content width:** Full screen (mobile-native, no max-width constraint)
- **Grid:** Single column, full-width cards and list rows
- **Alignment:** Left-aligned text, right-aligned prices/chevrons
- **Navigation:** Bottom tab bar (4 items), fixed position
- **Interaction model:** Bottom sheet with drag-to-expand, scrollable content within
- **Safe areas:** 20px horizontal padding, bottom safe area for tab bar and CTA

## Visual Effects

- **Border Radius:** 28px for buttons (pill), 16px for cards/sheets, 12px for inputs, 8px for small elements
- **Shadows:** Minimal — only on bottom sheets (upward shadow) and selected card glow. No general drop shadows.
- **Borders:** 1px solid #4A3D5C for inputs and chips; 2px solid #7B61FF for selected state; 1px solid #3A2F4A for dividers
- **Backgrounds:** Deep gradient (purple to black) for header; solid darks elsewhere
- **Blur:** Backdrop blur on map overlay elements (~12px)
- **Glow:** Purple glow (box-shadow) on selected/active cards
- **Transitions:** 200ms ease for state changes, 300ms for bottom sheet animation

## Design Tone

This system feels premium yet approachable — a night-mode interface that uses purple gradients and magenta accents to create energy without harshness. The lavender CTA buttons are soft and inviting rather than aggressive, while the glowing purple selection states feel modern and responsive. It's a system built for speed of decision-making: clear price hierarchies, quick-scan list layouts, and a single prominent action button anchored at the bottom.

## Usage Notes for AI Implementation

- Always use the deep purple-black background (#1A1025) as the base — never pure black (#000000)
- The lavender CTA (#B8A0FF) should be reserved for the single most important action on screen
- Purple glow borders indicate selection — use sparingly, only on the currently active/chosen item
- Magenta (#C850C0) is an accent for dynamic elements (routes, badges, sparkle icons) — not for text or backgrounds
- List rows should feel dense but scannable: thumbnail + title/subtitle left, price right, no extra decoration
- Bottom sheets are the primary interaction pattern — content lives in sheets that overlay the map
- Chip buttons in horizontal rows provide secondary actions without taking vertical space
- Green (#34D399) is strictly for promotional/reward content — never for success states in this context
- Tab bar icons should be simple outline style, filling or coloring on active state
- All text on dark backgrounds should be #FFFFFF or #A09AAF — avoid gray tones lighter than the surface colors
