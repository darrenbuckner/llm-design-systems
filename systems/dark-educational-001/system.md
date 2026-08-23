---
id: dark-educational-001
title: Carbon Academy
description: A sophisticated dark theme with warm accents for educational platforms and course content
tags: [dark, educational, warm-accent, professional, content-rich]
colors: ["#0D0D0D", "#1A1A1A", "#FFFFFF", "#F5A623", "#6B7280"]
created: 2025-01-16
---

# Carbon Academy

A refined dark educational interface that balances information density with visual clarity. Deep black backgrounds create focus while warm amber accents guide attention to calls-to-action and key information. The system excels at presenting course content, instructor profiles, and structured learning materials.

## Color Palette

**Primary Colors:**
- Primary Background: #0D0D0D — Main page background, creates depth
- Secondary Background: #1A1A1A — Cards, elevated surfaces, content containers
- Accent: #F5A623 — CTAs, highlights, interactive elements, star ratings

**Neutral Colors:**
- Surface Dark: #141414 — Subtle elevation layers
- Surface Medium: #262626 — Input fields, secondary containers
- Text Primary: #FFFFFF — Headlines, primary content
- Text Secondary: #9CA3AF — Body text, descriptions, metadata
- Text Tertiary: #6B7280 — Captions, timestamps, subtle labels
- Borders: #2A2A2A — Dividers, card borders, separators

**Accent/State Colors:**
- Success/Positive: #22C55E — Completion states, verified badges
- Warning: #F5A623 — Also serves as primary accent
- Error: #EF4444 — Error states, alerts
- Info Blue: #3B82F6 — Links, informational elements

**Gradient/Effect Colors:**
- Amber Glow: rgba(245, 166, 35, 0.1) — Subtle accent backgrounds
- Card Hover: #1F1F1F — Interactive card states

## Typography

**Font Families:**
- Primary: Inter, -apple-system, BlinkMacSystemFont, sans-serif
- Monospace: SF Mono, Monaco, monospace (for code/technical content)

**Type Scale:**
- Display: 48px, 700 weight, 1.1 line-height — Hero headlines
- Heading 1: 32px, 700 weight, 1.2 line-height — Section titles
- Heading 2: 24px, 600 weight, 1.3 line-height — Card titles, subsections
- Heading 3: 20px, 600 weight, 1.4 line-height — Component headers
- Heading 4: 16px, 600 weight, 1.4 line-height — List item titles
- Body Large: 18px, 400 weight, 1.6 line-height — Lead paragraphs
- Body: 16px, 400 weight, 1.6 line-height — Standard content
- Body Small: 14px, 400 weight, 1.5 line-height — Secondary content
- Caption: 12px, 500 weight, 1.4 line-height — Labels, metadata

