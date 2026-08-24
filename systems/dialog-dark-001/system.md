---
id: dialog-dark-001
title: Dialog Dark Design System
description: "Sophisticated dark theme with layered surfaces, serif headings, and professional modal dialogs."
tags: [dark, professional]
colors: ["#0D0D0D","#1E1E1E","#2B2B2B","#5B9FD5","#E8E6E1"]
created: 2025-12-12
---

# Dialog Dark Design System

## Color Palette

**Primary Colors:**
- Primary Action: #5B9FD5 — Used for interactive links and primary call-to-action elements
- Primary Text: #E8E6E1 — Main text color on dark backgrounds

**Neutral Colors:**
- Modal Background: #2B2B2B — Primary surface color for modal dialogs
- Card Background: #1E1E1E — Darker background for nested content cards
- Body Background: #0D0D0D — Deepest background layer
- Text Secondary: #999999 — Supporting text, descriptions, lower hierarchy content
- Text Tertiary: #666666 — Placeholder text, disabled states
- Border/Divider: #3D3D3D — Subtle separation lines between sections

**Interactive States:**
- Link Hover: #7AB8E5 — Lighter variant of primary action color
- Button Background: #2B2B2B — Default button surface (matches modal background)
- Button Border: #4D4D4D — Button outline in default state

## Typography

**Font Families:**
- Primary: Serif typeface for headings (similar to Lora, Merriweather, or Georgia)
- Secondary: Sans-serif for body text and UI elements (similar to SF Pro, Inter, or System UI)

**Type Scale:**
- Heading 1 (Modal Title): 32px, Regular (400), 40px line-height
- Heading 2 (Section Header): 18px, Medium (500), 24px line-height
- Body Large: 16px, Regular (400), 24px line-height
- Body Standard: 14px, Regular (400), 20px line-height
- Caption/Helper: 12px, Regular (400), 16px line-height

**Hierarchy Rules:**
- Modal titles use serif typeface for elegance and authority
- All UI text and descriptions use sans-serif for readability
- Primary headings are sentence case
- Secondary text uses reduced opacity (#999999) rather than lighter weight

## Spacing System

**Base Unit:** 4px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

**Common Patterns:**
- Modal padding: 40px all sides
- Card internal padding: 24px vertical, 24px horizontal
- Section spacing: 32px between major sections
- Element spacing: 12px between related items, 24px between groups
- Button padding: 16px horizontal, 12px vertical
- Icon-to-text spacing: 12px

## Component Styles

### Buttons

**Primary Button (Unpublish):**
- Background: #2B2B2B
- Text: #E8E6E1
- Border: 1px solid #4D4D4D
- Border-radius: 8px
- Padding: 12px 24px
- Font-size: 15px, Medium (500)
- Hover: Border brightens to #666666

**Text/Link Button (Copy link):**
- Background: Transparent
- Text: #5B9FD5
- Icon color: #5B9FD5
- No border
- Padding: 8px 16px
- Font-size: 15px, Medium (500)
- Hover: Text color brightens to #7AB8E5

### Cards

**Content Card:**
- Background: #1E1E1E
- Border: 1px solid #3D3D3D
- Border-radius: 12px
- Padding: 24px
- Shadow: None (flat design)

### Modals

**Dialog Container:**
- Background: #2B2B2B
- Border: None
- Border-radius: 16px
- Padding: 40px
- Max-width: 680px
- Shadow: 0 8px 32px rgba(0, 0, 0, 0.6)
- Backdrop: rgba(0, 0, 0, 0.75) blur

### Icons

- Size: 20px for inline icons, 24px for standalone
- Color: Inherits from text or uses primary action color
- Style: Outlined/line style, 1.5px stroke weight
- Globe icon for public/sharing
- Link icon for copy actions
- Arrow/chevron icons for navigation

### Text Inputs/URL Display

- Background: #1E1E1E
- Border: 1px solid #3D3D3D
- Border-radius: 8px
- Padding: 12px 16px
- Text color: #E8E6E1
- Font-size: 14px
- Read-only state: Same as default (no visual distinction)

## Layout Principles

- Max content width: 680px for modal dialogs
- Content is center-aligned within viewport
- Vertical rhythm: 24-32px spacing between content blocks
- Horizontal rhythm: 12-16px for inline elements
- Close button: Positioned top-right, 24px from edges
- Single column layout within modals
- Generous whitespace for breathing room
- Left-aligned text for readability

## Visual Effects

**Border Radius:**
- Modal container: 16px
- Cards: 12px
- Buttons: 8px
- Input fields: 8px
- Icons: No radius (line icons)

**Shadows:**
- Modal elevation: 0 8px 32px rgba(0, 0, 0, 0.6)
- No shadows on internal components (flat design within modals)

**Borders:**
- Thickness: 1px standard
- Style: Solid
- Color: #3D3D3D for subtle separation
- Usage: Cards, buttons, dividers, sections

**Backgrounds:**
- Solid colors only, no gradients
- Layered darkness: #0D0D0D → #1E1E1E → #2B2B2B
- Modal backdrop: Semi-transparent dark overlay with blur

## Design Tone

Sophisticated, professional, and content-focused. The design employs a layered dark theme with subtle depth created through strategic use of slightly different dark values rather than heavy shadows. The serif heading typeface adds elegance and authority while sans-serif UI text maintains clarity. The overall aesthetic is minimal and refined, prioritizing information hierarchy and readability through typography and spacing rather than decorative elements.

## Usage Notes for AI Implementation

- Maintain consistent layering: darkest backgrounds behind, progressively lighter surfaces forward
- Use the serif typeface sparingly—only for major headings, never for body text or UI elements
- Keep interactive elements (links, buttons) in the blue accent color (#5B9FD5) for instant recognition
- Preserve generous spacing—cramped layouts break the sophisticated feel
- Border radius should feel modern but not excessive; keep curves subtle
- Text hierarchy comes from color opacity and size, not weight variation
- All borders and dividers should be subtle (#3D3D3D)—never harsh separation
- Icons should always match text color or use the primary action color, never standalone colors