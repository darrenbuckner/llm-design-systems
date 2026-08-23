---
id: campfire-warm-001
title: Campfire Warm System
description: A friendly, warm data visualization system with cream backgrounds, orange accents, and playful rounded elements
tags: [light, warm, friendly, data-visualization, rounded]
colors: ["#F5EDE4", "#F97316", "#C9A07A", "#4B4B4B", "#1A1A1A", "#FFFFFF"]
created: 2024-12-23
---

# Campfire Warm System

A welcoming, approachable design system built for data visualization and survey results. Features a cream/beige foundation with vibrant orange accents, rounded pill shapes, and a friendly, non-intimidating aesthetic. The warmth of the palette evokes campfire gatherings and comfortable conversations around data.

## Color Palette

**Primary Colors:**
- Primary Orange: #F97316 — Primary accent color for highlights, progress bars, and interactive elements
- Warm Tan: #C9A07A — Secondary accent for tags, softer highlights, and filled bars

**Background Colors:**
- Cream Background: #F5EDE4 — Main page background, warm and inviting
- Card White: #FFFFFF — Card surfaces and elevated content areas
- Highlight Peach: #FDECD4 — Highlighted row backgrounds, top-ranked items

**Text Colors:**
- Text Primary: #1A1A1A — Main headings and important text
- Text Secondary: #4B4B4B — Body text and labels
- Text Muted: #8B8B8B — Captions, sample sizes, and tertiary information

**Accent Colors:**
- Tag Orange: #F97316 — Bright orange for primary category pills
- Tag Coral: #F87171 — Red-orange for secondary category pills
- Tag Gold: #D4A855 — Tan/gold for tertiary category pills
- Tag Cream: #E8DDD0 — Muted tan for inactive/other category pills

**UI Element Colors:**
- Border Tan: #D4C4B0 — Subtle borders on cards and dividers
- Navigation Gray: #4B4B4B — Arrow buttons and navigation controls
- Divider Line: #E8DDD0 — Horizontal separators between list items

## Typography

**Font Families:**
- Primary: Inter, system-ui, sans-serif — Clean, modern sans-serif for all text
- Alternative: -apple-system, BlinkMacSystemFont — System font fallbacks

**Type Scale:**
- Display: 48px, 800 (Extra Bold), 1.1 line-height — Main page titles
- Heading 1: 32px, 700 (Bold), 1.2 line-height — Section headers
- Heading 2: 24px, 600 (Semi-bold), 1.3 line-height — Subsection headers
- Body Large: 18px, 500 (Medium), 1.5 line-height — List item labels
- Body: 16px, 400 (Regular), 1.5 line-height — Standard body text
- Caption: 14px, 400 (Regular), 1.4 line-height — Subtitles, descriptions
- Small: 12px, 400 (Regular), 1.4 line-height — Sample sizes, footnotes

**Hierarchy Rules:**
- Headlines use extra-bold weight with tight letter-spacing (-0.02em)
- Percentages displayed in bold (700) at 18-20px for emphasis
- Category labels in medium weight for readability
- Muted text uses lighter gray color rather than reduced size

## Spacing System

**Base Unit:** 8px

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 80

**Common Patterns:**
- Component padding: 16px horizontal, 12px vertical (pills/tags)
- Card padding: 24px all sides
- Section spacing: 48px between major sections
- List item spacing: 16px between items
- Grid gaps: 24px for card grids
- Page margins: 48-64px on desktop, 24px on mobile

**Specific Measurements:**
- Tag/pill padding: 8px 16px
- Progress bar height: 24px
- Number badge size: 32px diameter
- Navigation arrow size: 56px diameter
- Card border radius containers: 16px

## Component Styles

### Buttons / Navigation Arrows
- Background: #4B4B4B (dark gray)
- Shape: Perfect circle, 56px diameter
- Icon: White arrow, 24px
- Hover: Slight scale increase (1.05)
- Shadow: Subtle drop shadow for depth
- Usage: Carousel/pagination navigation

### Category Pills / Tags
- Border radius: 9999px (fully rounded pill)
- Padding: 8px 16px
- Font size: 14px, weight 500
- Variants:
  - Primary: #F97316 background, white text
  - Secondary: #F87171 background, white text  
  - Tertiary: #D4A855 background, white text
  - Muted: #E8DDD0 background, #4B4B4B text
  - Outline: White background, 1px #D4C4B0 border, dark text

