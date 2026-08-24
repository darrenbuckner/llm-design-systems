---
id: dark-agency-bold-001
title: Ember Forge System
description: A bold, high-contrast dark theme with warm coral accents and confident typography for creative agencies and startups.
tags: [dark, bold, agency, high-contrast, coral-accent, professional]
colors: ["#000000", "#FFFFFF", "#FF6B4A", "#1A1A1A", "#666666", "#333333"]
created: 2026-01-10
---

# Ember Forge System

A commanding dark interface built for creative agencies and startup ecosystems. The design pairs deep blacks with confident white typography and a warm coral accent that adds energy without disrupting the professional tone. Large-scale headlines and generous whitespace create a gallery-like presentation that lets content breathe while maintaining visual impact.

## Color Palette

**Primary Colors:**
- Background Primary: #000000 — Main page background, creates maximum contrast
- Foreground Primary: #FFFFFF — Headlines, primary text, high-emphasis content
- Accent: #FF6B4A — Call-to-action elements, highlighted text, hover states

**Neutral Colors:**
- Surface Dark: #1A1A1A — Card backgrounds, elevated surfaces, secondary sections
- Surface Medium: #333333 — Borders, dividers, subtle separations
- Text Secondary: #999999 — Supporting text, descriptions, metadata
- Text Muted: #666666 — Captions, timestamps, tertiary information

**Functional Colors:**
- Success: #4ADE80 — Positive states, confirmations
- Warning: #FBBF24 — Alerts, caution states
- Error: #F87171 — Error messages, destructive actions
- Info: #60A5FA — Informational highlights

## Typography

**Font Families:**
- Primary: Inter (or similar geometric sans-serif like Neue Haas Grotesk, Söhne)
- Fallback: system-ui, -apple-system, sans-serif

**Type Scale:**
- Display: 72-96px, 600 weight, -0.02em tracking, 1.0 line-height
- Heading 1: 48-64px, 600 weight, -0.02em tracking, 1.1 line-height
- Heading 2: 32-40px, 600 weight, -0.01em tracking, 1.2 line-height
- Heading 3: 24-28px, 500 weight, normal tracking, 1.3 line-height
- Body Large: 18-20px, 400 weight, normal tracking, 1.6 line-height
- Body: 16px, 400 weight, normal tracking, 1.6 line-height
- Caption: 14px, 400 weight, 0.01em tracking, 1.4 line-height
- Label: 12px, 500 weight, 0.05em tracking, 1.2 line-height (often uppercase)

**Hierarchy Rules:**
- Headlines use semi-bold weight with tight tracking for impact
- Body text uses regular weight with generous line-height for readability
- Section numbers and labels use uppercase with wide tracking
- Accent color applied to key words within headlines for emphasis
- Maximum contrast: white text on black backgrounds

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 16, 24, 32, 48, 64, 96, 128px

**Common Patterns:**
- Section padding: 96-128px vertical, 24-48px horizontal
- Card padding: 24-32px
- Component gaps: 16-24px
- Text block spacing: 24px between paragraphs
- Grid gaps: 24-32px
- Mobile section padding: 64px vertical, 16-24px horizontal

## Component Styles

### Buttons

**Primary Button:**
- Background: #FF6B4A
- Text: #FFFFFF
- Padding: 16px 32px
- Border radius: 0px (sharp corners)
- Font: 14px, 500 weight, uppercase, 0.05em tracking
- Hover: Background lightens to #FF8066
- Active: Background darkens to #E55A3A

**Secondary Button:**
- Background: transparent
- Border: 1px solid #FFFFFF
- Text: #FFFFFF
- Padding: 16px 32px
- Border radius: 0px
- Hover: Background #FFFFFF, Text #000000

**Text Link:**
- Color: #FFFFFF
- Underline: none by default
- Hover: Color #FF6B4A or underline appears
- Often includes arrow indicator (→)

### Cards

**Content Card:**
- Background: #1A1A1A
- Border: none or 1px solid #333333
- Border radius: 0px (sharp corners throughout)
- Padding: 0 (image bleeds to edge)
- Image aspect ratio: 16:9 or 4:3
- Title: 20-24px, 500 weight, white
- Description: 14-16px, 400 weight, #999999
- Hover: Subtle scale transform (1.02) or overlay

