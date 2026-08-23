---
id: light-domain-001
title: Lime Registry
description: High-contrast domain search interface with electric lime accents and bold typography
tags: [light, bold, lime-accent, high-contrast, promotional]
colors: ["#CDDC39", "#673AB7", "#1A1A1A", "#FFFFFF", "#F0F7FF", "#4CAF50"]
created: 2025-01-04
---

# Lime Registry

A bold, high-energy interface design featuring electric lime green as its signature accent color against a clean white canvas. The system uses dramatic typography scale and high-contrast elements to create urgency and draw attention to key actions and promotional content.

## Color Palette

**Primary Colors:**
- Lime Accent: #CDDC39 — Primary brand color, announcement bars, promotional badges
- Purple Action: #673AB7 — Search buttons, floating action buttons, interactive elements

**Neutral Colors:**
- Pure White: #FFFFFF — Primary background
- Near Black: #1A1A1A — Primary headings, logo text
- Dark Gray: #333333 — Body text, secondary content
- Medium Gray: #666666 — Muted text, helper text
- Light Gray: #E0E0E0 — Borders, dividers

**Surface Colors:**
- Ice Blue: #F0F7FF — Card backgrounds, result containers
- Soft Lavender: #E8E4F0 — Active tab backgrounds, selected states
- Off White: #F5F5F5 — Input backgrounds, secondary surfaces

**State Colors:**
- Success/Sale: #4CAF50 — Savings indicators (lime-green variant)
- Lime Badge: #CDDC39 — "EXACT MATCH" badges, promotional tags
- Error: #E53935 — Strikethrough prices, error states

## Typography

**Font Families:**
- Primary: Inter, -apple-system, system-ui, sans-serif
- Alternative: SF Pro Display (for headings on Apple devices)

**Type Scale:**
- Display/Hero: 48-56px, 700 weight, -0.02em tracking, 1.1 line-height
- Heading 1: 36px, 700 weight, 1.2 line-height
- Heading 2: 24px, 600 weight, 1.3 line-height
- Body Large: 18px, 500 weight, 1.5 line-height
- Body: 16px, 400 weight, 1.5 line-height
- Caption: 14px, 400 weight, 1.4 line-height
- Small/Badge: 12px, 600 weight, 1.2 line-height, uppercase

**Hierarchy Rules:**
- Hero headlines use dramatic size (48-56px) with tight line-height for impact
- Tab labels use medium weight (500) for clear navigation
- Promotional badges use uppercase, small size, high contrast backgrounds
- Price display uses extra-large sizing with strikethrough for original prices

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 80

**Common Patterns:**
- Announcement bar padding: 12px 16px
- Section vertical spacing: 48-64px
- Card internal padding: 24px
- Input padding: 16px 20px
- Button padding: 16px 24px
- Tab padding: 12px 24px
- Badge padding: 6px 12px

## Component Styles

### Announcement Bar
- Background: #CDDC39 (lime)
- Text: #1A1A1A (near black)
- Padding: 12px 16px
- Full width, centered text
- Font: 14-16px, 500 weight
- Optional arrow icons flanking text

### Navigation Header
- Background: transparent/white
- Logo: Bold wordmark, near black
- Hamburger menu: 3 horizontal lines, 2px stroke
- Padding: 16px 24px
- Sticky behavior on scroll

### Tab Switcher
- Container: Rounded pill shape (32px radius)
- Background: #F5F5F5 (inactive), #E8E4F0 (active tab background)
- Active tab: Darker background, same text color
- Text: 16px, 500 weight
- Padding: 12px 24px per tab
- Transition: smooth background change

### Search Input
- Background: #FFFFFF
- Border: 2px solid #E0E0E0
- Border radius: 12px (container), 8px (button)
- Input padding: 16px 20px
- Placeholder: #666666
- Search button: #673AB7 background, white icon
- Button size: 56px square, right-aligned within container

### Result Cards
- Background: #F0F7FF (ice blue)
- Border radius: 16px
- Padding: 24px
- No border, relies on background contrast

### Badges
**Exact Match Badge:**
- Background: #CDDC39
- Text: #1A1A1A
- Border radius: 6px
- Padding: 6px 12px
- Font: 12px, 600 weight, uppercase

**Savings Badge:**
- Background: #CDDC39 (lighter lime)
- Text: #1A1A1A
- Border radius: 16px (pill shape)
- Padding: 4px 12px
- Font: 14px, 600 weight

### Floating Action Button (Chat/Help)
- Background: #673AB7 (purple)
- Icon + text: white
- Border radius: 24px (pill)
- Padding: 12px 20px
- Shadow: 0 4px 12px rgba(103, 58, 183, 0.3)
- Position: fixed bottom-right

### Pricing Display
- Current price: 32-40px, 700 weight, #1A1A1A
- Original price: 16-18px, 400 weight, #666666, strikethrough
- Helper text: 14px, 400 weight, #666666

## Layout Principles

- Max content width: 800-1000px for main content
- Full-width announcement bar
- Centered content alignment for hero sections
- Card-based results with generous spacing
- Mobile-first approach with single column on small screens

## Visual Effects

**Border Radius:**
- Buttons (pill): 24-32px
- Cards: 16px
- Inputs: 12px
- Badges: 6px (rectangular) or 16px (pill)
- Tab containers: 32px

**Shadows:**
- FAB shadow: 0 4px 12px rgba(103, 58, 183, 0.3)
- Card hover: 0 8px 24px rgba(0, 0, 0, 0.08)
- Input focus: 0 0 0 3px rgba(103, 58, 183, 0.2)

**Borders:**
- Input borders: 2px solid #E0E0E0
- Focus state: 2px solid #673AB7

**Backgrounds:**
- Solid colors dominate (no gradients)
- Ice blue (#F0F7FF) for highlighting important content
- Pure white for maximum contrast

## Design Tone

Bold, energetic, and conversion-focused. The electric lime creates immediate visual impact and urgency, while the purple action elements provide clear interactive affordances. The clean white background and generous spacing keep the interface feeling professional despite the bright accent colors. This system is optimized for promotional content and clear calls-to-action.

## Usage Notes for AI Implementation

1. **Lime accent is signature** — Use sparingly but prominently for announcements, badges, and promotional elements
2. **Purple for actions only** — Reserve #673AB7 exclusively for clickable/interactive elements
3. **High contrast is intentional** — Don't soften the lime/white contrast; it's meant to grab attention
4. **Typography scale is dramatic** — Hero text should feel oversized; this creates visual hierarchy
5. **Ice blue surfaces** — Use #F0F7FF to elevate important content areas from the white background
6. **Badges communicate urgency** — Uppercase, small text, high-contrast backgrounds
7. **Mobile-first spacing** — Generous padding on all interactive elements for touch targets
