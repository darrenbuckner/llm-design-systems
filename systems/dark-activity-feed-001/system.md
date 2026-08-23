---
id: dark-activity-feed-001
title: Midnight Activity Stream
description: A dark, athletic-focused interface with bold orange accents and clean data visualization for activity tracking
tags: [dark, minimal, athletic, data-focused, mobile-first]
colors: ["#FC4C02", "#1A1A1A", "#2A2A2A", "#FFFFFF", "#999999", "#333333"]
created: 2025-01-04
---

# Midnight Activity Stream

A sophisticated dark interface designed for athletic and fitness applications. The system combines deep black backgrounds with vibrant orange accents to create an energetic yet focused environment. Data is presented with bold typography and clear hierarchies, optimized for quick scanning of metrics and activity updates.

## Color Palette

**Primary Colors:**
- Primary/Accent: #FC4C02 — Vibrant orange, used for CTAs, active states, icons, and emphasis
- Primary Dark: #E54500 — Darker orange for hover states and secondary emphasis

**Neutral Colors:**
- Background Primary: #000000 — Pure black, main app background
- Background Elevated: #1A1A1A — Slightly elevated surfaces, cards
- Background Tertiary: #2A2A2A — Search fields, input backgrounds
- Surface Border: #333333 — Subtle dividers and separators

**Text Colors:**
- Text Primary: #FFFFFF — Headings, important values, usernames
- Text Secondary: #999999 — Labels, metadata, timestamps
- Text Tertiary: #666666 — Disabled states, hints

**State Colors:**
- Active/Success: #FC4C02 — Active tab indicator, completion states
- Notification Badge: #FC4C02 — Alert badges with white text
- Interactive: #FFFFFF — Icons in default state

## Typography

**Font Families:**
- Primary: SF Pro Display / -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif
- Numeric: SF Pro (tabular figures for aligned data)

**Type Scale:**
- Display/Value Large: 20px, weight 700, line-height 1.2 — Metric values (2.40 mi, 10:30)
- Heading 1: 20px, weight 700, line-height 1.3 — Activity titles (Morning Run)
- Heading 2: 17px, weight 600, line-height 1.4 — Section headers, usernames
- Body: 15px, weight 400, line-height 1.5 — Descriptions, supporting text
- Label: 13px, weight 400, line-height 1.4 — Metric labels (Distance, Pace, Time)
- Caption: 12px, weight 400, line-height 1.4 — Timestamps, metadata
- Tab Label: 11px, weight 500, line-height 1.2 — Bottom navigation labels

**Hierarchy Rules:**
- Metric values use bold weight with large size for instant readability
- Labels above metrics use smaller, lighter weight text in secondary color
- Usernames are bold white, timestamps are regular secondary gray
- Activity titles are bold and prominent, descriptions are regular weight

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 48

**Common Patterns:**
- Screen horizontal padding: 16px
- Card internal padding: 16px vertical, 16px horizontal
- Section spacing: 24px between major sections
- Metric group spacing: 32px between columns
- Avatar to content gap: 12px
- Label to value spacing: 4px
- Icon button spacing: Equal distribution (flex justify-between)

## Component Styles

### Navigation Tabs (Top)
- Background: transparent on #000000
- Inactive text: #999999, 17px, weight 400
- Active text: #FFFFFF, 17px, weight 600
- Active indicator: 3px height, #FC4C02, full tab width
- Tab padding: 12px vertical

### Bottom Navigation
- Background: #000000 with subtle top border
- Icon size: 24px
- Label: 11px, weight 500
- Inactive: #999999 (icon and text)
- Active: #FC4C02 (icon and text)
- Badge: 16px circle, #FC4C02 background, white text, positioned top-right of icon

### Search Input
- Background: #2A2A2A
- Border radius: 10px
- Height: 44px
- Padding: 12px 16px
- Icon: magnifying glass, #999999, 16px
- Placeholder: #666666, 15px

### Activity Cards
- Background: transparent (no distinct card background)
- Divider: 1px solid #333333 at bottom
- Padding: 16px vertical
- Avatar: 48px circle
- Content structure: Avatar left, content right (flex)

### Metric Display
- Layout: horizontal row, equal spacing
- Label: above value, 13px, #999999
- Value: 20px, bold, #FFFFFF
- Unit: same size as value, included inline

### Icon Buttons (Action Row)
- Size: 24px icons
- Color: #FFFFFF
- Spacing: flex justify-around or space-between
- Padding: 12px vertical for touch target
- Icons: thumbs-up (kudos), comment, share

### Promotional Banner
- Background: transparent or subtle #1A1A1A
- Icon container: 48px, rounded square, #2A2A2A background
- Icon: #FC4C02 accent color
- Title: 17px, bold, white
- Description: 15px, regular, #999999

### Avatar
- Size: 48px (feed), 32px (header profile)
- Shape: circle
- Border: none or subtle 1px #333333

### Badges/Tags
- Device badge: inline with timestamp
- Icon + text layout
- Icon: 12px, #999999
- Text: 12px, #999999

## Layout Principles

- **Max content width:** Full width mobile, no max-width constraint
- **Grid structure:** Single column feed layout
- **Responsive behavior:** Mobile-first, full-width cards
- **Alignment:** Left-aligned content, centered bottom navigation
- **Safe areas:** Respects iOS safe area insets (notch, home indicator)

## Visual Effects

- **Border Radius:**
  - Search inputs: 10px
  - Avatars: 50% (circle)
  - Icon containers: 12px
  - Buttons: 8px
  - Badges: 50% (pill/circle)

- **Shadows:** None visible — flat design approach

- **Borders:**
  - Dividers: 1px solid #333333
  - Active tab indicator: 3px solid #FC4C02

- **Backgrounds:**
  - Solid colors only, no gradients
  - Layered elevation through brightness (000 < 1A1A1A < 2A2A2A)

## Design Tone

This system embodies athletic energy and focused performance. The dark interface reduces visual fatigue during active use while the vibrant orange accents create urgency and motivation. Typography is bold and scannable, optimized for quick metric reading during or after physical activity. The overall aesthetic is modern, clean, and purposefully minimal — letting data and social content take center stage.

## Usage Notes for AI Implementation

1. **Orange accent is sacred** — Use #FC4C02 sparingly for primary actions, active states, and key highlights only. Overuse dilutes its impact.

2. **Maintain dark hierarchy** — Background layers go from pure black (#000000) to dark gray (#1A1A1A) to medium gray (#2A2A2A). Never skip levels.

3. **Metric display pattern** — Always place small gray labels above large white values. Use consistent column spacing for multi-metric rows.

4. **Touch targets** — All interactive elements need minimum 44px touch target, even if visual size is smaller.

5. **Icon consistency** — Use outline/stroke icons at 24px, white color by default, orange when active.

6. **Feed card rhythm** — Maintain consistent vertical spacing between cards. Use subtle dividers (#333333) rather than card backgrounds to separate items.

7. **Typography weight contrast** — Create hierarchy through weight (400 vs 600 vs 700) rather than size alone. Keep size differences subtle.

8. **No decorative elements** — This system is utilitarian. Avoid gradients, shadows, or ornamental graphics. Let content breathe.
