---
id: dark-finance-001
title: Carbon Ledger
description: A pure black finance interface with colorful category indicators and clean information hierarchy
tags: [dark, mobile-first, finance, minimal, high-contrast]
colors: ["#000000", "#1C1C1E", "#2C2C2E", "#FFFFFF", "#F87171", "#4ADE80"]
created: 2026-01-11
---

# Carbon Ledger

A sophisticated dark-mode financial interface built on a pure black foundation. The system uses stark contrast between the void-black background and bright white typography, punctuated by soft pastel category indicators. Cards float on elevated dark surfaces, creating depth through subtle layering rather than shadows. The overall effect is premium, focused, and easy to scan in low-light environments.

## Color Palette

**Background Colors:**
- Pure Black: #000000 — Primary app background, creates maximum contrast
- Card Surface: #1C1C1E — Elevated card backgrounds, modal overlays
- Card Surface Alt: #2C2C2E — Secondary cards, nested elements, expanded sections
- Input Surface: #3A3A3C — Form fields, interactive input areas

**Text Colors:**
- Primary Text: #FFFFFF — Headlines, primary values, active states
- Secondary Text: #8E8E93 — Labels, supporting text, inactive items
- Tertiary Text: #636366 — Timestamps, metadata, disabled states

**Accent Colors:**
- Coral Red: #F87171 — Primary CTA, alerts, referral prompts, notification badges
- Coral Red Border: rgba(248, 113, 113, 0.3) — Outlined buttons, selection states

**Category Indicator Colors:**
- Needs (Pink): #F9A8D4 — Housing, essentials
- Wants (Cream): #FDE68A — Discretionary spending
- Review (Amber): #FBBF24 — Items needing attention
- Savings (Mint): #4ADE80 — Savings goals, positive states
- Everything Else (Sky): #7DD3FC — Miscellaneous categories

**Chart/Visualization Colors:**
- Chart Fill: #3B82F6 — Area chart fill, progress bars
- Chart Line: #60A5FA — Chart stroke, trend lines
- Budget Line: #6B7280 — Dashed reference lines

**State Colors:**
- Success: #4ADE80 — Positive values, confirmations
- Warning: #FBBF24 — Attention needed
- Error: #F87171 — Negative values, alerts
- Info: #60A5FA — Informational states

## Typography

**Font Family:**
- Primary: SF Pro Display / SF Pro Text (system San Francisco)
- Fallback: -apple-system, BlinkMacSystemFont, "Segoe UI", system-ui, sans-serif

**Type Scale:**

- Display Large: 42px, weight 700, line-height 1.1 — Hero monetary values
- Heading 1: 28px, weight 600, line-height 1.2 — Screen titles
- Heading 2: 20px, weight 600, line-height 1.3 — Section headers, card titles
- Heading 3: 17px, weight 600, line-height 1.4 — List item titles
- Body: 17px, weight 400, line-height 1.5 — Primary content
- Body Small: 15px, weight 400, line-height 1.5 — Secondary descriptions
- Caption: 13px, weight 500, line-height 1.4 — Labels, section headers (uppercase)
- Micro: 11px, weight 500, line-height 1.3 — Timestamps, version numbers

**Typography Patterns:**
- Section headers use uppercase letters with generous letter-spacing (0.5-1px)
- Monetary values use tabular figures for alignment
- Secondary text beneath primary values provides context ("This Month", "$X last month")
- Quotation marks use smart quotes with italic styling for inspirational content

## Spacing System

**Base Unit:** 4px

**Spacing Scale:**
- 4px — Tight gaps (icon to text in compact rows)
- 8px — Default component internal padding
- 12px — Standard gap between related elements
- 16px — Card internal padding, section spacing
- 20px — Comfortable breathing room
- 24px — Section separation
- 32px — Major section breaks
- 48px — Screen-level vertical rhythm

**Common Patterns:**
- Card padding: 16px all sides
- List item padding: 16px horizontal, 12px vertical
- Icon-to-text gap: 12px
- Between stacked cards: 8-12px
- Section header margin-bottom: 12px
- Safe area insets respected on iOS

## Component Styles

### Cards

**Standard Card:**
- Background: #1C1C1E
- Border radius: 16px
- Padding: 16px
- No border, no shadow (relies on color contrast for elevation)

**Nested Card / Expandable Section:**
- Background: #2C2C2E
- Border radius: 12px
- Often contains subcategories or detailed breakdowns

**Dashboard Widget Card:**
- Background: #1C1C1E to #2C2C2E gradient (subtle)
- Border radius: 20px
- Larger padding: 20px
- Contains charts, summary data, pagination dots

### Buttons

**Primary CTA (Outlined):**
- Background: transparent
- Border: 2px solid rgba(248, 113, 113, 0.4)
- Border radius: 12px
- Text color: #FFFFFF
- Padding: 14px 20px
- Full width in cards

**Secondary Button:**
- Background: #2C2C2E
- Border: none
- Border radius: 8px
- Text color: #FFFFFF
- Padding: 12px 16px

