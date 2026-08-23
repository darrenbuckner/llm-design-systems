---
id: dark-marketplace-001
title: Midnight Marketplace System
description: A sophisticated dark-themed marketplace interface with premium card layouts and data-driven components
tags: dark, premium, data-heavy, marketplace, cards
colors: #0A0A0A, #1E1E22, #2D2D35, #FF8C00, #FFFFFF
created: 2024-12-10
---

# Midnight Marketplace System

A sophisticated dark-themed design system built for data-heavy marketplace interfaces. Features deep blacks with layered transparency, premium rounded cards, and clear data hierarchies perfect for showcasing metrics and listings.

## Color Palette

**Primary Colors:**
- Background Primary: #0A0A0A — Main application background, deepest layer
- Background Secondary: #1E1E22 — Card backgrounds, elevated surfaces
- Background Tertiary: #2D2D35 — Input fields, nested containers
- Accent Primary: #FF8C00 — Status tags, important indicators, "FOR SALE" badges

**Neutral Colors:**
- Text Primary: #FFFFFF — Headings, primary content, high-emphasis text
- Text Secondary: #A0A0A8 — Body text, descriptions, secondary information
- Text Tertiary: #6B6B73 — Placeholder text, de-emphasized content
- Border/Divider: #2D2D35 — Subtle separators, component borders

**Semantic Colors:**
- Success/Positive: #10B981 — Positive metrics, growth indicators
- Warning: #F59E0B — Attention states
- Info: #3B82F6 — Informational accents

## Typography

**Font Families:**
- Primary: System UI fonts (SF Pro, Inter, or Roboto style)
- Monospace: Monospace/Code fonts for API keys and technical content

**Type Scale:**
- Display/Hero: 32px, weight 600, line-height 1.2 — Section headers like "Leaderboard"
- Heading 1: 24px, weight 600, line-height 1.3 — Card titles, startup names
- Heading 2: 18px, weight 600, line-height 1.4 — Modal titles "Add your startup"
- Body Large: 16px, weight 400, line-height 1.5 — Primary descriptions
- Body: 14px, weight 400, line-height 1.5 — Standard text, form labels
- Caption/Small: 12px, weight 500, line-height 1.4 — Category tags, uppercase labels
- Micro: 11px, weight 400, line-height 1.4 — Helper text, metadata

