---
id: light-clinical-form-001
title: Sage Clinic System
description: A clean, accessible healthcare form interface with warm neutrals and teal accents
tags: [light, minimal, healthcare, forms, accessible]
colors: ["#2A9D8F", "#E76F51", "#FFFFFF", "#F8F7F5", "#1A1A1A", "#6B7280"]
created: 2025-01-08
---

# Sage Clinic System

A warm, approachable design system built for healthcare and clinical applications. Features a soft off-white background, clear typography hierarchy, and calming teal accent colors. The interface prioritizes accessibility and ease of use for form-heavy workflows.

## Color Palette

**Primary Colors:**
- Primary Teal: #2A9D8F — Progress bars, active states, primary actions
- Accent Coral: #E76F51 — Decorative elements, illustrations, secondary highlights

**Neutral Colors:**
- Background: #F8F7F5 — Page background, soft warm white
- Surface White: #FFFFFF — Cards, form containers, elevated surfaces
- Text Primary: #1A1A1A — Headings, primary content
- Text Secondary: #6B7280 — Subheadings, helper text, labels
- Border Light: #E5E5E5 — Card borders, dividers, input borders
- Border Focus: #D1D5DB — Input focus states, hover borders

**State Colors:**
- Success: #10B981 — Completed states, positive feedback
- Warning: #F59E0B — Caution states, attention needed
- Error: #EF4444 — Validation errors, required fields
- Info: #3B82F6 — Informational messages

## Typography

**Font Families:**
- Primary: System UI / -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif
- The interface uses clean system fonts optimized for readability

**Type Scale:**
- Page Title: 14px, 700 weight, uppercase, letter-spacing 0.05em — "PATIENT FORM"
- Section Heading: 28px, 700 weight, 1.2 line-height — "Additional Forms"
- Subsection Heading: 24px, 700 weight, 1.3 line-height — "Pre-Appointment Questionnaire"
- Body/Question: 16px, 600 weight, 1.5 line-height — Question text
- Option Label: 16px, 400 weight, 1.5 line-height — Radio button labels
- Helper Text: 14px, 400 weight, 1.5 line-height — Step indicators, descriptions
- Caption: 12px, 400 weight, 1.4 line-height — Fine print, timestamps

**Hierarchy Rules:**
- Uppercase small caps used for category labels (PATIENT FORM)
- Bold weights (600-700) distinguish questions from answers
- Generous line-height (1.5) for comfortable reading
- Dark text (#1A1A1A) on light backgrounds for maximum contrast

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64

**Common Patterns:**
- Page padding: 24px horizontal on mobile
- Card padding: 24px all sides
- Section spacing: 32px between major sections
- Question spacing: 24px between questions
- Option spacing: 12px between radio options
- Inner option padding: 16px vertical, 20px horizontal
- Progress bar height: 4px

## Component Styles

### Progress Indicator
- Container: Full width, 4px height, #E5E5E5 background
- Fill: #2A9D8F, rounded ends
- Step text: 14px, #6B7280, positioned below

### Section Cards
- Background: #FFFFFF
- Border: 1px solid #E5E5E5
- Border-left accent: 4px solid #E5E5E5 (subtle section indicator)
- Border-radius: 8px
- Padding: 24px
- Shadow: none (flat design)

### Radio Button Options
- Container: Full width, white background
- Border: 1px solid #E5E5E5
- Border-radius: 8px
- Padding: 16px 20px
- Gap between options: 12px

**Radio Button States:**
- Default: 24px diameter, 2px #D1D5DB border, white fill
- Hover: Border color darkens to #9CA3AF
- Selected: #2A9D8F border, #2A9D8F inner dot (12px)
- Focus: 2px #2A9D8F outline with 2px offset

### Form Questions
- Question number: Bold, inline with question text
- Question text: 16px, 600 weight, #1A1A1A
- Margin-bottom: 16px before options

### Illustration Style
- Simplified, flat illustrations
- Limited palette: Coral (#E76F51), teal (#2A9D8F), warm gray
- Geometric shapes with rounded corners
- Used sparingly for visual interest in headers

## Layout Principles

- Max content width: 600px for forms (optimized for reading)
- Single column layout for sequential form completion
- Left-aligned content throughout
- Generous whitespace between sections
- Mobile-first responsive approach

## Visual Effects

- **Border Radius:** 8px for cards and inputs, 50% for radio buttons
- **Shadows:** None — flat, card-based design
- **Borders:** 1px solid, light gray (#E5E5E5), used consistently
- **Backgrounds:** Subtle warm off-white (#F8F7F5) page background
- **Transitions:** 150ms ease for hover/focus states

## Design Tone

This system conveys trust, accessibility, and calm professionalism. The warm neutral palette avoids clinical coldness while maintaining a clean, organized appearance. Large touch targets and clear visual hierarchy make forms easy to complete on any device. The teal accent adds a modern, approachable feel without being distracting.

## Usage Notes for AI Implementation

When implementing this system:

1. **Prioritize accessibility** — Maintain high contrast ratios, large touch targets (min 44px), and clear focus states
2. **Use the warm off-white** (#F8F7F5) as page background, pure white (#FFFFFF) for cards and inputs
3. **Keep interactions simple** — Single-column forms, one question visible context at a time
4. **Progress indicators** should always show current step and total steps
5. **Radio options** should be full-width clickable areas, not just the radio button
6. **Section dividers** use subtle left borders or horizontal rules
7. **Typography hierarchy** is key — bold for questions, regular for options
8. **Teal accent** reserved for active/selected states and primary CTAs
