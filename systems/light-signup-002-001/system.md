---
id: light-signup-002
title: Sequoia Progress Form
description: Clean, professional multi-step form system with green progress indicators and warm orange CTAs
tags: [light, minimal, form, enterprise, professional]
colors: ["#FFFFFF", "#00875A", "#F35B04", "#333333", "#6B6B6B", "#E5E5E5"]
created: 2026-01-04
---

# Sequoia Progress Form

A clean, professional design system optimized for multi-step data collection flows. Features a pure white canvas with strategic use of forest green for progress indication and warm orange for primary actions. The system emphasizes clarity and trust through generous whitespace and clear visual hierarchy.

## Color Palette

**Primary Colors:**
- Primary Action: #F35B04 — Warm orange for CTAs and primary buttons
- Progress/Success: #00875A — Forest green for completed steps, validation, and progress indicators

**Neutral Colors:**
- Surface/Background: #FFFFFF — Pure white modal/card background
- Page Background: #F5F5F0 — Warm off-white/cream for underlying page
- Text Primary: #333333 — Near-black for headings and important text
- Text Secondary: #6B6B6B — Medium gray for supporting text and labels
- Text Tertiary: #999999 — Light gray for placeholder text

**Border & Divider Colors:**
- Border Default: #E5E5E5 — Light gray for input borders
- Border Focus: #CCCCCC — Slightly darker on focus
- Divider: #E0E0E0 — Subtle separators

**State Colors:**
- Success: #00875A — Green checkmark for valid inputs
- Error: #D32F2F — Red for validation errors (inferred)
- Inactive: #E5E5E5 — Gray circles for incomplete steps

## Typography

**Font Families:**
- Primary: System UI / -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif
- The typography appears to use the system font stack for optimal performance and native feel

**Type Scale:**
- Display/Hero: 32px, 700 (bold), 1.2 line-height — Main headline
- Heading 2: 24px, 600 (semibold), 1.3 line-height
- Heading 3: 18px, 600 (semibold), 1.4 line-height
- Body: 16px, 400 (regular), 1.5 line-height
- Label: 14px, 600 (semibold), 1.4 line-height — Form labels
- Caption: 14px, 400 (regular), 1.5 line-height — Supporting text
- Small: 12px, 400 (regular), 1.4 line-height

**Hierarchy Rules:**
- Headlines are bold and near-black (#333333) for maximum contrast
- Supporting text uses medium gray (#6B6B6B) to create clear hierarchy
- Form labels are semibold to distinguish from input values
- Centered alignment for hero text, left-aligned for form elements

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 80

**Common Patterns:**
- Modal padding: 24px horizontal, 32px vertical on mobile
- Section spacing: 32-48px between major sections
- Form field spacing: 24px between fields
- Label to input spacing: 8px
- Progress indicator spacing: 16px between steps
- Button padding: 16px 32px

## Component Styles

### Progress Stepper

**Structure:**
- Horizontal layout with numbered circles connected by lines
- Circle size: 32px diameter
- Connector lines: 40-60px width, 2px height

**States:**
- Completed: #00875A fill, white checkmark icon
- Current: #00875A fill, white number text
- Upcoming: #FFFFFF fill, #E5E5E5 border (1px), #6B6B6B number text

**Connector Lines:**
- Completed: #00875A solid
- Upcoming: #E5E5E5 solid

### Buttons

**Primary Button:**
- Background: #F35B04
- Text: #FFFFFF, 16px, 600 weight
- Padding: 14px 32px
- Border radius: 4px
- Hover: Darken to ~#E04D00
- Active: Darken further to ~#CC4400

**Secondary Button (inferred):**
- Background: transparent
- Border: 1px solid #E5E5E5
- Text: #333333
- Padding: 14px 32px
- Border radius: 4px

### Input Fields

**Default State:**
- Background: #FFFFFF
- Border: 1px solid #E5E5E5
- Border radius: 4px
- Padding: 14px 16px
- Font size: 16px
- Text color: #333333

**Focus State:**
- Border: 1px solid #CCCCCC
- Subtle shadow: 0 0 0 2px rgba(0, 135, 90, 0.1)

**Valid State:**
- Border: 1px solid #00875A
- Green checkmark icon on right side
- Checkmark color: #00875A

**Error State (inferred):**
- Border: 1px solid #D32F2F
- Error message below in #D32F2F

### Cards/Modals

**Modal Container:**
- Background: #FFFFFF
- Border radius: 12px (top corners visible)
- Shadow: 0 4px 24px rgba(0, 0, 0, 0.12)
- Max-width: 100% on mobile, ~480px on desktop

### Close Button

- Position: Top right
- Icon: X mark
- Size: 24px
- Color: #333333
- Hover: #000000

## Layout Principles

- **Max content width:** ~400px for form content within modal
- **Modal positioning:** Bottom sheet style on mobile, centered on desktop
- **Grid structure:** Single column form layout
- **Alignment:** Center-aligned headlines, left-aligned form elements
- **Content flow:** Vertical stacking with consistent spacing

## Visual Effects

**Border Radius:**
- Large containers (modals): 12px
- Buttons: 4px
- Input fields: 4px
- Progress circles: 50% (fully rounded)

**Shadows:**
- Modal: 0 4px 24px rgba(0, 0, 0, 0.12)
- No shadows on form elements (flat design)

**Borders:**
- Input borders: 1px solid
- Progress step borders: 1px solid (inactive only)
- Subtle, not prominent

**Backgrounds:**
- Pure white (#FFFFFF) for interactive surfaces
- Warm off-white (#F5F5F0) for page background
- Solid colors throughout, no gradients

## Design Tone

This system communicates professionalism, clarity, and trustworthiness through its restrained color palette and generous whitespace. The combination of forest green (success/progress) and warm orange (action) creates an approachable yet business-appropriate aesthetic. The design feels modern and efficient without being cold—ideal for forms where user trust and completion rates matter.

## Usage Notes for AI Implementation

When implementing this design system:

1. **Progress indication is key:** Always show users where they are in multi-step flows with clear completed/current/upcoming states
2. **Validate inline:** Use the green checkmark pattern for real-time validation feedback
3. **Generous spacing:** Don't compress the whitespace—it creates the professional, trustworthy feel
4. **Action alignment:** Primary CTAs align to the right on desktop, full-width on mobile
5. **Typography hierarchy:** Keep headlines bold and centered, form elements left-aligned
6. **Color restraint:** Use the orange accent only for primary actions, green only for success/progress states
7. **Mobile-first:** The bottom-sheet modal pattern works well for mobile forms
