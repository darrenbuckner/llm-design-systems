---
id: dark-vault-native-001
title: Vault Native Dark
description: A native mobile dark theme with vibrant category icons and subtle elevated surfaces
tags: [dark, native, mobile-first, minimal, system-ui]
colors: ["#000000", "#1C1C1E", "#2C2C2E", "#007AFF", "#30D158", "#FF9F0A", "#FF453A", "#32ADE6"]
created: 2025-01-10
---

# Vault Native Dark

A refined dark mobile interface designed for secure data management. Features a true black background with elevated card surfaces, vibrant multi-color category icons, and crisp SF-style typography. The aesthetic balances functional minimalism with visual hierarchy through subtle surface elevation and strategic color accents.

## Color Palette

**Base Colors:**
- Background: #000000 — True black base, maximizes OLED efficiency
- Surface Primary: #1C1C1E — Elevated cards and interactive containers
- Surface Secondary: #2C2C2E — Search fields and secondary containers
- Surface Tertiary: #3A3A3C — Hover/pressed states

**Text Colors:**
- Text Primary: #FFFFFF — Primary content and headings
- Text Secondary: #8E8E93 — Labels, placeholders, counts
- Text Tertiary: #636366 — Disabled or de-emphasized content

**Accent Colors:**
- Primary Blue: #007AFF — CTAs, links, and primary actions
- Success Green: #30D158 — Verified states, passkeys, connections
- Warning Amber: #FF9F0A — Caution indicators, codes
- Error Red: #FF453A — Security alerts, deletion actions
- Info Cyan: #32ADE6 — Network and connectivity indicators

**Icon Background Colors:**
- Blue Circle: #007AFF — All items category
- Green Circle: #30D158 — Passkeys and identity
- Amber Circle: #FF9F0A — Authentication codes
- Cyan Circle: #32ADE6 — Wi-Fi and network
- Red Circle: #FF453A — Security warnings
- Red-Orange Circle: #FF6961 — Deleted items (trash)

## Typography

**Font Families:**
- Primary: SF Pro Display / SF Pro Text (system San Francisco)
- Fallback: -apple-system, BlinkMacSystemFont, "Segoe UI", system-ui, sans-serif

**Type Scale:**
- Page Title: 34px, weight 700 (bold), line-height 1.2
- Section Header: 13px, weight 600, letter-spacing 0.5px, uppercase, color #8E8E93
- Card Label: 17px, weight 400 (regular), line-height 1.4
- Card Count: 17px, weight 400, color #8E8E93
- Body Text: 15px, weight 400, line-height 1.5
- Caption: 13px, weight 400, line-height 1.4, color #8E8E93
- Link Text: 15px, weight 400, color #007AFF

**Hierarchy Rules:**
- Page titles use bold weight with generous top margin
- Section headers are uppercase, subdued gray, small size
- Card content uses regular weight, high contrast white
- Secondary info (counts, descriptions) uses muted gray
- Interactive text (links) uses the primary blue accent

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 48, 64

**Common Patterns:**
- Page horizontal padding: 16px (mobile), 20px (larger screens)
- Page top padding: 64px (accounts for status bar)
- Card internal padding: 16px vertical, 16px horizontal
- Grid gap between cards: 12px
- Section spacing: 32px between major sections
- Icon size: 32px with 8px internal padding
- Chevron spacing: 8px from count text

**Card Grid:**
- 2-column grid on mobile
- Equal width columns with 12px gap
- Cards stack vertically on very narrow screens

## Component Styles

### Search Bar
- Background: #2C2C2E
- Border radius: 12px
- Height: 44px
- Padding: 12px 16px
- Placeholder color: #8E8E93
- Icon color: #8E8E93
- Features search icon (left) and microphone icon (right)

### Category Cards
- Background: #1C1C1E
- Border radius: 12px
- Padding: 16px
- Min-height: 80px
- Layout: Icon top-left, count + chevron top-right, label bottom-left
- Icon: 32px circular background with centered symbol (20px)
- Count + Chevron: Right-aligned, gray text with small chevron
- Hover state: Background lightens to #2C2C2E

### Icon Circles
- Size: 32px diameter
- Border radius: 50% (fully round)
- Background: Semantic color (blue, green, amber, etc.)
- Icon: White, centered, 18-20px
- Symbols: Key, person-badge, lock, wifi, warning, trash

### Action Row
- Background: #1C1C1E
- Border radius: 12px
- Padding: 14px 16px
- Height: ~48px
- Icon: 24px, #007AFF
- Text: 17px, #007AFF
- Full width, single row layout

### Promotional Card
- Background: #1C1C1E
- Border radius: 16px
- Padding: 16px
- Icon: 40px, gray (#8E8E93)
- Close button: 24px, top-right, gray
- Title: 17px, weight 600, white
- Description: 15px, weight 400, #8E8E93
- CTA Link: 15px, #007AFF

### Floating Action Button
- Size: 44px touch target
- Icon: 24px plus sign
- Color: #007AFF
- Position: Fixed bottom-right, 24px from edges
- No background (icon only)

## Layout Principles

- **Max content width:** 428px (mobile-optimized, but fluid)
- **Grid structure:** 2-column for category cards, single column for actions
- **Responsive behavior:** Cards maintain grid on mobile, search bar spans full width
- **Alignment:** Left-aligned titles and labels, right-aligned counts and chevrons
- **Safe areas:** Respects system status bar and home indicator

## Visual Effects

**Border Radius:**
- Large containers/cards: 12-16px
- Search fields: 12px
- Icon circles: 50% (fully round)
- Buttons: 8-12px

**Shadows:**
- No drop shadows (flat design, elevation via color)
- Depth created through background color differentiation

**Borders:**
- Minimal use of borders
- Occasional 1px dividers in #3A3A3C when needed

**Backgrounds:**
- Pure solid colors, no gradients
- True black (#000000) background for OLED optimization
- Elevated surfaces use progressively lighter grays

## Design Tone

This system embodies functional minimalism with a security-focused aesthetic. The true black background creates maximum contrast and visual weight for the colorful category icons, which serve as instant visual identifiers. The overall tone is professional, trustworthy, and efficient—designed for quick scanning and confident interaction with sensitive data.

## Usage Notes for AI Implementation

When implementing this design system:

1. **Color priority:** Always use true black (#000000) as the base—never dark gray. Elevated elements should step up to #1C1C1E.

2. **Typography:** Use system fonts (-apple-system stack) for native feel. SF Pro is ideal but falls back gracefully.

3. **Icon colors:** Each category should have a unique, vibrant background color. White icons on colored circles.

4. **Touch targets:** Maintain minimum 44px touch targets for all interactive elements.

5. **Card layout:** Use CSS Grid for the 2-column category layout. Flexbox for internal card alignment.

6. **States:** Hover/focus states should subtly lighten backgrounds. Active states can darken slightly.

7. **Spacing consistency:** Stick to the 8px base unit. Most internal padding is 16px, gaps are 12px.

8. **Responsive:** This is mobile-first. On larger screens, consider centering content with max-width constraint.

9. **Accessibility:** Ensure sufficient contrast (white on black achieves 21:1). Interactive elements need clear focus states.

10. **Animation:** Keep transitions subtle—150-200ms ease-out for background color changes. No flashy effects.
