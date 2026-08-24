---
id: light-premium-executive-001
title: Premium Executive Service System
description: Sophisticated pricing interface with deep green accent and warm neutral foundation
tags: [light, premium, minimal, professional]
colors: ["#0F3D2F", "#E8E4DC", "#F5F3EF", "#D4B896"]
created: 2025-12-13
---

# Premium Executive Service System

An elegant design system featuring deep forest green as the primary accent against warm neutral backgrounds, with sophisticated serif typography and generous spacing that conveys premium service quality.

## Color Palette

**Primary Colors:**
- Deep Forest Green: #0F3D2F — Primary accent color for cards, buttons, and key UI elements
- Sage Green: #A8C4B5 — Secondary surfaces and subtle backgrounds

**Neutral Colors:**
- Warm Cream Background: #F5F3EF — Main page background
- Light Warm Gray: #E8E4DC — Secondary backgrounds, card surfaces
- Medium Gray: #D4D4D4 — Borders and dividers
- Dark Text: #1A1A1A — Primary text color
- Medium Text: #4A4A4A — Secondary text, descriptions
- Light Text on Dark: #FFFFFF — Text on dark green surfaces

**Accent Colors:**
- Warm Gold: #D4B896 — Highlight badges and CTAs ("Better savings")
- Success Green: #28A745 — Toggle switches, success states
- Hover Dark Green: #0A2D23 — Button hover states

## Typography

**Font Families:**
- Primary Serif: Georgia or similar classic serif — Used for headings and display text
- Secondary Sans-serif: System fonts (SF Pro, Segoe UI) — Body text and UI elements

**Type Scale:**
- Large Display: 56px, weight 400, line-height 1.1 — Hero headings ("World-class assistants")
- Section Heading: 42px, weight 400, line-height 1.2 — Section titles ("Other plans")
- Card Title: 24px, weight 400, line-height 1.3 — Pricing plan names
- Price Display: 72px, weight 300, line-height 1 — Large pricing numbers
- Body Large: 18px, weight 400, line-height 1.6 — Descriptions and subtitles
- Body: 16px, weight 400, line-height 1.5 — Standard text
- Caption: 14px, weight 400, line-height 1.4 — Small details and metadata

**Hierarchy Rules:**
- Headings use serif fonts with light weights (300-400) for elegance
- Body text uses clean sans-serif for readability
- Price displays are oversized with light weight
- Ample letter-spacing on large headings (-0.02em)

## Spacing System

**Base Unit:** 8px
**Scale:** 8, 16, 24, 32, 40, 48, 64, 80, 120

**Common Patterns:**
- Card padding: 48px (large cards), 32px (medium cards)
- Section vertical spacing: 80-120px between major sections
- Component internal spacing: 16-24px
- Button padding: 16px vertical, 32px horizontal
- Input field padding: 12px vertical, 16px horizontal
- Grid gaps: 24-32px

## Component Styles

### Pricing Cards

**Large Featured Card (Dark):**
- Background: #0F3D2F (deep forest green)
- Border-radius: 24px
- Padding: 48px
- Shadow: 0 8px 32px rgba(0, 0, 0, 0.15)
- Text color: #FFFFFF

**Standard Card (Light):**
- Background: #E8E4DC or #F5F3EF
- Border-radius: 24px
- Padding: 48px
- Border: 2px solid #D4D4D4
- Shadow: 0 4px 16px rgba(0, 0, 0, 0.08)

**Card Elements:**
- Plan title: 24px serif, center-aligned
- Price: 72px, weight 300, center-aligned
- Subtext: 16px, opacity 0.8
- "View details" link: 16px, underlined, centered

### Buttons

**Primary Button (Dark):**
- Background: #0F3D2F
- Color: #FFFFFF
- Border-radius: 32px (pill shape)
- Padding: 14px 32px
- Font-size: 16px
- Font-weight: 500
- Hover: #0A2D23

