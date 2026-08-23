---
id: light-friendly-learning-001
title: Clover Classroom
description: A warm, approachable learning interface with soft edges, playful illustrations, and comprehensive course components
tags: [light, friendly, warm, minimal, educational, courses]
colors: ["#FFFFFF", "#F5F0E8", "#FFEFD5", "#1A1A1A", "#6B7280", "#22C55E", "#E5E7EB"]
created: 2025-01-15
---

# Clover Classroom

A warm and inviting design system built for learning experiences. Features a cream-toned palette, friendly rounded elements, and a balance of playful illustration with clean typography. The aesthetic feels approachable and encouraging—like a patient tutor rather than a cold institution. Includes comprehensive components for course content, quizzes, tables, and navigation.

## Color Palette

**Primary Colors:**
- Primary Black: #1A1A1A — Main text, primary buttons, key UI elements
- Primary White: #FFFFFF — Card backgrounds, input fields, clean surfaces, content areas

**Background Colors:**
- Warm Gray: #F5F0E8 — Page background, creates warmth without being distracting
- Cream Accent: #FFEFD5 — Soft highlight for secondary buttons, warm accents
- Light Gray: #F9FAFB — Subtle alternating row backgrounds, hover states

**Neutral Colors:**
- Text Primary: #1A1A1A — Headlines, important text, body copy
- Text Secondary: #6B7280 — Placeholder text, supporting content, muted labels
- Text Tertiary: #9CA3AF — Very light text, disabled states, metadata
- Border Light: #E5E7EB — Subtle borders, dividers, table lines
- Border Medium: #D1D5DB — More prominent borders, input outlines
- Border Dashed: #D1D5DB — Dashed separators between content sections

**Accent Colors:**
- Success/Brand Green: #22C55E — Accent icons, positive actions, correct answers
- Sage Green: #86EFAC — Soft green for secondary accents, hover states
- Muted Olive: #6B8068 — Tertiary buttons, promotional elements

**State Colors:**
- Hover Black: #2D2D2D — Button hover states
- Focus Ring: rgba(26, 26, 26, 0.2) — Focus indicators
- Selected/Active: #F5F0E8 — Active menu items, selected states
- Error: #EF4444 — Error states, incorrect answers
- Warning: #F59E0B — Warning indicators

## Typography

**Font Families:**
- Primary: System UI / SF Pro / -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto — Clean, readable system fonts
- Alternative: Inter or similar geometric sans-serif

**Type Scale:**
- Display: 32px, 700 weight, 1.2 line-height — Hero headlines, course titles
- Heading 1: 28px, 700 weight, 1.25 line-height — Page titles, major sections
- Heading 2: 24px, 600 weight, 1.3 line-height — Section headers within content (e.g., "Who Is Listening?")
- Heading 3: 18px, 600 weight, 1.4 line-height — Subsection headers, card titles
- Heading 4: 16px, 600 weight, 1.4 line-height — Small headers, table headers
- Body Large: 18px, 400 weight, 1.6 line-height — Primary reading content, course material
- Body: 16px, 400 weight, 1.5 line-height — Standard content
- Body Small: 14px, 400 weight, 1.5 line-height — Secondary content, descriptions, navigation items
- Caption: 12px, 400 weight, 1.4 line-height — Timestamps, metadata, labels

