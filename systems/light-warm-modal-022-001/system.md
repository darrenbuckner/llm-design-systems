---
id: light-warm-modal-022
title: Sandstone Assistant System
description: Warm, approachable modal interface with split-panel layout combining marketing content and product preview
tags: [light, warm, modal, split-layout, professional, approachable]
colors: ["#D4C8B8", "#FFFFFF", "#1A1A1A", "#2563EB", "#DA7756", "#F5F5F5"]
created: 2025-06-29
---

# Sandstone Assistant System

A warm, inviting interface design featuring a distinctive warm beige/taupe background with a clean split-panel modal layout. The left panel presents marketing messaging while the right showcases a product preview with layered UI cards. The overall aesthetic is professional yet approachable, using rounded corners and careful typography hierarchy to create trust and encourage action.

## Color Palette

**Primary Colors:**
- Primary Blue: #2563EB — Primary actions, links, share buttons
- Accent Orange/Coral: #DA7756 — Highlight badges, submit buttons, accent elements

**Neutral Colors:**
- Warm Beige Background: #D4C8B8 — Main modal background, creates warmth
- Pure White: #FFFFFF — Cards, panels, input backgrounds, button fills
- Near Black: #1A1A1A — Primary headings, strong emphasis text
- Dark Gray: #4A4A4A — Body text, secondary content
- Medium Gray: #6B6B6B — Tertiary text, timestamps, metadata
- Light Gray: #E5E5E5 — Borders, dividers, subtle separators
- Off-White: #F5F5F5 — Nested card backgrounds, subtle layering

**State Colors:**
- Focus Ring: #2563EB (with opacity) — Input focus states
- Hover State: Slight darkening of base color
- Comment Highlight: #FEF3C7 — Yellow highlight for annotations

## Typography

**Font Families:**
- Primary: System UI / -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
- Headings appear to use a slightly heavier weight of the system font

**Type Scale:**
- Display/Hero: 42px, 600 weight, 1.15 line-height — Modal main headline
- Heading 2: 18px, 600 weight, 1.3 line-height — Section headers like "Summary"
- Heading 3: 15px, 600 weight, 1.4 line-height — Sub-section headers
- Body: 15px, 400 weight, 1.5 line-height — Main content text
- Body Small: 14px, 400 weight, 1.5 line-height — Secondary descriptions
- Caption: 12px, 400 weight, 1.4 line-height — Timestamps, metadata
- Badge: 13px, 600 weight, 1.0 line-height — Tag labels

