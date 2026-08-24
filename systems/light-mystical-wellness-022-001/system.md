---
id: light-mystical-wellness-022
title: Celestial Wellness System
description: A warm, feminine mystical interface blending script typography with modern sans-serifs and playful hand-drawn accents
tags: [light, wellness, mystical, feminine, warm, playful]
colors: ["#000000", "#FFFFFF", "#E8A4B8", "#D4A8E0", "#F5F5F5", "#666666"]
created: 2025-12-29
---

# Celestial Wellness System

A spiritually-inspired design system that balances mystical warmth with modern clarity. The interface combines elegant script typography for personalized greetings with bold condensed sans-serifs for section headers, unified by hand-drawn wavy underlines and soft pink-purple gradient accents. The aesthetic feels personal, inviting, and gently cosmic.

## Color Palette

**Primary Colors:**
- Black: #000000 — Primary text, headers, icons, navigation labels
- White: #FFFFFF — Page background, card surfaces

**Accent Colors:**
- Soft Pink: #E8A4B8 — Gradient accents, active states, decorative elements
- Lavender Purple: #D4A8E0 — Gradient secondary, mystical accents
- Hot Pink: #E91E8C — Tab highlight, active navigation accent

**Neutral Colors:**
- Light Gray Surface: #F5F5F5 — Card backgrounds, secondary surfaces
- Medium Gray: #666666 — Secondary text, inactive tabs
- Dark Gray: #333333 — Body text on cards
- Dashed Border: #CCCCCC — Decorative dashed lines

**Decorative Colors (from illustration):**
- Deep Teal: #1A3A3A — Pattern background
- Magenta Dots: #C41E7A — Decorative circles
- Lime Yellow: #D4E84A — Accent dots

## Typography

**Font Families:**
- Display/Greeting: Script serif (similar to Playfair Display Italic or a handwritten script)
- Headers: Condensed sans-serif with wide letter-spacing (similar to Oswald or Bebas Neue)
- Body: Geometric sans-serif (similar to DM Sans or Inter)
- Navigation: Condensed sans-serif, small caps style

**Type Scale:**
- Greeting (Script): 32-36px, 400 weight, 1.2 line-height — Personal welcome messages
- Section Headers: 16-18px, 700 weight, 2.0+ letter-spacing (0.2em), uppercase — "YOUR DAILY HOROSCOPE"
- Body Text: 16-17px, 400 weight, 1.6 line-height — Reading content
- Date Display: 14px, 500 weight, 1.4 line-height, monospace feel — "Dec 28, 2025"
- Tab Labels: 13-14px, 600 weight, 0.1em letter-spacing, uppercase — "TODAY", "THIS WEEK"
- Navigation Labels: 10-11px, 500 weight, uppercase — "HOME", "GROW"

**Hierarchy Rules:**
- Script font creates intimate, personal connection for greetings
- Uppercase tracking on headers creates mystical, ceremonial feel
- Hand-drawn wavy underlines beneath section headers add whimsy
- Body text uses comfortable reading line-height for longer passages

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

**Common Patterns:**
- Page horizontal padding: 24px (mobile)
- Card internal padding: 24-32px
- Section vertical spacing: 24-32px
- Tab group padding: 16px vertical
- Navigation bar padding: 12px vertical
- Icon-to-label spacing: 4-6px
- Dashed border padding: 8px

## Component Styles

