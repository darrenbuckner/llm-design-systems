---
id: light-warm-wellness-001
title: Sage Grove System
description: A warm, nurturing design system with earthy greens and creamy neutrals for wellness and care applications
tags: [light, warm, organic, wellness, friendly, accessible]
colors: ["#4A5D4A", "#F5F2EC", "#E8E4DC", "#2D3B2D", "#6B7B6B"]
created: 2026-02-08
---

# Sage Grove System

A warm and nurturing design system built for wellness, care, and family-oriented applications. The aesthetic combines earthy sage greens with creamy off-white backgrounds, creating a sense of trust, calm, and natural warmth. Typography is friendly yet professional, with generous spacing that allows content to breathe.

## Color Palette

**Primary Colors:**
- Primary Green: #4A5D4A — Main brand color, used for headers, primary buttons, and key UI elements
- Primary Dark: #2D3B2D — Deep forest green for emphasis text and hover states

**Neutral Colors:**
- Background Cream: #F5F2EC — Primary page background, warm off-white
- Surface Light: #FDFCFA — Card backgrounds and elevated surfaces
- Surface Warm: #E8E4DC — Secondary backgrounds, section dividers
- Border Light: #D4CFC5 — Subtle borders and dividers
- Text Primary: #2D3B2D — Main body text, nearly black with green undertone
- Text Secondary: #6B7B6B — Supporting text, labels, captions
- Text Muted: #9A9A8A — Placeholder text, disabled states

**Accent/State Colors:**
- Success: #4A7D4A — Confirmation, positive states
- Warning: #B8934A — Alerts, caution states
- Error: #8B4A4A — Error messages, destructive actions
- Link: #4A5D4A — Interactive text links

## Typography

**Font Families:**
- Primary: Inter or system sans-serif stack (-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto)
- Display: Optional serif for hero headlines (Georgia or similar)

**Type Scale:**
- Display: 40px, 700 weight, 1.1 line-height — Hero headlines
- Heading 1: 32px, 600 weight, 1.2 line-height — Page titles
- Heading 2: 24px, 600 weight, 1.3 line-height — Section headers
- Heading 3: 20px, 600 weight, 1.4 line-height — Card titles
- Body Large: 18px, 400 weight, 1.6 line-height — Lead paragraphs
- Body: 16px, 400 weight, 1.6 line-height — Standard body text
- Body Small: 14px, 400 weight, 1.5 line-height — Supporting text
- Caption: 12px, 500 weight, 1.4 line-height — Labels, metadata

**Hierarchy Rules:**
- Headlines use darker green (#2D3B2D) for maximum contrast
- Body text uses slightly lighter shade for comfortable reading
- Section headers often centered with generous vertical spacing
- Subheadings may use secondary green (#4A5D4A) for visual variety

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 80, 96

**Common Patterns:**
- Component internal padding: 16px-24px
- Section vertical spacing: 64px-96px
- Card padding: 24px-32px
- Button padding: 12px horizontal, 16px-20px vertical
- Form field padding: 12px-16px
- Grid gaps: 24px-32px

## Component Styles

### Buttons

**Primary Button:**
- Background: #4A5D4A
- Text: #FFFFFF
- Border radius: 8px
- Padding: 16px 32px
- Font: 16px, 500 weight
- Hover: Background darkens to #3D4D3D
- Active: Background #2D3B2D

**Secondary Button:**
- Background: transparent
- Border: 1.5px solid #4A5D4A
- Text: #4A5D4A
- Border radius: 8px
- Padding: 16px 32px
- Hover: Background #F0EDE7

**Text Button:**
- Background: transparent
- Text: #4A5D4A
- Underline on hover
- Padding: 8px 0

### Cards

**Standard Card:**
- Background: #FDFCFA
- Border: 1px solid #E8E4DC
- Border radius: 12px
- Padding: 24px-32px
- Shadow: 0 2px 8px rgba(45, 59, 45, 0.06)

**Featured Card:**
- Background: #4A5D4A
- Text: #FFFFFF
- Border radius: 16px
- Padding: 32px-48px
- No border

### Input Fields

**Text Input:**
- Background: #FFFFFF
- Border: 1.5px solid #D4CFC5
- Border radius: 8px
- Padding: 14px 16px
- Font: 16px
- Focus: Border color #4A5D4A, subtle shadow
- Placeholder: #9A9A8A

**Select/Dropdown:**
- Same styling as text input
- Custom chevron icon in secondary color

### Navigation

**Header:**
- Background: transparent or #FDFCFA
- Logo: Dark green text mark
- Nav links: #2D3B2D, 14px, 500 weight
- Mobile: Hamburger menu icon

**Footer:**
- Background: #E8E4DC or #4A5D4A (inverse)
- Organized in columns
- Links: 14px, regular weight
- Social icons: 24px

## Layout Principles

- Max content width: 1200px (large), 800px (content-focused)
- Grid structure: 12-column on desktop, single column mobile
- Generous whitespace between sections (64px-96px)
- Content often centered with comfortable reading width (600-700px)
- Images frequently use rounded corners (12px-16px)
- Hero sections may include nature imagery with text overlay

## Visual Effects

**Border Radius:**
- Small elements (badges, tags): 4px
- Buttons, inputs: 8px
- Cards: 12px
- Large containers, images: 16px
- Pill shapes: 9999px (full radius)

**Shadows:**
- Subtle: 0 2px 4px rgba(45, 59, 45, 0.04)
- Card: 0 4px 12px rgba(45, 59, 45, 0.08)
- Elevated: 0 8px 24px rgba(45, 59, 45, 0.12)
- Focus rings: 0 0 0 3px rgba(74, 93, 74, 0.2)

**Borders:**
- Standard: 1px solid #E8E4DC
- Emphasized: 1.5px solid #D4CFC5
- Dividers: 1px solid #E8E4DC

**Backgrounds:**
- Solid cream: #F5F2EC
- Subtle gradient: linear-gradient(180deg, #FDFCFA 0%, #F5F2EC 100%)
- Hero overlays: Semi-transparent dark green on images

## Design Tone

This system embodies warmth, trust, and natural care. The earthy green palette evokes growth and wellness, while cream backgrounds create a soft, inviting atmosphere. Typography is approachable yet professional, avoiding clinical coldness. The overall effect is that of a trusted friend or caregiver—competent, warm, and genuinely supportive.

## Usage Notes for AI Implementation

- Always maintain generous whitespace; this system breathes
- Use the primary green sparingly for maximum impact
- Body text should never feel cramped; err on the side of larger line-heights
- Images should feel natural and authentic, avoid stock photo sterility
- Icons should be simple line-style, matching the friendly aesthetic
- CTAs should be clear but not aggressive; the tone is supportive, not pushy
- Mobile layouts should stack gracefully with maintained spacing ratios
- Form validation should feel helpful, not punitive
- Consider accessibility: ensure 4.5:1 contrast ratios for all text
