---
id: vintage-heritage-001
title: Heritage Emporium System
description: A warm, vintage-inspired design system with elegant script typography, cream backgrounds, and rich burgundy accents perfect for premium artisanal brands.
tags: [light, warm, vintage, premium, elegant, serif]
colors: ["#F5F0E6", "#8B2635", "#2C1810", "#C4A962", "#4A4A4A"]
created: 2024-12-22
---

# Heritage Emporium System

A sophisticated vintage design system that evokes old-world craftsmanship and timeless elegance. Features warm cream backgrounds, rich burgundy call-to-actions, elegant script typography for headlines, and gold/bronze accent tones. Perfect for premium artisanal products, luxury gifts, heritage brands, and curated collections.

## Color Palette

**Primary Colors:**
- Burgundy Primary: #8B2635 — Primary CTA buttons, accent elements, key interactive states
- Deep Brown: #2C1810 — Secondary buttons, dark text emphasis, premium touches

**Neutral Colors:**
- Cream Background: #F5F0E6 — Primary page background, warm foundation
- Warm White: #FAF8F3 — Card backgrounds, elevated surfaces
- Parchment: #EDE8DC — Secondary backgrounds, subtle sections
- Text Primary: #2C1810 — Headlines, primary body text
- Text Secondary: #4A4A4A — Supporting text, descriptions
- Text Muted: #8A8A8A — Reviews, timestamps, helper text
- Border Light: #E5DFD3 — Subtle dividers, card borders

**Accent Colors:**
- Gold/Bronze: #C4A962 — Star ratings, premium accents, decorative elements
- Tan/Khaki: #C9B896 — Promotional banners, secondary containers
- Warm Olive: #A69F7C — Supporting accent, muted backgrounds

**State Colors:**
- Success: #4A7C59 — Confirmation, positive states
- Warning: #C4A962 — Alerts, attention states
- Error: #8B2635 — Uses primary burgundy for errors

## Typography

**Font Families:**
- Display/Script: Playfair Display or similar elegant serif script — Headlines, product titles, decorative text
- Primary Serif: Georgia, Times New Roman, or similar traditional serif — Body text, descriptions
- UI Sans: -apple-system, system-ui, sans-serif — Small UI elements, buttons, labels

**Type Scale:**
- Display Script: 48-64px, 400 weight, 1.1 line-height (decorative headlines)
- Heading 1: 32-40px, 400 weight, 1.2 line-height (script/serif)
- Heading 2: 24-28px, 400 weight, 1.3 line-height (serif)
- Heading 3: 18-20px, 600 weight, 1.4 line-height (serif or sans)
- Body Large: 16-18px, 400 weight, 1.6 line-height
- Body: 14-16px, 400 weight, 1.6 line-height
- Caption: 12-14px, 400 weight, 1.5 line-height
- Label/Button: 12-14px, 500-600 weight, 1.2 line-height, letter-spacing: 0.5-1px

**Hierarchy Rules:**
- Script/cursive fonts reserved for main headlines and product names only
- ALL CAPS with letter-spacing for buttons and small labels
- Serif fonts for elegant body text
- Strong contrast between decorative headlines and functional UI text
- Price displayed in clean serif, medium weight

## Spacing System

**Base Unit:** 8px
**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 80, 96

**Common Patterns:**
- Container padding (mobile): 20-24px horizontal
- Container padding (desktop): 48-64px horizontal
- Section spacing: 48-64px vertical
- Card padding: 24-32px
- Button padding: 16px 32px (vertical/horizontal)
- Element gaps: 12-16px
- Text block spacing: 8-12px between elements
- Icon spacing: 8px from text

## Component Styles

### Buttons

**Primary Button (Burgundy):**
- Background: #8B2635
- Text: #FFFFFF
- Font: 12-14px, 600 weight, uppercase, 1-2px letter-spacing
- Padding: 16px 40px
- Border-radius: 50px (fully rounded/pill shape)
- Hover: Darken to #6B1D28, subtle shadow
- Active: Scale 0.98

**Secondary Button (Dark Brown):**
- Background: #2C1810
- Text: #FFFFFF
- Same styling as primary, different color

**Outline Button:**
- Background: transparent
- Border: 1.5px solid #2C1810
- Text: #2C1810
- Border-radius: 50px
- Hover: Background #2C1810, text #FFFFFF

**Quantity Stepper:**
- Background: #E5DFD3 (light) or transparent
- Border-radius: 50% for circular +/- buttons
- Size: 40-44px diameter
- Icon: 16-20px, #2C1810

### Cards