### Tab Selector (Pill Group)
- Container: Dashed border (#CCCCCC), rounded corners 24px
- Active tab: Black (#000000) background, white text, pill shape
- Inactive tabs: Transparent background, gray text (#666666)
- Tab padding: 12px 20px
- Font: Uppercase, letter-spacing 0.05em
- Dashed line style: 4px dash, 4px gap

### Cards
- Background: #F5F5F5 light gray
- Border radius: 16-20px
- Padding: 24-32px
- Shadow: None (flat design)
- Decorative element: Tilted illustration in corner (optional)
- Bottom accent: Soft pink-purple gradient glow

### Buttons (Pill Style)
- Background: White/transparent
- Border: 2px solid #000000
- Border radius: 50px (full pill)
- Padding: 14px 28px
- Text: Uppercase, letter-spacing 0.15em, 13-14px
- Icon: Small inline icon after text
- Hover: Invert to black background, white text

### Navigation Bar (Bottom)
- Background: White
- Height: 64-72px
- Icon size: 24px
- Label size: 10-11px
- Active state: Hot pink (#E91E8C) icon and label
- Inactive state: Black icons and labels
- Equal 5-column distribution

### Wavy Underline (Decorative)
- Style: Hand-drawn squiggle SVG or CSS wave
- Color: Black (#000000) or gradient (pink to purple)
- Width: ~60% of header width
- Position: Centered below header text
- Amplitude: ~4px wave height

### Notification Bell
- Style: Outlined icon
- Dot indicator: Pink (#E8A4B8) small circle
- Position: Top-right header

### Hamburger Menu
- Style: Three horizontal lines
- Stroke: 2px black
- Width: 24px

## Layout Principles

**Mobile-First Structure:**
- Full-width cards with horizontal page padding
- Vertically stacked sections
- Fixed bottom navigation
- Centered section headers

**Grid Structure:**
- Single column layout (mobile)
- 5-column bottom navigation (equal width)
- Cards span full content width

**Alignment:**
- Headers: Center-aligned with decorative underlines
- Body text: Left-aligned within cards
- Navigation: Center-aligned icons with labels below
- Greeting: Center-aligned script

## Visual Effects

**Border Radius:**
- Cards: 16-20px
- Buttons: 50px (full pill)
- Tabs: 24px (full pill)
- Active tab within group: 20px

**Shadows:**
- None used — flat, paper-like aesthetic
- Depth created through layered cards and color

**Borders:**
- Dashed decorative borders: 1px dashed #CCCCCC
- Button borders: 2px solid #000000
- No card borders (background color differentiation)

**Backgrounds:**
- Page: Pure white #FFFFFF
- Cards: Light gray #F5F5F5
- Gradient glow: Linear gradient from pink (#E8A4B8) to purple (#D4A8E0), soft feathered edges

**Decorative Elements:**
- Hand-drawn wavy underlines beneath headers
- Tilted decorative illustrations (abstract patterns, circles)
- Gradient glows at card bottoms
- Dashed border rectangles for tab groups

## Design Tone

Warmly mystical and personally inviting. The design balances feminine spirituality with modern usability—script greetings feel like a note from a friend, while bold uppercase headers carry ceremonial gravitas. Hand-drawn elements (wavy lines, playful illustrations) prevent the interface from feeling sterile, creating a cozy digital sanctuary. The pink-purple palette suggests intuition and transformation without overwhelming the clean white canvas.

## Usage Notes for AI Implementation

**When to use this system:**
- Wellness and self-care applications
- Astrology, tarot, or spirituality platforms
- Personal journaling or reflection tools
- Feminine lifestyle apps
- Daily ritual or habit tracking

**Key implementation details:**
- Use script fonts sparingly (greetings, special moments only)
- Always pair uppercase headers with wavy underline decoration
- Maintain generous line-height (1.6+) for body text readability
- Use gradient glows subtly—soft feathered edges, not harsh stops
- Keep illustrations small and corner-positioned, never overwhelming content
- Dashed borders should feel hand-drawn, not mechanical

**Accessibility considerations:**
- Ensure body text maintains minimum 16px size
- Black on white/light gray provides excellent contrast
- Script fonts should have fallback to readable serif
- Touch targets minimum 44px for navigation items

**Responsive behavior:**
- On larger screens, consider 2-column card layouts
- Maintain center-aligned headers across breakpoints
- Bottom navigation can transform to side navigation on desktop
- Preserve generous whitespace at all sizes
