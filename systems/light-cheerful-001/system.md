---
id: light-cheerful-001
title: Sky Blue Cheerful System
description: A playful, friendly design system with bright colors and rounded elements for wellness apps
tags: light, colorful, playful, friendly, rounded
colors: #5DBAEB, #FFFFFF, #4A9CC9, #FFB84D, #FF8C5A
created: 2025-01-05
---

# Sky Blue Cheerful System

A vibrant, welcoming design system built around bright sky blue and playful rounded elements. Perfect for wellness, self-care, and lifestyle applications targeting a friendly, approachable aesthetic with warm illustrated accents.

## Color Palette

**Primary Colors:**
- Primary Blue: #5DBAEB — Main background, primary brand color, creates cheerful sky-like atmosphere
- Deep Blue: #4A9CC9 — Text outlines, shadows, depth elements
- Pure White: #FFFFFF — Text, buttons, card backgrounds, high contrast elements

**Accent Colors:**
- Warm Yellow: #FFD966 — Illustrations, accents, cheerful highlights
- Soft Orange: #FFB84D — Secondary illustrations, warm accents
- Coral Orange: #FF8C5A — Tertiary illustrations, vibrant accents
- Mint Green: #7FD8BE — Illustration details, success states
- Soft Pink: #FFB8D1 — Illustration accents, decorative elements

**Neutral Colors:**
- Cream: #FFF9E6 — Subtle backgrounds, warm neutral
- Light Peach: #FFE5CC — Warm surface backgrounds
- Black: #000000 — App Store button backgrounds, high contrast elements

**Semantic Colors:**
- Star Yellow: #FFD700 — Ratings, favorites, positive feedback
- Success Green: #7FD8BE — Completion states, positive actions

## Typography

**Font Families:**
- Primary: Rounded bold sans-serif (similar to Fredoka One, Nunito Black, or Baloo)
- Secondary: Clean rounded sans-serif (similar to Nunito, Quicksand, or Poppins)

**Type Scale:**
- Hero Display: 56-72px, 800-900 weight, 1.1 line-height — Large hero statements with thick white outlines
- Display: 48px, 800 weight, 1.2 line-height — Major headings
- Heading 1: 32px, 700 weight, 1.3 line-height — Section headers
- Heading 2: 24px, 700 weight, 1.3 line-height — Component titles
- Body Large: 18px, 600 weight, 1.5 line-height — Primary content
- Body: 16px, 500 weight, 1.6 line-height — Standard text
- Caption: 14px, 600 weight, 1.4 line-height — Ratings, metadata

**Hierarchy Rules:**
- Hero text uses thick white stroke outlines (4-6px) with blue fill for maximum playfulness
- All headings use rounded, friendly font weights (700-900)
- Body text maintains medium weights for readability with softness
- Letter spacing slightly looser (+0.02em) for friendly feel

## Spacing System

**Base Unit:** 8px
**Scale:** 8, 16, 24, 32, 40, 48, 64, 80, 96

**Common Patterns:**
- Hero section padding: 64-96px vertical
- Content sections: 48-64px vertical spacing
- Component padding: 24-32px
- Button padding: 16px horizontal, 12px vertical
- Card padding: 24-32px
- Icon spacing: 16-24px from text

## Component Styles

### Buttons

**Primary Button (App Store):**
- Background: #000000
- Text: #FFFFFF
- Font: 18-20px, 600 weight
- Padding: 16px 32px
- Border radius: 12-16px (heavily rounded)
- Shadow: 0 4px 12px rgba(0,0,0,0.15)
- Hover: Slight scale (1.02) or subtle opacity change

**Secondary Button:**
- Background: #FFFFFF
- Text: #4A9CC9
- Border: 3px solid #4A9CC9
- Padding: 12px 28px
- Border radius: 24px (pill-shaped)
- Font: 16px, 700 weight

### Rating Display

- Large number: 48px, 800 weight, #4A9CC9
- Star icons: 32px, #FFD700 with slight shadow
- Caption text: 16px, 600 weight, #4A9CC9
- Alignment: Left-aligned number with right-aligned stars

### Logo Style

- Rounded rectangular container with soft edges
- Simple, friendly character illustration
- High contrast (light character on white background)
- 60-80px height for header logos

### Illustrations

- Soft, rounded organic shapes
- Layered overlapping elements (hills, characters)
- Warm gradient transitions (yellow → orange → green)
- Characters with simple geometric features
- Thick black outlines (3-4px) on character details
- Soft shadows and highlights for depth

## Layout Principles

- **Max content width:** 1200px for text content, full-bleed for backgrounds
- **Vertical rhythm:** Generous spacing (64-96px) between major sections
- **Alignment:** Centered content for hero sections, mixed alignment for variety
- **Illustration integration:** Large bottom illustrations (40-50% viewport height)
- **Whitespace:** Ample breathing room around all elements
- **Z-axis layering:** Illustrations layer over gradient backgrounds

## Visual Effects

- **Border Radius:** 
  - Small elements: 12-16px
  - Buttons: 12-20px
  - Cards/containers: 20-32px
  - Pills: 24-48px (full rounds)
  
- **Shadows:**
  - Subtle: 0 2px 8px rgba(0,0,0,0.08)
  - Medium: 0 4px 12px rgba(0,0,0,0.12)
  - Button: 0 4px 16px rgba(0,0,0,0.15)
  
- **Text Effects:**
  - Hero text: 4-6px white stroke outline
  - Slight text shadows on light backgrounds: 0 2px 4px rgba(0,0,0,0.1)
  
- **Backgrounds:**
  - Sky gradient: Solid #5DBAEB to lighter blue at horizon
  - Bottom gradient: Warm multi-color (yellow → orange → green → blue)
  - Smooth transitions between color zones

## Design Tone

Playful and nurturing with maximum approachability. The design radiates warmth and friendliness through bright sky blues, chunky rounded typography, and adorable illustrated characters. The thick outlined hero text and soft gradients create an inviting, stress-free environment perfect for wellness and self-care applications. Every element feels huggable and encouraging.

## Usage Notes for AI Implementation

**For Hero Sections:**
- Always use bright #5DBAEB backgrounds for primary hero areas
- Apply thick white text outlines (text-stroke CSS) to large display text
- Center-align hero content with generous vertical padding (80-120px)

**For Buttons:**
- Default to heavily rounded corners (16px minimum)
- Use high contrast (black with white text) for primary CTAs
- Include subtle hover animations (scale or lift effects)

**For Illustrations:**
- Place at bottom of sections with organic, flowing shapes
- Use warm gradient transitions (yellows, oranges, greens)
- Layer multiple colored shapes for depth
- Add soft character illustrations with simple, friendly features

**For Typography:**
- Load rounded sans-serif fonts (Nunito, Quicksand, or Poppins as fallbacks)
- Use heavy weights (700-900) for all headings
- Maintain loose letter spacing for friendliness
- Apply white outlines to hero text for playful emphasis

**Mobile Considerations:**
- Reduce hero text outlines to 3-4px on small screens
- Stack rating displays vertically below 600px
- Maintain generous padding (24-32px) on mobile
- Scale illustrations proportionally (30-40% viewport height)

**Color Usage:**
- Use primary blue (#5DBAEB) for 60-70% of interface
- White for content areas and high contrast elements
- Warm accents (yellow, orange) sparingly for highlights
- Never use dark backgrounds except for specific button types
