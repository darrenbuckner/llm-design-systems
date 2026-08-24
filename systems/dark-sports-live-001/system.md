---
id: dark-sports-live-001
title: Graphite Sports System
description: Dark theme sports score interface with bold typography and team color accents
tags: [dark, sports, minimal, mobile-first]
colors: ["#202124", "#303134", "#8AB4F8", "#DC143C", "#FFFFFF"]
created: 2026-01-08
---

# Graphite Sports System

A dark-themed sports score interface featuring bold, oversized typography for live game scores, pill-shaped navigation elements, and subtle card-based layouts. Designed for mobile-first consumption of real-time sports data.

## Color Palette

**Primary Dark Colors:**
- Background Primary: #202124 — Main app background
- Surface: #303134 — Card backgrounds, elevated surfaces
- Border/Divider: #3C4043 — Subtle separators and borders

**Neutral Colors:**
- Text Primary: #E8EAED — Main text, scores, headlines
- Text Secondary: #9AA0A6 — Supporting text, timestamps, secondary labels
- Text Tertiary: #5F6368 — De-emphasized text, metadata

**Accent Colors:**
- Link Blue: #8AB4F8 — Interactive elements, links, "Follow" buttons
- Team Accent Red: #DC143C — Team branding highlights
- Status Green: #34A853 — Live status, positive states
- Live Red: #EA4335 — "LIVE" indicators, urgent states

**State Colors:**
- Hover Overlay: rgba(232, 234, 237, 0.08) — Button/pill hover states
- Active Overlay: rgba(232, 234, 237, 0.12) — Active/selected states
- Card Hover: rgba(255, 255, 255, 0.02) — Subtle card hover effects

## Typography

**Font Families:**
- Primary: "Roboto", -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
- Monospace: "Roboto Mono", monospace — Score displays

**Type Scale:**
- Display Large: 64px, 400, 1.0 — Live game scores
- Heading 1: 24px, 400, 1.33 — Team names, page titles
- Heading 2: 18px, 400, 1.33 — Section headers
- Heading 3: 16px, 500, 1.5 — Card titles
- Body: 14px, 400, 1.43 — Standard text, navigation items
- Caption: 13px, 400, 1.54 — Records, timestamps
- Small: 12px, 400, 1.33 — Fine print, metadata

**Hierarchy Rules:**
- Scores use extremely large display type (64px+) with tabular/monospace numerals
- Team names are medium weight (400) at 24px
- Navigation and tabs are 14px regular weight
- Secondary information (records, standings) uses 13px captions
- Color contrast used for hierarchy: primary text (#E8EAED) > secondary (#9AA0A6) > tertiary (#5F6368)

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80

**Common Patterns:**
- Page padding: 16px mobile, 24px tablet+
- Card padding: 16px internal, 20px for larger cards
- Section spacing: 24-32px between major sections
- Component gaps: 8px between related items, 16px between sections
- Score card internal spacing: 24px vertical, 16px horizontal
- Navigation pills: 12px vertical padding, 20px horizontal padding

## Component Styles

### Score Card
- Background: #303134
- Border radius: 16px
- Padding: 24px
- Border: 1px solid #3C4043
- Contains: Team logos (48px), scores (64px), quarter information, standings table
- Hover: Subtle background lift to rgba(255, 255, 255, 0.02)

### Navigation Pills
- Background: Transparent default, #303134 when active
- Border radius: 20px (fully rounded)
- Padding: 12px vertical, 20px horizontal
- Text: 14px, 400 weight
- Active state: Background #303134, text remains #E8EAED
- Hover: Background rgba(232, 234, 237, 0.08)
- Border: 1px solid #3C4043 when active

### Action Buttons
- Primary style: Outlined with rounded corners
- Border radius: 20px (pill-shaped)
- Padding: 8px 16px
- Border: 1px solid #5F6368
- Text: 14px, 500 weight
- Hover: Border color to #8AB4F8, background rgba(138, 180, 248, 0.08)

### Input Fields (Search)
- Background: #303134
- Border radius: 24px (fully rounded)
- Padding: 12px 16px
- Border: None
- Placeholder: #5F6368
- Text: #E8EAED, 16px
- Icon size: 24px, color #9AA0A6

### Table/Standings
- Row height: 32px minimum
- Cell padding: 8px 12px
- Header text: #9AA0A6, 13px
- Data text: #E8EAED, 14px
- Border: None (relies on spacing)
- Hover row: Background rgba(255, 255, 255, 0.02)

### Status Badges
- "LIVE" indicator: Background #EA4335, text #FFFFFF
- "End of Q3" indicator: Background transparent, text #34A853
- Border radius: 4px for small badges
- Padding: 4px 8px
- Font: 12px, 500 weight

## Layout Principles

- Max content width: No strict max, fluid with padding constraints
- Grid structure: Single column mobile, adapts to multi-column on desktop
- Content padding: 16px mobile sides, increases with viewport
- Responsive behavior: Stacked vertical on mobile, horizontal score layout maintained
- Card spacing: 16px gaps between cards
- Alignment: Left-aligned text, centered scores in cards

## Visual Effects

- **Border Radius:** 
  - Pills/buttons: 20-24px (fully rounded)
  - Cards: 16px
  - Badges: 4px
  - Input fields: 24px
  
- **Shadows:** 
  - Cards: None (relies on background color difference)
  - Elevation indicated by background color shifts rather than shadows
  
- **Borders:** 
  - Width: 1px
  - Color: #3C4043 (subtle, low contrast)
  - Usage: Card outlines, active pill navigation, dividers
  
- **Backgrounds:** 
  - Solid colors only
  - Layering: #202124 (base) → #303134 (surface) → interaction states (overlays)
  - No gradients or textures

## Design Tone

Clean, information-dense sports interface with emphasis on readability and real-time data. The oversized score typography creates visual hierarchy and draws attention to live action. The dark theme reduces eye strain for extended viewing sessions. Pill-shaped navigation and rounded corners soften the technical nature of statistical displays. Color is used sparingly and purposefully—primarily for status indicators (live/final), interactive elements, and team branding accents.

## Usage Notes for AI Implementation

- Score displays should always use the largest typography size (64px minimum) for maximum readability
- Navigation pills should feel tactile with clear active/inactive states
- Maintain high contrast between text and backgrounds (minimum 7:1 for scores, 4.5:1 for body text)
- Use tabular/monospace numerals for scores and statistical data to ensure alignment
- Team logos should be 48-56px for balance with large score typography
- Status indicators ("LIVE", "Final", quarter updates) should use color to convey meaning
- Tables should be clean and scannable—rely on spacing rather than heavy borders
- Interactive elements (pills, buttons) should use the 20-24px border radius for the pill effect
- Keep information density high but organized through card-based grouping
- Mobile-first: ensure touch targets are 44px minimum, scores remain prominent at small sizes