**Hierarchy Rules:**
- Headlines use near-black (#1A1A1A) for maximum contrast
- Body text uses dark gray (#4A4A4A) for comfortable reading
- Metadata/timestamps use medium gray (#6B6B6B)
- Links and interactive elements use primary blue (#2563EB)

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

**Common Patterns:**
- Modal padding: 48px on desktop, 24px on mobile
- Section spacing: 32px between major sections
- Card internal padding: 20px - 24px
- List item spacing: 8px between items
- Button padding: 16px vertical, 24px horizontal (large), 12px/16px (medium)
- Comment bubble padding: 12px 16px
- Badge padding: 6px 12px

## Component Styles

### Buttons

**Primary Button (Outlined):**
- Background: #FFFFFF
- Border: 2px solid #1A1A1A
- Border Radius: 12px
- Padding: 16px 24px
- Font: 16px, 500 weight
- Hover: Background shifts to light gray (#F5F5F5)

**Secondary Button (Ghost):**
- Background: transparent
- Border: 2px solid #1A1A1A
- Border Radius: 12px
- Padding: 16px 24px
- Font: 16px, 500 weight

**Accent Button (Submit):**
- Background: #DA7756
- Border: none
- Border Radius: 50% (circular)
- Size: 32px × 32px
- Icon: White arrow or send icon

**Share Button:**
- Background: #2563EB
- Border Radius: 6px
- Padding: 8px 16px
- Font: 14px, 500 weight, white text
- Icon: Upload/share icon prefix

### Cards

**Preview Card (Right Panel):**
- Background: #FFFFFF
- Border Radius: 16px
- Box Shadow: 0 8px 32px rgba(0, 0, 0, 0.12)
- Padding: 0 (content handles internal padding)

**Nested Panel Card:**
- Background: #FFFFFF
- Border Radius: 12px
- Border: 1px solid #E5E5E5
- Box Shadow: 0 2px 8px rgba(0, 0, 0, 0.06)

**Comment Bubble:**
- Background: #F5F5F5
- Border Radius: 12px
- Padding: 12px 16px
- No border

### Input Fields

**Chat Input:**
- Background: #FFFFFF
- Border: 1px solid #E5E5E5
- Border Radius: 12px
- Padding: 12px 16px
- Placeholder: #9CA3AF

### Badges/Tags

**New Badge:**
- Background: #2563EB
- Border Radius: 6px
- Padding: 6px 12px
- Font: 13px, 600 weight, white text
- Text Transform: uppercase

### Comment Thread

**Comment Item:**
- Avatar: 32px circle with image or initials
- Name: 14px, 600 weight, #1A1A1A
- Timestamp: 12px, 400 weight, #6B6B6B
- Message: 14px, 400 weight, #4A4A4A
- Background: #F5F5F5
- Border Radius: 12px

### Navigation/Toolbar

**Icon Button:**
- Size: 32px × 32px
- Border Radius: 6px
- Background: transparent
- Hover: #F5F5F5
- Icon color: #4A4A4A

## Layout Principles

**Modal Layout:**
- Split panel design: ~55% left (content), ~45% right (preview)
- Max modal width: ~1100px
- Border Radius: 24px for main modal container
- Centered horizontally and vertically in viewport

**Grid Structure:**
- Flexible columns with gap of 24-32px
- Content left-aligned within columns
- Preview panel has layered card composition

**Alignment:**
- Left-aligned text for marketing copy
- Centered action buttons below copy
- Right panel showcases product at slight offset

## Visual Effects

**Border Radius:**
- Modal container: 24px
- Cards: 12-16px
- Buttons: 12px
- Badges: 6px
- Input fields: 12px
- Avatars: 50% (circular)
- Comment bubbles: 12px

**Shadows:**
- Modal: 0 24px 64px rgba(0, 0, 0, 0.2)
- Preview card: 0 8px 32px rgba(0, 0, 0, 0.12)
- Nested cards: 0 2px 8px rgba(0, 0, 0, 0.06)
- Floating toolbar: 0 4px 16px rgba(0, 0, 0, 0.1)

**Borders:**
- Cards: 1px solid #E5E5E5
- Inputs: 1px solid #E5E5E5
- Buttons: 2px solid #1A1A1A

**Backgrounds:**
- Warm beige (#D4C8B8) creates distinctive warmth
- White surfaces for content areas
- Off-white (#F5F5F5) for nested/recessed elements
- Dark overlay behind modal (~40% black opacity)

**Special Effects:**
- Close button (×): Large, positioned top-right of viewport
- Layered card composition creates depth
- Annotation highlight using warm yellow (#FEF3C7)

## Design Tone

This design system conveys approachability and trust through its warm beige backdrop, which softens what could otherwise feel like a typical tech modal. The split-panel layout efficiently combines marketing messaging with product demonstration, allowing users to understand value and see it in action simultaneously. The rounded corners throughout, combined with comfortable spacing and clear typography hierarchy, create a friendly yet professional impression suitable for productivity and collaboration tools.

## Usage Notes for AI Implementation

- Use the warm beige background (#D4C8B8) as a distinctive feature for modals and onboarding flows
- Maintain the split-panel layout for feature announcements or product tours
- Apply generous border radius (12-24px) consistently across all interactive elements
- Use the primary blue (#2563EB) sparingly for key actions and links
- Reserve the coral/orange accent (#DA7756) for primary CTAs and important highlights
- Layer cards with subtle shadows to create depth without overwhelming
- Keep comment/chat interfaces using the light gray (#F5F5F5) bubble style
- Typography should favor the system font stack for fast loading and native feel
- Ensure adequate contrast: near-black text on light backgrounds
