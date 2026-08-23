---
id: dark-entertainment-007
title: Reel Stream
description: Bold dark entertainment interface with vibrant yellow accent and clean typography
tags: [dark, entertainment, streaming, bold-accent, mobile-first]
colors: ["#0B0C10", "#1F2024", "#FAED26", "#FFFFFF", "#9CA3AF", "#374151"]
created: 2026-01-16
---

# Reel Stream

A cinematic dark interface designed for entertainment and media streaming. Features a deep charcoal/navy-black foundation with an electrifying yellow accent that commands attention. The system prioritizes content visibility through high contrast and generous whitespace, with a clean sans-serif type hierarchy that maintains readability across all device sizes.

## Color Palette

**Primary Colors:**
- Primary/Accent: #FAED26 — Electric yellow for CTAs, active states, and key actions
- Background Primary: #0B0C10 — Deep black-navy for main surfaces
- Background Secondary: #1F2024 — Slightly elevated surface for cards/components

**Neutral Colors:**
- Surface/Background: #0B0C10 — Primary background
- Card Surface: #1F2024 — Elevated components
- Text Primary: #FFFFFF — High contrast white for headings and primary text
- Text Secondary: #9CA3AF — Muted gray for metadata and supporting text
- Text Tertiary: #6B7280 — Lower emphasis labels
- Borders: #374151 — Subtle dark gray dividers

**Accent/State Colors:**
- Success: #10B981 — Green for positive states
- Warning: #F59E0B — Amber for cautions
- Error: #EF4444 — Red for errors
- Info: #FAED26 — Yellow doubles as info/highlight

**Tag/Badge Colors:**
- Rating Badge Background: #374151 — Dark gray pill background
- Rating Badge Text: #FFFFFF — White text on badges

## Typography

**Font Families:**
- Primary: System UI / -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
- Fallback: Arial, Helvetica, sans-serif

**Type Scale:**
- Display/Title: 28px, 700 weight, 1.2 line-height — Content titles
- Heading 1: 24px, 700 weight, 1.25 line-height — Section headers
- Heading 2: 18px, 600 weight, 1.3 line-height — Subsection headers
- Body Large: 16px, 400 weight, 1.5 line-height — Descriptions, paragraphs
- Body: 14px, 400 weight, 1.5 line-height — Standard content text
- Caption/Small: 12px, 400 weight, 1.4 line-height — Metadata, labels
- Button Text: 16px, 600 weight, 1 line-height — CTA buttons

**Hierarchy Rules:**
- Titles use bold weight with tight line-height for impact
- Body text uses regular weight with generous line-height for readability
- Metadata uses secondary gray color to create visual hierarchy
- Labels (like "Starring:", "Genre:") use secondary text color, values use primary text

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

**Common Patterns:**
- Component internal padding: 16px horizontal, 12-16px vertical
- Section spacing: 24-32px between major sections
- List item spacing: 8-12px between items
- Button padding: 16px vertical, 24px horizontal
- Card padding: 16-20px
- Container horizontal padding: 16-24px (mobile), 24-48px (desktop)

## Component Styles

### Buttons

**Primary Button (Yellow CTA):**
- Background: #FAED26
- Text: #0B0C10 (dark on light)
- Font: 16px, 600 weight
- Padding: 16px 24px
- Border Radius: 100px (fully rounded/pill)
- Height: ~52px
- Shadow: none
- Hover: Slight brightness increase, subtle scale
- Contains icon + text + badge layout

**Secondary Button (Outline):**
- Background: transparent
- Border: 1px solid #FFFFFF
- Text: #FFFFFF
- Border Radius: 100px (pill)
- Padding: 10px 20px

**Text Button/Link:**
- Color: #FFFFFF
- Hover: Underline or opacity change
- No background

### Badges/Tags

**Rating Badge (e.g., TV-MA):**
- Background: #374151
- Text: #FFFFFF
- Font: 12px, 500 weight
- Padding: 4px 8px
- Border Radius: 4px

**Free Badge:**
- Background: #0B0C10
- Text: #FFFFFF
- Font: 12px, 700 weight
- Padding: 4px 10px
- Border Radius: 4px
- Positioned within button

### Navigation

**Header/Navbar:**
- Background: #0B0C10 (can be transparent over hero)
- Height: ~60px
- Layout: Logo left, actions right
- Items: Icon buttons, outline register button, text sign-in link

**Menu Button:**
- Background: #1F2024
- Border Radius: 50% (circular)
- Size: 44px
- Icon: White hamburger lines

### Tabs

**Tab Bar:**
- Underline style indicator
- Active tab: White text + yellow/white underline (2px)
- Inactive tab: Gray text (#9CA3AF)
- Spacing: 24px between tabs
- Border bottom: 1px solid #374151

### Cards

**Content Card:**
- Background: Transparent or #1F2024
- Border Radius: 8px
- Image: Full bleed, rounded top corners
- Content padding: 16px
- Title: White, bold
- Metadata: Gray, regular

### Input Fields

**Search/Text Input:**
- Background: #1F2024
- Border: 1px solid #374151
- Border Radius: 8px
- Text: #FFFFFF
- Placeholder: #6B7280
- Padding: 12px 16px
- Focus: Border color #FAED26

## Layout Principles

- Max content width: 100% mobile, 1200px desktop container
- Grid structure: Single column mobile, multi-column grids for content browsing
- Responsive behavior: Full-width hero images, stacking content on mobile
- Alignment: Left-aligned text, centered CTAs
- Hero pattern: Full-bleed image with gradient overlay, content overlay at bottom

## Visual Effects

**Border Radius:**
- Buttons: 100px (pill/fully rounded)
- Cards: 8px
- Badges: 4px
- Input fields: 8px
- Avatar/icons: 50% (circular)
- Images: 0-8px depending on context

**Shadows:**
- Minimal shadow usage — relies on color contrast
- Subtle elevation for modals: 0 4px 24px rgba(0,0,0,0.5)

**Borders:**
- Dividers: 1px solid #374151
- Input borders: 1px solid #374151
- Outline buttons: 1px solid #FFFFFF

**Backgrounds:**
- Solid dark backgrounds
- Hero gradient overlay: linear-gradient(to top, #0B0C10 0%, transparent 50%)
- No textures or patterns

## Design Tone

Bold, cinematic, and content-focused. The design prioritizes the visual content (imagery) while maintaining clear hierarchy through high-contrast typography. The electric yellow accent creates energy and draws attention to primary actions without overwhelming the dark foundation. The overall feel is modern entertainment platform — confident, clean, and accessible.

## Usage Notes for AI Implementation

- Always use the dark background (#0B0C10) as the foundation
- Reserve the yellow accent (#FAED26) exclusively for primary CTAs and active/selected states
- Use generous whitespace between sections (24-32px minimum)
- Hero images should use a gradient overlay (transparent to #0B0C10) for text legibility
- Buttons should always be pill-shaped (border-radius: 100px)
- Maintain high contrast ratios — white text on dark backgrounds
- Tab navigation uses underline indicators, not background fills
- Metadata should be clearly subordinate (gray color, smaller size) to titles
- Mobile-first: ensure touch targets are minimum 44px
