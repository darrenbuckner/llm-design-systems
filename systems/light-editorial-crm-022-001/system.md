---
id: light-editorial-crm-022
title: Ivory Editorial
description: A clean, high-contrast monochrome system pairing bold serif headlines with minimal sans-serif body text for a refined editorial SaaS feel.
tags: light, editorial, minimal, serif, monochrome, premium, professional, SaaS
colors: ["#FFFFFF", "#000000", "#F7F7F7", "#E5E5E5", "#666666", "#999999"]
created: 2026-02-23
---

# Ivory Editorial

A striking monochrome design system that pairs large, expressive serif headlines with clean sans-serif body text. The aesthetic is editorial and confident — mostly black and white with carefully deployed grays for hierarchy. The system uses generous whitespace, bold typographic contrast, and dark pill-shaped CTAs to create a premium, modern SaaS feel. Sections alternate between white and near-black backgrounds for dramatic rhythm.

## Color Palette

**Primary Colors:**
- Primary: #000000 — Headlines, primary buttons, dark section backgrounds
- Primary Inverse: #FFFFFF — Text on dark backgrounds, page background

**Neutral Colors:**
- Surface Light: #FFFFFF — Main page background
- Surface Subtle: #F7F7F7 — Alternate section backgrounds, input field fills
- Surface Dark: #0A0A0A — Dark feature sections, footer area
- Text Primary: #000000 — Headlines, primary body text
- Text Secondary: #666666 — Supporting text, descriptions
- Text Tertiary: #999999 — Captions, metadata, placeholders
- Borders: #E5E5E5 — Card borders, dividers, table lines
- Border Subtle: #F0F0F0 — Light dividers, subtle separators

**Accent/State Colors:**
- Success: #22C55E — Confirmation states, positive indicators
- Warning: #F59E0B — Caution states
- Error: #EF4444 — Error states, destructive actions
- Info: #3B82F6 — Informational states
- Accent Gold: #C4A962 — Subtle warm accent for premium elements (sparingly used)

## Typography

**Font Families:**
- Primary (Headlines): Instrument Serif, Georgia, serif — Used for all hero text, section headlines, and large editorial statements
- Secondary (Body): Inter, -apple-system, system-ui, sans-serif — Used for body text, labels, navigation, buttons, and UI elements

**Type Scale:**
- Display: 48-56px, 400 weight, 1.1 line-height — Hero headlines, large editorial statements
- Heading 1: 36-40px, 400 weight, 1.15 line-height — Section titles (serif)
- Heading 2: 28-32px, 600 weight, 1.2 line-height — Feature titles (sans-serif, bold)
- Heading 3: 20-24px, 600 weight, 1.3 line-height — Card titles, subsections (sans-serif)
- Body Large: 18px, 400 weight, 1.6 line-height — Feature descriptions, introductory paragraphs
- Body: 16px, 400 weight, 1.6 line-height — Standard body text
- Small: 14px, 400 weight, 1.5 line-height — Captions, metadata, footer text
- Micro: 12px, 500 weight, 1.4 line-height — Tags, badges, uppercase labels

**Hierarchy Rules:**
- Display and H1 use serif font in regular weight — the typeface itself carries the visual weight
- H2 and below use sans-serif with semibold weight for emphasis
- Body text is always sans-serif at regular weight
- Uppercase tracking (0.05-0.1em) is used for small labels and category tags
- Links use underline decoration, no color change from surrounding text
- Feature link CTAs use bold weight with arrow indicator (→)

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 80, 96, 120

**Common Patterns:**
- Component internal padding: 16-24px
- Card padding: 24-32px
- Section vertical padding: 80-120px
- Section horizontal padding: 24px (mobile), 48-64px (desktop)
- Max content width: 1200px centered
- Grid gap: 24-32px
- Between heading and body text: 16-24px
- Between sections: 0 (sections use their own padding)
- Navigation padding: 16px vertical, 24px horizontal

## Component Styles

### Buttons

**Primary Button (CTA):**
- Background: #000000
- Text: #FFFFFF, 16px, 500 weight
- Padding: 16px 32px
- Border radius: 999px (full pill shape)
- Hover: Background #1A1A1A, subtle lift
- Min height: 48px
- Full-width on mobile

**Secondary Button (Text Link):**
- Background: transparent
- Text: #000000, 14-16px, 500 weight
- Decoration: underline on hover
- Often paired with arrow (→)
- Pattern: "Explore [feature] →"

