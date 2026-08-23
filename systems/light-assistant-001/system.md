---
id: light-assistant-001
title: Assistant Service Design System
description: A friendly, approachable design system with teal accent and warm neutrals for service platforms
tags: light, friendly, teal-accent, card-based, rounded
colors: #1a9c9c, #e8f9e6, #2b2d2e, #f5f4f2
created: 2024-12-14
---

# Assistant Service Design System

A warm, approachable design system built around a vibrant teal primary color with soft neutrals and friendly rounded corners. Designed for service platforms that emphasize human connection and ease of use.

## Color Palette

**Primary Colors:**
- Primary Teal: #1a9c9c — Main brand color, used for hero sections, primary CTAs
- Primary Dark: #157878 — Hover states, active elements

**Neutral Colors:**
- Background Light: #f5f4f2 — Primary background, card surfaces
- Background White: #ffffff — Card backgrounds, contrast surfaces
- Background Warm: #e8f4f3 — Subtle teal-tinted backgrounds
- Text Primary: #2b2d2e — Headings, primary copy
- Text Secondary: #5f6368 — Body text, descriptions
- Text Muted: #8e9195 — Supporting text, labels

**Accent Colors:**
- Accent Yellow: #e8f9e6 — Icon backgrounds, subtle highlights
- Accent Lime: #d4ed4b — Secondary accent for icons and highlights
- Border Gray: #e4e4e5 — Card borders, dividers

**State Colors:**
- Success: #4caf50 — (implied from service context)
- Warning: #ff9800 — (implied from service context)
- Error: #f44336 — (implied from service context)

## Typography

**Font Families:**
- Primary: System sans-serif (likely Inter, -apple-system, or similar)
- Monospace: Monospace stack for technical content

**Type Scale:**
- Hero Heading: 56px, 700 weight, 1.1 line-height
- Section Heading: 42px, 700 weight, 1.15 line-height
- Card Heading: 32px, 700 weight, 1.2 line-height
- Subheading: 24px, 600 weight, 1.3 line-height
- Body Large: 20px, 400 weight, 1.6 line-height
- Body: 16px, 400 weight, 1.5 line-height
- Small/Caption: 14px, 400 weight, 1.4 line-height
- Label: 12px, 500 weight, 1.3 line-height

**Hierarchy Rules:**
- All headings use 700 weight for strong presence
- Body text maintains 400 weight for readability
- Generous line-height (1.5-1.6) for comfortable reading
- Tight letter-spacing on large headings (-0.02em)

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 120

**Common Patterns:**
- Component padding: 24-32px
- Card internal padding: 40-48px
- Section vertical spacing: 80-120px
- Grid gaps: 16-24px
- Button padding: 14px vertical, 32px horizontal
- Icon container padding: 16-20px

## Component Styles

### Buttons

**Primary Button (CTA):**
- Background: #2b2d2e (dark)
- Text: #ffffff
- Border-radius: 48px (full pill shape)
- Padding: 18px 40px
- Font-size: 18px
- Font-weight: 500
- Border: 2px solid rgba(255, 255, 255, 0.2)
- Transition: all 0.2s ease

**Hover State:**
- Background: #1a1b1c
- Border-color: rgba(255, 255, 255, 0.3)
- Transform: translateY(-2px)

**Accordion/Disclosure Button:**
- Background: #ffffff
- Border: 1px solid #e4e4e5
- Border-radius: 48px (full pill)
- Padding: 20px 32px
- Font-size: 18px
- Text-align: left
- Icon: Chevron right-aligned

### Cards

**Standard Card:**
- Background: #ffffff
- Border: 1px solid #e4e4e5
- Border-radius: 24px
- Padding: 40px
- Box-shadow: 0 1px 3px rgba(0, 0, 0, 0.04)

**Card with Icon:**
- Icon container: 56px × 56px
- Icon background: #e8f9e6 or #d4ed4b
- Icon border-radius: 16px
- Icon size: 28-32px
- Icon color: #2b2d2e
- Margin-bottom: 24px

**Card Hover:**
- Box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08)
- Transform: translateY(-2px)
- Transition: all 0.3s ease

### Tables

**Table Structure:**
- Header background: transparent
- Row separator: 1px solid #e4e4e5
- Cell padding: 20px 16px
- Font-size: 16px

**Table Headers:**
- Font-weight: 600
- Color: #5f6368
- Text-transform: none

**Table Cells:**
- Color: #2b2d2e
- Vertical-align: middle

### Icons

**Icon Container:**
- Size: 56px × 56px
- Background: #e8f9e6 or #d4ed4b
- Border-radius: 16px
- Icon size: 28-32px within container
- Centered alignment

**Icon Only:**
- Size: 24-32px for inline use
- Color: #2b2d2e or contextual

## Layout Principles

**Content Width:**
- Max content width: 1200px
- Container padding: 24-40px horizontal
- Centered alignment

**Grid Structure:**
- 2-column card grid on desktop
- 16-24px gap between cards
- Single column on mobile
- Full-width hero sections

**Responsive Behavior:**
- Mobile: Single column, 16px padding
- Tablet: 2-column grid, 24px padding
- Desktop: 2-column grid, full spacing

**Alignment:**
- Text: Left-aligned in cards
- Hero content: Left-aligned
- Centered CTAs in hero sections

## Visual Effects

**Border Radius:**
- Buttons: 48px (full pill)
- Cards: 24px (generous rounding)
- Icon containers: 16px (moderate rounding)
- Small elements: 8-12px

**Shadows:**
- Default card: 0 1px 3px rgba(0, 0, 0, 0.04)
- Hover card: 0 4px 12px rgba(0, 0, 0, 0.08)
- Button: Minimal or none
- Depth: Very subtle, natural elevation

**Borders:**
- Thickness: 1px standard, 2px for emphasis
- Style: Solid
- Color: #e4e4e5 for neutral, rgba(255, 255, 255, 0.2) for buttons on dark

**Backgrounds:**
- Solid colors: #f5f4f2, #ffffff
- Tinted backgrounds: #e8f4f3 (subtle teal wash)
- No gradients in primary use
- Pattern/texture: Clean, minimal

**Transitions:**
- Duration: 0.2-0.3s
- Easing: ease or ease-in-out
- Properties: transform, box-shadow, background, border

## Design Tone

The system conveys approachability and competence through warm neutrals paired with a confident teal accent. Generous rounded corners and ample whitespace create a friendly, non-intimidating interface. Typography is clear and direct without being clinical. The design emphasizes clarity and ease of use while maintaining visual interest through the strategic use of the vibrant teal and playful yellow-green accents. Perfect for service platforms that want to feel helpful, trustworthy, and human-centered.

## Usage Notes for AI Implementation

When implementing this system in AI-generated interfaces:

1. **Use the teal (#1a9c9c) sparingly** for maximum impact — hero backgrounds, primary CTAs, and key accent moments
2. **Default to warm neutrals** (#f5f4f2, #ffffff) for most surfaces
3. **Apply generous spacing** — don't be afraid of whitespace, especially vertical spacing between sections (80-120px)
4. **Round everything** — 24px for cards, 48px for buttons creates the friendly aesthetic
5. **Use icon backgrounds** (#e8f9e6, #d4ed4b) to add visual interest without overwhelming
6. **Keep typography simple** — stick to system sans-serif at the documented sizes
7. **Subtle shadows only** — this isn't a heavy depth system, keep elevations minimal
8. **Consistent card structure** — icon at top, heading, description, optional action
9. **Mobile-first spacing** — reduce padding and gaps proportionally on smaller screens
10. **Maintain the warm, approachable tone** in both visual design and copy treatment
