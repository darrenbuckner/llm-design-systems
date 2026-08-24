---
id: dark-streaming-entertainment-001
title: Thunderbolt Stream
description: A bold dark entertainment interface with electric teal accents, red CTAs, and high-contrast live content cards
tags: [dark, entertainment, streaming, bold, electric, live-content]
colors: ["#000000", "#1A1A1A", "#2D2D2D", "#00D4AA", "#E50914", "#FFFFFF"]
created: 2026-01-12
---

# Thunderbolt Stream

A high-energy dark entertainment interface designed for streaming platforms and live content. Features deep blacks with electric teal lightning accents, bold red call-to-action buttons, and clean navigation chips. The system emphasizes visual drama through hero content cards while maintaining functional clarity in navigation and secondary elements.

## Color Palette

**Primary Colors:**
- Background Primary: #000000 — Main app background, deep black for maximum contrast
- Background Secondary: #1A1A1A — Card backgrounds, elevated surfaces
- Background Tertiary: #2D2D2D — Navigation chips, subtle UI elements

**Accent Colors:**
- Electric Teal: #00D4AA — Lightning graphics, decorative accents, brand energy
- Live Red: #E50914 — Primary CTA buttons, live indicators, urgent actions
- Live Red Hover: #B8070F — Button hover states

**Text Colors:**
- Text Primary: #FFFFFF — Headlines, primary content, high emphasis
- Text Secondary: #B3B3B3 — Timestamps, metadata, secondary labels
- Text Muted: #808080 — Inactive states, placeholder text

**Surface Colors:**
- Card Surface: #141414 — Content cards, hero backgrounds
- Chip Surface: #2D2D2D — Filter chips, category buttons
- Chip Border: #404040 — Subtle borders on interactive chips

**State Colors:**
- Success: #46D369 — Confirmation states, positive indicators
- Warning: #F5A623 — Caution states, expiring content
- Error: #E50914 — Error states, shared with live/CTA red

## Typography

**Font Families:**
- Primary: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif (System UI stack)
- Display: Condensed sans-serif for dramatic titles (similar to Bebas Neue or similar condensed typeface)

**Type Scale:**
- Display Title: 48px, 800 weight, 1.0 line-height, uppercase, condensed — Hero show titles
- Section Header: 20px, 600 weight, 1.3 line-height — "For Parents", "Mobile Games"
- Chip Text: 15px, 500 weight, 1.2 line-height — Navigation chips
- Body: 16px, 400 weight, 1.5 line-height — Descriptions, metadata
- Caption: 14px, 400 weight, 1.4 line-height — Timestamps, small labels
- Button Text: 16px, 600 weight, 1.2 line-height — CTA buttons

**Hierarchy Rules:**
- Display titles use condensed typeface with dramatic visual weight
- Section headers use standard weight with generous letter-spacing
- Navigation and buttons use medium weight for clickable clarity
- High contrast white text on dark backgrounds throughout

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

**Common Patterns:**
- Screen edge padding: 16px (mobile), 24px (tablet), 48px (desktop)
- Section vertical spacing: 32px between major sections
- Card padding: 0px (full-bleed hero images)
- Chip padding: 12px horizontal, 8px vertical
- Button padding: 16px horizontal, 12px vertical
- Grid gap: 12px between game tiles
- Navigation chip gap: 12px

## Component Styles

### Navigation Chips
- Background: #2D2D2D
- Border: 1px solid #404040
- Border Radius: 20px (pill shape)
- Padding: 8px 16px
- Text: 15px, #FFFFFF, 500 weight
- Hover: Background lightens to #3D3D3D
- Active: Background #404040, border #505050

### Primary Button (Watch Live)
- Background: #E50914
- Border Radius: 4px
- Padding: 12px 24px
- Text: 16px, #FFFFFF, 600 weight
- Icon: Left-aligned with 8px gap
- Hover: Background #B8070F
- Active: Background #8C0610
- Shadow: none (flat design)

### Secondary Button (My List)
- Background: #2D2D2D
- Border: none
- Border Radius: 4px
- Padding: 12px 24px
- Text: 16px, #FFFFFF, 600 weight
- Icon: Left-aligned "+" with 8px gap
- Hover: Background #404040

### Hero Content Card
- Background: #141414
- Border Radius: 8px
- Overflow: hidden
- Aspect Ratio: approximately 16:10 for hero
- Image: Full-bleed, object-fit cover
- Gradient Overlay: Linear gradient from transparent to rgba(0,0,0,0.8) at bottom
- Content positioning: Centered, bottom-aligned

### Game Tile Grid
- Tile Size: Square aspect ratio, approximately 100px
- Border Radius: 8px
- Overflow: hidden
- Gap: 12px
- Shadow: subtle drop shadow on hover

### Bottom Navigation
- Background: #141414
- Height: 64px + safe area
- Items: Icon + Label stacked
- Active State: Icon filled, text white
- Inactive State: Icon outline, text #808080
- Icon Size: 24px
- Label Size: 10px

## Layout Principles

- **Max content width:** Full bleed on mobile, 1200px max on desktop
- **Grid structure:** Single column mobile, multi-column tablet+
- **Alignment:** Center-aligned hero content, left-aligned sections
- **Safe areas:** Respects device safe areas for notches and home indicators
- **Content hierarchy:** Hero card dominates viewport, secondary content below fold
- **Horizontal scrolling:** Used for content rows (games, shows)

## Visual Effects

**Border Radius:**
- Buttons: 4px (squared, functional)
- Navigation chips: 20px (pill shape)
- Cards: 8px (gentle rounding)
- Game tiles: 8px
- Live indicator badge: 4px

**Shadows:**
- Minimal shadow use throughout
- Subtle elevation on hover states only
- No box shadows on primary UI elements

**Decorative Elements:**
- Lightning bolt graphics in teal (#00D4AA)
- Abstract grid patterns in background (very subtle, #1A1A1A)
- Live indicator: Pulsing red dot animation

**Gradients:**
- Hero card text protection: linear-gradient(to top, rgba(0,0,0,0.9) 0%, transparent 60%)
- No gradient backgrounds on UI elements

## Design Tone

This is a bold, entertainment-focused dark interface that prioritizes content visibility and dramatic visual impact. The electric teal lightning accents add energy and brand personality against the deep black canvas. Red CTAs create urgency for live content while the overall aesthetic remains sophisticated and cinematic. The system feels premium, immersive, and designed for nighttime viewing.

## Usage Notes for AI Implementation

**Color Application:**
- Always use pure black (#000000) as the base background
- Reserve red (#E50914) exclusively for primary CTAs and live indicators
- Use teal (#00D4AA) sparingly for decorative/brand moments
- Maintain high contrast ratios (minimum 7:1 for body text)

**Typography Implementation:**
- Load a condensed display font for hero titles (Bebas Neue, Oswald, or similar)
- Use system font stack for all UI text for performance
- Uppercase display titles for dramatic effect

**Component Guidelines:**
- Keep buttons flat (no shadows or gradients)
- Navigation chips should feel clickable but not dominant
- Hero cards should bleed to screen edges on mobile
- Maintain generous padding around interactive elements for touch targets

**Animation Recommendations:**
- Subtle hover state transitions (150ms ease)
- Live indicator pulse animation (1.5s infinite)
- Card hover slight scale (1.02) with shadow
- Navigation transitions should be instant (no delay)

**Accessibility Notes:**
- High contrast mode is inherent to the dark design
- Ensure teal accent passes contrast on dark backgrounds
- Red on black passes WCAG AA for large text
- Provide focus states for keyboard navigation (use teal outline)
