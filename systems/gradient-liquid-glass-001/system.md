---
id: gradient-liquid-glass-001
title: Aqua Glass System
description: A fluid, ethereal interface featuring soft gradient backgrounds with glassmorphic dark overlays and luminous accent elements.
tags: [gradient, dark-overlay, glassmorphism, onboarding, premium, fluid]
colors: ["#5BB8E0", "#3A9CC4", "#2D7A9E", "#1A1A1A", "#2D2D2D", "#FFFFFF"]
created: 2025-01-22
---

# Aqua Glass System

A serene, premium interface aesthetic that combines soft aquatic gradient backgrounds with dark glassmorphic content panels. The design evokes depth and fluidity through layered transparency effects, creating an immersive onboarding experience that feels both modern and calming.

## Color Palette

**Gradient Background Colors:**
- Sky Blue Light: #5BB8E0 — Upper gradient, creates airy openness
- Ocean Blue: #3A9CC4 — Mid gradient transition
- Deep Teal: #2D7A9E — Lower gradient anchor
- Seafoam Green: #4ABFAD — Accent gradient touches
- Warm Peach: #E8C9A0 — Subtle sunrise accent in imagery

**Surface Colors:**
- Panel Dark: #1A1A1A — Primary content panel background
- Panel Dark Elevated: #2D2D2D — Elevated elements, buttons
- Panel Dark Hover: #3A3A3A — Interactive hover states
- Frosted Glass: rgba(30, 30, 30, 0.85) — Glassmorphic overlays

**Text Colors:**
- Text Primary: #FFFFFF — Headlines, primary content
- Text Secondary: #A0A0A0 — Descriptions, supporting text
- Text Tertiary: #666666 — Disabled states, hints

**Accent Colors:**
- Link Blue: #007AFF — Interactive links, back buttons
- Active Indicator: #FFFFFF — Pagination dots active
- Inactive Indicator: #666666 — Pagination dots inactive
- Success Green: #32D74B — Confirmation states
- Warning Amber: #FFD60A — Attention states

## Typography

**Font Families:**
- Primary: SF Pro Display / -apple-system, BlinkMacSystemFont, "Segoe UI", system-ui
- Secondary: SF Pro Text (for body copy)
- Monospace: SF Mono (for technical content)

**Type Scale:**
- Display: 32px, 700 weight, 1.2 line-height — Welcome headlines
- Heading 1: 24px, 600 weight, 1.3 line-height — Section titles
- Heading 2: 20px, 600 weight, 1.35 line-height — Card titles
- Body Large: 17px, 400 weight, 1.5 line-height — Descriptions
- Body: 15px, 400 weight, 1.5 line-height — Standard text
- Caption: 13px, 400 weight, 1.4 line-height — Labels, hints
- Small: 11px, 500 weight, 1.3 line-height — Micro labels

