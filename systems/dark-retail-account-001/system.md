---
id: dark-retail-account-001
title: Carbon Pantry
description: A clean, high-contrast dark interface for retail and grocery account management with subtle card elevation and clear information hierarchy.
tags: [dark, minimal, mobile, retail, account-management]
colors: ["#000000", "#1C1C1E", "#2C2C2E", "#FFFFFF", "#0A84FF", "#E91E8D"]
created: 2026-01-10
---

# Carbon Pantry

A utilitarian dark theme designed for retail account management and grocery shopping apps. The system prioritizes readability and quick scanning of account information through high-contrast typography on pure black backgrounds, with subtle card elevation creating visual hierarchy without distraction.

## Color Palette

**Primary Colors:**
- Primary Action: #0A84FF — Interactive links, CTAs, primary actions
- Accent/Brand: #E91E8D — Secondary branding, membership badges, promotional elements

**Neutral Colors:**
- Background Primary: #000000 — Main screen background, true black for OLED
- Surface/Card: #1C1C1E — Elevated cards, containers, input backgrounds
- Surface Secondary: #2C2C2E — Subtle card variations, hover states
- Text Primary: #FFFFFF — Headlines, primary content, high-emphasis text
- Text Secondary: #8E8E93 — Metadata, timestamps, supporting text
- Text Tertiary: #636366 — Disabled states, placeholder text
- Border/Divider: #38383A — List separators, subtle borders

**State Colors:**
- Success: #30D158 — Confirmations, positive states
- Warning: #FFD60A — Alerts, attention indicators
- Error: #FF453A — Errors, destructive actions

## Typography

**Font Families:**
- Primary: SF Pro Display / System UI — Used for all interface text
- Fallback: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif

**Type Scale:**
- Display/Page Title: 34px, weight 700 (bold), line-height 1.2, letter-spacing -0.5px
- Section Header: 22px, weight 600 (semibold), line-height 1.3
- Card Title: 17px, weight 600 (semibold), line-height 1.4
- Body/List Item: 17px, weight 400 (regular), line-height 1.4
- Label: 13px, weight 400 (regular), line-height 1.3, uppercase optional
- Caption/Metadata: 13px, weight 400 (regular), line-height 1.3, secondary color
- Large Value: 28px, weight 600 (semibold), line-height 1.2

**Hierarchy Rules:**
- Page titles use large bold display text with slight negative letter-spacing
- Section headers are semibold with generous top margin
- Card titles and list items share the same base size, differentiated by weight
- Metadata and timestamps use smaller, muted text
- Interactive text (links) uses the primary blue color

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48

**Common Patterns:**
- Screen horizontal padding: 16px
- Card internal padding: 16px
- Section vertical spacing: 32px
- List item vertical padding: 16px
- Icon to text spacing: 12px
- Card gap (horizontal scroll): 12px

## Component Styles

### Cards

**Info Cards (Purchase History, Membership):**
- Background: #1C1C1E
- Border radius: 12px
- Padding: 16px
- Shadow: none (uses background contrast for elevation)
- Icon container: 40px × 40px, 8px border radius, #2C2C2E background

**Card Content Structure:**
- Header: Icon + Title row
- Body: Label (small caps) + Value (large) + Metadata
- Footer: Text link in primary blue

### Buttons

**Text Button/Link:**
- Font size: 17px
- Font weight: 400-600
- Color: #0A84FF
- No background or border
- Tap target: minimum 44px height

**Icon Button:**
- Size: 24px icon
- Color: #FFFFFF or #0A84FF
- Tap target: 44px × 44px minimum

### List Items

**Navigation List Item:**
- Height: 52px (including padding)
- Background: transparent
- Border bottom: 1px solid #38383A
- Padding: 16px horizontal
- Icon: 24px, #8E8E93 or #FFFFFF
- Text: 17px, #FFFFFF
- Chevron: 12px, #636366, right-aligned
- Active/Pressed: #1C1C1E background

### Input Fields

**Text Input (implied from design language):**
- Background: #1C1C1E
- Border: none or 1px solid #38383A
- Border radius: 8px
- Padding: 12px 16px
- Text color: #FFFFFF
- Placeholder: #636366
- Focus: 2px solid #0A84FF outline

### Navigation

**Top Bar:**
- Background: #000000
- Height: 44px (below status bar)
- Close icon: × symbol, 24px, #FFFFFF, left-aligned
- Action text: "Sign Out", #0A84FF, right-aligned

**Section Headers:**
- Font size: 22px
- Font weight: 600
- Color: #FFFFFF
- Margin top: 32px
- Margin bottom: 16px

## Layout Principles

- **Max content width:** Full width on mobile, 428px max on larger screens
- **Grid structure:** Single column layout for account screens
- **Card layout:** Horizontal scroll for related card groups, 12px gap
- **Alignment:** Left-aligned text throughout
- **Safe areas:** Respects iOS safe area insets

## Visual Effects

**Border Radius:**
- Cards: 12px
- Buttons: 8px
- Icons/Avatars: 8px
- Inputs: 8px
- Pills/Tags: 16px (full round)

**Shadows:**
- None used — elevation achieved through background color contrast

**Borders:**
- List dividers: 1px solid #38383A
- Card borders: none (rely on background contrast)

**Backgrounds:**
- Pure black (#000000) base for OLED optimization
- Elevated surfaces use subtle gray (#1C1C1E)
- No gradients in standard UI

## Design Tone

This system embodies a utilitarian, no-nonsense approach to mobile retail interfaces. The pure black background optimizes for OLED displays while creating strong contrast with white typography. The design prioritizes information density and quick scanning over decorative elements, with a clear visual hierarchy established through typography weight and subtle surface elevation rather than color or decoration.

## Usage Notes for AI Implementation

**When implementing this system:**

1. **True black backgrounds** — Use #000000 as the base, not dark gray. This is intentional for OLED power efficiency.

2. **Elevation through color, not shadow** — Create depth by layering #1C1C1E cards on #000000 backgrounds. Avoid drop shadows.

3. **High-contrast text** — Always use pure white (#FFFFFF) for primary text. The stark contrast is a feature, not a bug.

4. **Consistent list patterns** — Navigation lists should follow the icon + text + chevron pattern with hairline dividers.

5. **Link color consistency** — All interactive text uses #0A84FF. Don't mix link colors.

6. **Generous tap targets** — All interactive elements should be at least 44px in their tappable dimension.

7. **Section grouping** — Use bold section headers ("Shortcuts", "My Account") to group related list items.

8. **Card scrolling** — Related cards (like purchase history and membership) can scroll horizontally with 12px gaps.

9. **Icon treatment** — Use outline-style icons at 24px, either white or system gray depending on emphasis.

10. **Status bar** — Assume light content on dark background (white status bar text).
