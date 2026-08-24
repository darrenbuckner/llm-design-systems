---
id: dark-forest-enterprise-001
title: Forest Grove System
description: Deep teal enterprise aesthetic with luminous accents and clean modern typography
tags: [dark, premium, enterprise, minimal, professional]
colors: ["#0D3D38", "#FFFFFF", "#000000", "#4AE8C1", "#9B6FD9"]
created: 2025-12-20
---

# Forest Grove System

A sophisticated dark enterprise aesthetic built on deep forest teal backgrounds with crisp white typography. The system creates visual hierarchy through bold weight contrast and subtle luminous effects, conveying authority and modern professionalism. Rounded pill shapes soften the corporate feel while maintaining a polished, premium presence.

## Color Palette

**Primary Colors:**
- Forest Teal: #0D3D38 — Primary background, hero sections, main surface color
- Deep Forest: #0A2E2A — Darker variant for depth, secondary backgrounds
- Pure White: #FFFFFF — Primary text, high-contrast headings

**Neutral Colors:**
- Surface Dark: #0D3D38 — Main canvas color
- Surface Darker: #082824 — Footer, nested sections
- Text Primary: #FFFFFF — Headlines, primary content
- Text Secondary: #B8D4D0 — Subheadings, secondary content (teal-tinted white)
- Borders: #1A5550 — Subtle dividers, card edges

**Accent Colors:**
- Mint Glow: #4AE8C1 — Success states, highlights, luminous effects
- Orchid Purple: #9B6FD9 — Secondary accent, icons, interactive elements
- Warm Glow: #C4E8A0 — Tertiary accent for variety

**State Colors:**
- Success: #4AE8C1 — Mint green glow
- Warning: #F5C842 — Warm amber
- Error: #E85A5A — Soft red
- Info: #5AA8E8 — Sky blue

## Typography

**Font Families:**
- Primary: Inter, -apple-system, BlinkMacSystemFont, sans-serif
- Display: Inter with tight letter-spacing for impact headlines
- Monospace: JetBrains Mono (for code/data displays)

**Type Scale:**
- Display: 72px, 800 weight, -0.02em letter-spacing, 1.0 line-height
- Heading 1: 56px, 700 weight, -0.02em letter-spacing, 1.1 line-height
- Heading 2: 40px, 700 weight, -0.01em letter-spacing, 1.2 line-height
- Heading 3: 28px, 600 weight, normal letter-spacing, 1.3 line-height
- Body Large: 18px, 400 weight, normal, 1.6 line-height
- Body: 16px, 400 weight, normal, 1.6 line-height
- Caption: 14px, 500 weight, 0.02em letter-spacing, 1.4 line-height
- Small: 12px, 500 weight, 0.04em letter-spacing, 1.4 line-height

**Hierarchy Rules:**
- Headlines use stacked single-word lines with periods for emphasis (e.g., "Clarity. Automation. ROI.")
- Weight contrast creates hierarchy: 800/700 for headlines, 400 for body
- Tight letter-spacing on large display text
- All-caps with wide letter-spacing for labels and badges

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 16, 24, 32, 48, 64, 96, 128

**Common Patterns:**
- Component padding: 16px (buttons), 24px (cards), 32px (sections)
- Section spacing: 64px to 96px vertical rhythm
- Grid gaps: 24px between cards, 32px between major sections
- Container max-width: 1200px with 24px mobile padding
- Hero section padding: 96px top, 64px bottom

## Component Styles

### Buttons

**Primary Button (Pill):**
- Background: #FFFFFF
- Text: #000000
- Font: 16px, 700 weight
- Padding: 16px 32px
- Border-radius: 9999px (full pill)
- Shadow: none (flat design)
- Hover: Background #F0F0F0, subtle lift transform

**Secondary Button (Outline Pill):**
- Background: transparent
- Border: 2px solid #FFFFFF
- Text: #FFFFFF
- Padding: 14px 30px
- Border-radius: 9999px
- Hover: Background rgba(255,255,255,0.1)

**Ghost Button:**
- Background: transparent
- Text: #FFFFFF
- Underline on hover

### Cards

**Feature Card:**
- Background: rgba(255,255,255,0.05)
- Border: 1px solid rgba(255,255,255,0.1)
- Border-radius: 16px
- Padding: 32px
- Hover: Background rgba(255,255,255,0.08)

**Stat Card:**
- Background: #0A2E2A
- Border-radius: 12px
- Padding: 24px
- Large number in 48px bold
- Label in 14px caps

### Badges/Tags

**Pill Badge:**
- Background: #FFFFFF
- Text: #000000
- Font: 14px, 700 weight
- Padding: 12px 24px
- Border-radius: 9999px
- Used for labels like "After" in before/after comparisons

### Input Fields

**Text Input:**
- Background: rgba(255,255,255,0.1)
- Border: 1px solid rgba(255,255,255,0.2)
- Border-radius: 8px
- Text: #FFFFFF
- Placeholder: rgba(255,255,255,0.5)
- Padding: 16px
- Focus: Border color #4AE8C1

## Layout Principles

- Max content width: 1200px centered
- Grid: 12-column with 24px gutters
- Asymmetric layouts common: Large headline left, visual right
- Generous whitespace creates premium feel
- Content blocks stack vertically on mobile
- Full-bleed hero sections with contained content

## Visual Effects

**Border Radius:**
- Buttons/Pills: 9999px (full round)
- Cards: 16px
- Inputs: 8px
- Small elements: 4px

**Shadows:**
- Minimal shadow use — relies on color/contrast
- Subtle glow effects on hover: box-shadow: 0 0 40px rgba(74,232,193,0.2)
- Card lift on hover: translateY(-2px)

**Borders:**
- Thin borders: 1px solid rgba(255,255,255,0.1)
- Accent borders: 2px for emphasis
- Circular/arc decorative elements using thin strokes

**Backgrounds:**
- Primary: Solid deep teal #0D3D38
- Gradient accents: Subtle luminous glow from bottom
- Radial glow: rgba(74,232,193,0.15) positioned strategically

**Special Effects:**
- Luminous/aurora effect: Soft green-teal glow emanating from bottom of sections
- Circular diagram elements with thin white strokes
- Icon containers with subtle purple/orchid fills

## Design Tone

This system projects confident enterprise authority with a fresh, modern edge. The deep forest teal creates a distinctive alternative to typical dark modes, feeling organic yet technological. Single-word stacked headlines with periods create punchy, memorable messaging that emphasizes key value propositions. The overall effect is premium, trustworthy, and forward-thinking.

## Usage Notes for AI Implementation

When implementing this system:

1. **Headlines:** Stack single powerful words vertically with periods for hero impact. Use tight letter-spacing at large sizes.

2. **Color Application:** Use the deep teal for large surfaces, white for all primary text. Reserve mint glow and purple for small accent moments only.

3. **Contrast:** Ensure WCAG AA compliance — the white-on-teal combination provides excellent readability.

4. **Luminous Effects:** Add subtle radial gradients (rgba(74,232,193,0.15)) at strategic points to create the signature glow effect without overwhelming the interface.

5. **Buttons:** Default to pill shapes for CTAs. Use the white/black primary button for main actions, outline for secondary.

6. **Spacing:** Maintain generous vertical rhythm — when in doubt, add more space. This creates the premium feel.

7. **Icons:** Use simple line icons in white or the purple accent. Avoid heavy filled icons.

8. **Mobile:** Stack layouts vertically, maintain padding. The pill shapes and large typography scale well.
