---
id: dark-podcast-001
title: Midnight Audio Hub
description: A sleek, dark-themed media player interface with vibrant content cards and subtle depth
tags: [dark, media, cards, mobile-first, entertainment]
colors: ["#000000", "#1C1C1E", "#2C2C2E", "#FFFFFF", "#8E8E93", "#FF9500"]
created: 2026-01-04
---

# Midnight Audio Hub

A sophisticated dark-mode media interface designed for content discovery and playback. The system uses true black backgrounds to maximize OLED efficiency while employing vibrant, colorful content cards that pop against the darkness. Typography is clean and hierarchical, with clear distinctions between section headers, titles, and metadata.

## Color Palette

**Primary Colors:**
- Background Primary: #000000 — True black, main app background
- Background Elevated: #1C1C1E — Slightly lifted surfaces, cards in some contexts
- Background Tertiary: #2C2C2E — Card backgrounds, elevated containers

**Text Colors:**
- Text Primary: #FFFFFF — Headings, primary content
- Text Secondary: #8E8E93 — Metadata, timestamps, subtitles
- Text Tertiary: #636366 — Disabled states, hints

**Accent Colors:**
- Accent Orange: #FF9500 — Progress indicators, highlights, badges
- Accent White: #FFFFFF — Active icons, selected states

**Content Card Colors (for reference):**
- Vibrant Orange: #E8923A — Warm content cards
- Vibrant Blue: #0066CC — Cool content cards
- Vibrant Red: #D62828 — Alert/bold content cards

**UI Element Colors:**
- Separator: #38383A — Subtle dividers
- Icon Default: #8E8E93 — Inactive icons
- Icon Active: #FFFFFF — Selected navigation items
- Pill Background: rgba(255, 255, 255, 0.2) — Button overlays on cards

## Typography

**Font Families:**
- Primary: SF Pro Display / SF Pro Text (system San Francisco font)
- Fallback: -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif

**Type Scale:**
- Display/Page Title: 34px, weight 700 (bold), line-height 1.2
- Section Header: 22px, weight 600 (semibold), line-height 1.3
- Card Title: 17px, weight 600 (semibold), line-height 1.35
- Body/Description: 15px, weight 400 (regular), line-height 1.4
- Caption/Metadata: 13px, weight 500 (medium), line-height 1.3, letter-spacing 0.02em
- Tab Label: 11px, weight 500 (medium), line-height 1.2

**Hierarchy Rules:**
- Page titles are large and bold, positioned with generous top padding
- Section headers use semibold weight with arrow chevrons indicating expandability
- Card titles are compact but readable, limited to 2 lines with ellipsis truncation
- Metadata uses uppercase for labels (RESUME, NEW) with bullet separators

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 48

**Common Patterns:**
- Screen edge padding: 16px horizontal
- Section vertical spacing: 24px between sections
- Card internal padding: 12-16px
- Card gap in horizontal scroll: 12px
- Bottom navigation padding: 8px top, safe area bottom
- Card corner radius: 12px
- Pill/button corner radius: 16px (fully rounded)

## Component Styles

### Content Cards (Large)
- Background: Vibrant imagery or solid color
- Corner radius: 12px
- Aspect ratio: ~4:5 for featured cards
- Shadow: Subtle, 0 4px 12px rgba(0,0,0,0.3)
- Overlay gradient: Linear from transparent to rgba(0,0,0,0.6) at bottom
- Title position: Bottom-aligned within card
- Metadata: Uppercase label + bullet + timestamp

### Content Cards (Small/Grid)
- Background: Content imagery
- Corner radius: 8px
- Aspect ratio: 1:1 (square)
- Border: 1px solid rgba(255,255,255,0.1) on some variants
- Category label below: 15px, secondary color
- Update frequency: 13px, tertiary color

### Playback Control Pills
- Background: rgba(255, 255, 255, 0.2) — frosted appearance
- Corner radius: 16px (fully rounded)
- Padding: 8px 12px
- Icon + text layout: Horizontal with 6px gap
- Progress indicator: Orange accent line

### Bottom Tab Bar
- Background: #000000 with subtle top border
- Height: 49px + safe area
- Icon size: 24px
- Label size: 11px
- Active state: White icon + label
- Inactive state: Gray (#8E8E93) icon + label
- Items: 4 equal-width sections

### Now Playing Bar
- Background: #1C1C1E
- Corner radius: 12px (top corners only when docked)
- Height: ~64px
- Layout: Thumbnail (40px) + title stack + controls
- Controls: Play button + skip 30s

### Section Headers
- Layout: Text + chevron icon
- Text: 22px semibold white
- Chevron: 18px, slightly smaller, same color
- Subtitle (optional): 15px secondary color below

## Layout Principles

- **Max content width:** Full screen on mobile, constrained on tablet
- **Grid structure:** Horizontal scroll carousels for content discovery
- **Scroll behavior:** Horizontal scroll with snap points on cards
- **Vertical sections:** Stack with 24px spacing
- **Card overflow:** Peek of next card visible (encourages scrolling)
- **Safe areas:** Respects iOS safe area insets top and bottom

## Visual Effects

- **Border Radius:** 
  - Cards: 12px
  - Pills/buttons: 16px (fully rounded)
  - Thumbnails: 8px
  - Avatar: 50% (circular)
  
- **Shadows:** 
  - Cards: 0 4px 12px rgba(0,0,0,0.3)
  - Now playing bar: 0 -4px 12px rgba(0,0,0,0.2)
  
- **Borders:** 
  - Subtle separators: 1px #38383A
  - Card borders (optional): 1px rgba(255,255,255,0.1)
  
- **Backgrounds:** 
  - True black (#000000) for maximum OLED efficiency
  - Elevated surfaces use subtle gray lift
  - Content cards use vibrant, saturated colors

- **Overlays:**
  - Card gradient: linear-gradient(transparent 40%, rgba(0,0,0,0.7) 100%)
  - Frosted glass effect on pills: backdrop-filter blur where supported

## Design Tone

This interface embodies a premium, content-forward media experience. The true black background creates an immersive canvas that makes colorful content artwork the star of the show. The design is confident and minimal — relying on typography hierarchy and spacing rather than decorative elements. It feels native to iOS while maintaining a distinctive personality through its bold color choices and refined micro-interactions.

## Usage Notes for AI Implementation

When implementing this system, prioritize contrast ratios for accessibility — white text on dark backgrounds must maintain 4.5:1 minimum. Use the horizontal scroll pattern for content discovery sections, always showing a partial peek of the next item. The true black background is essential for the premium feel — avoid dark grays for the main background. Content cards should use vibrant, saturated artwork colors that pop against the black. For the bottom tab bar, ensure the active state is immediately distinguishable through both color and potentially subtle weight changes. The now-playing bar should be sticky at the bottom, above the tab bar, and collapse/expand smoothly.
