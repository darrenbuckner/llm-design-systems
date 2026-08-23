---
id: light-gallery-brutalist-001
title: Concrete Gallery System
description: Brutalist showcase design with textured backgrounds, hand-drawn borders, and bold impact typography
tags: light, brutalist, textured, bold, gallery
colors: ["#E8E4DC", "#000000", "#FFFFFF", "#3A3A3A"]
created: 2025-01-05
---

# Concrete Gallery System

A brutalist design system featuring grungy textured backgrounds, hand-drawn borders, and ultra-bold condensed typography. Perfect for showcasing content with raw, unpolished authenticity and maximum visual impact.

## Color Palette

**Primary Colors:**
- Background Surface: #E8E4DC — Warm concrete/paper texture base
- Primary Text: #000000 — Pure black for maximum contrast
- Card Surface: Various (see accent colors) — Colorful card backgrounds
- Border/Accent: #1A1A1A — Hand-drawn border simulation

**Neutral Colors:**
- Light Gray: #F5F3EF — Subtle surface variation
- Medium Gray: #808080 — Secondary elements
- Dark Gray: #3A3A3A — Borders, shadows, depth

**Accent/Card Colors:**
- Orange Warm: #FF6B35 — Energy, warmth (Campfire inspiration)
- Black Bold: #000000 — Stark, minimalist (Block inspiration)
- Cream Clean: #FAF9F6 — Light, refined (Canvas inspiration)
- Lavender Soft: #C8B6D6 — Elegant, serene
- Teal Dark: #2C4F52 — Deep, sophisticated
- Cyan Accent: #00CFC1 — Bright highlight
- Yellow Pop: #F7FF00 — Vibrant, energetic

## Typography

**Font Families:**
- Primary: Impact, "Franklin Gothic Heavy", "Arial Black", sans-serif — Ultra-bold condensed
- Secondary: "Helvetica Neue", Arial, sans-serif — Clean supporting text
- Accent: "Courier New", monospace — Technical/metadata

**Type Scale:**
- Display/Hero: 72px, 900 weight, 0.85 line-height — Massive showcase headers
- Heading 1: 48px, 900 weight, 0.9 line-height — Section titles
- Heading 2: 32px, 700 weight, 1.1 line-height — Card titles
- Body: 16px, 400 weight, 1.5 line-height — Descriptive text
- Small/Meta: 12px, 700 weight, 1.3 line-height — Tags, labels

**Hierarchy Rules:**
- All major headings use ultra-condensed, ultra-bold fonts (Impact style)
- Text is UPPERCASE for maximum impact
- Tight letter-spacing (-0.02em) on headlines
- High contrast between heading weight (900) and body (400)

## Spacing System

**Base Unit:** 8px
**Scale:** 8, 16, 24, 32, 40, 48, 64, 80, 96

**Common Patterns:**
- Card padding: 24px-32px internal spacing
- Card gaps: 16-24px between cards
- Section spacing: 48-64px between major sections
- Border width: 3-5px for hand-drawn effect
- Edge margins: 40-48px from viewport edges

## Component Styles

### Gallery Cards
- **Size:** Variable (typically 320-400px wide)
- **Background:** Solid color or gradient fill
- **Border:** 3-4px solid black, slightly irregular/hand-drawn appearance
- **Padding:** 24px all sides
- **Corner Radius:** 0px (sharp, brutalist)
- **Shadow:** 4-6px offset black shadow for depth
- **Text:** UPPERCASE, ultra-bold, black on light cards or white on dark cards

### Card Variants
- **Warm Cards:** Orange/red backgrounds with flame/texture overlays
- **Dark Cards:** Black or dark teal backgrounds with bright accent text
- **Light Cards:** Cream/white backgrounds with black bold text
- **Gradient Cards:** Yellow-green or multi-color gradients

### Typography Cards
- **Header:** System name in ultra-bold condensed caps
- **Alignment:** Centered or left-aligned within card
- **Contrast:** Minimum 7:1 for WCAG AAA compliance

### Grid Layout
- **Desktop:** 3 columns, 24px gaps
- **Tablet:** 2 columns, 16px gaps
- **Mobile:** 1 column, full width with 16px margins

## Layout Principles

- **Max content width:** 1200px centered container
- **Grid structure:** CSS Grid with repeat(auto-fit, minmax(300px, 1fr))
- **Responsive behavior:** Cards stack vertically on mobile, expand to grid on desktop
- **Alignment:** Cards within grid, content centered within cards
- **Texture:** Background uses concrete/paper texture overlay at low opacity

## Visual Effects

- **Border Radius:** 0px — Sharp corners throughout
- **Shadows:** 
  - Card shadow: 4px 4px 0px #000000 (hard shadow, no blur)
  - Hover shadow: 6px 6px 0px #000000 (lifted effect)
- **Borders:** 
  - Card borders: 3-4px solid black, slightly irregular
  - Optional: Inner borders at 1-2px for nested elements
- **Backgrounds:** 
  - Main surface: Textured (concrete, paper grain) at ~95% opacity
  - Cards: Solid colors or gradients
  - Overlays: Flame, grain, or noise textures on accent cards
- **Textures:** Grungy, distressed, hand-drawn aesthetic

## Design Tone

Raw, unpolished, and boldly authentic. This system embraces brutalist principles with hand-drawn borders, textured surfaces, and ultra-bold typography that demands attention. The aesthetic feels tactile and physical, like screen-printed posters or protest signs—designed for maximum impact with minimal refinement. Perfect for showcasing creative work, design portfolios, or galleries where content should speak louder than polish.

## Usage Notes for AI Implementation

**When using this system:**
1. Always apply texture overlays to background surfaces (concrete, paper, grain)
2. Use Impact or similar ultra-condensed bold fonts for all major headings
3. Cards should have hard black borders (3-4px) with slight irregularity for hand-drawn feel
4. Implement hard shadows (no blur) with 4-6px offset
5. Keep corner radius at 0px for brutalist aesthetic
6. Use high-contrast color combinations (black on light, white on dark)
7. Text should be UPPERCASE for headlines and card titles
8. Grid layouts should be responsive: 3-col desktop → 2-col tablet → 1-col mobile
9. Consider adding subtle noise/grain textures to accent cards
10. Maintain generous spacing between cards (24px+) for breathing room

**Color Application:**
- Use neutral concrete background (#E8E4DC) as base
- Apply vibrant accent colors to individual cards
- Ensure text contrast meets WCAG AAA (7:1 minimum)
- Dark cards get white/cyan text, light cards get black text

**Responsive Considerations:**
- Cards should be min 300px wide, max 400px
- Stack vertically on screens < 768px
- Maintain consistent padding across breakpoints
- Touch targets minimum 44x44px on mobile