**Product Card:**
- Background: #FAF8F3
- Border: 1px solid #E5DFD3
- Border-radius: 0px (sharp corners for vintage feel) or 4px subtle
- Shadow: none or very subtle (0 2px 8px rgba(0,0,0,0.05))
- Padding: 24px

**Promotional Banner Card:**
- Background: #C9B896 (tan/khaki)
- Border-radius: 8-12px
- Padding: 16-24px
- Layout: Flex row with image, text, and button

### Input Fields

**Quantity Input:**
- Background: transparent
- Text: #2C1810, 16-18px, centered
- Width: 40-48px
- Flanked by circular stepper buttons

### Navigation

**Header:**
- Background: transparent or #F5F0E6
- Height: 60-72px
- Logo: Centered, circular badge with portrait illustration style
- Menu: Hamburger icon left, cart icon right
- Cart: Icon with item count in parentheses

### Rating Stars

**Star Rating:**
- Filled: #C4A962 (gold)
- Empty: #E5DFD3
- Size: 16-20px
- Gap: 2-4px between stars
- Accompanying text: "(4.89) 74 reviews" in muted gray

### Accordion/Expandable Sections

**Accordion Item:**
- Background: #C9B896 or #EDE8DC
- Border-radius: 8px
- Padding: 16-20px 24px
- Text: Uppercase, 12-14px, 600 weight
- Icon: Plus/minus, right-aligned
- Divider: None between items, or 1px #E5DFD3

### Trust Badges/Icons

**Icon Row:**
- Layout: Flex row, space-evenly or centered
- Icon: 32-40px, line-style, #2C1810
- Text: 12-14px, centered below icon
- Gap: 32-48px between items

## Layout Principles

- Max content width: 480px mobile, 1200px desktop
- Single column layout for mobile product pages
- Generous vertical whitespace (48-64px between sections)
- Centered alignment for hero sections
- Left-aligned for product details and pricing
- Full-bleed imagery for hero illustrations
- Sticky header on scroll (optional)

## Visual Effects

**Border Radius:**
- Buttons: 50px (pill shape)
- Cards: 0-4px (sharp/minimal for vintage feel)
- Banner cards: 8-12px
- Icons/Avatars: 50% (circular)
- Input containers: 4-8px

**Shadows:**
- Minimal use — vintage aesthetic favors flat design
- Subtle card shadow: 0 2px 8px rgba(0,0,0,0.05)
- Elevated elements: 0 4px 16px rgba(0,0,0,0.08)

**Borders:**
- Thin borders: 1px solid #E5DFD3
- Progress indicators: 3-4px solid bar
- Decorative use with gold/bronze tones

**Backgrounds:**
- Solid cream: #F5F0E6
- Textured paper effect (optional): subtle noise or grain
- Illustrated scenes as hero backgrounds
- Tan/khaki for promotional sections

**Decorative Elements:**
- Hand-drawn illustration style
- Victorian/vintage engraving aesthetic
- Stars and flourishes
- Circular badge/seal logos
- Whimsical scenes with storytelling elements

## Design Tone

This system embodies **nostalgic elegance** and **artisanal craftsmanship**. The warm cream palette combined with rich burgundy creates a sense of heritage and quality. Script typography adds personality and celebration while serif fonts maintain readability. The overall feeling is of a curated, premium experience — like discovering a treasure in an old bookshop. Playful illustrated elements add warmth and storytelling without compromising sophistication.

## Usage Notes for AI Implementation

**Color Application:**
- Use cream (#F5F0E6) as the default page background
- Reserve burgundy (#8B2635) strictly for primary CTAs — don't overuse
- Dark brown (#2C1810) for important secondary actions and text
- Gold (#C4A962) sparingly for ratings, accents, and premium touches
- Tan (#C9B896) for promotional banners and secondary containers

**Typography Strategy:**
- Script/display fonts ONLY for main headlines and product titles
- Never use script for body text, buttons, or UI labels
- Buttons always uppercase with letter-spacing
- Maintain high contrast between decorative and functional type

**Component Guidelines:**
- Keep buttons pill-shaped for this system
- Cards should feel flat and vintage — avoid heavy shadows
- Use illustration-style icons where possible
- Trust badges work best in simple line-icon style
- Ratings always use gold stars

**Spacing Consistency:**
- Maintain generous whitespace — don't crowd elements
- 48-64px between major sections
- 24-32px internal card padding
- 16px standard element gaps

**Maintaining Authenticity:**
- This system suits celebratory, gift-oriented, and heritage contexts
- Avoid modern/minimal tech aesthetics
- Embrace warmth, texture, and storytelling
- Illustrations and decorative elements strengthen the brand feel
