---
id: dark-minimal-snippet-022
title: Carbon Notes
description: A dark minimal interface for capturing and organizing text fragments with teal accents
tags: [dark, minimal, note-taking, monospace, teal-accent]
colors: ["#1A1D21", "#2A2F35", "#3ECFB2", "#FFFFFF", "#8A9199", "#F0C24E"]
created: 2026-01-10
---

# Carbon Notes

A focused, distraction-free dark interface designed for capturing and organizing text snippets. The system emphasizes content over chrome with a near-black background, subtle card separation, and distinctive teal accent color for interactive elements. Typography leans on monospace for input areas, creating a developer-friendly aesthetic.

## Color Palette

**Primary Colors:**
- Primary Accent: #3ECFB2 — Interactive elements, focus states, links, highlights
- Primary Dark: #2D9A86 — Hover states, secondary accent usage

**Background Colors:**
- Base Background: #1A1D21 — Main application background, deepest layer
- Card Surface: #2A2F35 — Elevated cards, input containers
- Input Background: #1A1D21 — Text input areas (same as base for seamless feel)

**Text Colors:**
- Text Primary: #FFFFFF — Headings, important content, primary labels
- Text Secondary: #8A9199 — Timestamps, metadata, secondary information
- Text Muted: #6B7280 — Placeholder text, disabled states

**Border Colors:**
- Border Default: #3ECFB2 — Active/focused input borders
- Border Subtle: #3A3F45 — Card borders, dividers
- Border Muted: #2A2F35 — Subtle separations

**Accent Colors:**
- Warning/Note: #F0C24E — Edit indicators, attention items
- Success: #3ECFB2 — Confirmation states (uses primary accent)
- Info Dot: #5BA4E6 — Unread/notification indicators

**Emoji Accents (UI Elements):**
- Fire: 🔥 — Streak/activity indicators
- Brain: 🧠 — Fragment/knowledge count
- Lightning: ⚡ — Peak activity, quick actions

## Typography

**Font Families:**
- Primary: System UI / -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
- Monospace: "SF Mono", "Monaco", "Inconsolata", "Fira Code", monospace — Used for input areas

**Type Scale:**
- App Title: 20px, weight 600, line-height 1.3
- Card Title: 16px, weight 500, line-height 1.4
- Body Text: 14px, weight 400, line-height 1.5
- Metadata: 13px, weight 400, line-height 1.4
- Stats Bar: 14px, weight 500, line-height 1.4