**Hierarchy Rules:**
- Headlines use bold white for maximum contrast against dark panels
- Descriptions use lighter gray (#A0A0A0) for visual hierarchy
- Interactive text (links) use system blue (#007AFF)
- All text is left-aligned except pagination indicators which are centered

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96

**Common Patterns:**
- Content panel padding: 48px horizontal, 40px vertical
- Section spacing: 32px between major sections
- Element spacing: 16px between related items
- Button internal padding: 16px vertical, 32px horizontal
- Card padding: 24px all sides
- Pagination dot spacing: 8px between dots

**Layout Dimensions:**
- Content panel max-width: 1200px
- Content panel border-radius: 24px (large, rounded corners)
- Button border-radius: 24px (pill-shaped)
- Card border-radius: 16px
- Icon container border-radius: 12px

## Component Styles

### Buttons

**Primary Button (Dark):**
- Background: #2D2D2D
- Text: #FFFFFF, 17px, 500 weight
- Padding: 16px 32px
- Border-radius: 24px (full pill)
- Min-width: 120px
- Hover: Background #3A3A3A
- Active: Background #1A1A1A
- Shadow: none (flat design)

**Secondary Button (Outline):**
- Background: transparent
- Border: 1px solid #3A3A3A
- Text: #FFFFFF
- Same dimensions as primary

**Icon Button (Back):**
- Size: 48px × 48px
- Background: rgba(0, 0, 0, 0.3)
- Icon: #007AFF chevron
- Border-radius: 50%
- Hover: Background rgba(0, 0, 0, 0.5)

### Cards / Content Panels

**Main Content Panel:**
- Background: #1A1A1A
- Border-radius: 24px
- Padding: 48px
- Shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5)
- Backdrop-filter: blur(20px) — when over gradient

**Image Container:**
- Border-radius: 16px
- Overflow: hidden
- Shadow: 0 20px 40px rgba(0, 0, 0, 0.3)

### Pagination Indicators

**Dot Style:**
- Size: 8px × 8px
- Border-radius: 50%
- Active: #FFFFFF
- Inactive: #666666
- Spacing: 8px gap
- Centered horizontally

### App Icons (Dock Style)

**Icon Container:**
- Size: 64px × 64px (or 80px for large)
- Border-radius: 16px (iOS-style squircle approximation)
- Shadow: 0 4px 12px rgba(0, 0, 0, 0.15)
- Background: varies per app (gradients common)

**Dock Bar:**
- Background: rgba(200, 200, 200, 0.3)
- Backdrop-filter: blur(30px) saturate(180%)
- Border-radius: 20px
- Padding: 8px 16px
- Border: 1px solid rgba(255, 255, 255, 0.2)

## Layout Principles

- **Centered Composition:** Content panels are horizontally and vertically centered
- **Layered Depth:** Gradient background → glassmorphic elements → dark content panel → text/images
- **Generous Whitespace:** Large padding creates breathing room and premium feel
- **Visual Hierarchy:** Dark panels create focus areas against colorful backgrounds
- **Responsive Behavior:** Panels maintain aspect ratio, scale down proportionally on mobile
- **Full-bleed Backgrounds:** Gradients extend to viewport edges

## Visual Effects

**Border Radius:**
- Extra Large (panels): 24px
- Large (buttons, cards): 16-24px
- Medium (icons): 12-16px
- Small (inputs): 8px
- Circle (dots, avatars): 50%

**Shadows:**
- Panel Shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5)
- Card Shadow: 0 20px 40px rgba(0, 0, 0, 0.3)
- Icon Shadow: 0 4px 12px rgba(0, 0, 0, 0.15)
- No shadows on buttons (flat style)

**Backgrounds:**
- Primary: Linear gradient from #5BB8E0 (top) through #3A9CC4 to #2D7A9E (bottom)
- Can include subtle radial gradient overlays for depth
- Gradient angle: 180deg (top to bottom) or slight diagonal

**Glassmorphism:**
- Backdrop-filter: blur(20px) saturate(150%)
- Background: rgba(30, 30, 30, 0.85)
- Border: 1px solid rgba(255, 255, 255, 0.1)

**Transitions:**
- Duration: 200ms for hover states
- Easing: ease-out
- Properties: background-color, transform, opacity

## Design Tone

This system embodies a premium, futuristic calm. The fluid gradients suggest depth and movement like looking through water, while the dark content panels provide grounded focus areas. The aesthetic is sophisticated yet approachable, using soft curves and generous spacing to create an experience that feels both high-end and welcoming. It's particularly suited for onboarding flows, welcome screens, and immersive product experiences.

## Usage Notes for AI Implementation

1. **Background First:** Always establish the gradient background before adding content layers
2. **Dark Panel Focus:** Use #1A1A1A panels for any content that needs clear readability
3. **Generous Spacing:** When in doubt, add more padding — this system breathes
4. **Pill Buttons:** All buttons should be fully rounded (border-radius equal to half height)
5. **System Fonts:** Prefer system font stack for authentic feel, or use Inter as web alternative
6. **Centered Layouts:** Default to centered compositions with max-width constraints
7. **Subtle Animations:** Add gentle transitions on hover/focus for polish
8. **Image Treatment:** Device mockups and imagery should have subtle shadows and rounded corners
9. **Accessibility:** Maintain WCAG AA contrast — white text on #1A1A1A meets requirements
10. **Mobile Adaptation:** Stack elements vertically, reduce padding slightly, maintain border radii
