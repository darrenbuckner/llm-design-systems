---
id: gradient-coral-faq-001
title: Coral Bloom System
description: A warm, inviting gradient-to-light design system with friendly typography and accessible FAQ patterns
tags: [gradient, light, warm, friendly, SaaS]
colors: ["#F83B72", "#FF6B8A", "#4B5EFF", "#1A1A2E", "#F8F9FA", "#6B7280"]
created: 2026-01-10
---

# Coral Bloom System

A warm and approachable design system featuring a vibrant coral-to-pink gradient hero transitioning into clean, light content sections. The aesthetic balances energetic brand presence with highly readable FAQ and content areas, creating an inviting yet professional SaaS experience.

## Color Palette

**Gradient Colors:**
- Gradient Start: #F83B72 — Vibrant coral pink, used at top of hero
- Gradient Mid: #FF6B8A — Soft coral, mid-gradient transition
- Gradient End: #FFB3C1 — Light pink wash, bottom of gradient

**Primary Colors:**
- Primary Action: #F83B72 — Used for primary buttons and CTAs
- Link/Accent: #4B5EFF — Bright indigo blue for text links

**Neutral Colors:**
- Background Light: #F8F9FA — Subtle off-white for FAQ sections
- Surface White: #FFFFFF — Pure white for cards and buttons
- Text Primary: #1A1A2E — Near-black for headings and body text
- Text Secondary: #6B7280 — Medium gray for supporting text
- Border Light: #E5E7EB — Subtle gray for dividers and card borders

**State Colors:**
- Success: #10B981 — Green for positive states
- Warning: #F59E0B — Amber for caution states
- Error: #EF4444 — Red for error states

## Typography

**Font Families:**
- Primary: Inter (or similar geometric sans-serif)
- Fallback: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif

**Type Scale:**
- Display/Hero: 18px, 500 weight, 1.5 line-height — White on gradient
- Heading 1: 42px, 400 weight, 1.2 line-height — FAQ main heading
- Heading 2: 24px, 600 weight, 1.3 line-height — FAQ question headings
- Body: 18px, 400 weight, 1.6 line-height — FAQ answer text
- Body Small: 16px, 400 weight, 1.5 line-height — Supporting content
- Caption: 14px, 400 weight, 1.4 line-height — Cookie banner text
- Button: 16-18px, 500-600 weight — CTA buttons

**Hierarchy Rules:**
- Hero text uses white on gradient for maximum contrast
- FAQ headings use dark near-black for readability
- Body text in a softer dark shade with generous line-height
- Links stand out with bright indigo color and no underline by default

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 80, 96

**Common Patterns:**
- Section padding: 64px vertical, 24px horizontal (mobile)
- Component padding: 16-24px
- FAQ item spacing: 32px between questions
- Button padding: 16px 32px (large), 12px 24px (medium)
- Card padding: 24px
- Container max-width: ~800px for content areas

## Component Styles

### Buttons

**Primary Button (White on Gradient):**
- Background: #FFFFFF
- Text: #F83B72 (gradient primary color)
- Padding: 20px 48px
- Border-radius: 8px
- Font-weight: 600
- Font-size: 18px
- Shadow: none
- Full-width on mobile

**Secondary/Ghost Button (On Gradient):**
- Background: transparent
- Text: #FFFFFF
- Padding: 12px 24px
- Font-weight: 500
- Icon: Right arrow (→)
- Hover: Slight opacity change

**Cookie Banner Buttons:**
- Accept: Background #4B5EFF, Text #FFFFFF, Border-radius: 8px
- Decline: Background #F3F4F6, Text #1A1A2E, Border-radius: 8px
- Link style: Underlined text

### Cards

**Cookie Consent Modal:**
- Background: #FFFFFF
- Border-radius: 16px
- Shadow: 0 -4px 20px rgba(0,0,0,0.1)
- Padding: 24px
- Position: Fixed bottom
- Width: 100% on mobile

### Navigation

**Header:**
- Background: Transparent on gradient
- Logo + wordmark left-aligned
- Hamburger menu icon (mobile)
- Primary CTA button right-aligned
- Button style: Filled with gradient background, white text

### Input Fields

**Text Inputs:**
- Background: #FFFFFF
- Border: 1px solid #E5E7EB
- Border-radius: 8px
- Padding: 12px 16px
- Focus: Border color #4B5EFF

### Links

**Text Links:**
- Color: #4B5EFF
- Text-decoration: none (hover: underline)
- Font-weight: 400-500

## Layout Principles

- **Max content width:** ~800px for text content, centered
- **Grid structure:** Single column on mobile, content-focused layout
- **Responsive behavior:** Full-width gradient hero, contained content below
- **Alignment:** Left-aligned text in FAQ sections, centered hero content
- **Mobile-first:** Generous touch targets, stacked layouts

## Visual Effects

**Border Radius:**
- Buttons: 8px
- Cards/Modals: 16px
- Inputs: 8px
- Small elements: 4px

**Shadows:**
- Modal: 0 -4px 20px rgba(0,0,0,0.1)
- Cards: 0 2px 8px rgba(0,0,0,0.05)
- Elevated: 0 4px 16px rgba(0,0,0,0.1)

**Borders:**
- Dividers: 1px solid #E5E7EB
- Inputs: 1px solid #E5E7EB
- Cards: Optional 1px solid #E5E7EB or shadow only

**Gradients:**
- Hero: linear-gradient(180deg, #F83B72 0%, #FF6B8A 50%, #FFB3C1 100%)
- Subtle fade to light section below

## Design Tone

The Coral Bloom System projects warmth, friendliness, and approachability through its vibrant gradient hero that immediately captures attention, then transitions to clean, highly readable content sections. The design feels modern and SaaS-appropriate without being cold or corporate—it's the visual equivalent of a helpful conversation. The generous whitespace, clear typography hierarchy, and inviting color palette make complex information feel accessible and easy to navigate.

## Usage Notes for AI Implementation

**When implementing this system:**

1. **Gradient Hero Sections:** Use the coral-to-pink gradient sparingly—primarily for hero areas and key CTAs. The gradient creates visual hierarchy by drawing attention upward.

2. **Typography Contrast:** Maintain high contrast ratios. White text on gradient, dark text on light backgrounds. Never use gradient text or low-contrast combinations.

3. **FAQ Patterns:** Keep questions as bold headings (h2/h3) with regular-weight answers below. Generous vertical spacing between Q&A pairs improves scannability.

4. **Button Hierarchy:** Primary actions get the white-on-gradient treatment. Secondary actions use ghost buttons or the indigo accent color.

5. **Mobile Considerations:** Full-width buttons, adequate padding (min 24px container), and touch-friendly tap targets (min 44px).

6. **Color Usage:** Reserve the coral pink for primary brand moments. Use the indigo blue for interactive text elements. Keep content sections predominantly white/light gray.

7. **Modals and Overlays:** Use rounded corners (16px) and subtle shadows for floating elements. Position cookie/consent banners at bottom with full-width on mobile.
