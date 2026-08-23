---
id: light-signup-001
title: Sky Blue Signup System
description: Clean, friendly signup interface with soft blue gradient background and bold primary button
tags: [light, minimal, blue-gradient, modern, friendly]
colors: [#A8D5F7, #0D47A1, #1976D2, #1E3A5F]
created: 2024-12-11
---

# Sky Blue Signup System

A clean, approachable signup interface featuring a soft blue gradient background with bold, high-contrast primary actions. The design emphasizes simplicity and trust with generous spacing and clear visual hierarchy.

## Color Palette

**Primary Colors:**
- Primary Button: #0D47A1 — Deep blue for primary CTAs, strong contrast on light backgrounds
- Primary Hover: #1565C0 — Slightly lighter blue for hover states
- Link/Interactive: #1976D2 — Medium blue for links and secondary interactive elements

**Background Colors:**
- Background Gradient Start: #D5E8F7 — Light sky blue at top
- Background Gradient End: #A8D5F7 — Slightly deeper blue at bottom
- Surface/Card: #FFFFFF — Pure white for input fields and cards

**Text Colors:**
- Heading Text: #1E3A5F — Deep navy for main headings
- Body Text: #5F7A8A — Muted gray-blue for body copy
- Label Text: #2C3E50 — Dark blue-gray for form labels

**Border Colors:**
- Input Border Default: #1976D2 — Blue border for input fields
- Input Border Active: #0D47A1 — Darker blue on focus
- Divider: #E0E0E0 — Light gray for subtle separators

## Typography

**Font Families:**
- Primary: Sans-serif (likely Inter, Circular, or similar geometric sans)
- All text uses same family with weight variation

**Type Scale:**
- Heading 1 (Sign up): 64px, 600-700 weight, 1.1 line-height
- Subheading: 22px, 400 weight, 1.4 line-height
- Button Text: 20px, 600 weight, 1.2 line-height
- Body/Label: 18px, 500 weight, 1.5 line-height
- Link Text: 16px, 400 weight, 1.5 line-height
- Footer/Legal: 16px, 400 weight, 1.6 line-height

**Hierarchy Rules:**
- Main heading uses heavy weight and very large size (64px)
- Subheading is significantly smaller (22px) creating strong contrast
- Form labels use medium weight for clarity
- Links use standard weight with blue color for differentiation
- Legal text maintains readable size despite lower hierarchy

## Spacing System

**Base Unit:** 8px
**Scale:** 8, 16, 24, 32, 48, 64, 96, 128

**Common Patterns:**
- Button padding: 20px vertical, 48px horizontal
- Input padding: 20px vertical, 24px horizontal
- Section spacing (heading to button): 48px
- Between form elements: 32px
- Button to divider: 32px
- Footer spacing from content: 96px
- Side margins: 48-64px

## Component Styles

### Primary Button (OAuth/Social Login)
- Background: #0D47A1 (solid deep blue)
- Text color: #FFFFFF
- Border radius: 48px (full pill shape)
- Padding: 20px vertical, 48px horizontal
- Font size: 20px
- Font weight: 600
- Icon: White Google "G" icon with spacing
- Hover state: Slightly lighter blue background
- Full width on mobile, max-width ~600px on desktop

### Text Input Fields
- Background: #FFFFFF
- Border: 3px solid #1976D2
- Border radius: 12px
- Padding: 20px vertical, 24px horizontal
- Font size: 18px
- Placeholder color: #B0BEC5 (light gray)
- Focus state: Border darkens to #0D47A1
- Full width layout

### Text Links
- Color: #1976D2 (medium blue)
- Font size: 16-18px
- Font weight: 400
- Text decoration: Underline on hover
- Inline with text or standalone

### Language Selector (Top Right)
- Icon: Globe icon (#2C3E50)
- Text: "English"
- Font size: 18px
- Layout: Horizontal with 8px gap
- Position: Absolute top-right

### Divider Text
- Text: "or"
- Color: #5F7A8A
- Font size: 18px
- Centered with implied divider lines

## Layout Principles

- Max content width: ~600px for form area
- Vertical centering: Content appears centered vertically
- Horizontal padding: 48-64px on sides
- Alignment: All elements left-aligned within container
- Responsive behavior: Stack elements vertically, maintain padding ratios
- Single column layout throughout

## Visual Effects

- **Border Radius:** 
  - Buttons: 48px (full pill)
  - Inputs: 12px (rounded corners)
  - Cards/containers: 8-12px
  
- **Shadows:** 
  - Minimal or no shadows used
  - Focus states may have subtle glow
  
- **Borders:** 
  - Input fields: 3px solid
  - Strong, visible borders for clarity
  
- **Backgrounds:** 
  - Vertical gradient: Light blue (#D5E8F7) to medium blue (#A8D5F7)
  - Smooth transition across viewport height
  - Subtle texture possible but not prominent

## Design Tone

This design system projects a friendly, trustworthy, and modern aesthetic. The soft blue gradient creates an approachable atmosphere while the bold primary button provides clear direction. The generous spacing and large typography make the interface feel breathable and easy to use, prioritizing user comfort over density.

## Usage Notes for AI Implementation

When implementing this system, maintain the strong visual hierarchy through size contrast (64px heading vs 22px body). The blue gradient background should cover the full viewport and be generated programmatically. Ensure the primary button has sufficient contrast (minimum 4.5:1) against the background. The pill-shaped button should maintain its proportion across screen sizes. Form inputs should have clear focus states with border color changes. Keep the legal text readable but visually de-emphasized. For dark mode adaptations, invert the gradient to use darker blues and adjust text colors for appropriate contrast.
