---
id: dark-developer-terminal-001
title: Carbon Terminal System
description: A minimal dark interface with monospace typography and terminal-inspired aesthetics for developer tools
tags: [dark, minimal, developer, monospace, terminal]
colors: ["#000000", "#171717", "#262626", "#A3A3A3", "#FFFFFF", "#525252"]
created: 2025-02-04
---

# Carbon Terminal System

A stark, high-contrast dark interface built around monospace typography and terminal-inspired design patterns. The system emphasizes information density, scannable lists, and developer-familiar interactions like code snippets and command-line syntax.

## Color Palette

**Primary Colors:**
- Background: #000000 — Primary page background, pure black
- Surface: #171717 — Elevated surfaces, code blocks, input fields
- Surface Elevated: #262626 — Cards, interactive elements on hover

**Text Colors:**
- Text Primary: #FFFFFF — Headings, primary content, high emphasis
- Text Secondary: #A3A3A3 — Labels, descriptions, metadata
- Text Tertiary: #525252 — Disabled states, subtle hints

**Border & Divider Colors:**
- Border Default: #262626 — Subtle dividers between list items
- Border Strong: #404040 — Input field borders, card outlines

**Accent Colors:**
- Accent Primary: #FFFFFF — Active states, selected tabs (underline)
- Code Syntax: #22D3EE — Terminal prompt symbols, code highlights (cyan)

**State Colors:**
- Success: #22C55E — Positive metrics, confirmations
- Warning: #F59E0B — Caution states
- Error: #EF4444 — Error states, destructive actions

## Typography

**Font Families:**
- Primary: SF Mono, JetBrains Mono, Fira Code, or similar monospace
- All text uses monospace — headings, body, labels, and code

**Type Scale:**
- Display/Hero: 24px, 600 weight, 1.2 line-height
- Section Headers: 12px, 500 weight, 1.5 line-height, uppercase, letter-spacing: 0.1em
- List Item Title: 16px, 600 weight, 1.4 line-height
- List Item Subtitle: 14px, 400 weight, 1.4 line-height
- Body: 14px, 400 weight, 1.5 line-height
- Caption/Small: 12px, 400 weight, 1.4 line-height
- Metrics/Numbers: 16px, 500 weight, tabular-nums

**Hierarchy Rules:**
- Section labels use ALL CAPS with generous letter-spacing (0.05-0.1em)
- List items use bold title + muted subtitle pattern
- Numbers and metrics right-aligned with tabular figures
- Minimal font weight variation — hierarchy through size and color

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 48, 64

**Common Patterns:**
- Page horizontal padding: 24px (mobile), 32px (desktop)
- Section vertical spacing: 32px between sections
- List item padding: 16px vertical, 0 horizontal
- Code block padding: 16px all sides
- Icon spacing: 24px between icon items in horizontal row
- Search field padding: 12px vertical, 16px horizontal

## Component Styles

### Breadcrumb Navigation
- Font: 16px monospace, 500 weight
- Separator: "/" with 8px horizontal margin
- Color: #FFFFFF for current, #A3A3A3 for parents
- Icon: Triangular logo mark, 24px

### Code Blocks / Command Display
- Background: #171717
- Border-radius: 8px
- Padding: 16px
- Font: 14px monospace
- Prompt symbol: "$" in default text color
- Copy button: Ghost icon button, right-aligned

### Search Input
- Background: transparent
- Border-bottom: 1px solid #262626
- Padding: 12px 0
- Icon: Search icon, 16px, #A3A3A3
- Placeholder: #525252, 14px monospace

### Tab Bar / Filter Tabs
- Layout: Horizontal, left-aligned
- Font: 14px monospace
- Inactive: #A3A3A3
- Active: #FFFFFF with 2px bottom border
- Spacing: 24px between tabs
- Include counts in parentheses: "All Time (39,874)"

### Leaderboard / Ranked List
- Layout: Full-width rows with bottom border
- Rank number: 16px, #A3A3A3, left column (24px width)
- Title: 16px, 600 weight, #FFFFFF
- Subtitle: 14px, 400 weight, #A3A3A3
- Metric: 16px, 500 weight, #FFFFFF, right-aligned
- Row padding: 16px vertical
- Border: 1px solid #262626 bottom

### Icon Row / Agent Badges
- Layout: Horizontal flex, 48px gap
- Icon size: 24px
- Icon color: #A3A3A3
- Background: none (transparent)

### Bottom Navigation Bar (Mobile)
- Background: #000000 with subtle top blur
- Height: 64px + safe area
- Items: Icon buttons with pill-shaped active state
- Active pill: #262626 background, rounded-full
- Center element: Domain label with refresh icon

## Layout Principles

- Max content width: 720px for content, full-width for navigation
- Grid structure: Single column, linear vertical scroll
- Alignment: Left-aligned text, right-aligned metrics
- Visual rhythm: Consistent 16px vertical spacing for list items
- Information density: High — many items visible at once

## Visual Effects

- **Border Radius:** 8px for containers/code blocks, 9999px (pill) for buttons/tags
- **Shadows:** None — flat design with border separation
- **Borders:** 1px solid, used for dividers and input underlines
- **Backgrounds:** Solid colors only, no gradients
- **Icons:** Outlined style, 1.5-2px stroke weight

## Design Tone

Utilitarian and developer-centric. The interface feels like a well-designed terminal or IDE — information-dense but scannable, with monospace typography creating a technical, code-native atmosphere. The pure black background and high contrast create sharp visual separation, while the minimal decoration keeps focus on content and data.

## Usage Notes for AI Implementation

This system works best for developer tools, documentation sites, dashboards with ranked/listed data, and technical product interfaces. Key principles:

1. **Use monospace everywhere** — Even for UI labels and navigation, not just code
2. **Embrace information density** — Tight spacing, many visible items
3. **Minimize decoration** — Let typography and spacing create hierarchy
4. **Right-align numbers** — Use tabular figures for aligned metrics
5. **Use uppercase sparingly** — Only for section labels, with letter-spacing
6. **Keep interactions subtle** — Simple hover states, underline for active tabs
7. **Mobile-first lists** — Optimized for vertical scrolling on touch devices
