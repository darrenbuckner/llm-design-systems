---
id: light-warm-playbook-025
title: Terracotta Playbook
description: Warm editorial layout with bold serif headings, soft peach backgrounds, coral CTAs, and numbered card grids for structured content
tags: [light, warm, editorial, serif, cards, structured, playbook]
colors: ["#F5EDE4", "#E8573D", "#1A1A1A", "#FFFFFF", "#5C5C5C", "#E8E0D6"]
created: 2026-03-20
---

# Terracotta Playbook

A warm, confident editorial system built for structured content playbooks and resource pages. Combines bold serif display headings with clean sans-serif body text on a soft peach/cream canvas. Coral-red primary actions pop against muted earth tones. Numbered card grids organize content into clear, scannable sequences. The overall feel is authoritative yet approachable — like a well-designed handbook you'd actually want to read.

## Color Palette

**Primary Colors:**
- Primary/CTA: #E8573D — Coral-red used for primary buttons, link text, and badge accents
- Background: #F5EDE4 — Warm peach-cream page background; the dominant surface color

**Neutral Colors:**
- Surface/Cards: #FFFFFF — White card backgrounds, providing contrast against the warm page
- Text Primary: #1A1A1A — Near-black for headlines and bold content
- Text Secondary: #5C5C5C — Muted gray for body copy, descriptions, and supporting text
- Text Tertiary: #8A8A8A — Lighter gray for numbering, metadata, and captions
- Borders: #E8E0D6 — Warm light border, slightly darker than the page background
- Card Border: #EAEAEA — Neutral light gray border on white cards

**Accent/State Colors:**
- Badge Background: #FFF0ED — Very light coral tint behind category badges
- Badge Text: #E8573D — Coral text inside badges, matching primary
- Badge Alternate BG: #F0F0F0 — Neutral light gray for secondary badge categories
- Badge Alternate Text: #444444 — Dark gray for secondary badge text
- Success: #2E7D32 — Forest green (inferred)
- Warning: #E8A73D — Warm amber (inferred)
- Error: #D32F2F — Standard red (inferred)

## Typography

**Font Families:**
- Display/Headlines: Serif typeface — appears to be a bold condensed/display serif similar to "DM Serif Display" or "Playfair Display" with tight tracking. Very high contrast letterforms, slightly condensed.
- Body/UI: Clean geometric sans-serif — appears to be Inter, system-ui, or similar neutral grotesque
- Badges/Labels: Same sans-serif as body, used at small sizes with medium weight

**Type Scale:**
- Display (Hero H1): ~56-64px, 800/Black weight, tight line-height (~1.05), serif. Very bold and commanding.
- Subtitle (Hero H2): ~22-24px, 500/Medium weight, ~1.4 line-height, sans-serif italic. Secondary messaging below the main headline.
- Section Heading (H2): ~32-36px, 700/Bold weight, ~1.2 line-height, serif. Used for "7 AI Skills..." style section titles.
- Card Title (H3): ~18-20px, 700/Bold weight, ~1.3 line-height, sans-serif. Card headings like skill names.
- Body: 16px, 400/Regular weight, ~1.6 line-height, sans-serif. Comfortable reading size.
- Card Body: 15px, 400/Regular weight, ~1.5 line-height, sans-serif. Slightly smaller in cards.
- Link/CTA Text: 15-16px, 600/SemiBold weight, sans-serif with arrow (→).
- Badge: 12-13px, 500/Medium weight, sans-serif, uppercase or title case.
- Card Number: 14px, 500/Medium weight, sans-serif, muted color.

**Hierarchy Rules:**
- Display headings use serif font for maximum impact and editorial feel
- All body text, UI elements, and interactive text use sans-serif for clarity
- Headlines carry the personality; body text stays functional
- Category badges are small, rounded pills that classify without dominating
- Numbered sequences (01, 02, 03...) use sans-serif in muted gray, positioned top-left of cards

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 96

**Common Patterns:**
- Page horizontal padding: ~96px (desktop), ~24px (mobile)
- Section vertical spacing: 64-80px between major sections
- Card internal padding: 24-32px
- Card grid gap: 16-20px
- Badge padding: 6px 12px (small pill shape)
- Button padding: 14px 28px
- Hero to content spacing: 48px
- Testimonial/quote card padding: 24px with avatar offset
- Between heading and body text: 16px
- Between body text and CTA link: 24px

## Component Styles

