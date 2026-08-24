---
id: light-warm-gradient-022
title: Sunrise Product System
description: A warm, inviting light theme with soft gradients and purple accents for friendly SaaS products
tags: [light, gradient, warm, friendly, modern, saas]
colors: ["#7C3AED", "#EC4899", "#F59E0B", "#1F2937", "#F8F5F2", "#FFFFFF"]
created: 2026-01-10
---

# Sunrise Product System

A warm and inviting design system featuring soft peach-to-lavender gradients, vibrant purple primary actions, and a friendly typographic hierarchy. This system creates an approachable, modern feel perfect for productivity tools and SaaS platforms targeting creative professionals and teams.

## Color Palette

**Primary Colors:**
- Primary Purple: #7C3AED — Primary actions, CTA buttons, key interactive elements
- Primary Purple Hover: #6D28D9 — Hover state for primary buttons

**Accent Colors:**
- Pink Accent: #EC4899 — Gradient text highlights, emphasis numbers
- Amber Accent: #F59E0B — Secondary highlights, star ratings, icons
- Teal Accent: #14B8A6 — Alternative accent for links and stats

**Gradient Definitions:**
- Hero Gradient: Linear gradient from #FDE8E0 (peach) through #F5E6F0 (lavender) to #E8E0F5 (soft purple)
- Text Gradient: Linear gradient from #7C3AED (purple) through #EC4899 (pink) to #F59E0B (amber)
- Mountain Illustration: Soft layers of #F5D0C5, #E8C8D8, #D0C0E8 with varying opacity

**Neutral Colors:**
- Background: #FFFFFF — Page background, cards
- Surface Warm: #F8F5F2 — Subtle warm background tint
- Hero Background: #FDF8F5 — Warm cream base for gradient sections
- Text Primary: #1F2937 — Main headings and body text
- Text Secondary: #6B7280 — Supporting text, descriptions
- Text Muted: #9CA3AF — Placeholder text, tertiary content
- Border Light: #E5E7EB — Card borders, dividers
- Border Subtle: #F3F4F6 — Very light separators

**State Colors:**
- Success: #10B981 — Positive states, confirmations
- Warning: #F59E0B — Caution states, alerts
- Error: #EF4444 — Error states, destructive actions
- Info: #3B82F6 — Informational highlights

## Typography

**Font Families:**
- Primary: Inter, system-ui, -apple-system, sans-serif — All UI text
- Display: Inter with tighter letter-spacing — Large headlines

**Type Scale:**
- Display/Hero: 42px, weight 400 (light), line-height 1.2, letter-spacing -0.02em
- Heading 1: 36px, weight 600, line-height 1.25
- Heading 2: 28px, weight 600, line-height 1.3
- Heading 3: 22px, weight 600, line-height 1.4
- Body Large: 18px, weight 400, line-height 1.6
- Body: 16px, weight 400, line-height 1.6
- Body Bold: 16px, weight 700, line-height 1.6
- Caption: 14px, weight 500, line-height 1.5
- Small: 12px, weight 400, line-height 1.5

**Hierarchy Rules:**
- Hero headlines use lighter weight (400) with gradient color effects on key words
- Body text within hero uses mix of regular and bold weights for emphasis
- Stats and numbers use accent colors (pink, amber) for visual pop
- Links use teal/purple colors with underline on hover

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96

**Common Patterns:**
- Component internal padding: 16px - 24px
- Button padding: 16px vertical, 32px horizontal (large), 12px vertical, 24px horizontal (medium)
- Card padding: 24px - 32px
- Section spacing: 64px - 96px vertical
- Container max-width: 1200px with 24px horizontal padding
- Mobile container padding: 16px - 20px

**Grid System:**
- 12-column grid at desktop
- 24px gap between columns
- Single column on mobile with full-width stacking

## Component Styles

### Buttons

**Primary Button:**
- Background: #7C3AED (purple)
- Text: #FFFFFF, 16px, weight 600
- Padding: 16px 32px
- Border-radius: 12px
- Shadow: 0 4px 14px rgba(124, 58, 237, 0.25)
- Hover: Background #6D28D9, shadow increases
- Active: Scale 0.98
- Icon: Arrow right (→) with 8px left margin
- Full-width on mobile

**Secondary Button:**
- Background: #FFFFFF
- Text: #7C3AED, 16px, weight 600
- Border: 1px solid #E5E7EB
- Padding: 16px 32px
- Border-radius: 12px
- Shadow: 0 1px 3px rgba(0, 0, 0, 0.05)
- Hover: Border color #7C3AED, subtle purple tint
- Icon: Play triangle (▶) for video/demo CTAs

**Pill/Tag Button:**
- Background: #FFFFFF
- Text: #1F2937, 14px, weight 500
- Padding: 10px 20px
- Border-radius: 999px (full pill)
- Shadow: 0 2px 8px rgba(0, 0, 0, 0.08)
- Icon: Sparkle emoji (✨) for "new" indicators

