---
id: dark-warm-event-001
title: Ember Events
description: A warm, inviting dark theme with rich burgundy-brown tones and clean modern typography
tags: [dark, warm, event, minimal, professional]
colors: ["#1A0A0A", "#2D1810", "#F97316", "#FFFFFF", "#A8A29E"]
created: 2026-01-16
---

# Ember Events

A sophisticated dark interface built on warm burgundy and deep brown tones, creating an inviting atmosphere that feels premium yet approachable. The design balances rich, earthy backgrounds with bright orange accents and clean white typography for excellent readability.

## Color Palette

**Primary Colors:**
- Primary Orange: #F97316 — Call-to-action buttons, accent elements, live indicators
- Primary White: #FFFFFF — Headings, primary text, high-contrast elements

**Background Colors:**
- Deep Burgundy: #1A0A0A — Page background, darkest surface
- Warm Brown: #2D1810 — Card backgrounds, elevated surfaces
- Rich Mahogany: #3D241A — Secondary cards, hover states
- Dark Chocolate: #1F0F0A — Footer, deepest sections

**Neutral Colors:**
- Text Primary: #FFFFFF — Headings, important text
- Text Secondary: #A8A29E — Body text, descriptions, metadata
- Text Muted: #78716C — Timestamps, tertiary information
- Border Light: rgba(255, 255, 255, 0.1) — Subtle dividers, card borders

**Accent/State Colors:**
- Live Red: #EF4444 — Live event indicator dot
- Success Green: #22C55E — Confirmation states
- Link Blue: #60A5FA — Text links (subtle use)

**Tag Colors:**
- Tag Background: rgba(255, 255, 255, 0.15) — Pill backgrounds
- Tag Text: #FFFFFF — Tag labels

## Typography

**Font Families:**
- Primary: Inter, system-ui, -apple-system, sans-serif
- Monospace: SF Mono, Monaco, monospace (for codes/numbers)

**Type Scale:**
- Display/Hero: 32px, 800 (Extra Bold), 1.1 line-height, tight letter-spacing
- Heading 1: 24px, 700 (Bold), 1.2 line-height
- Heading 2: 18px, 600 (Semibold), 1.3 line-height
- Heading 3: 16px, 600 (Semibold), 1.4 line-height
- Body Large: 16px, 400 (Regular), 1.6 line-height
- Body: 14px, 400 (Regular), 1.5 line-height
- Caption: 12px, 500 (Medium), 1.4 line-height
- Label: 11px, 600 (Semibold), 1.3 line-height, uppercase, 0.5px letter-spacing

**Hierarchy Rules:**
- Hero text uses extra bold weight with tight line-height for impact
- Section headings use semibold with generous spacing above
- Body text maintains comfortable reading line-height
- Labels and metadata use smaller sizes with medium weight
- Strong contrast between heading and body weights

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

**Common Patterns:**
- Container padding: 16px mobile, 24px tablet, 32px desktop
- Section spacing: 32-48px vertical gaps
- Card padding: 16-20px internal padding
- Component gaps: 12-16px between related items
- List item spacing: 12px between items
- Inline element gaps: 8px

**Layout Measurements:**
- Max content width: 480px (mobile-focused event layout)
- Card border radius: 12px
- Button height: 48px
- Input height: 48px
- Avatar size: 40px (hosts), 32px (attendees)

## Component Styles

### Buttons

**Primary Button:**
- Background: #FFFFFF
- Text: #1A0A0A
- Font: 14px, 500 weight
- Padding: 12px 24px
- Border radius: 8px
- Border: 1px solid #FFFFFF
- Hover: Slight opacity reduction (0.9)

**Secondary/Ghost Button:**
- Background: transparent
- Text: #FFFFFF
- Border: 1px solid rgba(255, 255, 255, 0.3)
- Padding: 8px 16px
- Border radius: 6px
- Hover: Background rgba(255, 255, 255, 0.1)

**Subscribe Button:**
- Background: transparent
- Text: #A8A29E
- Border: 1px solid rgba(255, 255, 255, 0.2)
- Padding: 8px 16px
- Border radius: 6px
- Font: 14px, 500 weight

### Cards

**Event Card (Hero):**
- Background: #2D1810
- Border radius: 16px
- Padding: 24px
- No border, uses elevation via background contrast
- Contains gradient or image overlay

