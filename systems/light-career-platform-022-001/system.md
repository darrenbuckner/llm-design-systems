---
id: light-career-platform-022
title: Aspire Platform
description: A friendly, approachable light theme for professional development and career tools
tags: [light, friendly, professional, clean, rounded]
colors: ["#4285F4", "#34A853", "#F1F5F9", "#FFFFFF", "#1F2937", "#6B7280"]
created: 2026-01-08
---

# Aspire Platform

A warm, approachable design system optimized for professional development tools and career-focused applications. Features a clean white and soft gray foundation with vibrant blue-to-green gradient accents, creating an encouraging and trustworthy atmosphere.

## Color Palette

**Primary Colors:**
- Primary Blue: #4285F4 — Main interactive elements, buttons, links
- Secondary Green: #34A853 — Success states, growth indicators, secondary accent
- Teal Gradient: linear-gradient(90deg, #4285F4, #34A853) — Logo text, feature highlights

**Neutral Colors:**
- Surface White: #FFFFFF — Cards, primary content areas
- Background Gray: #F1F5F9 — Page backgrounds, secondary sections
- Muted Background: #E8EEF3 — Footer sections, subtle dividers
- Border Light: #E2E8F0 — Card borders, dividers

**Text Colors:**
- Text Primary: #1F2937 — Headings, body text
- Text Secondary: #6B7280 — Captions, helper text, metadata
- Text Muted: #9CA3AF — Placeholder text, disabled states

**State Colors:**
- Success: #34A853 — Positive feedback, completion states
- Info: #4285F4 — Informational states
- Error: #DC2626 — Error states, warnings
- Link: #2563EB — Underlined links, hover states

## Typography

**Font Families:**
- Primary: 'Inter', system-ui, sans-serif — All UI text
- Fallback: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto

**Type Scale:**
- Display: 32px, 700 weight, 1.2 line-height — Page titles
- Heading 1: 24px, 600 weight, 1.3 line-height — Section headers
- Heading 2: 20px, 600 weight, 1.4 line-height — Card titles
- Heading 3: 16px, 600 weight, 1.4 line-height — Subsection headers
- Body: 16px, 400 weight, 1.6 line-height — Primary content
- Body Small: 14px, 400 weight, 1.5 line-height — Secondary content
- Caption: 12px, 400 weight, 1.4 line-height — Metadata, labels

**Hierarchy Rules:**
- Headings use semi-bold (600) to bold (700) weights
- Body text uses regular (400) weight
- Clear size differentiation between hierarchy levels
- Generous line-height for readability

## Spacing System

**Base Unit:** 4px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80

**Common Patterns:**
- Component internal padding: 16px - 24px
- Card padding: 24px
- Section padding: 48px - 64px vertical
- Button padding: 12px 24px
- Grid gaps: 16px - 24px
- Container max-width: 800px (content), 1200px (full width)

## Component Styles

### Buttons

**Primary Button:**
- Background: #4285F4
- Text: #FFFFFF
- Font: 14px, 500 weight
- Padding: 12px 24px
- Border-radius: 8px
- Hover: Darken 10% (#3574E0)
- Active: Darken 15%

**Secondary Button:**
- Background: transparent
- Border: 1px solid #E2E8F0
- Text: #1F2937
- Font: 14px, 500 weight
- Padding: 10px 20px
- Border-radius: 20px (pill shape)
- Hover: Background #F1F5F9

**Text Link:**
- Color: #2563EB
- Text-decoration: underline
- Hover: Color #1D4ED8

### Cards

**Standard Card:**
- Background: #FFFFFF
- Border: 1px solid #E2E8F0
- Border-radius: 12px
- Padding: 24px
- Box-shadow: none or 0 1px 3px rgba(0,0,0,0.05)

**Feature Card (with icon):**
- Background: #FFFFFF
- Border: 1px solid #E2E8F0
- Border-radius: 12px
- Padding: 20px
- Icon: Sparkle/star icon in teal (#34A853)
- Title: 16px, 600 weight, centered
- Description: 14px, 400 weight, #6B7280, centered
- CTA button at bottom

### Input Fields

**Text Input:**
- Background: #FFFFFF
- Border: 1px solid #E2E8F0
- Border-radius: 8px
- Padding: 12px 16px
- Font: 16px
- Focus: Border #4285F4, box-shadow: 0 0 0 3px rgba(66,133,244,0.1)
- Placeholder: #9CA3AF

### Navigation

**Header:**
- Background: #FFFFFF
- Height: 64px
- Padding: 0 24px
- Border-bottom: none (clean)
- Logo: Gradient text (blue to green)
- CTA button: Primary blue, rounded

**Footer:**
- Background: #E8EEF3 (muted gray)
- Padding: 48px 24px
- Text: #6B7280
- Links: #2563EB with underline

## Layout Principles

- **Max content width:** 800px for reading content
- **Grid structure:** Single column for forms/content, 3-column grid for feature cards
- **Responsive behavior:** Cards stack on mobile, expand on desktop
- **Alignment:** Center-aligned for hero sections, left-aligned for body content
- **White space:** Generous padding creates breathing room

## Visual Effects

**Border Radius:**
- Small (buttons, inputs): 8px
- Medium (cards): 12px
- Large (featured sections): 16px
- Pill (badges, tags): 20px - 9999px

**Shadows:**
- Subtle: 0 1px 3px rgba(0,0,0,0.05) — Cards at rest
- Medium: 0 4px 12px rgba(0,0,0,0.08) — Elevated cards, hover states
- None: Most cards rely on borders rather than shadows

**Borders:**
- Default: 1px solid #E2E8F0
- Focused: 1px solid #4285F4
- Dividers: 1px solid #E2E8F0

**Backgrounds:**
- Primary surfaces: Solid white (#FFFFFF)
- Secondary sections: Soft gray (#F1F5F9)
- Footer/muted areas: Warmer gray (#E8EEF3)
- No gradients on backgrounds (gradients reserved for accent text)

## Design Tone

This system conveys **approachability, trust, and professional growth**. The clean white foundation with soft gray accents creates a calm, focused environment, while the blue-to-green gradient adds energy and optimism. The rounded corners and generous spacing soften the professional aesthetic, making it feel supportive rather than corporate. Perfect for career development, learning platforms, or professional tools that want to feel encouraging rather than intimidating.

## Usage Notes for AI Implementation

1. **Color application:** Use the blue primary (#4285F4) sparingly for CTAs and interactive elements. Reserve the gradient for logo/brand moments only.

2. **Typography:** Stick to Inter or a similar geometric sans-serif. Maintain clear hierarchy through weight and size changes.

3. **Cards:** Use white cards on gray backgrounds for visual separation. Keep borders subtle (#E2E8F0).

4. **Buttons:** Primary blue buttons for main CTAs, pill-shaped outline buttons for secondary actions.

5. **Spacing:** Be generous with whitespace. 48px+ between major sections, 24px card padding.

6. **Icons:** Use simple line icons, colored in teal/green (#34A853) or gray (#6B7280).

7. **Footer:** Always use the muted gray background (#E8EEF3) with subtle text colors.

8. **Accessibility:** Ensure sufficient contrast. Blue on white passes WCAG AA. Gray text (#6B7280) on white is borderline—use sparingly.