**Hierarchy Rules:**
- Titles use white (#FFFFFF) for maximum contrast
- Body content uses white for readability
- All metadata (dates, times) use secondary gray (#8A9199)
- Links inherit the teal accent color
- Placeholder text uses muted gray in monospace

## Spacing System

**Base Unit:** 4px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 48

**Common Patterns:**
- Card padding: 16px (all sides)
- Card gap/margin: 12px between cards
- Section padding: 24px horizontal container padding
- Stats bar padding: 12px vertical, 16px horizontal
- Input padding: 16px internal padding
- Button padding: 12px vertical, full-width

**Vertical Rhythm:**
- Between header and content: 16px
- Between cards: 12px
- Between text lines in card: 8px
- Between metadata items: 4px

## Component Styles

### Header Bar
```
Background: #1A1D21
Padding: 16px 20px
Layout: Center-aligned title with settings icon right
Title: 20px, weight 600, white, with emoji icon prefix
Stats row: Centered, items separated by dots
Stats text: 14px, secondary color with emoji prefixes
```

### Text Input Area
```
Background: #1A1D21 (matches page background)
Border: 2px solid #3ECFB2
Border Radius: 8px
Padding: 16px
Min Height: 120px
Font: Monospace, 14px, #6B7280 placeholder
Resize: Vertical allowed
Focus: Border color intensifies slightly
```

### Primary Button (Save)
```
Background: #2A2F35
Text: #FFFFFF, 15px, weight 500
Padding: 12px 24px
Border Radius: 8px
Width: 100%
Border: none
Hover: Background lightens to #3A3F45
Active: Slight scale down (0.98)
```

### Content Cards
```
Background: #2A2F35
Border Radius: 12px
Padding: 16px
Border: 1px solid transparent (or #3A3F45 subtle)
Margin Bottom: 12px

Content Layout:
- Title/URL: 16px, white, weight 500, top
- Body text: 14px, white, weight 400
- Metadata row: Bottom, flex space-between
  - Date: 13px, #8A9199, left
  - Time: 13px, #8A9199, right

Hover: Subtle background lighten or border appear
```

### Card with Actions
```
Same as content card plus:
- Action buttons: Right side of content, inline
- Icon buttons: 32px square, rounded
- Edit icon: Yellow/amber (#F0C24E)
- More menu: Ellipsis icon, same style
```

### Notification Dot
```
Size: 8px
Background: #5BA4E6
Border Radius: 50%
Position: Absolute, right edge of card
```

### Settings Icon
```
Size: 24px
Color: #8A9199
Position: Top right of header
Hover: Color lightens to white
```

## Layout Principles

**Container:**
- Max width: 100% (mobile-first, full bleed)
- Padding: 0 (cards go edge to edge with small margin)
- Background: #1A1D21

**Content Width:**
- Cards: Full width minus 16px margin each side
- Effective content: ~343px on mobile (375px - 32px)

**Grid Structure:**
- Single column layout
- Vertically stacked cards
- No multi-column breakpoints visible

**Alignment:**
- Header: Center-aligned
- Stats: Center-aligned with dot separators
- Cards: Left-aligned content
- Metadata: Space-between (date left, time right)

## Visual Effects

**Border Radius:**
- Cards: 12px
- Buttons: 8px
- Inputs: 8px
- Icon buttons: 8px
- Notification dots: 50% (circle)

**Shadows:**
- None visible — relies on background color differentiation
- Flat design aesthetic

**Borders:**
- Input focus: 2px solid #3ECFB2
- Cards: 1px solid transparent or very subtle #3A3F45
- Dividers: None (spacing creates separation)

**Backgrounds:**
- Solid colors only
- No gradients
- No patterns or textures
- Color layering creates depth (darker = further back)

## Design Tone

Carbon Notes embodies a focused, developer-friendly aesthetic that prioritizes content capture over visual decoration. The near-black background with teal accents creates a calm, low-eye-strain environment suitable for extended use. The monospace input field signals technical utility while the clean card-based layout keeps information scannable and organized. Emoji usage for stats adds personality without undermining the minimal, functional core.

## Usage Notes for AI Implementation

**When implementing this system:**

1. **Color Application:** Use the base background (#1A1D21) for the main canvas, card surface (#2A2F35) for elevated content containers. The teal accent (#3ECFB2) should be reserved for interactive states and focus indicators only — overuse dilutes its impact.

2. **Typography:** Default to system sans-serif for general UI. Switch to monospace only for user input areas where code or technical content is expected. Keep text sizes modest (14-16px) for the content-dense nature of note-taking.

3. **Card Design:** Cards should feel like they float slightly above the background through color alone, not shadows. The 12px border radius keeps things soft without being overly rounded.

4. **Interactive States:** Use the teal border for focus states on inputs. Buttons should subtly lighten on hover. Avoid dramatic state changes — keep interactions calm and predictable.

5. **Metadata Pattern:** Always position timestamps with date on left, time on right, using the secondary gray. This creates consistent scannability across cards.

6. **Mobile-First:** This system is designed for mobile-first usage. Cards span full width with minimal margins. Scale up for larger screens by adding max-width constraints and centering the container.

7. **Emoji Integration:** The emoji stats pattern (🔥 days, 🧠 fragments, ⚡ peak) adds personality. Use sparingly and consistently — they work as quick visual indicators, not decoration.
