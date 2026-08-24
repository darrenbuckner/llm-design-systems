---
id: gradient-advisory-001
title: Horizon Advisory System
description: Bold gradient typography with mint accents for professional community platforms
tags: [light, bold, gradient, professional, modern]
colors: ["#1E3A8A", "#8B5CF6", "#A78BFA", "#6EE7B7", "#FFFFFF", "#0F172A"]
created: 2025-12-20
---

# Horizon Advisory System

A confident, professional design system featuring bold gradient typography and fresh mint accents. Built for advisory platforms, mentorship communities, and professional networks where credibility meets modern energy.

## Color Palette

**Primary Colors:**
- Navy Primary: #1E3A8A — Primary headings, key text, trust-building elements
- Royal Blue: #2563EB — Secondary text, links, interactive states
- Violet: #8B5CF6 — Gradient midpoint, accent highlights
- Lavender: #A78BFA — Gradient endpoint, hover states

**Accent Colors:**
- Mint Green: #6EE7B7 — Background accents, success states, fresh energy
- Seafoam: #A7F3D0 — Lighter mint for backgrounds, cards

**Neutral Colors:**
- Background: #FFFFFF — Clean white base
- Surface Light: #F8FAFC — Card backgrounds, sections
- Text Primary: #0F172A — Body text, maximum contrast
- Text Secondary: #64748B — Captions, metadata, supporting text
- Border Light: #E2E8F0 — Subtle dividers, card borders

