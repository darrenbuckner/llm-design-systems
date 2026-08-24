---
id: soho-premium-001
title: Soho Premium Design System
description: "Premium lifestyle brand aesthetic with warm earth tones, elegant serif typography, and understated refinement."
tags: [light, minimal, premium, warm, editorial, gradient]
colors: ["#F5F3EF","#1A1A1A","#666666","#FFFFFF"]
created: 2025-12-12
---

![[Pasted image 20251202125505.png]]
# Soho Premium Membership Design System

## Color Palette

**Primary Colors:**

- Background Primary: #F5F3EF — Warm off-white, main canvas color for pages
- Background Secondary: #FFFFFF — Pure white for cards and elevated surfaces
- Text Primary: #1A1A1A — Near-black for headings and primary text
- Text Secondary: #666666 — Medium gray for body copy and descriptions

**Neutral Colors:**

- Surface Light: #FAFAF8 — Subtle warm tint for secondary backgrounds
- Border Light: #E8E6E2 — Soft warm gray for subtle dividers
- Border Medium: #D4D2CE — Slightly darker for defined borders

**Accent Colors:**

- Primary Action: #1A1A1A — Black for primary buttons and key CTAs
- Link/Interactive: #1A1A1A — Underlined black text for links
- Success/Green: #2D5016 — Deep forest green (seen in natural imagery accents)

**State Colors:**

- Hover (Buttons): #333333 — Slightly lighter than primary black
- Focus: #1A1A1A with 2px border offset
- Disabled: #CCCCCC — Light gray with reduced opacity

## Typography

**Font Families:**

- Primary: Clean serif font family, similar to Georgia/Freight Text — used for headings and display text
- Secondary: Sans-serif font family, similar to Helvetica/Arial — used for body text, navigation, and UI elements

**Type Scale:**

- Hero Heading: 48-56px, Regular (400), 1.1 line-height — Large display text
- Heading 1: 36-42px, Regular (400), 1.2 line-height — Section headings
- Heading 2: 28-32px, Regular (400), 1.3 line-height — Subsection headings
- Heading 3: 20-24px, Regular (400), 1.4 line-height — Card titles
- Body Large: 18px, Regular (400), 1.6 line-height — Lead paragraphs
- Body: 16px, Regular (400), 1.6 line-height — Standard body text
- Body Small: 14px, Regular (400), 1.5 line-height — Captions and secondary info
- Caption: 12px, Regular (400), 1.4 line-height — Fine print and labels

**Hierarchy Rules:**

- Headings use serif font for editorial feel
- Body text and UI elements use sans-serif for clarity
- Generous line-height (1.6) for readability
- Weight stays primarily at Regular (400) with occasional Medium (500) for emphasis
- Letter-spacing: tight (-0.02em) on large headings, normal on body

## Spacing System

**Base Unit:** 8px

**Scale:** 8, 16, 24, 32, 40, 48, 64, 80, 96, 120

**Common Patterns:**

- Component padding: 16-24px for small elements, 32-48px for larger containers
- Section spacing: 80-120px vertical spacing between major sections
- Grid gaps: 24-32px between grid items
- Card padding: 32px on desktop, 24px on mobile
- Button padding: 16px vertical, 32px horizontal
- Inline element gaps: 8-16px between adjacent elements

## Component Styles

### Buttons

**Primary Button:**

- Background: #1A1A1A (black)
- Text: #FFFFFF (white)
- Padding: 16px 32px
- Border-radius: 24px (pill shape)
- Font: 14-16px, Medium (500), sans-serif
- Hover: Background #333333, slight scale (1.02)
- Height: 48px minimum

**Secondary Button (Outlined):**

- Background: Transparent
- Border: 2px solid #1A1A1A
- Text: #1A1A1A
- Padding: 14px 30px (adjusted for border)
- Border-radius: 24px
- Hover: Background #1A1A1A, text #FFFFFF

**Text Button:**

- Background: None
- Text: #1A1A1A with underline
- Padding: 4px 0
- Hover: Underline thickens or text color shifts to #333333

### Cards

**Standard Card:**

- Background: #FFFFFF
- Border: None (uses shadow for elevation)
- Border-radius: 8px
- Padding: 32px
- Shadow: 0 2px 16px rgba(0, 0, 0, 0.08) — subtle, soft
- Hover: Shadow increases to 0 4px 24px rgba(0, 0, 0, 0.12)

**Image Card:**

- Image: Full-width within card, 16:10 or 3:2 aspect ratio
- Border-radius: 8px 8px 0 0 (on image top corners)
- Content padding: 24px below image
- Text overlay option: Gradient overlay from transparent to rgba(0,0,0,0.6)

