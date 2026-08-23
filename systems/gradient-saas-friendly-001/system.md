---
id: gradient-saas-friendly-001
title: Citrus Cloud
description: A bright, approachable SaaS design system featuring vibrant purple-to-pink gradients, generous whitespace, and friendly rounded components
tags: [light, gradient, friendly, modern, saas, rounded]
colors: ["#7C3AED", "#EC4899", "#22C55E", "#FFFFFF", "#1F2937", "#6B7280"]
created: 2025-01-10
---

# Citrus Cloud

A warm, inviting design system built for SaaS platforms that prioritizes approachability and trust. The aesthetic combines vibrant gradient accents with clean white space, creating a professional yet friendly atmosphere. Bold purple-to-magenta gradients serve as the signature visual element, while soft shadows and generous border radii create a modern, polished feel.

## Color Palette

**Primary Gradient:**
- Gradient Start: #7C3AED — Rich violet, used as primary brand anchor
- Gradient Mid: #A855F7 — Transitional purple
- Gradient End: #EC4899 — Vibrant magenta/pink, adds energy and warmth

**Accent Colors:**
- Success Green: #22C55E — Used for positive actions, confirmations, checkmarks
- Teal Accent: #14B8A6 — Secondary accent for variety
- Soft Mint: #A7F3D0 — Light success backgrounds

**Neutral Colors:**
- Surface Primary: #FFFFFF — Primary background
- Surface Secondary: #F9FAFB — Subtle section differentiation
- Surface Tertiary: #F3F4F6 — Card backgrounds, input fields
- Text Primary: #1F2937 — Headings, important content
- Text Secondary: #4B5563 — Body text, descriptions
- Text Tertiary: #6B7280 — Captions, metadata
- Text Muted: #9CA3AF — Placeholder text, disabled states
- Border Light: #E5E7EB — Subtle dividers, card borders
- Border Medium: #D1D5DB — Input borders, stronger separation

**State Colors:**
- Error: #EF4444 — Validation errors, destructive actions
- Warning: #F59E0B — Caution states
- Info: #3B82F6 — Informational highlights

## Typography

**Font Families:**
- Primary: Inter, system-ui, -apple-system, sans-serif
- Monospace: ui-monospace, "SF Mono", Consolas, monospace (for code/labels)

**Type Scale:**
- Display: 48px, 800 weight, -0.02em letter-spacing, 1.1 line-height
- Heading 1: 36px, 700 weight, -0.02em letter-spacing, 1.2 line-height
- Heading 2: 28px, 700 weight, -0.01em letter-spacing, 1.25 line-height
- Heading 3: 22px, 600 weight, normal letter-spacing, 1.3 line-height
- Heading 4: 18px, 600 weight, normal letter-spacing, 1.4 line-height
- Body Large: 18px, 400 weight, 1.6 line-height
- Body: 16px, 400 weight, 1.6 line-height
- Body Small: 14px, 400 weight, 1.5 line-height
- Caption: 12px, 500 weight, 0.02em letter-spacing, 1.4 line-height
- Label: 13px, 600 weight, 0.05em letter-spacing, uppercase

**Hierarchy Rules:**
- Headings use tight letter-spacing for impact
- Body text uses generous line-height (1.6) for readability
- Labels and section markers use uppercase with wide letter-spacing
- Important numbers and metrics use tabular figures

## Spacing System

**Base Unit:** 4px

**Scale:**
- 4px (xs) — Tight inline spacing
- 8px (sm) — Icon gaps, tight component padding
- 12px (md) — Standard component padding
- 16px (base) — Default spacing, input padding
- 20px — Medium gaps
- 24px (lg) — Section padding, card padding
- 32px (xl) — Major section gaps
- 48px (2xl) — Page section spacing
- 64px (3xl) — Hero padding, major breaks
- 96px (4xl) — Full section separation

**Common Patterns:**
- Button padding: 12px 24px (small), 16px 32px (default), 20px 40px (large)
- Card padding: 24px (compact), 32px (default), 40px (spacious)
- Section spacing: 64px to 96px between major sections
- Grid gap: 24px (cards), 16px (tight grids)
- Input padding: 12px 16px

## Component Styles

### Buttons

