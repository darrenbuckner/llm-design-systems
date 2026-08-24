---
id: warm-social-001
title: Nordic Social Design System
description: Warm, inviting design system with beige surfaces, bold typography, and social media-inspired card layouts
tags: light, warm, social, modern, playful
colors: #1C1C1C, #E8DCC8, #FFFFFF, #F0E5D4, #FFD166
created: 2025-12-08
---

# Nordic Social Design System

A warm, approachable design system featuring high-contrast typography on dark surfaces, complemented by soft beige content areas and social media-inspired card layouts. The system balances bold messaging with inviting warmth through its color palette and generous spacing.

## Color Palette

**Primary Colors:**
- Deep Charcoal: #1C1C1C — Primary headers, navigation bars, high-impact text areas
- Warm Beige: #E8DCC8 — Main content backgrounds, card surfaces, secondary sections

**Accent Colors:**
- Bright Yellow: #FFD166 — Call-to-action elements, decorative accents, interactive highlights
- Soft Cream: #F0E5D4 — Subtle backgrounds, hover states, light variations

**Neutral Colors:**
- Pure White: #FFFFFF — Card backgrounds, text on dark surfaces, clean contrast elements
- Medium Gray: #666666 — Secondary text, captions, metadata
- Light Gray: #E0E0E0 — Borders, dividers, subtle separators

**Semantic Colors:**
- Information Blue: #4A90E2 — Links, social media indicators
- Success Green: #7CB342 — Confirmations, positive states
- Black: #000000 — Body text on light surfaces, maximum contrast elements

## Typography

**Font Families:**
- Primary Display: Sans-serif, likely custom or system font with strong geometric qualities
- Body Text: System sans-serif stack (similar to -apple-system, BlinkMacSystemFont)

**Type Scale:**
- Hero Display: 72px, weight 700-900, line-height 1.0, ultra-bold presence
- Section Heading: 32px, weight 600-700, line-height 1.2
- Card Title: 20px, weight 600, line-height 1.3
- Body Text: 16px, weight 400, line-height 1.5
- Caption/Metadata: 14px, weight 400, line-height 1.4
- Small Label: 12px, weight 500, line-height 1.3

**Hierarchy Rules:**
- Headers use maximum contrast with dark backgrounds (white on deep charcoal)
- Display text employs extreme weights (800-900) for bold personality
- Body content maintains comfortable reading with standard weights
- Uppercase is avoided except for small labels and tags
- Letter-spacing is tight on large headings (-0.02em) for impact

## Spacing System

**Base Unit:** 8px
**Scale:** 8, 16, 24, 32, 40, 48, 56, 64, 80

**Common Patterns:**
- Card padding: 24px on mobile, 32px on larger screens
- Section vertical spacing: 64px between major sections
- Content margins: 16-24px for comfortable flow
- Header padding: 24px vertical, 16px horizontal
- Inter-card gaps: 16px in grids
- Icon-to-text spacing: 12px
- Button padding: 16px vertical, 32px horizontal

## Component Styles

### Header Bar
- Background: #1C1C1C (deep charcoal)
- Height: 80px minimum
- Content: Left-aligned oversized text with accent dot
- Icon: Right-aligned notification bell in white
- Accent element: Circular yellow dot with centered asterisk
- Typography: Extra-bold sans-serif, white text

