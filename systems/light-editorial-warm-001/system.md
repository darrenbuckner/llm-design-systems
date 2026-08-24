---
id: light-editorial-warm-001
title: Sandstone Editorial System
description: A warm, typographically-rich editorial design system with cream surfaces, bold serif headlines, and restrained accent color
tags: [light, editorial, warm, minimal, serif, premium]
colors: ["#F5F0E8", "#191919", "#C4784A", "#E8E0D4", "#6B6256", "#000000"]
created: 2026-01-18
---

# Sandstone Editorial System

A warm, sophisticated editorial design system built on cream-toned surfaces and bold typographic hierarchy. The aesthetic is confident and restrained — relying on large-scale serif and sans-serif type, generous whitespace, and a single earthy accent color to create a premium, content-first experience. The overall feel is that of a modern research journal or high-end editorial publication.

## Color Palette

**Primary Colors:**
- Primary Action: #C4784A — Warm terracotta/copper used for primary CTAs and active links
- Primary Text: #191919 — Near-black used for headlines and primary content
- Logo/Mark: #000000 — Pure black for brand marks and emphatic elements

**Neutral Colors:**
- Surface/Background: #F5F0E8 — Warm cream/parchment, the dominant background
- Card Surface: #E8E0D4 — Slightly deeper warm beige for elevated cards and feature areas
- Text Secondary: #6B6256 — Warm gray-brown for body text and secondary content
- Text Tertiary: #9A9189 — Lighter warm gray for labels, captions, and metadata
- Borders: #DDD6CB — Subtle warm divider lines
- Borders Light: #E8E2D8 — Even lighter dividers for nested content

**Accent/State Colors:**
- Success: #4A8C5C — Muted forest green
- Warning: #C4784A — Shares the primary accent (terracotta)
- Error: #B54A3A — Deeper warm red
- Link Underline: #191919 — Black underlines on inline text links

## Typography

**Font Families:**
- Primary Headlines: A high-contrast transitional serif (closest match: "Freight Display" or "Tiempos Headline"; use **Playfair Display** or **Source Serif 4** as Google Fonts approximations)
- Secondary Headlines/Nav: A geometric/grotesque sans-serif, medium weight (closest match: system sans or **Inter**)
- Body Text: Same sans-serif as secondary, lighter weight — clean and highly readable
- Feature Display: Mixed serif/italic for editorial emphasis — italic serif used for stylistic contrast within headlines

**Type Scale:**
- Display/Hero: 48–56px, 700 weight, 1.05 line-height (tight, impactful)
- Heading 1: 32–40px, 700 weight, 1.15 line-height
- Heading 2: 24–28px, 600 weight, 1.2 line-height
- Heading 3: 20px, 600 weight, 1.3 line-height
- Body Large: 18–20px, 400 weight, 1.6 line-height
- Body: 16px, 400 weight, 1.6 line-height
- Label/Overline: 12–13px, 500 weight, 1.4 line-height, letter-spacing: 0.08em, uppercase
- Caption: 14px, 400 weight, 1.5 line-height

**Hierarchy Rules:**
- Headlines use the serif font at heavy weights with very tight line-height for dramatic impact
- Body text uses the sans-serif at regular weight with generous line-height for readability
- Overline labels (like "FEATURED", "DATE", "CATEGORY") use uppercase, small size, wide letter-spacing
- Inline links are underlined with the text color (not the accent color)
- Editorial emphasis uses italic serif mixed into sans-serif headlines

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 80, 96, 120

**Common Patterns:**
- Container horizontal padding: 24px (mobile), 48–64px (tablet), 80–120px (desktop)
- Section vertical spacing: 64–96px between major sections
- Card internal padding: 24–32px
- Navigation item vertical padding: 20–24px
- List item vertical spacing: 16–20px with border separators
- Paragraph spacing: 24px between body paragraphs
- Hero headline to body text: 32px

## Component Styles

### Buttons

