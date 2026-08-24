---
id: light-scheduler-001
title: Pearl Scheduler
description: A clean, minimal scheduling interface with stark black-and-white contrast and rounded pill elements
tags: [light, minimal, scheduling, mobile-first, high-contrast]
colors: ["#FFFFFF", "#F5F5F5", "#000000", "#6B6B6B", "#E5E5E5", "#FF3B30"]
created: 2026-01-04
---

# Pearl Scheduler

A pristine, minimal scheduling and booking interface characterized by stark black-and-white contrast, generous whitespace, and rounded pill-shaped elements. The design prioritizes clarity and ease of use through extreme simplicity and high-contrast interactive states.

## Color Palette

**Primary Colors:**
- Pure White: #FFFFFF — Primary background, modal backgrounds, content areas
- Pure Black: #000000 — Primary text, selected states, CTA buttons, active calendar dates

**Neutral Colors:**
- Surface Gray: #F5F5F5 — Page background, subtle surface differentiation
- Secondary Text: #6B6B6B — Subtext, descriptions, metadata, inactive labels
- Separator: #E5E5E5 — Divider lines between list items
- Disabled/Unavailable: #E8E8E8 — Striped pattern background for unavailable dates

**Accent/State Colors:**
- Alert Red: #FF3B30 — Notification badges, warning indicators
- Avatar Background: #D9D9D9 — Default avatar placeholder background

**UI Element Colors:**
- Close Button: #8E8E93 — X icon in dialogs
- Chevron: #C7C7CC — Navigation arrows
- Border Outline: #E5E5E5 — Button outlines, calendar date rings

## Typography

**Font Families:**
- Primary: SF Pro Display / -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif
- The system uses the native platform font for optimal rendering

**Type Scale:**
- Page Title: 28px, weight 700 (bold), line-height 1.2
- Section Header: 22px, weight 600 (semibold), line-height 1.3
- Card Title/Name: 17px, weight 600 (semibold), line-height 1.4
- Body/Description: 15px, weight 400 (regular), line-height 1.5
- Label/Caption: 13px, weight 400 (regular), line-height 1.4
- Small/Meta: 12px, weight 500 (medium), line-height 1.3

**Hierarchy Rules:**
- Page titles use bold weight with generous top padding
- Section labels use uppercase with secondary text color (e.g., "PAST")
- List item titles are semibold black, descriptions are regular gray
- Calendar day abbreviations are small, uppercase, secondary color

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 48, 64

**Common Patterns:**
- Page horizontal padding: 24px (mobile), 32px (tablet+)
- Section vertical spacing: 32px between major sections
- List item vertical padding: 20px
- Component internal padding: 16px
- Modal top padding: 24px
- Calendar grid gap: 8px horizontal, 12px vertical
- Avatar to text gap: 16px

## Component Styles

### Buttons

**Primary CTA (View Order style):**
- Background: #000000
- Text: #FFFFFF, 17px, weight 600
- Padding: 18px 24px
- Border radius: 16px (large pill)
- Full width with price right-aligned
- Shadow: none

**Secondary/Outline Button (Today):**
- Background: transparent
- Border: 1px solid #E5E5E5
- Text: #000000, 15px, weight 500
- Padding: 8px 16px
- Border radius: 20px (full pill)

**Icon Button (Close):**
- Size: 32px × 32px
- Background: #F5F5F5
- Icon color: #8E8E93
- Border radius: 50%

### Cards & List Items

**Appointment Card:**
- Background: transparent (on white surface)
- Bottom border: 1px solid #E5E5E5
- Padding: 20px 0
- Layout: Avatar (56px) + Content with 16px gap
- Avatar: 56px × 56px, border-radius 12px

**Menu List Item:**
- Padding: 20px 0
- Bottom border: 1px solid #E5E5E5
- Text: 17px, weight 400 (or 600 for profile name)
- Chevron: #C7C7CC, right-aligned

### Calendar

**Calendar Grid:**
- 7 columns, equal width
- Day headers: 13px, uppercase, #6B6B6B
- Date cells: 44px × 44px minimum touch target

