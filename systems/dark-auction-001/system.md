---
id: dark-auction-001
title: Cinder Auction System
description: Dark-themed auction marketplace with vibrant orange CTAs and playful illustrations
tags: dark, auction, vibrant-accents, playful
colors: #1C1E21, #2A2D31, #FF6B35, #FFFFFF, #9CA3AF
created: 2026-01-08
---

# Cinder Auction System

A dark-themed auction marketplace design system featuring high contrast with vibrant orange call-to-action elements, clean card-based layouts, and playful illustrated mascots. The system balances professional auction functionality with approachable, friendly visual language.

## Color Palette

**Primary Colors:**
- Background Primary: #1C1E21 — Main app background, creates deep immersive environment
- Surface: #2A2D31 — Card backgrounds, elevated surfaces, content containers
- Primary Action: #FF6B35 — Primary CTAs, active states, brand accent throughout
- Orange Accent: #F97316 — Secondary orange for highlights and emphasis

**Text Colors:**
- Text Primary: #FFFFFF — Headings, primary content, high emphasis text
- Text Secondary: #9CA3AF — Supporting text, metadata, time stamps
- Text Tertiary: #6B7280 — Disabled states, subtle information

**Semantic Colors:**
- Success/Positive: #10B981 — Successful bids, positive indicators
- Border: #374151 — Card borders, dividers, subtle separations

**Illustration Colors:**
- Ice Blue: #7DD3FC — Character/mascot primary color
- Cream: #FEF3C7 — Warm accent in illustrations
- Purple: #A78BFA — Secondary illustration accent

## Typography

**Font Families:**
- Primary: SF Pro Display / System UI (iOS native)
- Fallback: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif

**Type Scale:**
- Page Title: 32px, 700 (Bold), 1.2 line-height — Main screen headers
- Card Title: 20px, 600 (Semibold), 1.3 line-height — Domain names, primary card content
- Body Large: 16px, 500 (Medium), 1.4 line-height — Search placeholders, action labels
- Body: 15px, 400 (Regular), 1.5 line-height — Standard text
- Metadata: 14px, 400 (Regular), 1.4 line-height — Time remaining, bid counts
- Price Display: 20-24px, 700 (Bold), 1.2 line-height — Auction prices
- Tab Labels: 14px, 500 (Medium), 1.3 line-height — Navigation elements
- Button Text: 16px, 600 (Semibold), 1.0 line-height — CTA button labels

**Hierarchy Rules:**
- White text for all primary content maintains strong contrast on dark backgrounds
- Gray hierarchy (light to dark) indicates information priority
- Orange text exclusively for CTAs and interactive elements
- Bold weights (600-700) reserved for prices, titles, and actions
- Regular weight (400) for supporting metadata and descriptions

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 56, 64

**Common Patterns:**
- Screen padding: 16px horizontal, 12px vertical edges
- Card internal padding: 20px all sides
- Card vertical spacing: 16px between cards
- Icon-to-text spacing: 8px
- Section spacing: 24px between major sections
- Button padding: 16px vertical, 24px horizontal
- Search bar padding: 16px all sides
- Tab bar height: 56px with internal 12px padding
- Modal content padding: 24px

**Component Spacing:**
- Auction card content: 20px padding, 12px between elements
- Metadata rows: 8px vertical gap
- Price and CTA alignment: 16px gap
- Filter tabs: 12px horizontal gap, 40px height
- Navigation icons: 24px size with 16px padding zones

## Component Styles

### Buttons

**Primary CTA (Orange):**
- Background: #FF6B35
- Text: #FFFFFF, 16px, 600 weight
- Border radius: 12px
- Padding: 14px vertical, 32px horizontal
- No border
- Shadow: subtle 0 2px 8px rgba(255, 107, 53, 0.3)
- Hover/Press: Slight opacity reduction to 0.9

**Secondary CTA (Orange Text):**
- Background: transparent
- Text: #FF6B35, 16px, 500 weight
- No border, no background
- Touch target: 44px minimum

**Bottom Sheet CTA:**
- Background: #FF6B35
- Full width minus 32px horizontal margin
- Height: 56px
- Border radius: 12px
- Text: 16px, 600 weight, white

### Cards

**Auction Card:**
- Background: #2A2D31
- Border radius: 16px
- Border: 1px solid #374151
- Padding: 20px
- Shadow: subtle 0 2px 12px rgba(0, 0, 0, 0.2)
- Layout: Title + metadata rows + price/CTA split

