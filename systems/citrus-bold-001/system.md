---
id: citrus-bold-001
title: Citrus Pop System
description: A vibrant, playful design system featuring bold electric blue backgrounds with sunny yellow accents and energetic green highlights
tags: [light, colorful, playful, bold, startup]
colors: ["#3B6BF5", "#FFD93D", "#3DEB64", "#FFFFFF", "#1A1A1A"]
created: 2025-12-18
---

# Citrus Pop System

A high-energy, approachable design system built around a vibrant electric blue canvas with sunny citrus accents. The aesthetic is playful yet professional, designed to feel welcoming and accessible while maintaining visual impact. Perfect for platforms targeting non-technical users or those wanting to convey friendliness and ease-of-use.

## Color Palette

**Primary Colors:**
- Electric Blue: #3B6BF5 — Primary background, creates energetic foundation
- Citrus Yellow: #FFD93D — Primary accent, CTAs, brand elements, icons

**Secondary Colors:**
- Lime Green: #3DEB64 — Highlight text, emphasis, success states
- Soft Khaki: #C4B896 — Secondary text, muted headlines

**Neutral Colors:**
- Pure White: #FFFFFF — Button backgrounds, card surfaces, body text
- Charcoal Black: #1A1A1A — Button text, strong contrast elements
- Slate Shadow: #2D3A5C — Drop shadows, depth effects

**State Colors:**
- Success: #3DEB64 (Lime Green)
- Warning: #FFD93D (Citrus Yellow)
- Error: #FF5C5C (estimated complement)
- Info: #3B6BF5 (Electric Blue)

## Typography

**Font Families:**
- Primary Headlines: Heavy condensed sans-serif (appears to be Impact/Bebas Neue style or custom display font)
- Body Text: Clean geometric sans-serif (Inter, Poppins, or similar)
- UI Elements: Same as body, medium weight

**Type Scale:**
- Hero Headline: ~80-100px, Black/Heavy weight, tight line-height (0.95), all-caps
- Section Label: ~18px, Bold weight, uppercase, letter-spacing 0.1em
- Body Large: ~18px, Regular weight, line-height 1.5
- Button Text: ~16px, Semi-bold weight

**Hierarchy Rules:**
- Headlines use condensed, heavy display type with strong vertical rhythm
- Color differentiation for emphasis (khaki for setup text, green for key terms)
- Body text is clean and readable with comfortable spacing
- All-caps used sparingly for labels and hero text

## Spacing System

**Base Unit:** 8px
**Scale:** 8, 16, 24, 32, 48, 64, 80, 120

**Common Patterns:**
- Hero section padding: ~80-120px vertical
- Button padding: 16px vertical, 32px horizontal
- Text block spacing: 16-24px between paragraphs
- Icon to text gap: 12-16px
- Section margins: 64-80px

## Component Styles

### Buttons

**Primary Button (CTA):**
- Background: #FFD93D (Citrus Yellow)
- Text: #1A1A1A (Charcoal Black)
- Border-radius: 50px (fully rounded pill)
- Padding: 16px 32px
- Font-size: 16px
- Font-weight: 600
- Shadow: 0 4px 12px rgba(0,0,0,0.15)
- Icon: Inline emoji/icon with 8px gap

**Hover State:**
- Background: #FFE566 (lighter yellow)
- Transform: translateY(-2px)
- Shadow: 0 6px 16px rgba(0,0,0,0.2)

### Cards

**Standard Card:**
- Background: #FFFFFF
- Border-radius: 16px
- Padding: 32px
- Shadow: 0 8px 32px rgba(45, 58, 92, 0.15)

### Icons/Brand Elements

**Circular Icon Badge:**
- Size: Large, ~200-300px for hero
- Background: #FFD93D with darker outline
- Inner elements: White fills with black outlines
- Shadow: 8px 8px 0 rgba(45, 58, 92, 0.3) (offset shadow style)
- Style: 3D-ish with depth shadow, playful illustration style

## Layout Principles

- **Max content width:** ~1200px
- **Grid structure:** Flexible, asymmetric hero layouts
- **Alignment:** Left-aligned text with centered CTAs
- **Hero pattern:** Large illustrative element left, text stack right
- **Responsive behavior:** Stack vertically on mobile, scale illustrations

## Visual Effects

**Border Radius:**
- Buttons: 50px (full pill)
- Cards: 16px
- Icons/badges: Full circle or custom shapes
- Small elements: 8px

**Shadows:**
- Hero icons: Offset shadow (x:8px y:8px) with semi-transparent dark
- Buttons: Soft diffused shadow (0 4px 12px)
- Cards: Medium elevation (0 8px 32px)

**Borders:**
- Icon elements: 3px black outlines for illustration style
- Minimal use elsewhere

**Backgrounds:**
- Solid, flat color fields
- No gradients in main design
- High contrast color blocking

## Design Tone

This system radiates approachability and energy. The combination of electric blue with citrus yellow creates a sunny, optimistic feeling that suggests "easy" and "fun" rather than complex or intimidating. The playful illustrated icon and punchy typography make technical concepts feel accessible to non-technical users. It's startup-friendly, modern, and distinctly memorable without being childish.

## Usage Notes for AI Implementation

**When to use this system:**
- Platforms targeting non-technical users
- Onboarding flows and getting-started experiences
- Products emphasizing ease-of-use and accessibility
- Startup landing pages wanting high energy
- AI/automation tools wanting to feel friendly

**Key implementation notes:**
1. The electric blue background is the hero—use it boldly for main sections
2. Yellow should be reserved primarily for CTAs and brand accent moments
3. Green highlights work for emphasizing key terms within headlines
4. Keep body text white on blue backgrounds for readability
5. The illustrated icon style (outlined, slightly 3D) is core to the personality
6. Don't overuse the bold condensed type—save it for hero moments
7. Maintain generous whitespace to let the colors breathe
8. Pill-shaped buttons are essential to the friendly aesthetic

**Color accessibility:**
- White text on #3B6BF5 passes WCAG AA
- Black text on #FFD93D passes WCAG AAA
- Green (#3DEB64) on blue may need slight adjustment for accessibility