**Date States:**
- Available: Black circle (#000000) with white text
- Selected/Today: Black circle with white ring outline inside
- Unavailable: Gray (#E8E8E8) with diagonal stripe pattern, gray text
- Past/Empty: No background, gray text (#999999)

**Current Date Indicator:**
- Small dot below the date number
- White color on black background

### Avatars

**Profile Avatar (Large):**
- Size: 80px × 80px
- Border radius: 16px
- Background: #D9D9D9 (with initials)
- Initials: 28px, weight 500, #6B6B6B

**List Avatar (Medium):**
- Size: 56px × 56px
- Border radius: 12px
- Displays photo or initials

**Provider Avatar (Small with badge):**
- Size: 64px × 64px
- Border radius: 12px
- Notification badge: 20px circle, #FF3B30, positioned top-right overlapping

### Input Fields

**Not prominently shown, but inferred:**
- Background: #FFFFFF or #F5F5F5
- Border: 1px solid #E5E5E5
- Border radius: 12px
- Padding: 16px
- Focus state: Border color #000000

### Modals & Sheets

**Bottom Sheet:**
- Background: #FFFFFF
- Border radius: 24px (top corners only)
- Top handle: 36px × 5px, #E5E5E5, centered
- Max height: ~90% viewport
- Shadow: 0 -4px 24px rgba(0,0,0,0.08)

**Slide-over Panel:**
- Width: ~85% viewport on mobile
- Background: #F5F5F5
- Full height
- Content background: #FFFFFF areas where needed

## Layout Principles

- **Max content width:** Full width on mobile, 480px max on larger screens
- **Grid structure:** Single column on mobile, content-driven widths
- **Responsive behavior:** Mobile-first, scales up with larger touch targets
- **Alignment:** Left-aligned text, centered avatars in list context
- **Safe areas:** Respects device safe areas (notch, home indicator)

## Visual Effects

**Border Radius Scale:**
- Small (inputs, small buttons): 8px
- Medium (cards, avatars): 12px
- Large (CTAs, modals): 16px
- Full pill (date circles, tags): 50% or 20px+
- Sheet corners: 24px

**Shadows:**
- Minimal shadow usage
- Bottom sheet: 0 -4px 24px rgba(0,0,0,0.08)
- Elevated elements: 0 2px 8px rgba(0,0,0,0.04)

**Borders:**
- Thickness: 1px consistently
- Style: solid
- Used for: List separators, outline buttons, input fields
- Color: #E5E5E5

**Backgrounds:**
- Solid colors only, no gradients
- Striped pattern for unavailable states (45deg diagonal lines)

## Design Tone

This design system embodies extreme minimalism and clarity. It uses stark black-and-white contrast to create unmistakable hierarchy and actionable states. The generous whitespace and consistent rounded elements create a calm, focused experience that guides users through booking flows without visual noise. The aesthetic feels premium yet accessible, professional yet friendly.

## Usage Notes for AI Implementation

1. **High contrast is key:** Always use pure black (#000000) for primary actions and selected states against white backgrounds. Never use dark gray as a substitute.

2. **Pill shapes define interactivity:** Calendar dates, tags, and CTAs use pill/rounded shapes. Square corners are reserved for containers and cards.

3. **Striped unavailable pattern:** Use CSS diagonal stripes (repeating-linear-gradient) for unavailable/disabled calendar dates, not solid gray.

4. **Avatar flexibility:** Support both image avatars and initial-based fallbacks. Initials use 2 letters, centered, on gray background.

5. **Touch targets:** Maintain minimum 44px touch targets for all interactive elements, especially calendar dates.

6. **Typography restraint:** Only 2-3 font weights (regular, medium, semibold/bold). Avoid light weights.

7. **Color discipline:** The palette is intentionally limited. Red (#FF3B30) is reserved only for alerts/notifications.

8. **Mobile-first patterns:** Bottom sheets for modals, slide-over panels for menus, full-width CTAs pinned to bottom.