**Hierarchy Rules:**
- Primary headings use weight 600 for clear emphasis
- Uppercase styling at 12px for category labels and table headers
- Monospace for technical content (API keys, code snippets)
- Gray text (#A0A0A8) for secondary information
- White text (#FFFFFF) for primary emphasis

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

**Common Patterns:**
- Card padding: 24px all sides
- Section spacing: 32-48px between major sections
- Component gap: 16px between related elements
- Inline spacing: 8-12px for tight groups
- Search input padding: 16px vertical, 20px horizontal
- Button padding: 12px vertical, 24px horizontal
- Modal padding: 32px all sides

## Component Styles

### Cards (Listing Cards)
- **Background:** #1E1E22 with slight transparency
- **Border-radius:** 20px (generous rounding)
- **Padding:** 24px
- **Structure:** 
  - Logo/icon top (48-64px circle)
  - Title + category below
  - Metrics grid (3 columns: REVENUE, PRICE, MULTIPLE)
  - "FOR SALE" tag positioned top-right
- **Shadow:** Subtle 0 4px 24px rgba(0,0,0,0.3)
- **Hover:** Slight scale (1.02) or border highlight

### Buttons

**Primary Button (CTA):**
- Background: #FFFFFF (light) or #2D2D35 (dark variant)
- Text: #0A0A0A or #FFFFFF
- Border-radius: 12px
- Padding: 12px vertical, 32px horizontal
- Font: 14px, weight 600
- Hover: Slight opacity change (0.9)

**Secondary Button:**
- Background: Transparent
- Border: 1px solid #2D2D35
- Text: #FFFFFF
- Same dimensions as primary

### Input Fields
- **Background:** #2D2D35 (elevated from card background)
- **Border:** None (borderless design) or 1px solid #3D3D45
- **Border-radius:** 12px
- **Padding:** 16px vertical, 20px horizontal
- **Text:** 14px, #FFFFFF
- **Placeholder:** 14px, #6B6B73
- **Focus:** Border highlight #4D4D55 or subtle glow

### Search Bar
- **Style:** Large prominent input
- **Icon:** Search icon left-aligned, 20px
- **Placeholder:** Descriptive, lowercase style
- **Width:** Full-width or max 600px centered
- **Height:** 56px minimum

### Navigation Pills (Chip Tabs)
- **Background:** #1E1E22 or #2D2D35
- **Border-radius:** 16px (pill shape)
- **Padding:** 12px horizontal, 8px vertical
- **Text:** 14px, weight 500
- **Icon:** 20px, left-aligned
- **Hover:** Background lightens slightly
- **Active:** Brighter background or border accent

### Status Tags
- **"FOR SALE" Badge:**
  - Background: #FF8C00
  - Text: #FFFFFF, 11px, weight 700, uppercase
  - Padding: 6px 12px
  - Border-radius: 6px
  - Position: Absolute top-right of cards

### Modal/Dialog
- **Background:** #1E1E22
- **Border-radius:** 24px (top corners)
- **Padding:** 32px
- **Overlay:** rgba(0,0,0,0.7) backdrop
- **Max-width:** 600px
- **Close button:** X icon top-right, 24px

### Dropdown/Select
- **Background:** #2D2D35
- **Border-radius:** 12px
- **Padding:** 12px 16px
- **Chevron icon:** Right-aligned
- **Text:** 14px, #FFFFFF
- **Options:** Dropdown list with hover states

### Data Grid (Metrics Display)
- **Layout:** 3-column grid
- **Column gap:** 32px
- **Label:** Uppercase, 11px, #6B6B73, weight 600
- **Value:** 20-24px, weight 700, #FFFFFF
- **Alignment:** Left-aligned in columns

## Layout Principles

- **Max content width:** 1200px for main content area
- **Grid structure:** Flexible card grid, 2-3 columns responsive
- **Responsive behavior:** 
  - Desktop: 3-column card layout
  - Tablet: 2-column
  - Mobile: Single column stacked
- **Alignment:** Left-aligned content, centered modals
- **Scrolling:** Smooth scroll, sticky navigation possible
- **Density:** Generous spacing, not cramped

## Visual Effects

- **Border Radius:** 
  - Cards/major components: 20px
  - Buttons/inputs: 12px
  - Pills/tags: 16px (pill shape)
  - Small badges: 6px
  - Modals: 24px
- **Shadows:** 
  - Elevated cards: 0 4px 24px rgba(0,0,0,0.3)
  - Modals: 0 8px 48px rgba(0,0,0,0.5)
  - Subtle: 0 2px 8px rgba(0,0,0,0.2)
- **Borders:** 
  - Primarily borderless design
  - Subtle borders when needed: 1px solid #2D2D35
  - Used for input focus states and dividers
- **Backgrounds:** 
  - Solid dark colors with layered transparency
  - No gradients in main interface
  - Slight transparency on overlays (rgba)
- **Transitions:**
  - Smooth 200ms ease for hover states
  - Scale transforms on cards (1.02)
  - Opacity fades for modals

## Design Tone

This system embodies a premium, data-centric marketplace aesthetic with sophisticated dark theming. The deep black backgrounds create focus, while generous rounded corners and ample spacing convey a modern, polished feel. Orange accent tags provide visual hierarchy without overwhelming the interface. The design balances dense information display with breathing room, making it ideal for platforms showcasing metrics, listings, and transactional data.

## Usage Notes for AI Implementation

When implementing this system:
1. **Maintain the deep dark hierarchy** — Use #0A0A0A as base, #1E1E22 for cards, #2D2D35 for inputs
2. **Orange sparingly** — Reserve #FF8C00 for critical status indicators only
3. **Round everything generously** — 20px on cards creates the premium feel
4. **White text for primary content** — Gray (#A0A0A8) for secondary only
5. **Metrics display needs emphasis** — Large bold numbers (20-24px, weight 700)
6. **Monospace for technical content** — API keys, codes, technical identifiers
7. **Card hover states** — Subtle scale or border highlight, never dramatic
8. **Consistent 24px card padding** — Creates uniform rhythm across components
9. **Search should feel prominent** — Large, borderless, with clear placeholder
10. **Modal overlays need strong backdrop** — 70% black overlay for focus