### Cards
- Background: #FFFFFF
- Border: 1px solid #D4C4B0
- Border radius: 16px
- Padding: 24px
- Shadow: None (relies on border for definition)
- Highlighted variant: #FDECD4 background for top items

### Progress Bars
- Container: Implicit (no visible track for simple version)
- Fill: #F97316 (bright orange) or #C9A07A (tan)
- Height: 20-24px
- Border radius: 4px (slightly rounded ends)
- Sizing: Proportional to percentage value

### List Items / Rows
- Layout: Horizontal flex with space-between
- Separator: 1px solid #E8DDD0 between items
- Highlighted rows: Full #FDECD4 background, #F97316 border
- Number badges: 32px circle, outline style (#1A1A1A border)
- Icon containers: 24px, inline with text

### Data Visualization Bars
- Solid bars: #F97316 or #C9A07A fill
- Ghost/future bars: Dashed border (#C9A07A), no fill
- Labels: Percentage inside or adjacent
- Delta indicators: +XX.Xpp format for changes

### Icon Containers
- Size: 40px square
- Border radius: 8px
- Background: Varies (dark for emphasis, white for subtle)
- Icon color: Contrasting to background

## Layout Principles

**Max Content Width:** 1200px for main content area

**Grid Structure:**
- Single column for data lists
- Flexible card arrangements for comparison data
- Consistent left alignment for labels
- Right alignment for numerical values

**Responsive Behavior:**
- Cards stack vertically on mobile
- Navigation arrows become smaller or hidden
- Tags wrap naturally
- Minimum padding maintained at 16px

**Alignment:**
- Left-aligned labels and headings
- Right-aligned percentages and values
- Centered navigation controls
- Cards have internal left alignment

## Visual Effects

**Border Radius:**
- Pills/Tags: 9999px (fully rounded)
- Cards: 16px
- Progress bars: 4px
- Navigation circles: 50%
- Small elements: 8px

**Shadows:**
- Generally not used; relies on borders
- Navigation arrows: subtle shadow (0 2px 8px rgba(0,0,0,0.1))

**Borders:**
- Cards: 1px solid #D4C4B0
- Highlighted cards: 2px solid #F97316
- Dividers: 1px solid #E8DDD0
- Dashed borders for "projected" data: 2px dashed #C9A07A

**Backgrounds:**
- Page: Solid #F5EDE4 cream
- Cards: Solid white
- Highlights: Solid #FDECD4 peach
- No gradients in core system

**Decorative Elements:**
- Campfire icon/logo in top right (brand element)
- Circled numbers for rankings
- Simple line icons for categories

## Design Tone

This system exudes warmth and approachability, making data feel accessible rather than intimidating. The cream and orange palette creates a cozy, campfire-like atmosphere that encourages exploration and engagement. The rounded shapes and playful pill components add friendliness without sacrificing clarity or professionalism. It's designed to make survey results and analytics feel like a conversation rather than a report.

## Usage Notes for AI Implementation

**When to use this system:**
- Survey results and poll data
- Rankings and leaderboards
- Comparison charts and preference data
- Dashboards with a friendly, non-corporate feel
- Community-facing analytics

**Key implementation notes:**
- Always use the cream (#F5EDE4) background for page-level surfaces
- Reserve bright orange (#F97316) for primary actions and key data points
- Use tan (#C9A07A) for secondary data and softer emphasis
- Highlight top 3 items with peach background and orange border
- Keep typography weights consistent: bold for headlines, medium for labels
- Maintain generous padding and spacing for the open, airy feel
- Use circular navigation arrows for carousel/pagination patterns
- Category pills should be fully rounded (pill shape)
- Numbers in circles should use outline style, not filled

**Color usage priority:**
1. Cream background as foundation
2. White cards for content containers
3. Orange for primary/active states
4. Tan for secondary/inactive states
5. Peach for highlighting important rows

**Accessibility considerations:**
- Orange on cream provides adequate contrast for UI elements
- Text should remain dark (#1A1A1A) on light backgrounds
- White text only on orange or dark backgrounds
- Ensure 4.5:1 contrast ratio for body text