**Gradient Definitions:**
- Hero Gradient: linear-gradient(135deg, #1E3A8A 0%, #2563EB 25%, #8B5CF6 60%, #A78BFA 100%)
- Accent Gradient: linear-gradient(90deg, #6EE7B7 0%, #A7F3D0 100%)

## Typography

**Font Families:**
- Primary Display: Inter or SF Pro Display — Bold weights for headlines
- Secondary Display: A condensed sans-serif like Barlow Condensed or Inter Tight — For "BOARD" style text
- Body: Inter, system-ui — Clean readable body text

**Type Scale:**
- Display XL: 72px, 800 weight, -0.02em tracking, 0.9 line-height
- Display: 56px, 800 weight, -0.02em tracking, 1.0 line-height
- Heading 1: 48px, 700 weight, -0.01em tracking, 1.1 line-height
- Heading 2: 36px, 700 weight, 0 tracking, 1.2 line-height
- Heading 3: 24px, 600 weight, 0 tracking, 1.3 line-height
- Body Large: 18px, 400 weight, 0.01em tracking, 1.6 line-height
- Body: 16px, 400 weight, 0 tracking, 1.5 line-height
- Caption: 14px, 500 weight, 0.02em tracking, 1.4 line-height
- Label: 12px, 600 weight, 0.05em tracking, 1.3 line-height (uppercase)

**Hierarchy Rules:**
- Display text uses gradient fill for maximum impact
- Secondary display uses solid navy, condensed weight, often uppercase
- Strong contrast between display and body creates clear hierarchy
- Letter-spacing tightens as size increases

## Spacing System

**Base Unit:** 4px

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 96, 128

**Common Patterns:**
- Component internal padding: 16px - 24px
- Section vertical spacing: 64px - 96px
- Grid gaps: 24px - 32px
- Card padding: 24px - 32px
- Button padding: 12px 24px (small), 16px 32px (large)

## Component Styles

### Buttons

**Primary Button:**
```css
background: linear-gradient(135deg, #1E3A8A 0%, #8B5CF6 100%);
color: #FFFFFF;
padding: 14px 28px;
border-radius: 8px;
font-weight: 600;
font-size: 16px;
border: none;
box-shadow: 0 4px 14px rgba(139, 92, 246, 0.25);
transition: transform 0.2s, box-shadow 0.2s;
```

**Primary Hover:**
```css
transform: translateY(-2px);
box-shadow: 0 6px 20px rgba(139, 92, 246, 0.35);
```

**Secondary Button:**
```css
background: transparent;
color: #1E3A8A;
padding: 14px 28px;
border-radius: 8px;
font-weight: 600;
border: 2px solid #1E3A8A;
```

**Mint Accent Button:**
```css
background: #6EE7B7;
color: #0F172A;
padding: 14px 28px;
border-radius: 8px;
font-weight: 600;
border: none;
```

### Cards

**Profile Card:**
```css
background: #FFFFFF;
border-radius: 16px;
overflow: hidden;
box-shadow: 0 4px 20px rgba(0, 0, 0, 0.08);
border: 1px solid #E2E8F0;
```

**Feature Card:**
```css
background: linear-gradient(180deg, #F8FAFC 0%, #FFFFFF 100%);
border-radius: 12px;
padding: 32px;
border: 1px solid #E2E8F0;
```

**Mint Accent Card:**
```css
background: linear-gradient(135deg, #A7F3D0 0%, #6EE7B7 100%);
border-radius: 16px;
padding: 32px;
color: #0F172A;
```

### Input Fields

**Text Input:**
```css
background: #FFFFFF;
border: 2px solid #E2E8F0;
border-radius: 8px;
padding: 14px 16px;
font-size: 16px;
color: #0F172A;
transition: border-color 0.2s;
```

**Focus State:**
```css
border-color: #8B5CF6;
outline: none;
box-shadow: 0 0 0 3px rgba(139, 92, 246, 0.1);
```

### Tags/Badges

**Role Badge:**
```css
background: linear-gradient(135deg, #1E3A8A 0%, #8B5CF6 100%);
color: #FFFFFF;
padding: 6px 14px;
border-radius: 20px;
font-size: 12px;
font-weight: 600;
text-transform: uppercase;
letter-spacing: 0.05em;
```

**Mint Badge:**
```css
background: #6EE7B7;
color: #0F172A;
padding: 6px 14px;
border-radius: 20px;
font-size: 12px;
font-weight: 600;
```

## Layout Principles

- **Max content width:** 1280px
- **Grid structure:** 12-column grid, 24px gutters
- **Photo grids:** 2x2 or flexible grid with square/portrait aspect ratios
- **Responsive behavior:** Stack to single column below 768px
- **Alignment:** Left-aligned text with occasional centered hero sections
- **Asymmetry:** Text overlays on image grids create dynamic tension

## Visual Effects

**Border Radius:**
- Small elements (buttons, inputs): 8px
- Medium elements (cards): 12px - 16px
- Large elements (hero sections): 24px
- Badges/pills: 20px (fully rounded)

**Shadows:**
- Subtle: 0 2px 8px rgba(0, 0, 0, 0.04)
- Card: 0 4px 20px rgba(0, 0, 0, 0.08)
- Elevated: 0 8px 30px rgba(0, 0, 0, 0.12)
- Gradient glow: 0 4px 14px rgba(139, 92, 246, 0.25)

**Borders:**
- Default: 1px solid #E2E8F0
- Focus: 2px solid #8B5CF6
- Emphasis: 2px solid #1E3A8A

**Backgrounds:**
- White base for maximum contrast
- Mint accent blocks for section breaks
- Subtle gradients for depth

## Design Tone

Bold, confident, and approachable. This system projects expertise and credibility through strong typography while remaining fresh and modern with mint accents. The gradient treatment adds energy and contemporary flair without sacrificing professionalism. Perfect for platforms where trust and authority matter, but shouldn't feel stuffy or corporate.

## Usage Notes for AI Implementation

1. **Gradient Text:** Apply the hero gradient to large display text only. Use `-webkit-background-clip: text` with `color: transparent` for the gradient fill effect. Always ensure fallback solid color.

2. **Photo Grids:** Overlap text on photo grids for visual interest. Use semi-transparent overlays or strategic placement to maintain readability.

3. **Mint Accents:** Use mint sparingly as an accent—for section backgrounds, success states, or call-to-action highlights. It provides fresh contrast against the navy-violet palette.

4. **Typography Contrast:** Create strong hierarchy by pairing extra-bold condensed uppercase text with regular-weight body copy. The contrast drives visual interest.

5. **White Space:** Let the bold typography breathe. Generous margins (64-96px between sections) prevent the design from feeling heavy.

6. **Interactive States:** Use subtle lift (translateY) and enhanced shadows on hover. The gradient glow effect on buttons reinforces the color system.