**Hierarchy Rules:**
- Headlines use pure white (#FFFFFF) for maximum contrast
- Body text uses muted gray (#9CA3AF) to reduce eye strain
- Interactive text elements use accent color on hover
- All caps with letter-spacing (0.05em) for small labels and tags

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96

**Common Patterns:**
- Component internal padding: 16px-24px
- Card padding: 24px
- Section spacing: 64px-80px
- Grid gaps: 16px-24px
- Inline element spacing: 8px-12px
- Form field padding: 12px 16px

**Vertical Rhythm:**
- Paragraph spacing: 16px
- List item spacing: 12px
- Section header to content: 24px
- Between major sections: 64px

## Component Styles

### Buttons

**Primary Button:**
- Background: #F5A623
- Text: #0D0D0D
- Padding: 12px 24px
- Border Radius: 8px
- Font: 14px, 600 weight
- Hover: brightness(1.1), slight scale(1.02)
- Transition: all 0.2s ease

**Secondary Button:**
- Background: transparent
- Border: 1px solid #2A2A2A
- Text: #FFFFFF
- Padding: 12px 24px
- Border Radius: 8px
- Hover: background #1A1A1A, border #3A3A3A

**Ghost Button:**
- Background: transparent
- Text: #9CA3AF
- Hover: text #FFFFFF

### Cards

**Standard Card:**
- Background: #1A1A1A
- Border: 1px solid #2A2A2A
- Border Radius: 12px
- Padding: 24px
- Hover: border-color #3A3A3A, subtle lift

**Feature Card:**
- Background: linear-gradient(135deg, #1A1A1A 0%, #141414 100%)
- Border: 1px solid #2A2A2A
- Border Radius: 16px
- Shadow: 0 4px 24px rgba(0, 0, 0, 0.3)

**Profile Card:**
- Circular avatar: 48-64px
- Name: 16px, 600 weight, white
- Role/Title: 14px, 400 weight, gray
- Vertical stack with 8px gap

### Input Fields

**Text Input:**
- Background: #262626
- Border: 1px solid #2A2A2A
- Border Radius: 8px
- Padding: 12px 16px
- Text: #FFFFFF
- Placeholder: #6B7280
- Focus: border-color #F5A623, box-shadow 0 0 0 2px rgba(245, 166, 35, 0.2)

### Navigation

**Header:**
- Background: #0D0D0D with subtle blur
- Height: 64px
- Logo: Left aligned
- Nav items: Center or right
- CTA button: Right aligned

**Nav Links:**
- Text: #9CA3AF
- Hover: #FFFFFF
- Active: #FFFFFF with subtle underline or accent

### Lists & Content Blocks

**Curriculum List:**
- Icon/number left (accent color)
- Title: 16px, 500 weight
- Description: 14px, muted
- Checkmark or status indicator right
- Divider: 1px solid #2A2A2A

**Testimonial Block:**
- Avatar: 48px circular
- Quote text: 16px, italic optional
- Author name: 14px, 600 weight
- Role: 14px, muted

### Badges & Tags

**Tag:**
- Background: #262626
- Text: #9CA3AF
- Padding: 4px 12px
- Border Radius: 4px
- Font: 12px, 500 weight

**Rating:**
- Star icons: #F5A623 filled, #2A2A2A empty
- Size: 16px
- Gap: 2px

## Layout Principles

- Max content width: 1200px (centered)
- Content area: 720px for long-form text
- Grid: 12-column base
- Responsive breakpoints: 640px, 768px, 1024px, 1280px
- Mobile-first approach
- Generous whitespace to reduce cognitive load

**Common Layouts:**
- Hero: Full-width, centered content, 80-120px vertical padding
- Two-column: 60/40 or 50/50 split on desktop, stacked on mobile
- Card grid: 3 columns desktop, 2 tablet, 1 mobile
- Sidebar layout: 280px fixed sidebar, fluid content

## Visual Effects

**Border Radius:**
- Small (buttons, inputs, tags): 8px
- Medium (cards): 12px
- Large (feature sections): 16px
- Circular (avatars): 50%

**Shadows:**
- Subtle: 0 2px 8px rgba(0, 0, 0, 0.2)
- Medium: 0 4px 16px rgba(0, 0, 0, 0.3)
- Large: 0 8px 32px rgba(0, 0, 0, 0.4)
- Accent glow: 0 0 24px rgba(245, 166, 35, 0.15)

**Borders:**
- Default: 1px solid #2A2A2A
- Hover/Focus: 1px solid #3A3A3A or accent
- Dividers: 1px solid #1A1A1A

**Backgrounds:**
- Primary: Solid #0D0D0D
- Cards: Solid #1A1A1A
- Subtle gradients for depth
- No patterns or textures

## Design Tone

This system projects intellectual authority and premium quality while remaining approachable for learning contexts. The dark palette reduces eye strain during extended study sessions, while warm amber accents create visual warmth and guide users through educational journeys. The overall aesthetic suggests expertise, trustworthiness, and modern professionalism — ideal for courses, workshops, and knowledge-sharing platforms.

## Usage Notes for AI Implementation

When implementing this system:

1. **Contrast is critical** — Ensure text maintains WCAG AA compliance against dark backgrounds. White (#FFFFFF) on #0D0D0D and #9CA3AF on #1A1A1A both pass.

2. **Use accent sparingly** — The amber accent (#F5A623) should highlight only primary CTAs and key interactive elements. Overuse diminishes its impact.

3. **Layer backgrounds thoughtfully** — Use #0D0D0D for page, #1A1A1A for cards, #262626 for inputs/nested elements to create visual hierarchy.

4. **Typography hierarchy** — Reserve white text for headlines and primary content. Use gray (#9CA3AF) for body text to reduce visual intensity.

5. **Interactive states** — All interactive elements need clear hover/focus states. Brightness increases and subtle border changes work well.

6. **Mobile considerations** — Increase touch targets to 44px minimum. Ensure adequate padding on mobile (16-24px container padding).

7. **Content density** — This system supports information-rich layouts. Use spacing and subtle dividers to organize content without feeling cluttered.