### Cards

**Standard Card:**
- Background: #FFFFFF
- Border: 1px solid #E5E7EB
- Border-radius: 16px
- Padding: 24px
- Shadow: 0 4px 12px rgba(0, 0, 0, 0.05)

**Hero Section Card:**
- Background: Linear gradient (peach to lavender)
- Border-radius: 24px
- Padding: 48px 24px
- Contains decorative mountain/wave illustration

### Input Fields

**Text Input:**
- Background: #FFFFFF
- Border: 1px solid #E5E7EB
- Border-radius: 10px
- Padding: 14px 16px
- Font: 16px, weight 400, color #1F2937
- Placeholder: #9CA3AF
- Focus: Border #7C3AED, ring 0 0 0 3px rgba(124, 58, 237, 0.1)

### Navigation

**Header:**
- Background: #FFFFFF
- Border-bottom: 1px solid #E5E7EB
- Height: 72px
- Logo: Icon + wordmark, left-aligned
- Menu: Hamburger icon on mobile, inline links on desktop
- CTA Button: Primary purple "Sign Up" button, right-aligned

**Logo Style:**
- Icon: Rounded square with gradient (purple to pink)
- Wordmark: 20px, weight 700, color #1F2937

### Social Proof Section

**Stats Display:**
- Number: 24px, weight 700, color #EC4899 or #14B8A6
- Label: 16px, weight 400, color #1F2937
- Arrangement: Inline with comma separation or stacked

**Rating Display:**
- Star icon: #F59E0B (amber)
- Text: 16px, weight 500, color #6B7280

### Chat Widget

**Floating Button:**
- Background: #374151 (dark gray)
- Icon: Chat bubble, white
- Size: 56px diameter
- Border-radius: 50%
- Position: Fixed, bottom-right, 24px offset
- Shadow: 0 4px 12px rgba(0, 0, 0, 0.15)

## Layout Principles

- **Max content width:** 1200px for main content, 800px for text-heavy sections
- **Hero sections:** Full-width gradient backgrounds with contained content
- **Grid structure:** Single column mobile, 2-3 columns tablet, flexible desktop
- **Alignment:** Center-aligned for hero/marketing sections, left-aligned for content
- **Responsive behavior:** Stack at 768px breakpoint, reduce spacing on mobile

## Visual Effects

**Border Radius:**
- Small (inputs, tags): 8px - 10px
- Medium (buttons, cards): 12px - 16px
- Large (hero sections): 24px
- Full (pills, avatars): 999px

**Shadows:**
- Subtle: 0 1px 3px rgba(0, 0, 0, 0.05)
- Card: 0 4px 12px rgba(0, 0, 0, 0.05)
- Button: 0 4px 14px rgba(124, 58, 237, 0.25)
- Elevated: 0 8px 24px rgba(0, 0, 0, 0.1)

**Borders:**
- Default: 1px solid #E5E7EB
- Subtle: 1px solid #F3F4F6
- Active/Focus: 1px solid #7C3AED

**Backgrounds:**
- Gradient hero: Soft peach-to-lavender watercolor effect
- Decorative elements: Abstract mountain/wave shapes in muted gradient tones
- Texture: Subtle grain overlay at 2-3% opacity for organic feel

**Gradient Text:**
- Applied to key words in headlines
- Direction: Left to right
- Colors: #7C3AED → #EC4899 → #F59E0B
- Implementation: background-clip: text with transparent text color

## Design Tone

This system embodies warmth, approachability, and modern professionalism. The soft gradient backgrounds create an inviting atmosphere while purple primary actions convey creativity and innovation. The friendly typography with strategic bold emphasis guides users naturally through content. Overall, the aesthetic balances playfulness with credibility—ideal for tools that want to feel both powerful and accessible.

## Usage Notes for AI Implementation

1. **Gradient text effect**: Use `background: linear-gradient()` with `background-clip: text` and `-webkit-text-fill-color: transparent` for highlighted words in headlines

2. **Hero sections**: Wrap content in a container with the warm gradient background; use subtle decorative shapes at low opacity for depth

3. **Button hierarchy**: Primary purple for main CTA, white/bordered for secondary actions; always include arrow icon on primary buttons

4. **Social proof**: Use pink (#EC4899) for impressive numbers, combine with descriptive text; include star rating with amber color

5. **Mobile considerations**: Full-width buttons, reduced padding (16-20px), stacked layouts, maintain gradient effects

6. **Emphasis pattern**: Use bold weight (700) within body text to highlight key phrases rather than relying on color alone

7. **Whitespace**: Generous vertical spacing (64-96px between sections) creates breathing room and premium feel

8. **Interactive states**: All clickable elements need clear hover states—buttons darken, links get underlines, cards lift slightly