**Feature Card:**
- Background: #000000
- Border-top: 1px solid #333333
- Padding: 32px 0
- Section number: 12px uppercase, #666666
- Title: 24-32px, 600 weight, white

### Navigation

**Header Navigation:**
- Background: transparent or #000000
- Logo: White, left-aligned
- Links: 14px, 400 weight, white, uppercase optional
- Spacing: 32px between items
- Mobile: Hamburger menu with full-screen overlay

**Footer Navigation:**
- Background: #000000
- Border-top: 1px solid #333333
- Columns: Logo/address, Navigation links, Social links
- Link color: #999999, hover #FFFFFF
- Padding: 64px vertical

### Section Numbers

- Format: "01 /" or "/01"
- Font: 12-14px, 400 weight
- Color: #666666 or #999999
- Position: Above section title or inline
- Tracking: 0.1em

### Tags/Labels

- Background: transparent or #1A1A1A
- Border: 1px solid #333333
- Text: 12px, 500 weight, uppercase
- Padding: 8px 16px
- Color: #999999

## Layout Principles

**Container:**
- Max width: 1400px
- Padding: 24-48px horizontal
- Center aligned

**Grid Structure:**
- 12-column grid on desktop
- 16-32px column gaps
- Cards typically span 4-6 columns
- Full-bleed sections break the grid

**Responsive Behavior:**
- Desktop (1200px+): Full grid, large typography
- Tablet (768-1199px): Reduced columns, slightly smaller type
- Mobile (< 768px): Single column, stacked layout, 48-64px display text

**Alignment:**
- Left-aligned text throughout
- Section titles often span full width
- Cards in grid alignment
- Generous asymmetric whitespace

## Visual Effects

**Border Radius:**
- Buttons: 0px (sharp corners)
- Cards: 0px (sharp corners)
- Images: 0px (sharp corners)
- Inputs: 0px (sharp corners)
- Overall: Deliberately angular, no rounded corners

**Shadows:**
- Minimal to none
- Elevation created through background color differences
- Occasional subtle shadow on hover: 0 8px 32px rgba(0,0,0,0.3)

**Borders:**
- Thickness: 1px
- Color: #333333 (subtle) or #FFFFFF (emphasis)
- Used sparingly for section dividers
- Horizontal rules between content sections

**Backgrounds:**
- Solid colors only (no gradients in UI)
- Image backgrounds with dark overlays
- Alternating #000000 and #1A1A1A for section differentiation

**Animations:**
- Subtle hover transitions: 0.2-0.3s ease
- Scale transforms on cards: transform: scale(1.02)
- Color transitions on links and buttons
- Optional: Smooth scroll, fade-in on scroll

## Design Tone

This system projects confidence and creative authority through its stark contrast and bold typographic choices. The complete absence of border radius creates a sharp, editorial quality reminiscent of print design and gallery spaces. The warm coral accent prevents the dark palette from feeling cold or corporate, adding approachability to the professional foundation. This is a system that takes itself seriously without being unapproachable—perfect for creative agencies, venture studios, and brands that want to signal both expertise and energy.

## Usage Notes for AI Implementation

When implementing this system:

1. **Prioritize contrast** — Always ensure WCAG AA compliance; white text on black backgrounds naturally achieves this
2. **Use the accent sparingly** — Coral (#FF6B4A) should highlight key actions and important text, not dominate the palette
3. **Maintain sharp corners** — Border radius of 0 is intentional; do not round corners on any elements
4. **Scale typography confidently** — Headlines should be large and impactful; don't shy away from 64-96px display text
5. **Embrace whitespace** — Large margins and padding are essential to the gallery-like presentation
6. **Section numbers add structure** — Use "01 /" format to create visual hierarchy in long-form pages
7. **Keep animations subtle** — This system relies on typography and contrast, not motion
8. **Images should be high-quality** — The minimal UI puts focus on imagery; low-quality images will stand out negatively