### Input Fields

**Text Input:**

- Border: 1px solid #D4D2CE
- Background: #FFFFFF
- Border-radius: 4px
- Padding: 12px 16px
- Height: 48px
- Font: 16px, Regular
- Focus: Border #1A1A1A, 2px, shadow 0 0 0 3px rgba(26,26,26,0.1)

**Textarea:**

- Same as text input
- Min-height: 120px
- Resize: vertical only

### Navigation

**Top Navigation:**

- Background: #F5F3EF (matches page background)
- Height: 72px
- Padding: 0 32px
- Border-bottom: 1px solid #E8E6E2
- Font: 14px, Medium (500), sans-serif
- Link color: #1A1A1A
- Hover: Underline appears

**Footer:**

- Background: #1A1A1A (black)
- Text: #FFFFFF
- Padding: 64px 32px
- Link color: #FFFFFF
- Link hover: Opacity 0.7
- Multi-column layout with 24px gaps

### Lists

**Bullet List (Benefits):**

- Bullet: Small circle or checkmark
- Item spacing: 12px between items
- Font: 16px, Regular
- Bullet color: #666666 or #1A1A1A

**Icon + Text List:**

- Icon size: 24px
- Icon-to-text gap: 16px
- Vertical alignment: center
- Item spacing: 16-24px

## Layout Principles

**Max Content Width:**

- Primary content: 1280px maximum
- Text-heavy content: 720px maximum for readability
- Full-width sections: 100% with internal padding

**Grid Structure:**

- 12-column grid on desktop
- 8-column on tablet
- 4-column on mobile
- Column gap: 24-32px
- Outer margins: 32px (mobile), 48px (tablet), 64px (desktop)

**Responsive Behavior:**

- Breakpoints: 640px, 1024px, 1280px
- Images: Scale proportionally, maintain aspect ratios
- Text: Reduces 1-2 sizes on mobile
- Stack columns vertically on mobile
- Padding reduces by ~25% on smaller screens

**Alignment:**

- Primary alignment: Left-aligned text for body content
- Centered: Headings in hero sections, CTAs
- Justified: Never used
- Images: Often centered with text content aligned left

## Visual Effects

**Border Radius:**

- Buttons: 24px (pill shape)
- Cards: 8px
- Images: 8px
- Input fields: 4px
- Badges/tags: 16px (small pill)

**Shadows:**

- Subtle elevation: 0 2px 16px rgba(0, 0, 0, 0.08)
- Medium elevation: 0 4px 24px rgba(0, 0, 0, 0.12)
- High elevation: 0 8px 32px rgba(0, 0, 0, 0.16)
- No inner shadows used

**Borders:**

- Thickness: 1px standard, 2px for emphasis
- Style: Solid only, no dashed or dotted
- Usage: Minimal — primarily for input fields and subtle dividers
- Color: Warm neutrals (#E8E6E2, #D4D2CE)

**Backgrounds:**

- Solid colors: Primary approach
- Gradients: Subtle overlays on images (linear, transparent to black)
- Patterns: None
- Textures: Natural photography with warm, earthy tones
- Image treatment: High-quality lifestyle photography, often with natural lighting

## Design Tone

Premium yet approachable luxury lifestyle brand aesthetic. The design balances sophistication with warmth through a muted earth-tone palette, generous whitespace, and elegant serif typography for headings paired with clean sans-serif for functionality. The overall feel is understated refinement — not flashy or ostentatious, but quietly confident and inviting. Photography plays a central role, featuring natural settings, architectural details, and lifestyle moments that convey exclusivity and community.

## Usage Notes for AI Implementation

- **Restraint over decoration:** Use ample whitespace; don’t fill every pixel
- **Photography-first:** High-quality lifestyle imagery is essential to the brand; text should support, not compete with images
- **Hierarchy through space, not weight:** Create visual hierarchy primarily through spacing and size rather than heavy font weights
- **Warm neutrals throughout:** Avoid cool grays; maintain the warm, inviting tone in all neutral colors
- **Pill-shaped buttons only:** All CTAs should use the signature rounded pill shape (24px radius)
- **Minimal borders:** Rely on whitespace and subtle shadows for separation rather than borders
- **Serif for emotion, sans-serif for clarity:** Headings carry the editorial voice; UI elements prioritize legibility
- **Accessibility baseline:** Maintain minimum 4.5:1 contrast ratios; black text on warm off-white backgrounds passes WCAG AA
- **Touch targets:** Minimum 48px height for all interactive elements
- **Consistent rhythm:** Use the 8px spacing scale religiously to maintain visual consistency​​​​​​​​​​​​​​​​