**Registration Card:**
- Background: #2D1810
- Border radius: 12px
- Padding: 20px
- Contains heading, description, and CTA button

**Info Card:**
- Background: transparent or #2D1810
- Border: none or 1px solid rgba(255, 255, 255, 0.1)
- Border radius: 8px
- Padding: 16px

### Tags/Badges

**Live Badge:**
- Background: #EF4444
- Text: #FFFFFF
- Font: 11px, 600 weight, uppercase
- Padding: 4px 8px
- Border radius: 4px
- Includes pulsing dot animation

**Category Tag:**
- Background: rgba(255, 255, 255, 0.15)
- Text: #FFFFFF
- Font: 12px, 500 weight
- Padding: 6px 12px
- Border radius: 16px (pill shape)

**Showcase Badge:**
- Background: rgba(255, 255, 255, 0.2)
- Text: #FFFFFF
- Font: 11px, 600 weight, uppercase
- Padding: 4px 10px
- Border radius: 4px

### Date Display

**Calendar Icon Style:**
- Background: #2D1810
- Border radius: 8px
- Width/Height: 48px
- Month label: 10px uppercase, orange (#F97316)
- Day number: 20px bold, white

### Lists

**Bullet Lists:**
- Bullet style: Filled circle
- Bullet color: #A8A29E
- Bullet size: 6px
- Text indent: 20px
- Item spacing: 8px

**Host List:**
- Avatar: 40px circle
- Name: 14px, 500 weight, white
- Subtitle: 12px, 400 weight, muted
- Social icons: 20px, muted color
- Row padding: 12px vertical

### Navigation

**Header:**
- Background: transparent (overlays content)
- Logo: White wordmark
- Links: 14px, 400 weight, white with hover underline
- Height: 56px
- Padding: 0 16px

**Footer:**
- Background: #1A0A0A (slightly darker)
- Border top: 1px solid rgba(255, 255, 255, 0.1)
- Logo: White, smaller size
- Links: 12px, muted color
- Padding: 24px 16px

## Layout Principles

- **Mobile-first:** Designed primarily for mobile viewing
- **Single column:** Content stacks vertically
- **Max width:** ~480px centered on larger screens
- **Generous whitespace:** Sections breathe with 32-48px gaps
- **Sticky elements:** Registration CTA may stick on scroll
- **Content hierarchy:** Hero → Details → Registration → About → Hosts

## Visual Effects

**Border Radius:**
- Cards/Containers: 12-16px
- Buttons: 6-8px
- Tags/Pills: 4px or 16px (full pill)
- Avatars: 50% (circle)
- Inputs: 8px

**Shadows:**
- Minimal shadow use — relies on background contrast
- Subtle lift on hover: 0 4px 12px rgba(0, 0, 0, 0.2)

**Borders:**
- Thickness: 1px
- Style: Solid
- Color: rgba(255, 255, 255, 0.1) to rgba(255, 255, 255, 0.3)
- Used sparingly for separation

**Backgrounds:**
- Solid colors dominate
- Subtle gradients on hero images
- Image overlays use dark gradient: linear-gradient(to bottom, transparent, #1A0A0A)

**Special Effects:**
- Live indicator: Pulsing red dot animation
- Hover transitions: 150ms ease
- Focus rings: 2px offset, orange (#F97316)

## Design Tone

This system exudes warmth and sophistication through its rich burgundy-brown palette, creating an intimate atmosphere perfect for event and community platforms. The design feels premium yet welcoming — like a well-appointed venue rather than a sterile corporate interface. Clean typography and generous spacing ensure content remains highly readable despite the dark theme, while orange accents provide energetic focal points without overwhelming the warm foundation.

## Usage Notes for AI Implementation

- Maintain the warm, earthy color temperature throughout — avoid cool grays
- Use the orange accent sparingly for key CTAs and live indicators
- Ensure sufficient contrast: white text on dark backgrounds, dark text on white buttons
- Keep the mobile-first mindset: single column, touch-friendly targets
- Lists should feel scannable with clear visual hierarchy
- Host/attendee sections should feel personal with circular avatars
- Registration sections should stand out but not feel aggressive
- Footer should recede visually while remaining functional