**Secondary Button (Outline):**
- Background: transparent
- Color: #0F3D2F
- Border: 2px solid #0F3D2F
- Border-radius: 32px
- Padding: 14px 32px
- Hover: Background #0F3D2F, Color #FFFFFF

**CTA Button:**
- Background: #0F3D2F
- Width: 100% (full-width on mobile)
- Max-width: 800px
- Padding: 18px 48px
- Font-size: 18px

### Toggle Switch

**Pricing Toggle:**
- Background container: #E8E4DC
- Border-radius: 24px (pill)
- Padding: 4px
- Active state: #28A745 (green)
- Inactive state: Gray
- Labels: 16px sans-serif

**Badge:**
- Background: #D4B896 (warm gold)
- Color: #1A1A1A
- Border-radius: 16px
- Padding: 8px 20px
- Font-size: 14px
- Font-weight: 500

### Text Links

- Color: #0F3D2F
- Text-decoration: underline
- Font-size: 16px
- Hover: opacity 0.7

### List Items (Features)

- Icon: Checkmark in circle
- Icon color: #FFFFFF on dark cards, #0F3D2F on light
- Text: 16px, line-height 1.6
- Spacing: 16px between items

## Layout Principles

- Max content width: 1280px
- Container padding: 24px (mobile), 48px (tablet), 64px (desktop)
- Centered layouts with generous whitespace
- Single-column on mobile, adaptive cards on larger screens
- Vertical rhythm maintained with 8px grid

**Responsive Behavior:**
- Cards stack vertically on mobile (<768px)
- Cards display in grid on tablet/desktop (2-3 columns)
- Hero text scales from 36px (mobile) to 56px (desktop)
- Buttons full-width on mobile, auto-width on desktop

**Alignment:**
- Headings: Center-aligned
- Card content: Center-aligned
- Body paragraphs: Center-aligned with max-width constraint
- CTA buttons: Center-aligned

## Visual Effects

**Border Radius:**
- Cards: 24px
- Buttons: 32px (pill shape)
- Badges: 16px
- Toggle containers: 24px
- Small elements: 8px

**Shadows:**
- Featured cards: 0 8px 32px rgba(0, 0, 0, 0.15)
- Standard cards: 0 4px 16px rgba(0, 0, 0, 0.08)
- Hover elevation: 0 12px 40px rgba(0, 0, 0, 0.2)
- Subtle elements: 0 2px 8px rgba(0, 0, 0, 0.05)

**Borders:**
- Thickness: 2px for card borders
- Color: #D4D4D4 for neutral borders
- Style: Solid

**Backgrounds:**
- Solid colors primarily
- Subtle texture possible on warm cream background
- No gradients in main interface

## Design Tone

This system conveys premium service quality through elegant serif typography, generous spacing, and a sophisticated color palette anchored by deep forest green. The warm neutral backgrounds create an approachable yet professional atmosphere, while the large serif headings and oversized pricing displays command attention without appearing aggressive. The design balances minimal aesthetics with clarity and hierarchy.

## Usage Notes for AI Implementation

When implementing this design system:

1. **Prioritize readability**: Use the large type scale and generous line-heights to ensure text is always comfortable to read
2. **Maintain hierarchy**: Serif headings should always be significantly larger than body text (3:1 ratio minimum)
3. **Color discipline**: Use deep forest green (#0F3D2F) exclusively for primary actions and featured content; avoid overuse
4. **Spacing consistency**: Apply the 8px grid rigorously—every margin and padding should be a multiple of 8
5. **Center-align strategically**: Centered layouts work for pricing and marketing content; consider left-alignment for dense information
6. **Mobile-first buttons**: Default to full-width pill buttons on small screens for easy tap targets
7. **Card elevation**: Featured/premium options should use darker backgrounds and stronger shadows to create clear visual hierarchy
8. **Warm neutrals**: The cream and light gray backgrounds (#F5F3EF, #E8E4DC) are essential to the premium feel—avoid pure white
