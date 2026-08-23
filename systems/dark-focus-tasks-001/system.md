---
id: dark-focus-tasks
title: Focus Tasks Dark
description: Clean, focused task-oriented dark mode interface emphasizing calm productivity through generous spacing and restrained color palette
tags: dark, minimal, productivity, tasks, clean
colors: #FDB022, #1C1C1E, #2C2C2E, #3A3A3C, #FFFFFF, #8E8E93
created: 2024-12-14
---

# Focus Tasks Dark

Clean, focused, task-oriented dark mode interface that emphasizes calm productivity through generous spacing, soft borders instead of shadows, and a restrained color palette optimized for quick task review and completion.

## Color Palette

**Primary Colors:**
- Accent/Brand: #FDB022 — Used for icon branding and key visual markers
- Primary Action: #FFFFFF — Used for primary text and emphasis

**Neutral Colors:**
- Background Deep: #1C1C1E — Main application background
- Surface Dark: #2C2C2E — Card/elevated surface background
- Surface Darker: #1F1F21 — Slightly darker variant for depth
- Border Subtle: #3A3A3C — Card borders and dividers
- Text Primary: #FFFFFF — Main heading and body text
- Text Secondary: #8E8E93 — Placeholder and hint text
- Text Tertiary: #636366 — Subtle instructional text

**Interactive States:**
- Checkbox Inactive: #4A4A4C — Unchecked state border
- Checkbox Active: (Not visible in current state, likely brand color or white)

## Typography

**Font Families:**
- Primary: System font (SF Pro / Roboto equivalent) — Clean, highly legible sans-serif optimized for mobile

**Type Scale:**
- Page Title: 28px, Bold (600-700), 34px line-height
- Card Title: 24px, Bold (700), 30px line-height
- Body/Task Text: 20px, Medium (500), 28px line-height
- Footer Instructions: 15px, Regular (400), 20px line-height

**Hierarchy Rules:**
- Page title uses gray text with icon for branding, not maximum contrast
- Task cards use white text for maximum readability against dark surface
- All text is left-aligned within cards
- Footer instructions use significantly smaller, muted text

## Spacing System

**Base Unit:** 8px
**Scale:** 8, 16, 24, 32, 40, 48

**Common Patterns:**
- Card padding: 32px vertical, 28px horizontal
- Card spacing (between cards): 24px vertical gap
- Header spacing: 40px from top of screen to title
- Footer spacing: 32px from last card to instruction text
- Icon-to-text spacing: 16px horizontal
- Text line spacing within cards: 28px (tight, optimized for readability)

## Component Styles

### Task Cards
- Background: #2C2C2E
- Border: 1px solid #3A3A3C
- Border Radius: 16px
- Padding: 32px vertical, 28px horizontal
- Minimum height: ~150px (allows for 2-3 lines of text)
- Text color: #FFFFFF
- Font size: 20px
- Font weight: 500 (Medium)
- Line height: 28px

### Checkboxes
- Size: 28px × 28px
- Border: 2px solid #4A4A4C
- Border radius: 14px (perfectly circular)
- Position: Right-aligned, vertically centered within card
- Margin: 16px from right edge
- Checked state: (Not shown, but likely filled with brand color or white checkmark)

### Header Section
- Icon: 32px × 32px circular container with #FDB022 background
- Icon symbol: Lightning bolt, white fill
- Title text: "The Next Three" — #8E8E93 (secondary gray)
- Title size: 28px, Bold
- Refresh icon: Right-aligned, #8E8E93, ~24px size
- Vertical padding: 40px top, 48px bottom

### Footer Instructions
- Text: "Hold item to complete"
- Color: #636366 (tertiary gray)
- Size: 15px
- Weight: Regular (400)
- Alignment: Centered
- Position: Bottom of screen, 32px from bottom edge

## Layout Principles

- Max content width: Full screen width with 20px horizontal margins
- Vertical scroll: Content flows vertically with consistent spacing
- Safe areas: Respects iOS status bar (top) and home indicator (bottom)
- Card alignment: All cards aligned to same left/right margins
- Consistent card width: Cards stretch full width between margins
- Stacking: Cards stack vertically with equal spacing

## Visual Effects

**Border Radius:**
- Cards: 16px
- Checkboxes: 14px (circular)
- Icon container: 16px (circular)

**Shadows:**
- None — Flat design using borders for depth

**Borders:**
- Cards: 1px solid subtle gray (#3A3A3C)
- Checkboxes: 2px solid medium gray (#4A4A4C)

**Backgrounds:**
- Solid colors only, no gradients
- Layered depth: Background → Surface → No elevation shadows

## Design Tone

Clean, focused, task-oriented dark mode interface with minimal decoration. The design emphasizes calm productivity through generous spacing, soft borders instead of shadows, and a restrained color palette. The single accent color (golden yellow) provides just enough visual energy without distraction. The overall feel is modern, professional, and distraction-free — optimized for quick task review and completion.

## Usage Notes for AI Implementation

- Use the golden yellow (#FDB022) exclusively for branding elements and key icons — never for text or large fills
- Maintain high contrast between card backgrounds and app background to ensure clear card separation
- Text should always be white on dark card surfaces for maximum legibility
- Keep card padding generous (32px vertical) to prevent cramped feeling
- Checkboxes should be right-aligned and consistently positioned across all cards
- No shadows — use 1px borders to define edges and create subtle depth
- Interactive elements should have adequate touch targets (minimum 44px for mobile)
- Respect safe area insets on iOS devices for status bar and home indicator
- Footer instruction text should remain subtle and non-intrusive
