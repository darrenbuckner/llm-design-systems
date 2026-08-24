---
id: dark-bold-marketing-001
title: Velocity Dark System
description: High-contrast dark interface with bold condensed typography and vibrant green accents
tags: [dark, bold, marketing, high-contrast, condensed]
colors: ["#0D1117", "#FFFFFF", "#7AE582", "#8B949E", "#1C2128"]
created: 2025-12-20
---

# Velocity Dark System

A commanding dark interface system built for impact. Features ultra-bold condensed typography that demands attention, paired with a vibrant mint-green accent that cuts through the darkness. The aesthetic is confident, modern, and optimized for conversion-focused marketing pages.

## Color Palette

**Primary Colors:**
- Background Primary: #0D1117 — Deep charcoal-black, main canvas
- Background Secondary: #1C2128 — Slightly lighter dark for cards/sections
- Accent Green: #7AE582 — Vibrant mint-green for CTAs and highlights

**Text Colors:**
- Text Primary: #FFFFFF — Pure white for headlines and primary content
- Text Secondary: #8B949E — Muted gray for supporting text
- Text Accent: #7AE582 — Green for emphasized words within headlines

**UI Colors:**
- Border: #30363D — Subtle dark borders for separation
- Surface Elevated: #161B22 — Elevated cards and containers
- Success: #7AE582 — Same as accent
- Star/Rating: #FFFFFF — White filled stars with gray outlines

## Typography

**Font Families:**
- Primary Headlines: Inter (or similar geometric sans-serif), Condensed/Compressed variant
- Body Text: Inter or system sans-serif
- Testimonial/Quote: Italic variant of body font

**Type Scale:**
- Display/Hero: 96-120px, Black (900), condensed, -0.02em tracking, 0.9 line-height
- Heading 1: 72px, Black (900), condensed, -0.02em tracking
- Heading 2: 48px, Bold (700), normal width
- Heading 3: 32px, Bold (700), normal width
- Body Large: 20px, Regular (400), 1.6 line-height
- Body: 16px, Regular (400), 1.5 line-height
- Caption: 14px, Medium (500), 1.4 line-height

**Typography Patterns:**
- Headlines use ALL CAPS with extreme weight
- Mixed-color headlines: white text with single green accent word
- Italic styling for testimonial quotes
- Strong contrast between massive headlines and refined body text

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 16, 24, 32, 48, 64, 96, 128

**Common Patterns:**
- Section padding: 96px vertical, 48px horizontal
- Component internal padding: 16px 32px (buttons)
- Card padding: 32px - 48px
- Stack spacing (text blocks): 24px
- Tight text groupings: 8px - 16px

## Component Styles

### Buttons

**Primary CTA Button:**
- Background: #7AE582
- Text: #0D1117 (dark on light)
- Font: 18px, SemiBold (600)
- Padding: 16px 32px
- Border Radius: 8px
- Border: none
- Hover: Brightness increase to ~#8FEB96
- Active: Slight scale down (0.98)

**Secondary/Ghost Button:**
- Background: transparent
- Border: 2px solid #30363D
- Text: #FFFFFF
- Hover: Border color #8B949E

### Cards

**Testimonial Card:**
- Background: #1C2128
- Border Radius: 12px
- Padding: 32px
- Border: 1px solid #30363D (optional)
- Quote text: Italic, #8B949E
- Attribution: Regular, #FFFFFF

### Star Ratings

- Filled stars: #FFFFFF
- Empty stars: #30363D outline
- Size: 20-24px
- Gap: 4px

### Logo/Wordmark

- Two-weight wordmark pattern
- First word: Bold/Black weight
- Second word: Light/Regular weight
- Color: #FFFFFF
- Size: 18-24px

## Layout Principles

**Grid Structure:**
- 12-column grid on desktop
- Max content width: 1200px
- Gutter: 32px
- Side margins: 48-64px

**Section Layout:**
- Hero sections: Full-width, centered content
- Split layouts: 50/50 or 60/40 content/visual
- Generous vertical spacing between sections (96-128px)

**Alignment:**
- Headlines: Left-aligned (marketing) or centered (hero)
- Body text: Left-aligned
- CTAs: Left-aligned under content blocks

## Visual Effects

**Border Radius:**
- Buttons: 8px
- Cards: 12px
- Input fields: 8px
- Small elements (tags, badges): 4px

**Shadows:**
- Minimal shadow usage
- Elevated elements: 0 4px 24px rgba(0,0,0,0.4)
- Focus rings: 0 0 0 3px rgba(122, 229, 130, 0.3)

**Borders:**
- Subtle borders: 1px solid #30363D
- Dividers: 1px solid #30363D
- Focus/active states: 2px solid #7AE582

**Background Treatment:**
- Solid dark backgrounds
- Optional subtle noise texture (2-3% opacity)
- No gradients in base system

## Design Tone

This system projects confidence and authority through its extreme typographic contrast. The ultra-bold condensed headlines create immediate visual impact, while the vibrant mint-green accent adds energy without compromising the professional dark aesthetic. It's designed for brands that want to appear modern, decisive, and results-focused—perfect for SaaS, fintech, or any conversion-driven marketing context.

## Usage Notes for AI Implementation

**Headlines:** Use ALL CAPS with Black/Heavy weight for hero text. The condensed styling is essential—if Inter Tight or a condensed variant isn't available, use letter-spacing: -0.03em to simulate compression.

**Color Accent Pattern:** When implementing the green accent word within headlines, ensure it's a single impactful word (verbs or key benefits work best: "GROWTH", "RESULTS", "IMPACT").

**Button Hierarchy:** Only one primary green CTA per viewport. Supporting actions should use ghost/outline style.

**Dark Mode Only:** This system is designed exclusively for dark contexts. Light mode would require a complete palette inversion.

**Testimonials:** Always use italic styling for quote content, regular weight for attribution. The contrast between quote and attribution is important for scanability.