### Buttons
**Primary Button:**
- Background: #E8573D (coral-red)
- Text: #FFFFFF, 15-16px, SemiBold
- Padding: 14px 28px
- Border-radius: 8px (soft rounded)
- Arrow indicator (→) appended to label
- Hover: Slightly darker shade (~#D14A32), subtle shadow
- No visible border

**Secondary/Ghost Button:**
- Background: transparent
- Border: 1.5px solid #1A1A1A
- Text: #1A1A1A, 15-16px, SemiBold
- Padding: 14px 28px
- Border-radius: 8px
- Arrow indicator (→) appended to label
- Hover: Light fill (#F5EDE4 or slight darken)

**Text Link/CTA:**
- Text: #E8573D, 15px, SemiBold
- No background, no border
- Arrow (→) appended
- Hover: underline or slight opacity shift

### Cards
**Content Card (Numbered):**
- Background: #FFFFFF
- Border: 1px solid #EAEAEA
- Border-radius: 12px (generous rounding)
- Padding: 24-28px
- Shadow: none or very subtle (0 1px 3px rgba(0,0,0,0.04))
- Layout: Number (top-left) + Badge (top-right) → Title → Description → CTA link (bottom)
- Number style: 14px, muted gray, "01", "02", etc.
- Hover: very subtle shadow increase or border darken

**Testimonial/Quote Card:**
- Background: #FFFFFF
- Border: 1px solid #EAEAEA
- Border-radius: 12px
- Padding: 24px
- Contains: avatar (48px circle), name (bold, linked), role description
- Author name is a link (underline on hover)

### Badges/Tags
**Primary Badge:**
- Background: #FFF0ED (light coral)
- Text: #E8573D, 12-13px, Medium weight
- Padding: 4px 12px
- Border-radius: 20px (full pill)
- No border

**Secondary Badge:**
- Background: #F0F0F0 (neutral gray)
- Text: #444444
- Same sizing and radius as primary

**Resource Badge (top of page):**
- Background: #FFF0ED
- Text: #E8573D
- Includes dot indicator (●) before text
- Slightly larger padding: 6px 16px
- Border-radius: 20px

### Input Fields (Inferred)
- Background: #FFFFFF
- Border: 1px solid #E8E0D6
- Border-radius: 8px
- Padding: 12px 16px
- Font: 16px sans-serif
- Focus: border color shifts to #E8573D
- Placeholder: #8A8A8A

## Layout Principles

- **Max content width:** ~960-1040px, centered
- **Grid structure:** 3-column card grid on desktop, equal width columns, 16-20px gap
- **Responsive behavior:** 3-col → 2-col → 1-col stack. Hero content stays single column throughout.
- **Alignment:** Left-aligned text throughout. Cards use top-alignment for mixed content lengths.
- **Content hierarchy:** Badge/resource label → Display heading → Subtitle/description → CTA buttons → Supporting content (testimonial) → Section heading → Card grid
- **Visual rhythm:** Large serif headlines create clear section breaks; numbered cards create scannable sequences

## Visual Effects

- **Border Radius:** 8px for buttons and inputs, 12px for cards, 20px (full pill) for badges
- **Shadows:** Minimal to none. Cards rely on border + white background contrast against warm page. Possible very subtle shadow on hover.
- **Borders:** 1px solid, light warm tones (#E8E0D6 page-level, #EAEAEA card-level). Used consistently on cards.
- **Backgrounds:** Warm peach-cream (#F5EDE4) is the dominant page color. White (#FFF) cards float on top. No gradients, no textures.
- **Decorative elements:** Dot indicator (●) on resource badges. Arrow (→) on all interactive text/buttons. Numbered sequence markers on cards.
- **Avatar:** Circular, ~48px, used in testimonial/attribution blocks.

## Design Tone

Confident and editorial with warmth. The bold serif display headings bring a magazine-like authority while the warm peach background and coral accents keep things approachable and inviting. This system is designed for structured educational or resource content — playbooks, skill libraries, step-by-step frameworks. It takes itself seriously enough to feel professional but not so seriously that it becomes cold. The numbered card grid pattern signals clear progression and completeness.

## Usage Notes for AI Implementation

- Pair a bold display serif (DM Serif Display, Playfair Display, or similar) with Inter or a neutral sans-serif. The contrast between the two is essential to the personality.
- The warm background (#F5EDE4) is NOT optional — it defines the system. White is reserved for cards/surfaces floating on top.
- Always include the coral-red (#E8573D) for primary actions and links. It's the energy in an otherwise subdued palette.
- Cards should always include numbered sequences when presenting lists of features, steps, or resources. The numbering reinforces the structured/playbook feel.
- Badges are small and lightweight — they classify content without drawing focus from titles.
- Keep button text concise with arrow indicators (→) for forward momentum.
- This system works best for: landing pages, resource hubs, playbook/guide pages, course outlines, feature grids, and structured content marketing.
- Avoid using this for data-heavy dashboards or minimal developer-facing tools — the warm editorial aesthetic won't suit those contexts.