**Card Content Structure:**
- Title: Top aligned, white, 20px semibold
- Metadata rows: 8px gap, icon + text pairs
- Price: Right aligned, 20-24px bold
- CTA button: Bottom right, auto width

### Input Fields

**Search Bar:**
- Background: #2A2D31
- Border radius: 24px (pill shape)
- Height: 48px
- Padding: 16px horizontal
- Placeholder: #9CA3AF, 16px
- Icon: 20px, #9CA3AF, 12px left padding
- Border: none
- Focus state: slight glow with orange tint

**Code Input:**
- Background: #2A2D31
- Border: 1px solid #374151
- Border radius: 12px
- Height: 56px
- Text: #FFFFFF, 18px, centered
- Padding: 16px
- Focus: Orange border #FF6B35

### Navigation

**Tab Bar:**
- Background: #1C1E21
- Height: 56px + safe area
- Border top: 1px solid #374151
- Icons: 24px, #9CA3AF inactive, #FF6B35 active
- Labels: 12px, #9CA3AF inactive, #FF6B35 active
- 4 evenly spaced items

**Filter Tabs (Horizontal):**
- Background: transparent
- Height: 40px
- Icon: 24px above label
- Text: 14px, 500 weight
- Active: Orange underline 2px, #FF6B35 text
- Inactive: #9CA3AF text
- Gap: 12px between tabs

### Modals & Overlays

**Modal Card:**
- Background: #2A2D31
- Border radius: 24px top corners
- Padding: 24px
- Close button: Top right, 32px touch target
- Content: Centered text with 20px vertical rhythm

**Bottom Sheet CTA Bar:**
- Background: #1C1E21 with top border
- Height: 80px + safe area
- Padding: 16px
- Full-width orange button

### Icons & Illustrations

**System Icons:**
- Size: 20-24px standard, 16px small
- Style: Outlined, 2px stroke
- Color: #9CA3AF default, #FF6B35 active
- Usage: Navigation, metadata indicators, actions

**Mascot Illustration:**
- Style: Playful, friendly character design
- Colors: Ice blue (#7DD3FC), cream (#FEF3C7), purple (#A78BFA)
- Usage: Onboarding, empty states, confirmations
- Placement: Bottom or center of modals

## Layout Principles

- Max content width: Full screen on mobile (responsive to device width)
- Card grid: Single column on mobile, stacked vertically
- Responsive behavior: Fixed header, scrollable content, fixed bottom actions
- Alignment: Left-aligned content, right-aligned prices and actions
- Vertical rhythm: Consistent 16px card gaps, 24px section spacing
- Safe areas: Respects iOS notch and home indicator zones

## Visual Effects

- **Border Radius:** 
  - Cards: 16px
  - Buttons: 12px
  - Inputs: 12px (rectangular), 24px (search pill)
  - Modals: 24px top corners
  - Tabs: No radius (sharp rectangles)
  
- **Shadows:** 
  - Cards: 0 2px 12px rgba(0, 0, 0, 0.2)
  - Primary buttons: 0 2px 8px rgba(255, 107, 53, 0.3)
  - Floating elements: 0 4px 16px rgba(0, 0, 0, 0.3)
  
- **Borders:** 
  - Thickness: 1px standard, 2px for active states
  - Style: Solid
  - Color: #374151 for divisions, #FF6B35 for active states
  - Usage: Card outlines, tab indicators, input fields
  
- **Backgrounds:** 
  - Solid colors throughout
  - No gradients in UI (gradients reserved for illustrations)
  - Subtle contrast between surface (#2A2D31) and background (#1C1E21)

## Design Tone

Dark, sophisticated, and professional with strategic bursts of vibrant orange energy. The system balances auction marketplace credibility with playful, approachable character through illustrated mascots. High contrast ensures excellent readability while the warm orange accent creates urgency and excitement around bidding actions. The design feels modern, tech-forward, and optimized for extended viewing sessions in the dark interface.

## Usage Notes for AI Implementation

This system prioritizes mobile-first design with iOS conventions. Always use the orange accent (#FF6B35) exclusively for actionable elements—never for decoration. Maintain strict contrast ratios (WCAG AA minimum) between text and backgrounds. The dark theme reduces eye strain for extended browsing sessions. When implementing cards, ensure consistent 16px vertical spacing and 20px internal padding. Reserve illustrations for key moments (onboarding, verification, empty states) rather than throughout the interface. The tab bar should always remain accessible with clear active state indicators. Price displays should be prominent and right-aligned for quick scanning.
