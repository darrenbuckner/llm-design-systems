---
id: light-celebration-001
title: Meadow Celebration System
description: A playful, organic design system featuring soft greens, coral accents, and flowing abstract shapes for celebratory content
tags: [light, colorful, playful, organic, celebration, cards]
colors: ["#8BC78B", "#4A90D9", "#F5B8A8", "#D6E4F0", "#FF8A70", "#1A1A1A"]
created: 2024-12-17
---

# Meadow Celebration System

A vibrant, approachable design system built around organic flowing shapes and a fresh spring palette. The aesthetic combines soft pastel backgrounds with bold accent colors, creating celebratory moments that feel warm and personal. Abstract curved forms create visual interest while maintaining a friendly, non-corporate tone.

## Color Palette

**Primary Colors:**
- Meadow Green: #8BC78B — Primary background, establishes fresh, optimistic tone
- Ocean Blue: #4A90D9 — Accent shapes, creates visual depth and movement

**Secondary Colors:**
- Soft Coral: #F5B8A8 — Secondary accent shapes, adds warmth
- Pale Sky: #D6E4F0 — Card backgrounds, neutral surface for content

**Accent Colors:**
- Sunset Coral: #FF8A70 — Bottom accent bar, draws attention
- Deep Charcoal: #1A1A1A — Text, buttons, icons

**Neutral Colors:**
- Pure White: #FFFFFF — Card surface, text contrast
- Soft Gray: #F5F5F5 — Subtle backgrounds
- Medium Gray: #666666 — Secondary text

## Typography

**Font Families:**
- Primary: System Sans-Serif (SF Pro Display / -apple-system / Segoe UI)
- The design uses native system fonts for optimal rendering

**Type Scale:**
- Display Name: 36px, Bold (700), 1.1 line-height — Featured person/item names
- Supporting Text: 16px, Regular (400), 1.4 line-height — Descriptive captions
- Button Text: 15px, Semi-bold (600), 1.0 line-height — Action buttons

**Hierarchy Rules:**
- Names use bold weight with tight line-height for impact
- Supporting text uses regular weight with comfortable reading line-height
- Multi-line names stack naturally without additional spacing
- High contrast (dark text on light card) ensures readability

## Spacing System

**Base Unit:** 8px
**Scale:** 8, 16, 24, 32, 48, 64

**Common Patterns:**
- Card padding: 24px internal padding
- Avatar offset: Positioned asymmetrically within flowing shapes
- Text block margin: 24px from card edges
- Button spacing: 16px gap between buttons
- Section margins: 48px above/below card

## Component Styles

### Celebration Cards
- Background: #FFFFFF with subtle shadow
- Border radius: 16px (rounded, friendly)
- Internal layout: Asymmetric, organic placement
- Bottom accent: 8px solid color bar (#FF8A70)
- Shadow: 0 4px 24px rgba(0,0,0,0.1)

### Avatar Circles
- Shape: Perfect circle
- Border: 4px solid #FFFFFF (creates separation from shapes)
- Size: Large (120px) and Medium (80px) variants
- Placement: Overlapping abstract shapes
- Shadow: 0 2px 8px rgba(0,0,0,0.15)

### Abstract Shape Elements
- Style: Organic, flowing curves
- Colors: Blue (#4A90D9) and Coral (#F5B8A8)
- Opacity: 100% (solid fills)
- Pattern: Interlocking curves creating visual rhythm
- Coverage: ~60% of card background

### Action Buttons
- **Primary Button:**
  - Background: #1A1A1A (charcoal)
  - Text: #FFFFFF
  - Border radius: 24px (pill shape)
  - Padding: 14px 24px
  - Icon: Left-aligned with 8px gap

- **Secondary Button:**
  - Background: #FFFFFF
  - Border: 1.5px solid #1A1A1A
  - Text: #1A1A1A
  - Border radius: 24px (pill shape)
  - Padding: 14px 24px
  - Icon: Left-aligned with 8px gap

### Progress Indicators
- Style: Segmented horizontal bar
- Active segment: #1A1A1A (solid)
- Inactive segment: #1A1A1A at 30% opacity
- Height: 3px
- Gap between segments: 8px
- Border radius: 2px per segment

## Layout Principles

- **Card-centric:** Content lives within rounded card containers
- **Full-bleed background:** Vibrant color extends edge-to-edge
- **Asymmetric balance:** Elements placed off-center for organic feel
- **Layered depth:** Shapes overlap to create visual interest
- **Bottom-anchored actions:** Buttons fixed at screen bottom

## Visual Effects

**Border Radius:**
- Cards: 16px
- Buttons: 24px (full pill)
- Avatars: 50% (perfect circle)
- Progress segments: 2px

**Shadows:**
- Card shadow: 0 4px 24px rgba(0,0,0,0.1)
- Avatar shadow: 0 2px 8px rgba(0,0,0,0.15)
- Button hover: 0 2px 12px rgba(0,0,0,0.12)

**Borders:**
- Avatar border: 4px solid white
- Secondary button: 1.5px solid charcoal
- Bottom accent bar: 8px solid coral

**Backgrounds:**
- Page: Solid meadow green (#8BC78B)
- Card: White with abstract shape overlay
- Shapes: Solid blue and coral fills

## Design Tone

This system radiates warmth and celebration through its combination of natural greens, playful coral accents, and organic flowing shapes. The aesthetic feels personal and human rather than corporate—like a hand-crafted greeting card brought to digital life. The bold typography and high-contrast buttons ensure clarity while the soft, rounded forms maintain approachability.

## Usage Notes for AI Implementation

**When to use this system:**
- Year-in-review or milestone celebrations
- User achievement showcases
- Relationship/connection highlights
- Personalized content cards
- Social sharing moments

**Key implementation details:**
- Abstract shapes should be SVG for crisp rendering at any size
- Maintain the organic, asymmetric placement—avoid grid rigidity
- The bottom coral bar is signature—include it on celebratory cards
- Avatar images should be high-quality; the circular crop draws attention
- Green background creates strong brand recognition—use consistently

**Color application rules:**
- Meadow green for full-bleed backgrounds only
- Blue shapes should be larger, coral shapes smaller
- White cards provide breathing room from vibrant background
- Charcoal for all text and primary actions

**Responsive considerations:**
- Cards should maintain aspect ratio on resize
- Abstract shapes can simplify on smaller screens
- Button row should stack vertically on narrow viewports
- Avatar sizes can scale down proportionally