**Primary Button (CTA):**
- Background: #C4784A (terracotta)
- Text: #FFFFFF, 16px, 500 weight
- Padding: 16px 32px
- Border-radius: 8px
- Full-width on mobile
- Hover: darken to #B06A3E

**Secondary/Outline Button:**
- Background: transparent
- Border: 1px solid #DDD6CB
- Text: #191919, 16px, 500 weight
- Padding: 16px 32px
- Border-radius: 8px
- Full-width on mobile
- Hover: background #E8E0D4

**Text Button/Link:**
- Text: #191919, underlined
- Arrow icon (→) appended for navigation links
- No background or border
- Hover: opacity 0.7

### Cards

**Feature Card:**
- Background: #E8E0D4 (warm beige)
- Border-radius: 16px
- Padding: 32px
- No border, no shadow
- Contains overline label, large headline, body text, and text link

**Dark Feature Card (Editorial):**
- Background: #000000
- Text: #FFFFFF
- Border-radius: 16px
- Used for featured/hero editorial content
- Mixed serif typography for dramatic effect

### Navigation

**Mobile Menu:**
- Full-screen overlay on white/cream background
- Large serif/sans headlines for top-level items (28–32px, 700 weight)
- Accordion expand/collapse with chevron icons (∨/∧)
- Thin border separators between items (#DDD6CB)
- Close button (×) replaces hamburger
- Category labels in small uppercase (#9A9189)
- Sub-items at 18px, 400 weight

**Header Bar:**
- Logo mark left, hamburger menu right
- Minimal — no background color change, sits on page surface
- Sticky behavior assumed

### Metadata/Detail Rows

- Two-column layout: label left, value right
- Label: uppercase, small, letter-spaced (#9A9189)
- Value: regular weight, #191919
- Separated by thin border lines
- Used for dates, categories, specifications

### Input Fields
- Not prominently visible in screenshots
- Inferred: border-bottom style, minimal chrome, matching the warm palette

## Layout Principles

- Max content width: ~720px for text content, ~1200px for full layouts
- Single column dominant on mobile
- Generous margins — content breathes significantly
- Left-aligned text throughout (no centering except for feature card content)
- Featured content uses centered text within cards
- Strong vertical rhythm maintained with consistent spacing
- Full-bleed cards within container padding

## Visual Effects

- **Border Radius:** 8px for buttons, 16px for cards and feature areas
- **Shadows:** None — completely flat design, relies on color differentiation for depth
- **Borders:** 1px solid, warm gray (#DDD6CB), used as horizontal rules/separators extensively
- **Backgrounds:** Solid fills only — cream (#F5F0E8) and beige (#E8E0D4), no gradients
- **Textures:** None — clean and flat
- **Decorative Elements:** Inline underlines on links, arrow icons (→) for navigation

## Design Tone

This system exudes the quiet confidence of a premium editorial publication — think literary journal meets modern research institution. It's warm without being folksy, authoritative without being cold. The restrained color palette (essentially cream, black, and a single terracotta accent) forces the typography to do all the heavy lifting, creating a hierarchy that feels both sophisticated and effortlessly readable. The generous whitespace and absence of shadows or decorative elements signal "we trust our content to speak for itself."

## Usage Notes for AI Implementation

- The terracotta accent (#C4784A) should be used sparingly — only for primary CTAs and occasional emphasis. Overuse will break the restrained aesthetic.
- Headlines should be large and bold — this system is not afraid of 48px+ type on mobile. Let headings breathe with tight line-height but generous surrounding space.
- Inline text links should use underlines (not color changes) for a classic editorial feel.
- Cards differentiate through background color, not shadows or borders. Use #E8E0D4 for standard cards on the #F5F0E8 surface.
- For dark feature cards, switch to #000000 background with #FFFFFF text and bring in serif italic for editorial drama.
- Maintain extremely generous vertical spacing between sections — this system uses whitespace as a design element.
- The uppercase overline labels (small, letter-spaced) are a key pattern for adding structure without visual weight.
- On mobile, buttons should go full-width. Navigation uses a full-screen overlay with large type, not a cramped drawer.
