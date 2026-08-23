---
id: dark-builder-001
title: Forge Builder System
description: A sophisticated dark interface for creative tool builders with subtle depth and clean hierarchy
tags: [dark, minimal, mobile-first, builder, input-focused]
colors: ["#000000", "#1A1A1A", "#2A2A2A", "#3A3A3A", "#FFFFFF", "#A0A0A0", "#666666"]
created: 2025-01-04
---

# Forge Builder System

A refined dark interface designed for creative building tools. Features a true black background with subtle gray card elevations, creating depth without distraction. The system emphasizes input-focused workflows with clean segmented controls and minimal iconography.

## Color Palette

**Primary Colors:**
- Background: #000000 — True black base, maximum contrast foundation
- Surface Primary: #1A1A1A — Elevated cards and containers
- Surface Secondary: #2A2A2A — Active/selected tab backgrounds
- Surface Tertiary: #3A3A3A — Borders and subtle dividers

**Text Colors:**
- Text Primary: #FFFFFF — Headlines and primary content
- Text Secondary: #A0A0A0 — Body text, placeholders, descriptions
- Text Tertiary: #666666 — Subtle labels, inactive states

**Neutral Grays:**
- Border Light: #3A3A3A — Card borders, dividers
- Border Dark: #2A2A2A — Subtle separations
- Icon Default: #A0A0A0 — Standard icon color
- Icon Active: #FFFFFF — Active/selected icons

**State Colors:**
- Active Tab: #2A2A2A with #FFFFFF text
- Inactive Tab: Transparent with #A0A0A0 text
- Bottom Bar Active: #3A3A3A background
- Disabled: #666666

## Typography

**Font Families:**
- Primary: Inter, -apple-system, BlinkMacSystemFont, system-ui, sans-serif
- Monospace: SF Mono, Monaco, monospace (for code contexts)

**Type Scale:**
- Display: 24px, 600 weight, 1.3 line-height — Main greeting headlines
- Heading 1: 20px, 600 weight, 1.4 line-height — Section titles
- Heading 2: 16px, 500 weight, 1.4 line-height — Card headers
- Body: 15px, 400 weight, 1.5 line-height — Descriptions, placeholders
- Label: 14px, 500 weight, 1.4 line-height — Tab labels, buttons
- Caption: 12px, 400 weight, 1.4 line-height — Bottom nav labels

**Hierarchy Rules:**
- Headlines use 600 weight for prominence on dark backgrounds
- Body text uses reduced opacity (#A0A0A0) rather than lighter weight
- All caps avoided; sentence case throughout
- Center-aligned headlines for greeting/onboarding contexts

## Spacing System

**Base Unit:** 4px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 48, 64

**Common Patterns:**
- Card padding: 16px horizontal, 12px vertical
- Section spacing: 24px between major sections
- Icon spacing: 8px from labels
- Tab internal padding: 12px vertical, 24px horizontal
- Bottom nav item spacing: Equal distribution with 48px tap targets
- Container horizontal padding: 20px on mobile

## Component Styles

### Workspace Selector (Pill)
- Background: #2A2A2A
- Border-radius: 24px (full pill)
- Padding: 8px 16px
- Avatar circle: 32px, background #3A3A3A
- Text: 14px, #FFFFFF
- Includes overflow menu (three dots)

### Segmented Control (Tabs)
- Container: Background #1A1A1A, border-radius 12px, border 1px solid #2A2A2A
- Tab padding: 12px 24px
- Active state: Background #2A2A2A, text #FFFFFF
- Inactive state: Transparent, text #A0A0A0
- Icons: 18px, inline with 8px gap
- Border-radius on tabs: 8px

### Text Input Area
- Background: Transparent (inherits card)
- Placeholder: #666666, 15px
- No visible border on input itself
- Full-width within card container
- Min-height: 80px for multiline

### Toolbar Row
- Height: 48px
- Icon buttons: 24px icons, #A0A0A0 default
- Dropdown triggers: Icon + label + chevron
- Action button ("Start →"): Text only, #A0A0A0, right-aligned
- Separator: Visual grouping through spacing

### Bottom Navigation
- Background: #000000 with top border #1A1A1A
- Height: 80px (including safe area)
- Items: Icon (24px) + Label (12px), centered vertically
- Active state: Icon #FFFFFF
- Inactive state: Icon and label #666666
- Center action: 40px circle, border 1px #3A3A3A

### Cards
- Background: #1A1A1A
- Border: 1px solid #2A2A2A
- Border-radius: 16px
- Padding: 16px
- Shadow: None (elevation through color only)

### Dropdown Triggers
- Display: Icon + Label + Chevron
- Icon: 18px
- Label: 14px, #A0A0A0
- Chevron: 12px, #666666
- Gap: 6px between elements

## Layout Principles

- Full-width mobile layout, edge-to-edge dark background
- Content max-width: 100% on mobile, 480px centered on tablet+
- Vertical rhythm: 24px between major sections
- Cards have consistent 20px horizontal margin from screen edge
- Bottom navigation fixed, content scrolls beneath
- Safe area respected for notch/home indicator

## Visual Effects

**Border Radius:**
- Small (inputs, inner elements): 8px
- Medium (cards, tabs): 12px
- Large (main cards): 16px
- Full (pills, avatars): 50% or 24px+

**Shadows:**
- None used — elevation conveyed through background color steps
- True black (#000000) base makes gray surfaces appear elevated

**Borders:**
- Thickness: 1px throughout
- Style: Solid
- Color: #2A2A2A or #3A3A3A depending on context
- Used for: Card outlines, dividers, segmented control containers

**Backgrounds:**
- Solid colors only, no gradients
- Color steps: #000000 → #1A1A1A → #2A2A2A → #3A3A3A
- Each step represents one level of elevation

## Design Tone

This system embodies focused minimalism for creative workflows. The true black background creates a canvas-like environment where content and controls feel purposeful rather than decorative. Typography is clean and functional, avoiding flourishes. The overall impression is professional, modern, and distraction-free — letting the user's creation be the focus rather than the interface itself.

## Usage Notes for AI Implementation

When implementing this system, prioritize the elevation hierarchy: true black base, with each interactive layer stepping up through the gray scale. Avoid introducing new colors — the monochromatic palette is intentional for focus.

Segmented controls should feel chunky and tappable on mobile — generous padding is key. The pill-shaped workspace selector is a signature element; use it for any account/context switching UI.

Bottom navigation should always respect device safe areas. The center action button (circle with plus) is a floating creation trigger — use it for primary "new" actions.

Input areas are intentionally minimal — no visible borders, just placeholder text that's clearly differentiated from user input through color. The toolbar row beneath inputs provides contextual actions without cluttering the input space itself.

Icons should be outline-style, consistent weight, around 1.5-2px stroke. Avoid filled icons except for active/selected states in navigation.