**Ghost Button:**
- Background: transparent
- Border: 1px solid #E5E5E5
- Text: #000000, 14px, 500 weight
- Padding: 12px 24px
- Border radius: 999px
- Hover: Background #F7F7F7

### Cards

**Feature Card:**
- Background: #FFFFFF
- Border: 1px solid #E5E5E5
- Border radius: 12px
- Padding: 32px
- No shadow (flat design)
- Hover: subtle border darken to #CCCCCC

**Dark Feature Card:**
- Background: #1A1A1A
- Border: 1px solid #333333
- Border radius: 12px
- Padding: 32px
- Text: #FFFFFF (primary), #999999 (secondary)

### Input Fields

**Email Input:**
- Background: #F7F7F7
- Border: 1px solid #E5E5E5
- Border radius: 999px (pill shape)
- Padding: 16px 24px
- Font: 16px, regular weight
- Placeholder color: #999999
- Focus: border-color #000000
- Often paired inline with pill CTA button

### Navigation

**Top Navigation:**
- Background: #FFFFFF
- Border bottom: 1px solid #E5E5E5
- Logo: left-aligned, bold sans-serif with icon
- Nav links: 14px, 500 weight, #000000
- CTA button: pill-shaped, right-aligned
- Height: ~64px
- Sticky on scroll

### Pricing Table

**Structure:**
- Column layout with plan tiers side by side
- Plan toggle tabs at top (Monthly/Annual)
- Price: large serif number
- Feature list: simple text with subtle dividers
- CTA button at bottom of each plan
- Highlighted/recommended plan uses dark background (#0A0A0A) with white text

### Tabs

**Horizontal Tabs:**
- Inactive: #666666 text, no border
- Active: #000000 text, 2px bottom border
- Font: 14px, 500 weight
- Spacing: 24px between tabs
- Underline indicator slides on selection

## Layout Principles

- Max content width: 1200px, centered with auto margins
- Single column layout on mobile, expands to 2-column grid on desktop
- Content sections alternate between full-width white and full-width dark backgrounds
- Heavy use of centered text alignment for hero/headline sections
- Feature grids use 2-column layout with equal spacing
- Asymmetric layouts for feature showcases (text left, visual right or vice versa)
- Generous vertical spacing (80-120px) between major sections

## Visual Effects

- **Border Radius:** 12px for cards and containers, 999px (full pill) for buttons and inputs, 8px for small elements and tags
- **Shadows:** Minimal to none — flat design philosophy. Occasional very subtle shadow on hover (0 2px 8px rgba(0,0,0,0.06))
- **Borders:** 1px solid, always subtle (#E5E5E5 on light, #333333 on dark). Used as primary visual container definition instead of shadows
- **Backgrounds:** Solid colors only — white (#FFFFFF), near-white (#F7F7F7), and near-black (#0A0A0A). No gradients
- **Decorative Elements:** Abstract geometric illustrations using thin strokes and the monochrome palette. Chevron/wave patterns. Large typographic statements used as visual elements
- **Transitions:** Smooth 200ms ease for hover states, color changes, and border shifts

## Design Tone

Ivory Editorial is confident and restrained. It uses the tension between large, elegant serif headlines and precise sans-serif UI text to create a sense of authority without being heavy. The monochrome palette feels intentional rather than limiting — every element earns its place through typography and spacing rather than color. The overall personality is modern editorial meets enterprise SaaS: serious enough for business, refined enough to feel premium.

## Usage Notes for AI Implementation

- Always pair serif headlines with sans-serif body — never use serif for body text or UI elements
- The pill shape (border-radius: 999px) is a defining pattern — use it for all buttons and primary inputs
- Dark sections should be used sparingly for emphasis, not as the default — the system is primarily white
- When in doubt, add more whitespace. This system breathes through generous spacing
- Keep color usage minimal. Resist adding accent colors beyond the monochrome palette unless for functional states (success, error, etc.)
- Hero sections should use the large serif display text with minimal supporting copy
- Feature CTAs follow the pattern: bold text + arrow → (e.g., "Explore automation →")
- Cards use borders, not shadows, for containment
- The pricing table recommended plan inverts to dark background — use this pattern for emphasis
- Maintain the editorial rhythm: alternate white and dark sections for visual pacing
- Input + button combinations should be inline (side by side) on desktop, stacked on mobile
