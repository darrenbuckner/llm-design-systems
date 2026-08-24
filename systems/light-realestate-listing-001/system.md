---
id: light-realestate-listing-001
title: Riverstone Listings
description: Clean, card-based property listing interface with subtle shadows and clear information hierarchy
tags: [light, minimal, cards, mobile-first, real-estate]
colors: ["#FFFFFF", "#F7F7F7", "#2D2D2D", "#6B7280", "#007A5C", "#C82333", "#E5E7EB"]
created: 2026-01-16
---

# Riverstone Listings

A clean, mobile-first listing interface designed for property discovery. The system emphasizes readability and quick scanning through strong typographic hierarchy, subtle card elevations, and strategic use of accent colors for calls-to-action. The design feels trustworthy and professional while remaining approachable.

## Color Palette

**Primary Colors:**
- Primary Green: #007A5C — Primary accent, links, positive indicators, status badges
- Primary Red: #C82333 — Primary CTA buttons, urgency indicators

**Neutral Colors:**
- Background: #FFFFFF — Main page background
- Surface/Card: #FFFFFF — Card backgrounds with shadow elevation
- Surface Muted: #F7F7F7 — Subtle section backgrounds, summary cards
- Text Primary: #2D2D2D — Headlines, prices, key information
- Text Secondary: #6B7280 — Supporting text, metadata, descriptions
- Border: #E5E7EB — Card borders, dividers, input outlines

**Semantic Colors:**
- Success/Active: #007A5C — "For Sale" status, links
- Action/Urgent: #C82333 — Primary action buttons
- Info Accent: #E85D5D — Trend indicators, popularity markers (coral/salmon variant)

## Typography

**Font Families:**
- Primary: System UI / -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif
- The interface uses system fonts for optimal performance and native feel

**Type Scale:**
- Display/Price: 32px, weight 700, line-height 1.2 — Large monetary values
- Heading 1: 24px, weight 700, line-height 1.3 — Section titles ("About this home")
- Heading 2: 18px, weight 600, line-height 1.4 — Card titles, summary headers
- Body: 16px, weight 400, line-height 1.6 — Description text, details
- Body Small: 14px, weight 400, line-height 1.5 — Metadata, specs, secondary info
- Caption: 12px, weight 500, line-height 1.4 — Labels, status badges, fine print

**Hierarchy Rules:**
- Prices and key numbers use extra-bold weight for immediate scanning
- Section headings are bold but not oversized, maintaining reading flow
- Body text has generous line-height for comfortable reading
- Links and interactive text use color (green) rather than underlines
- Bullet points use standard disc markers with adequate spacing

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 48, 64

**Common Patterns:**
- Card internal padding: 16-20px
- Section spacing: 24-32px between major sections
- Component gaps: 8-12px between related elements
- List item spacing: 12px between bullet points
- Button padding: 16px vertical, 24px horizontal
- Screen edge padding: 16px on mobile

**Specific Measurements:**
- Card margin from edges: 16px
- Space between cards: 12px
- Icon to text spacing: 12px
- Price to specs spacing: 8px

## Component Styles

### Status Badge
- Background: transparent
- Text color: #2D2D2D
- Font size: 12px, weight 500, uppercase tracking
- Green dot indicator: 8px circle, #007A5C
- Dot spacing: 8px from text

### Price Display
- Font size: 32px
- Font weight: 700
- Color: #2D2D2D
- Letter-spacing: -0.5px (slightly tight)

### Property Specs Row
- Format: "X bd • Y ba • Z sq ft"
- Separator: bullet point (•) with 8px spacing
- Font size: 16px
- Font weight: 600
- Color: #2D2D2D

### Cards
- Background: #FFFFFF
- Border: 1px solid #E5E7EB
- Border radius: 12px
- Shadow: 0 1px 3px rgba(0,0,0,0.08)
- Padding: 16-20px
- Margin between cards: 12px

### Summary Card (Nested)
- Background: #F7F7F7
- Border: none
- Border radius: 8px
- Padding: 16px
- Nested within parent card

### Buttons

**Primary Button (Filled):**
- Background: #C82333
- Text: #FFFFFF
- Font size: 16px
- Font weight: 600
- Padding: 16px 24px
- Border radius: 24px (pill shape)
- Full width on mobile or flex-grow

**Secondary Button (Outlined):**
- Background: transparent
- Border: 1.5px solid #2D2D2D
- Text: #2D2D2D
- Font size: 16px
- Font weight: 600
- Padding: 16px 24px
- Border radius: 24px (pill shape)

**Text Button/Link:**
- Color: #007A5C
- Font size: 16px
- Font weight: 600
- No underline
- Chevron icon for expandable sections

### Navigation Header
- Background: #FFFFFF
- Height: 56px
- Border bottom: none (or very subtle)
- Back arrow: 24px, #2D2D2D
- Title: 16px, weight 400
- Action icons: 24px, #2D2D2D, spaced 16px apart

### Map Thumbnail
- Border radius: 8px
- Size: ~120px width, aspect ratio maintained
- Position: Top right of listing header
- Shows location pin in brand green

### Popularity Indicator
- Icon: Chart/trending icon in coral (#E85D5D)
- Text: "This home is popular" in bold
- Subtext: Regular weight with green link
- Layout: Icon left, text stack right
- Container: Full-width card section

## Layout Principles

- **Max content width:** Full width on mobile, 600px max on tablet+
- **Grid structure:** Single column, card-based layout
- **Responsive behavior:** Mobile-first, stacks vertically
- **Alignment:** Left-aligned text, full-width cards
- **Fixed elements:** Bottom action bar with dual buttons

**Card Stacking Pattern:**
1. Header area (no card) - status, price, specs, address
2. Popularity card
3. About section card with nested summary card
4. Action buttons (fixed or inline)

## Visual Effects

**Border Radius:**
- Cards: 12px
- Nested cards: 8px
- Buttons: 24px (pill)
- Map thumbnails: 8px
- Status dot: 50% (circle)

**Shadows:**
- Card shadow: 0 1px 3px rgba(0,0,0,0.08)
- No heavy shadows — very subtle elevation
- Pressed states: inset subtle shadow

**Borders:**
- Card borders: 1px solid #E5E7EB
- Button outlines: 1.5px solid #2D2D2D
- Dividers: 1px solid #E5E7EB

**Backgrounds:**
- Solid white primary
- Light gray (#F7F7F7) for nested/summary sections
- No gradients in main UI

## Design Tone

Clean, trustworthy, and efficient. The interface prioritizes scanability with bold prices and clear hierarchy, while maintaining warmth through rounded corners and the coral/green accent palette. It feels modern but not trendy — designed to build confidence in high-stakes decisions. The mobile-first approach shows respect for users' time and context.

## Usage Notes for AI Implementation

1. **Price prominence:** Always make prices the largest, boldest element — users scan for this first
2. **Card hierarchy:** Use border + subtle shadow for primary cards, background color change for nested/secondary information
3. **CTA pairing:** Pair a high-contrast filled button with an outlined secondary option for clear action hierarchy
4. **Status indicators:** Use small colored dots + text rather than full badges for listing status
5. **Link styling:** Green text without underlines for inline links; add chevrons for expandable sections
6. **Mobile bottom bar:** Fixed position CTAs work well on mobile when space allows
7. **Bullet lists:** Standard disc markers with comfortable 12px spacing for feature lists
8. **Map integration:** Small thumbnail maps in corners help spatial orientation without dominating
9. **System fonts:** Use system font stack for optimal performance and native feel on mobile
10. **Generous touch targets:** Buttons should be at least 48px tall for comfortable mobile tapping