**Ghost Button / Text Action:**
- Background: transparent
- Text color: #FFFFFF or #8E8E93
- Underline on hover (optional)

**Add Button (Outline):**
- Background: transparent
- Border: 1px solid #3A3A3C
- Border radius: 12px
- Icon + text layout
- Full width

### Category Indicators

**Icon Badge Style:**
- Size: 40px × 40px
- Border radius: 50% (full circle)
- Background: Category color at 20% opacity
- Icon: Category color at 100%, centered
- Icon size: 20px

**Color-coded Categories:**
- Each spending/saving category has a unique pastel color
- Icons are line-style, not filled
- Badge appears to left of category name

### List Items

**Standard List Row:**
- Height: auto (content-driven)
- Padding: 16px horizontal, 14px vertical
- Icon badge: 40px circle, left aligned
- Text stack: Title (17px 600) + Subtitle (13px 400 #8E8E93)
- Right side: Value + optional edit icon
- Divider: 1px solid #2C2C2E (inset from icon)

**Expandable List Item:**
- Chevron rotates on expand
- Nested items indent with subtle background change

### Navigation

**Bottom Tab Bar:**
- Background: #000000 with subtle top border
- Height: ~83px (includes safe area)
- 5 tabs evenly distributed
- Active: White icon + label
- Inactive: #8E8E93 icon + label
- Icon size: 24px
- Label: 10px, medium weight

**Settings Menu:**
- Full-screen overlay or sheet
- Grouped sections with visual separation
- Premium badge: Purple pill with diamond icon

### Input Fields

**Text Input:**
- Background: #2C2C2E
- Border: none (or 1px solid #3A3A3C on focus)
- Border radius: 10px
- Padding: 12px 16px
- Text: #FFFFFF
- Placeholder: #636366

### Charts

**Area Chart:**
- Fill: Linear gradient from #3B82F6 (top) to transparent (bottom)
- Stroke: #60A5FA, 2px
- Current point: 8px circle, filled #60A5FA
- Reference line (budget): Dashed #6B7280
- Label: Uppercase "BUDGET" in caption style

**Progress Bar:**
- Height: 6px
- Background: #2C2C2E
- Fill: Linear gradient #3B82F6 to #60A5FA
- Border radius: 3px

### Badges & Pills

**Notification Badge:**
- Background: #F87171
- Size: 18px min-width, pill shape
- Text: White, 11px, bold
- Positioned top-right of parent

**Status Pill:**
- Background: varies by status
- Border radius: 999px
- Padding: 4px 10px
- Text: 12px, medium weight

## Layout Principles

**Screen Structure:**
- Safe areas respected (notch, home indicator)
- Scrollable content with fixed bottom navigation
- Cards as primary content containers
- No visible grid lines; organic stacking

**Grid System:**
- Single column on mobile (primary use case)
- 2-column grid for dashboard widgets (watchlist cards)
- Card gap: 12px
- Container padding: 16px horizontal

**Hierarchy:**
- Large numerical values dominate (spending amounts)
- Supporting context below in smaller, muted text
- Section headers provide scannable organization
- Icons add visual interest and quick recognition

## Visual Effects

**Border Radius Scale:**
- Micro: 4px — Small badges, tags
- Small: 8px — Buttons, small cards
- Medium: 12px — Input fields, list item groups
- Large: 16px — Standard cards
- XL: 20px — Hero cards, dashboard widgets
- Full: 50% or 999px — Circular elements, pills

**Shadows:**
- None used — System relies on layered surfaces and color contrast

**Borders:**
- Minimal use
- When present: 1px solid #2C2C2E or rgba color
- CTA borders use accent color at reduced opacity

**Backgrounds:**
- Solid colors only
- No gradients on surfaces (exception: charts)
- Pure black (#000000) enables true black on OLED screens

## Design Tone

This system embodies focused clarity through high contrast. The pure black background eliminates visual noise, allowing white typography and colorful category indicators to command attention. The aesthetic is premium yet approachable—serious enough for financial data while remaining friendly through rounded corners and pastel category colors. Every element serves the user's need to quickly scan and understand their financial position.

## Usage Notes for AI Implementation

When implementing this system:

1. **Prioritize readability** — Large, bold monetary values are the primary focus. Supporting data should be visually subordinate.

2. **Use pure black backgrounds** — #000000 specifically, to enable OLED black and maximum contrast. Avoid dark grays for the base layer.

3. **Layer surfaces thoughtfully** — Cards sit on #1C1C1E, nested content on #2C2C2E. This creates depth without shadows.

4. **Category colors are functional** — Each pastel indicator represents a specific type of data. Maintain consistency; don't use decoratively.

5. **Maintain generous touch targets** — List items should have at least 44px touch height. Buttons need comfortable padding.

6. **Respect the type hierarchy** — Don't let secondary labels compete with primary values. Use color (not just size) to differentiate.

7. **Keep animations minimal** — This is a utility interface. Subtle transitions (expand/collapse, tab switches) are sufficient.

8. **Support dark mode exclusively** — This system is designed for dark environments. A light mode variant would require a separate design system.
