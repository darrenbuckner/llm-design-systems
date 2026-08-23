---
id: dark-terminal-cli-001
title: Cipher Terminal System
description: A dark, terminal-inspired interface with vibrant accent colors and monospace typography for developer tools
tags: [dark, technical, terminal, developer, minimal]
colors: ["#0D0D0D", "#1A1A1A", "#3B82F6", "#22C55E", "#FFFFFF", "#6B7280"]
created: 2025-01-15
---

# Cipher Terminal System

A sophisticated dark interface inspired by command-line environments, featuring deep black backgrounds, vibrant blue and green accents, and monospace typography. The aesthetic combines the familiarity of terminal emulators with modern UI polish, creating a technical yet approachable developer experience.

## Color Palette

**Primary Colors:**
- Primary Blue: #3B82F6 — Headlines, links, primary actions, branded text
- Primary Green: #22C55E — Success states, secondary headlines, bracketed accents

**Background Colors:**
- Deep Black: #0D0D0D — Page background, primary surface
- Terminal Dark: #1A1A1A — Card backgrounds, elevated surfaces
- Terminal Header: #2D2D2D — Window chrome, toolbar backgrounds

**Text Colors:**
- Text Primary: #FFFFFF — Main content, headings, high-emphasis text
- Text Secondary: #9CA3AF — Descriptions, labels, subdued content
- Text Muted: #6B7280 — Placeholder text, disabled states
- Code Dimmed: #4B5563 — Background code snippets, decorative text

**Accent Colors:**
- Amber Glow: #F59E0B — Warm gradient accent (background effect)
- Deep Orange: #EA580C — Secondary warm accent
- Teal: #14B8A6 — Tertiary accent for variety

**State Colors:**
- Success: #22C55E — Confirmations, positive feedback
- Warning: #F59E0B — Caution states
- Error: #EF4444 — Error messages, destructive actions
- Info: #3B82F6 — Informational highlights

## Typography

**Font Families:**
- Primary: SF Pro Display, -apple-system, system-ui, sans-serif — Headlines, UI text
- Monospace: SF Mono, Menlo, Monaco, "Courier New", monospace — Code, terminal output, technical content

**Type Scale:**
- Display: 48px, weight 600, line-height 1.1 — Hero headlines
- Heading 1: 36px, weight 600, line-height 1.2 — Section titles
- Heading 2: 24px, weight 500, line-height 1.3 — Subsection headers
- Body Large: 18px, weight 400, line-height 1.6 — Intro paragraphs
- Body: 16px, weight 400, line-height 1.6 — Standard content
- Code: 15px, weight 400, line-height 1.7 — Terminal/code blocks
- Caption: 13px, weight 400, line-height 1.5 — Labels, hints

**Hierarchy Rules:**
- Headlines use vibrant blue (#3B82F6) for brand emphasis
- Bracketed text uses green (#22C55E) for visual interest: [like this]
- Code and terminal content always in monospace
- Secondary text uses muted gray for contrast hierarchy

## Spacing System

**Base Unit:** 4px

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96

**Common Patterns:**
- Component internal padding: 16px - 24px
- Card padding: 24px - 32px
- Section spacing: 64px - 96px
- Inline spacing (text elements): 8px - 12px
- Terminal line spacing: 8px between lines

## Component Styles

### Terminal Window
- Background: #1A1A1A
- Border: 1px solid #2D2D2D
- Border radius: 12px
- Header dots: Three circles (#4B5563) at 12px diameter, 8px gap
- Padding: 24px
- Inner code block: Additional padding 20px, background #0D0D0D or transparent

### Code Block
- Background: Transparent or subtle #0D0D0D
- Border: 1px solid #374151
- Border radius: 8px
- Padding: 20px
- Font: Monospace, 15px
- Line numbers: Optional, #4B5563

### Command Prompt
- Prefix style: `>_` in primary text color
- Command text: White, monospace
- Parameters: Color-coded (blue for values, gray for flags)
- Comments/hints: #6B7280

### Buttons (Implied)
- Primary: #3B82F6 background, white text, 8px radius
- Secondary: Transparent, #3B82F6 border and text
- Ghost: Transparent, white text, hover reveals background
- Padding: 12px 24px
- Font weight: 500

### Navigation Links
- Default: #9CA3AF
- Hover: #FFFFFF
- Active: #3B82F6
- Transition: 150ms ease

## Layout Principles

- **Max content width:** 1200px centered
- **Grid structure:** Flexible, content-driven layouts
- **Alignment:** Left-aligned text, centered hero sections
- **Responsive behavior:** Single column on mobile, multi-column on desktop
- **Terminal windows:** Often offset or floating for visual interest

## Visual Effects

**Border Radius:**
- Small (buttons, inputs): 6px - 8px
- Medium (cards, modals): 12px
- Large (hero elements): 16px

**Shadows:**
- Subtle: 0 4px 6px rgba(0, 0, 0, 0.3)
- Medium: 0 8px 24px rgba(0, 0, 0, 0.4)
- Glow (accent): 0 0 40px rgba(59, 130, 246, 0.15)

**Borders:**
- Default: 1px solid #2D2D2D
- Subtle: 1px solid #1F1F1F
- Focus: 2px solid #3B82F6

**Background Effects:**
- Gradient glow: Radial gradient with amber/orange tones bleeding through dark background
- Code watermark: Faded code snippets in background (#1A1A1A at 30% opacity)
- Blur effects: Subtle backdrop-blur on floating elements

## Design Tone

This system conveys technical sophistication and developer credibility through its terminal-native aesthetic. The deep blacks create focus and reduce eye strain during extended use, while the vibrant blue and green accents inject energy and brand personality. The overall feeling is professional, modern, and purpose-built for technical audiences who appreciate clean, functional design with thoughtful details.

## Usage Notes for AI Implementation

- Use the blue/green accent pattern sparingly — headlines and key CTAs only
- Terminal windows should feel authentic: proper spacing, realistic command structure
- Background code effects add depth but should never compete with foreground content
- Maintain strong contrast ratios (WCAG AA minimum) despite the dark theme
- The bracketed green text pattern [like this] works well for taglines and emphasis
- Monospace typography is essential for any code or technical content
- Warm gradient glows in backgrounds add sophistication without overwhelming the interface