**Primary Button:**
- Background: linear-gradient(135deg, #7C3AED 0%, #EC4899 100%)
- Text: #FFFFFF, 16px, 600 weight
- Padding: 14px 28px
- Border-radius: 12px
- Box-shadow: 0 4px 14px rgba(124, 58, 237, 0.35)
- Hover: brightness(1.05), shadow intensifies
- Active: brightness(0.95), shadow reduces
- Transition: all 0.2s ease

**Secondary Button:**
- Background: #FFFFFF
- Border: 1.5px solid #E5E7EB
- Text: #1F2937, 16px, 600 weight
- Padding: 14px 28px
- Border-radius: 12px
- Hover: background #F9FAFB, border-color #D1D5DB
- Active: background #F3F4F6

**Ghost Button:**
- Background: transparent
- Text: #7C3AED, 16px, 600 weight
- Padding: 14px 28px
- Hover: background rgba(124, 58, 237, 0.08)

**Text Link:**
- Color: #7C3AED
- Underline on hover
- Font-weight: 500

### Cards

**Default Card:**
- Background: #FFFFFF
- Border: 1px solid #E5E7EB
- Border-radius: 16px
- Padding: 24px to 32px
- Box-shadow: 0 1px 3px rgba(0, 0, 0, 0.05)

**Elevated Card:**
- Background: #FFFFFF
- Border: none
- Border-radius: 20px
- Padding: 32px
- Box-shadow: 0 10px 40px rgba(0, 0, 0, 0.08)

**Gradient Accent Card:**
- Same as elevated, with top border:
- Border-top: 4px solid transparent
- Border-image: linear-gradient(90deg, #7C3AED, #EC4899) 1

**Feature Card:**
- Background: #F9FAFB
- Border-radius: 16px
- Padding: 24px
- Icon container: 48px circle with gradient background

### Input Fields

**Default Input:**
- Background: #FFFFFF
- Border: 1.5px solid #D1D5DB
- Border-radius: 10px
- Padding: 14px 16px
- Font-size: 16px
- Placeholder color: #9CA3AF

**Focus State:**
- Border-color: #7C3AED
- Box-shadow: 0 0 0 3px rgba(124, 58, 237, 0.15)
- Outline: none

**Error State:**
- Border-color: #EF4444
- Box-shadow: 0 0 0 3px rgba(239, 68, 68, 0.15)

### Navigation

**Header:**
- Background: #FFFFFF
- Border-bottom: 1px solid #E5E7EB
- Height: 72px
- Padding: 0 24px (mobile), 0 48px (desktop)
- Box-shadow: 0 1px 3px rgba(0, 0, 0, 0.03)

**Nav Links:**
- Color: #4B5563
- Font-size: 15px
- Font-weight: 500
- Hover: color #1F2937
- Active: color #7C3AED

### Badges & Tags

**Default Badge:**
- Background: #F3F4F6
- Color: #4B5563
- Padding: 4px 10px
- Border-radius: 6px
- Font-size: 13px
- Font-weight: 500

**Gradient Badge:**
- Background: linear-gradient(135deg, rgba(124, 58, 237, 0.1), rgba(236, 72, 153, 0.1))
- Color: #7C3AED
- Border: 1px solid rgba(124, 58, 237, 0.2)

**Success Badge:**
- Background: #DCFCE7
- Color: #166534
- Border: 1px solid #BBF7D0

### Feature Numbers/Labels

**Section Label:**
- Format: "E/1", "M/2" style alphanumeric codes
- Font: Monospace
- Size: 14px
- Weight: 600
- Color: #7C3AED or gradient text
- Used for feature numbering

## Layout Principles

**Max Content Width:**
- Prose content: 720px
- Standard layout: 1120px
- Wide layout: 1280px
- Full-bleed sections allowed

**Grid Structure:**
- 12-column grid (desktop)
- 24px gutters
- 2-column, 3-column, and 4-column layouts for features
- Single column on mobile (<768px)

**Responsive Breakpoints:**
- Mobile: < 640px
- Tablet: 640px - 1024px
- Desktop: > 1024px

**Alignment:**
- Left-aligned text throughout
- Centered headings for hero sections
- Feature grids use consistent alignment

**Section Pattern:**
- Hero sections: generous padding (80px-120px vertical)
- Content sections: 64px vertical padding
- Alternating background colors (white/off-white) for rhythm

## Visual Effects

**Border Radius:**
- Buttons: 10px - 12px
- Cards: 16px - 20px
- Inputs: 10px
- Badges: 6px
- Full round: 9999px (pills, avatars)
- Subtle: 8px

**Shadows:**
- Subtle: 0 1px 3px rgba(0, 0, 0, 0.05)
- Card: 0 4px 6px rgba(0, 0, 0, 0.05)
- Elevated: 0 10px 40px rgba(0, 0, 0, 0.08)
- Button glow: 0 4px 14px rgba(124, 58, 237, 0.35)
- Focus ring: 0 0 0 3px rgba(124, 58, 237, 0.15)

**Borders:**
- Default: 1px solid #E5E7EB
- Strong: 1.5px solid #D1D5DB
- Accent: 2px solid with gradient

**Gradients:**
- Primary: linear-gradient(135deg, #7C3AED 0%, #EC4899 100%)
- Soft: linear-gradient(135deg, rgba(124, 58, 237, 0.1) 0%, rgba(236, 72, 153, 0.1) 100%)
- Text gradient: background-clip text with primary gradient

**Background Patterns:**
- Subtle dot grid pattern on hero sections
- Gradient orbs as decorative blurs
- Soft radial gradients for depth

## Design Tone

This system projects warmth, accessibility, and modern professionalism. The vibrant purple-to-pink gradient adds personality without sacrificing credibility, while generous whitespace and rounded corners create an inviting, low-friction experience. It feels like software built by people who genuinely care about making complex tools feel simple—approachable enough for first-time users, polished enough for enterprise.

## Usage Notes for AI Implementation

**Gradient Application:**
- Use gradients sparingly—primarily on CTAs, hero accents, and feature highlights
- Never use gradients on body text except for decorative headings
- Apply gradient to icons via background-clip when appropriate

**Typography Consistency:**
- Always use Inter or a similar geometric sans-serif
- Maintain the established size/weight hierarchy
- Use -0.02em letter-spacing on headings larger than 24px

**Component Assembly:**
- Combine elevated cards with gradient badges for feature highlights
- Use section labels (E/1, M/2 format) for numbered features
- Pair ghost buttons with primary buttons in CTAs

**Spacing Discipline:**
- Stick to the 4px base unit
- Use 64px+ for section separation
- Cards should have consistent 24-32px internal padding

**Color Usage:**
- Reserve the primary gradient for highest-priority actions
- Use #7C3AED as the standalone brand color when gradient isn't appropriate
- Maintain high contrast ratios (4.5:1 minimum for body text)

**Responsive Behavior:**
- Stack columns on mobile
- Reduce heading sizes by ~20% on mobile
- Maintain touch targets of 44px minimum