### Content Section Headers
- Background: Warm beige (#E8DCC8)
- Centered alignment for primary content
- Title: 32px bold, black text
- Subtitle: 16px regular, dark gray
- Navigation arrows: Simple chevrons, 24px, positioned symmetrically
- Padding: 48px vertical, 24px horizontal
- Information icon: Circular, outlined, right-aligned

### Social Cards
- Background: White (#FFFFFF)
- Border-radius: 24px (highly rounded corners)
- Padding: 24px
- Shadow: Subtle, 0 4px 12px rgba(0, 0, 0, 0.08)
- Header section: Instagram icon + username + location in horizontal layout
- Image area: Full-width, 16:10 aspect ratio approximately
- Footer: Product count badge (pill-shaped, right-aligned)
- Product thumbnails: Circular, 48px diameter, grouped horizontally
- Spacing between elements: 16px

### Navigation Arrows
- Style: Simple chevrons (< >)
- Size: 32px height
- Color: Black (#000000)
- Background: None (transparent)
- Spacing: Centered with generous padding between

### Product Badge
- Shape: Pill (fully rounded ends)
- Background: Translucent or solid depending on context
- Text: "X products" with product icon
- Padding: 12px vertical, 20px horizontal
- Typography: 14px medium weight
- Border: Optional 1px subtle border

### Buttons (Circular/Pill)
- Border-radius: 50% for circular icons, 24px for pills
- Sizes: 48px circular for icons, variable width for text buttons
- Primary style: Black background, white text
- Secondary style: White background, black text
- Padding: 16px vertical, 24px horizontal for text buttons
- Hover state: Slight scale (1.05) or background darkening

## Layout Principles

- Max content width: 1200px for main content areas
- Grid structure: Horizontal scrollable carousel for cards
- Card width: 480-520px on desktop, full-width minus margins on mobile
- Alignment: Center-aligned headers, left-aligned card content
- Responsive behavior: Stacks vertically on mobile, maintains horizontal scroll on desktop
- Header: Fixed or sticky behavior likely
- Whitespace: Generous vertical spacing (64-80px) between sections

## Visual Effects

- **Border Radius:** 
  - Cards: 24px (highly rounded, friendly)
  - Buttons/Pills: 24-48px (fully rounded ends)
  - Product thumbnails: 50% (perfect circles)
  - Icons: 50% (circular containers)

- **Shadows:**
  - Cards: 0 4px 12px rgba(0, 0, 0, 0.08) — subtle elevation
  - Hover cards: 0 8px 24px rgba(0, 0, 0, 0.12) — increased depth
  - Minimal shadow usage overall, relies on color contrast

- **Borders:**
  - Generally avoided in favor of shadow and color separation
  - When used: 1px, subtle gray (#E0E0E0)
  - Product thumbnails may have 2px white borders for separation

- **Backgrounds:**
  - Solid colors dominate
  - Two-tone split: dark header, warm beige content
  - White cards create strong contrast against beige
  - No gradients or complex patterns visible

## Design Tone

This system projects warmth and approachability through its soft beige palette while maintaining confidence with bold, oversized typography on dark surfaces. The social media-inspired card layouts with generous rounding and clean photography create an inviting, contemporary feel. The design balances playful personality (the yellow accent dot, friendly greetings) with sophisticated simplicity, making it feel both accessible and premium. The high contrast between dark headers and warm content areas creates clear visual hierarchy while the Instagram-style cards add social proof and community connection.

## Usage Notes for AI Implementation

**Color Discipline:**
- Use #1C1C1C exclusively for high-impact header areas and maximum-contrast moments
- Default to #E8DCC8 for main content backgrounds to maintain warmth
- Reserve #FFD166 yellow for singular accent elements (1-2 per screen maximum)
- White cards on beige backgrounds create the primary content structure

**Typography Hierarchy:**
- Hero text should be extremely bold (800-900 weight) and large (60-80px)
- Maintain tight letter-spacing on large headings for impact
- Use standard weights (400-600) for all body content
- Keep card titles at 20px for consistency

**Component Assembly:**
- Cards must have 24px border-radius for the friendly, modern aesthetic
- Maintain 16px spacing in card grids
- Product thumbnails are always circular (50% border-radius)
- Social attribution (Instagram icon + username) is a consistent header pattern

**Spacing Rhythm:**
- Use 8px base unit consistently
- Major sections: 64px vertical spacing
- Card padding: 24-32px internal
- Maintain generous whitespace around centered headers

**Interactive Elements:**
- Circular icon buttons at 48px diameter
- Pill-shaped badges with 24px border-radius
- Subtle hover states (don't over-animate)
- Tag/price indicators should be small and unobtrusive

**Mobile Considerations:**
- Cards remain wide, encourage horizontal scrolling
- Reduce header text size to 48-56px on small screens
- Maintain card border-radius at full 24px even on mobile
- Stack navigation arrows vertically if needed