**Hierarchy Rules:**
- Headlines use bold weight (700) for clear visual hierarchy
- Section headers within content use semibold (600)
- Body text maintains comfortable reading weight (400)
- Secondary text uses muted gray (#6B7280) rather than lighter weight
- Generous line-height (1.6) for long-form reading content

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80

**Common Patterns:**
- Component internal padding: 16-20px
- Card padding: 16-24px
- Content card padding: 20-32px
- Section spacing: 32-48px
- Paragraph spacing: 24px between paragraphs
- List item spacing: 12-16px between items
- Table cell padding: 12-16px vertical, 16px horizontal
- Input field padding: 16px horizontal, 14px vertical
- Button padding: 12px horizontal, 10px vertical (small), 16px horizontal, 12px vertical (medium)
- Grid gaps: 12-16px between cards
- Page margins: 16-24px on mobile

## Component Styles

### Buttons

**Primary Button (Dark):**
- Background: #1A1A1A
- Text: #FFFFFF
- Border-radius: 50px (pill shape)
- Padding: 14px 24px
- Font-size: 15px, weight 500
- Hover: #2D2D2D
- Used for primary actions like "Advance"

**Secondary Button (Cream/Outlined):**
- Background: #FFEFD5 or transparent
- Text: #1A1A1A
- Border: 1px solid #D1D5DB (when outlined)
- Border-radius: 50px (pill shape)
- Padding: 10px 20px
- Font-size: 14px, weight 500

**Tertiary Button (Muted):**
- Background: #6B8068 (muted olive)
- Text: #FFFFFF
- Border-radius: 50px
- Padding: 12px 16px
- Used for promotional/secondary CTAs

**Icon Button:**
- Size: 40-44px
- Border-radius: 50% (circle) or 8px (rounded square)
- Background: varies (black for primary, transparent for secondary)
- Border: 1px solid #E5E7EB (when outlined)

**Close Button:**
- Size: 32px
- Border-radius: 8px
- Border: 1px solid #E5E7EB
- Background: transparent
- Icon: × centered
- Hover: background #F5F0E8

### Cards

**Content Card (Course Overview):**
- Background: #FFFFFF
- Border: 1px solid #E5E7EB
- Border-radius: 16px
- Padding: 20-24px
- Shadow: none or very subtle
- Contains hero image, title, chapter list

**Hero Image in Card:**
- Width: 100%
- Border-radius: 12px
- Aspect ratio: ~16:9 or similar
- Object-fit: cover

**Thumbnail in Card:**
- Size: 48-56px square
- Border-radius: 8px
- Object-fit: cover

**Modal/Overlay Card:**
- Background: #FFFFFF
- Border-radius: 16px (top corners when sheet-style)
- Padding: 24px
- Shadow: 0 -4px 20px rgba(0,0,0,0.1) for bottom sheets
- Close button in top-right corner

### Navigation

**Header Nav:**
- Height: ~56px
- Background: transparent (inherits page background)
- Logo: left aligned, ~32px icon in circular container
- Breadcrumb/title: center-left with dropdown chevron
- Auth buttons: right aligned
- Spacing: 8-12px between buttons

**Logo Container:**
- Size: 40px
- Border-radius: 8px
- Border: 1px solid #E5E7EB
- Contains brand icon centered

**Breadcrumb/Course Selector:**
- Font-size: 14px
- Color: #1A1A1A
- Truncated with ellipsis if too long
- Dropdown chevron (▼) follows text
- Separated from logo by vertical line (1px #E5E7EB)

**Chapter/Section Navigation (Sidebar/Modal):**
- List style with no bullets
- Font-size: 15px
- Color: #1A1A1A
- Padding: 12px 16px per item
- Active item: background #F5F0E8
- Hover: background #F9FAFB
- Dashed separator line before special sections (e.g., "Final Exam")

**Section Footer Navigation:**
- Border-top: 1px solid #E5E7EB
- Padding: 24px
- "Next Section:" label in regular weight
- Section name in bold weight
- "Advance" button aligned right

### Tables

**Data Table:**
- Background: #FFFFFF (or transparent on white)
- Border: none (borderless style)
- Header row: font-weight 600, color #1A1A1A
- Body rows: font-weight 400, color #1A1A1A
- Cell padding: 12-16px vertical
- No visible row borders (clean, minimal)
- Columns auto-width based on content
- Right-aligned numbers when applicable
- Scrollable container with subtle scrollbar on right edge

**Table Header:**
- Font-size: 14px
- Font-weight: 600
- Color: #1A1A1A
- Text-transform: none (sentence case)
- Border-bottom: none visible

**Table Cell:**
- Font-size: 15px
- Font-weight: 400
- Line-height: 1.5
- Vertical alignment: top or middle

### Quiz/Assessment Components

**Multiple Choice Question:**
- Question text: 18px, weight 400, color #1A1A1A
- Line-height: 1.6 for readability
- Margin-bottom: 24px after question

**Answer Option:**
- Layout: letter badge + answer text
- Padding: 16px vertical
- Border-bottom: 1px solid #E5E7EB (except last item)
- Hover: background #F9FAFB
- Selected: background #F5F0E8, border-left accent possible

**Letter Badge:**
- Size: 32px × 32px
- Border-radius: 8px
- Border: 1px solid #E5E7EB
- Background: #FFFFFF
- Font-size: 14px
- Font-weight: 500
- Color: #1A1A1A
- Text-align: center
- Letters: A, B, C, D...

**Selected State:**
- Badge background: #1A1A1A
- Badge text: #FFFFFF
- Row background: #F5F0E8

### Input Fields

**Search/Text Input:**
- Background: #FFFFFF
- Border: 1px solid #E5E7EB
- Border-radius: 50px (pill shape)
- Padding: 14px 16px
- Font-size: 16px
- Placeholder color: #9CA3AF
- Focus border: #1A1A1A or #6B7280

**Input with Actions:**
- Right side contains icon buttons
- Icons: brand icon, plus (+), submit arrow
- Icon spacing: 8-12px between icons
- Submit button embedded at right edge

### Content Layout

**Course Content Page:**
- Max-width: ~680px for readable line lengths
- Background: #FFFFFF
- Padding: 24-32px horizontal
- Generous vertical spacing between sections

**Long-form Text:**
- Font-size: 18px
- Line-height: 1.6-1.7
- Paragraph spacing: 24px
- Color: #1A1A1A

**Section Header (within content):**
- Font-size: 24px
- Font-weight: 600
- Margin-top: 40px
- Margin-bottom: 20px

### Labels/Tags

**Category Label:**
- Font-size: 14px
- Color: #6B7280
- Icon: small chart/trend icon (16px)
- Icon + text layout with 8px gap

## Layout Principles

- Max content width: ~680px for reading content, ~600px for cards/forms
- Centered layout for hero/onboarding flows
- Left-aligned for course content reading
- Card grids stack vertically on mobile
- Generous whitespace around focal elements
- Illustrations centered above headlines
- Input fields span nearly full width with padding
- Tables full-width within content container
- Footer navigation spans full width with border-top separator

## Visual Effects

**Border Radius:**
- Buttons: 50px (full pill)
- Cards: 16px
- Modal/sheets: 16px (top corners)
- Thumbnails/images: 12px
- Letter badges: 8px
- Icon containers: 8px or 50% (circle)
- Close buttons: 8px

**Shadows:**
- Minimal shadow usage
- Cards rely on borders rather than shadows
- Modal/sheets: 0 -4px 20px rgba(0,0,0,0.1)
- Optional subtle shadow: 0 1px 3px rgba(0,0,0,0.05)

**Borders:**
- Primary border color: #E5E7EB
- Border width: 1px consistently
- Dashed borders: 1px dashed #D1D5DB for section separators
- Used on cards, inputs, icon containers
- Creates definition without heaviness

**Backgrounds:**
- Page: warm gray #F5F0E8
- Cards/content: clean white #FFFFFF
- Selected states: #F5F0E8
- Hover states: #F9FAFB
- No gradients in main UI
- Illustrations add visual interest with colorful, stylized artwork

**Illustrations:**
- Colorful, stylized artwork (not black line art)
- Bold geometric shapes and colors
- Orange, teal, gray color schemes common
- Represents course subject matter
- Full-width within card containers
- ~200-300px height

## Design Tone

Friendly and approachable, like a welcoming classroom environment. The warm cream background creates comfort while the clean white cards maintain clarity. Playful illustrations add personality without being childish—suitable for adult learners. The overall feeling is encouraging: "learning should be enjoyable, not intimidating."

The interface balances visual warmth with functional clarity. Course content prioritizes readability with generous line-heights and comfortable font sizes. Quiz components use clear visual hierarchy with letter badges that feel tactile and interactive. Tables present data cleanly without visual clutter.

## Usage Notes for AI Implementation

1. **Maintain warmth**: Always use the warm gray (#F5F0E8) for page backgrounds, never pure gray or white pages
2. **Pill shapes are signature**: Buttons and inputs should use full border-radius (50px) for the characteristic friendly feel
3. **Illustration placement**: When adding visual interest, center illustrations above primary content or as hero images in cards
4. **Restrained color**: Primary actions use black, not colored buttons—color appears only in accents and illustrations
5. **Card structure**: Content cards follow thumbnail-left, text-right pattern with minimal styling
6. **Typography simplicity**: Stick to system fonts, let content hierarchy come from weight and size, not font variety
7. **Subtle borders**: Prefer light borders (#E5E7EB) over shadows for element definition
8. **Touch-friendly**: All interactive elements should be at least 44px for comfortable tapping
9. **Reading experience**: For long-form content, use 18px font size with 1.6+ line-height
10. **Quiz design**: Letter badges (A, B, C, D) should be square with rounded corners, not circles
11. **Table minimalism**: Use borderless tables with clean typography, no visible grid lines
12. **Section navigation**: Use dashed separators to distinguish special sections like exams from regular content
13. **Footer navigation**: Always include section progression with "Next Section:" pattern and right-aligned action button
