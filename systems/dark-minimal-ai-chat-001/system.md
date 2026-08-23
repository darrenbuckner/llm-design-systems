---
id: dark-minimal-ai-chat-001
title: Dark Minimal AI Chat
description: Sophisticated dark mode design system with warm terracotta accents and nearly monochromatic palette for focused conversation interfaces
tags: dark, minimal, ai-chat, sophisticated
colors: #D4714A, #1A1A1A, #2A2A2A, #F5F5F5, #A0A0A0, #4A90D9
created: 2024-12-14
---

# Dark Minimal AI Chat

A sophisticated dark mode design system featuring warm terracotta accents and a nearly monochromatic palette. Designed for focused conversation interfaces that prioritize readability and calm productivity.

## Color Palette

**Primary Colors:**
- Primary Accent: #D4714A — Used for brand elements, decorative icons, warm accent touches
- Interactive Blue: #4A90D9 — Links and interactive text elements

**Neutral Colors:**
- Background Primary: #1A1A1A — Main app background, deep charcoal black
- Background Secondary: #0D0D0D — Sidebar background, true black
- Surface/Card: #2A2A2A — Input fields, cards, file attachment containers
- Surface Elevated: #3A3A3A — Hover states, chips, badges
- Text Primary: #F5F5F5 — Main body text, high contrast off-white
- Text Secondary: #A0A0A0 — Placeholder text, muted labels, timestamps
- Text Tertiary: #6B6B6B — Disabled states, very subtle text
- Borders: #3A3A3A — Subtle dividers and input borders
- Border Focus: #4A4A4A — Active/focus state borders

**Accent/State Colors:**
- Success: #4CAF50 (inferred)
- Warning: #D4714A — Warm orange, matches brand accent
- Error: #E57373 (inferred)

**UI Element Colors:**
- Icon Default: #A0A0A0 — Navigation icons in default state
- Icon Active: #F5F5F5 — Active/selected navigation icons
- Badge Background: #3A3A3A — Chips like "1 artifact", project badges

## Typography

**Font Families:**
- Primary: Clean sans-serif, similar to SF Pro Display / Inter — used throughout for UI and body text
- Monospace: SF Mono or similar — for code elements

**Type Scale:**
- Logo/Brand: ~28px, weight 600, letter-spacing -0.02em
- Heading 1: 24px, weight 600, line-height 1.3
- Heading 2 (Section Headers): 16px, weight 700, line-height 1.4
- Body: 16px, weight 400, line-height 1.5
- Body Bold: 16px, weight 700, inline emphasis within paragraphs
- Navigation Items: 16px, weight 400, line-height 1.4
- Caption/Small: 14px, weight 400, line-height 1.4 — badges, metadata
- Micro: 12px, weight 500 — chips, status indicators

**Hierarchy Rules:**
- Headings use semibold to bold weight, same color as body text
- Emphasis within body text uses bold weight (700), not color change
- Links are underlined and use blue color (#4A90D9)
- Section labels use muted text color and lighter weight

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 48, 64

**Common Patterns:**
- Component internal padding: 12-16px
- Navigation item vertical spacing: 12px between items
- Section spacing: 24-32px between major sections
- List item spacing: 16-20px between bullet points
- Card padding: 16px horizontal, 12px vertical
- Screen edge padding: 16-20px on mobile

## Component Styles

### Buttons
- **Primary Button:** Background #D4714A, text #FFFFFF, padding 12px 20px, border-radius 20px
- **Icon Button:** 44px touch target, transparent background, #A0A0A0 icon, hover #F5F5F5
- **Add Button (Blue Circle):** Background #4A90D9, icon #FFFFFF, 32px diameter, fully rounded

### Cards
- Background: #2A2A2A
- Border: 1px solid #3A3A3A
- Border Radius: 12px
- Padding: 12px 16px
- Shadow: none (flat design)

### Input Fields
- Background: #2A2A2A
- Border: 1px solid #3A3A3A
- Border Radius: 24px (pill shape for chat input)
- Focus State: Border #4A4A4A, no glow
- Padding: 12px 16px
- Placeholder Color: #6B6B6B

### Navigation Items
- Background Default: transparent
- Background Hover: #2A2A2A
- Text: #A0A0A0 default, #F5F5F5 active
- Icon: 20px, matching text color
- Padding: 8px 12px
- Border Radius: 8px

### Chips/Badges
- Background: #3A3A3A
- Text: #A0A0A0
- Padding: 4px 10px
- Border Radius: 16px (pill)
- Font Size: 12-14px

### File Attachments
- Background: #2A2A2A
- Border: 1px solid #3A3A3A
- Border Radius: 12px
- Icon: 24px, muted color
- Padding: 12px 16px
- Download button: circular, subtle

### Lists (Bulleted)
- Bullet: solid circle, 6px, #F5F5F5
- Bullet margin-right: 12px
- Line spacing: 8px between lines within item
- Item spacing: 16px between bullet points

## Layout Principles

- Max content width: ~680px for main content area
- Sidebar width: ~280px fixed
- Grid structure: Single column for chat, sidebar + main for desktop
- Responsive behavior: Sidebar collapsible on mobile, full-screen chat
- Alignment: Left-aligned throughout, centered greeting message

## Visual Effects

**Border Radius:**
- Small elements (badges, chips): 16px (pill)
- Medium elements (cards, inputs): 12px
- Large inputs (chat box): 24px
- Buttons: 20-24px
- Navigation items: 8px

**Shadows:**
- None used — entirely flat design with border-based depth

**Borders:**
- Thickness: 1px consistently
- Style: solid
- Used sparingly for input fields, cards, dividers

**Backgrounds:**
- Solid colors only
- No gradients
- No patterns or textures
- Subtle contrast between layers (sidebar darker than main)

**Icons:**
- Line-style icons, 1.5-2px stroke weight
- Consistent 20-24px sizing
- Emoji used freely inline with navigation items

## Design Tone

This is a sophisticated, minimal dark interface that prioritizes readability and focus. The nearly monochromatic palette with warm terracotta accents creates a premium, calm aesthetic that avoids the harshness of pure black-and-white. The design feels modern and professional while maintaining approachability through generous spacing, rounded corners, and playful emoji integration in navigation.

## Usage Notes for AI Implementation

- Use the warm accent color (#D4714A) extremely sparingly — only for brand moments, primary CTAs, and decorative flourishes
- Maintain strict color discipline: most UI should be grayscale, with color reserved for meaning
- Text hierarchy relies on weight, not size variation — keep sizes consistent, vary boldness
- All interactive elements need generous touch targets (44px minimum)
- Prefer pill-shaped (fully rounded) inputs and buttons for a softer feel
- Emoji are acceptable and encouraged in navigation labels and user-generated content
- Links should always be underlined, not just color-differentiated
- Keep shadows at zero — depth comes from background color layering only
- High contrast is essential: #F5F5F5 text on #1A1A1A background minimum
