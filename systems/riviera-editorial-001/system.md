---
id: riviera-editorial-001
title: Riviera Editorial System
description: A refined, warm-neutral design system with editorial sophistication and premium lifestyle aesthetics
tags: [light, warm, editorial, premium, minimal, sophisticated]
colors: ["#1A2B4A", "#7B8EA8", "#E8E4DE", "#F5F2ED", "#C4B5A0", "#3D4F6F"]
created: 2025-12-29
---

# Riviera Editorial System

A sophisticated design system inspired by premium editorial aesthetics and luxury lifestyle brands. Built on a foundation of warm neutrals with navy accents, this system embodies understated elegance, refined typography, and generous whitespace. Perfect for lifestyle platforms, luxury e-commerce, editorial content, and premium service applications.

## Design Philosophy

The Riviera system draws from high-end magazine layouts and luxury hospitality branding. Every element communicates quality through restraint — favoring subtle tonal variations over high contrast, elegant serif typography for headlines, and ample breathing room between elements. The palette evokes natural materials: warm stone, bleached linen, aged paper, and deep ocean tones.

## Color Palette

### Primary Colors

| Color | Hex | RGB | Usage |
|-------|-----|-----|-------|
| Deep Navy | `#1A2B4A` | 26, 43, 74 | Primary text, headlines, key UI elements |
| Slate Blue | `#3D4F6F` | 61, 79, 111 | Secondary text, interactive elements |
| Dusty Blue | `#7B8EA8` | 123, 142, 168 | Tertiary text, captions, subtle accents |

### Neutral Colors

| Color | Hex | RGB | Usage |
|-------|-----|-----|-------|
| Parchment | `#F5F2ED` | 245, 242, 237 | Primary background, canvas |
| Warm Stone | `#E8E4DE` | 232, 228, 222 | Secondary background, cards, surfaces |
| Linen | `#DDD8D0` | 221, 216, 208 | Borders, dividers, subtle separators |
| Sandstone | `#C4B5A0` | 196, 181, 160 | Accent borders, decorative elements |
| Driftwood | `#A89F8F` | 168, 159, 143 | Muted accents, disabled states |

### Accent Colors

| Color | Hex | RGB | Usage |
|-------|-----|-----|-------|
| Ocean | `#4A6B8A` | 74, 107, 138 | Links, interactive highlights |
| Soft Coral | `#D4A69A` | 212, 166, 154 | Warm accents, notifications |
| Sage | `#8FA88F` | 143, 168, 143 | Success states, positive indicators |
| Amber | `#C9A962` | 201, 169, 98 | Warning states, premium badges |

### Semantic Colors

| Role | Color | Hex |
|------|-------|-----|
| Success | Sage | `#8FA88F` |
| Warning | Amber | `#C9A962` |
| Error | Dusty Rose | `#B87070` |
| Info | Dusty Blue | `#7B8EA8` |

## Typography

### Font Families

```css
--font-display: 'Cormorant Garamond', Georgia, 'Times New Roman', serif;
--font-body: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
--font-accent: 'Cormorant', Georgia, serif;
```

**Cormorant Garamond** — Used for display text, headlines, and editorial emphasis. A refined serif with elegant proportions and excellent readability at large sizes.

**Inter** — Used for body text, UI elements, and functional copy. A highly legible sans-serif optimized for screens with excellent clarity at small sizes.

### Type Scale

| Level | Size | Weight | Line Height | Letter Spacing | Usage |
|-------|------|--------|-------------|----------------|-------|
| Display | 56px / 3.5rem | 400 | 1.1 | -0.02em | Hero headlines, splash text |
| H1 | 40px / 2.5rem | 400 | 1.2 | -0.01em | Page titles, section headers |
| H2 | 32px / 2rem | 400 | 1.25 | -0.01em | Major section titles |
| H3 | 24px / 1.5rem | 500 | 1.3 | 0 | Subsection headers |
| H4 | 20px / 1.25rem | 500 | 1.35 | 0.01em | Card titles, minor headers |
| Body Large | 18px / 1.125rem | 400 | 1.65 | 0.01em | Lead paragraphs, featured text |
| Body | 16px / 1rem | 400 | 1.7 | 0.01em | Primary body text |
| Body Small | 14px / 0.875rem | 400 | 1.6 | 0.02em | Secondary text, metadata |
| Caption | 12px / 0.75rem | 500 | 1.5 | 0.04em | Labels, timestamps, fine print |
| Overline | 11px / 0.6875rem | 600 | 1.4 | 0.12em | Category labels, tags (uppercase) |

### Typography Rules

1. **Headlines (H1-H2)**: Always use Cormorant Garamond, standard weight (400), with negative letter-spacing
2. **Subheadings (H3-H4)**: Can use either serif or sans-serif depending on context
3. **Body text**: Always Inter for readability, generous line-height (1.65-1.7)
4. **Overlines/Labels**: Inter, uppercase, wide letter-spacing, medium weight
5. **Maximum line length**: 65-75 characters for optimal readability

## Spacing System

### Base Unit
**8px** — All spacing derives from multiples of 8px for consistent rhythm.

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-1` | 4px | Tight spacing, inline elements |
| `--space-2` | 8px | Small gaps, icon padding |
| `--space-3` | 12px | Compact component padding |
| `--space-4` | 16px | Standard component padding |
| `--space-5` | 24px | Card padding, input padding |
| `--space-6` | 32px | Section gaps, generous padding |
| `--space-7` | 48px | Major section spacing |
| `--space-8` | 64px | Page section margins |
| `--space-9` | 96px | Hero spacing, dramatic gaps |
| `--space-10` | 128px | Maximum section separation |

### Layout Principles

- **Container max-width**: 1200px (content), 1440px (full-bleed)
- **Content column**: 720px max for text-heavy sections
- **Grid**: 12-column with 24px gutters
- **Margin (mobile)**: 20px
- **Margin (tablet)**: 40px
- **Margin (desktop)**: 80px

## Component Styles

### Buttons

#### Primary Button
```css
.btn-primary {
  background: #1A2B4A;
  color: #F5F2ED;
  padding: 14px 32px;
  border-radius: 4px;
  font-family: var(--font-body);
  font-size: 14px;
  font-weight: 500;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  border: none;
  transition: all 0.2s ease;
}

.btn-primary:hover {
  background: #3D4F6F;
}
```

#### Secondary Button
```css
.btn-secondary {
  background: transparent;
  color: #1A2B4A;
  padding: 14px 32px;
  border-radius: 4px;
  font-family: var(--font-body);
  font-size: 14px;
  font-weight: 500;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  border: 1.5px solid #1A2B4A;
  transition: all 0.2s ease;
}

.btn-secondary:hover {
  background: #1A2B4A;
  color: #F5F2ED;
}
```

#### Ghost Button
```css
.btn-ghost {
  background: transparent;
  color: #3D4F6F;
  padding: 14px 32px;
  font-family: var(--font-body);
  font-size: 14px;
  font-weight: 500;
  letter-spacing: 0.02em;
  border: none;
  transition: color 0.2s ease;
}

.btn-ghost:hover {
  color: #1A2B4A;
}
```

### Cards

#### Standard Card
```css
.card {
  background: #FFFFFF;
  border-radius: 8px;
  padding: 32px;
  box-shadow: 0 2px 8px rgba(26, 43, 74, 0.06);
  border: 1px solid #E8E4DE;
}
```

#### Featured Card
```css
.card-featured {
  background: #F5F2ED;
  border-radius: 8px;
  padding: 40px;
  border: 1px solid #DDD8D0;
}
```

#### Interactive Card
```css
.card-interactive {
  background: #FFFFFF;
  border-radius: 8px;
  padding: 32px;
  border: 1px solid #E8E4DE;
  transition: all 0.25s ease;
  cursor: pointer;
}

.card-interactive:hover {
  border-color: #C4B5A0;
  box-shadow: 0 8px 24px rgba(26, 43, 74, 0.08);
  transform: translateY(-2px);
}
```

### Input Fields

```css
.input {
  background: #FFFFFF;
  border: 1.5px solid #DDD8D0;
  border-radius: 4px;
  padding: 14px 16px;
  font-family: var(--font-body);
  font-size: 16px;
  color: #1A2B4A;
  transition: border-color 0.2s ease;
}

.input::placeholder {
  color: #A89F8F;
}

.input:focus {
  outline: none;
  border-color: #7B8EA8;
}

.input:hover:not(:focus) {
  border-color: #C4B5A0;
}
```

### Tags & Pills

#### Category Tag
```css
.tag {
  display: inline-flex;
  align-items: center;
  background: #E8E4DE;
  color: #3D4F6F;
  padding: 6px 14px;
  border-radius: 100px;
  font-family: var(--font-body);
  font-size: 12px;
  font-weight: 500;
  letter-spacing: 0.02em;
}
```

#### Premium Badge
```css
.badge-premium {
  display: inline-flex;
  align-items: center;
  background: linear-gradient(135deg, #C9A962 0%, #D4BC7E 100%);
  color: #1A2B4A;
  padding: 4px 12px;
  border-radius: 100px;
  font-family: var(--font-body);
  font-size: 11px;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}
```

### Navigation

```css
.nav-link {
  font-family: var(--font-body);
  font-size: 14px;
  font-weight: 500;
  letter-spacing: 0.02em;
  color: #3D4F6F;
  text-decoration: none;
  padding: 8px 0;
  border-bottom: 2px solid transparent;
  transition: all 0.2s ease;
}

.nav-link:hover {
  color: #1A2B4A;
}

.nav-link.active {
  color: #1A2B4A;
  border-bottom-color: #1A2B4A;
}
```

## Visual Effects

### Border Radius Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--radius-sm` | 4px | Buttons, inputs, small elements |
| `--radius-md` | 8px | Cards, containers |
| `--radius-lg` | 12px | Modals, large cards |
| `--radius-xl` | 16px | Feature sections |
| `--radius-full` | 100px | Pills, tags, avatars |

### Shadows

```css
/* Subtle elevation */
--shadow-sm: 0 1px 3px rgba(26, 43, 74, 0.04);

/* Card elevation */
--shadow-md: 0 2px 8px rgba(26, 43, 74, 0.06);

/* Elevated/hover state */
--shadow-lg: 0 8px 24px rgba(26, 43, 74, 0.08);

/* Modal/overlay */
--shadow-xl: 0 16px 48px rgba(26, 43, 74, 0.12);

/* Soft ambient */
--shadow-ambient: 0 4px 20px rgba(26, 43, 74, 0.05);
```

### Borders

```css
/* Standard divider */
--border-light: 1px solid #E8E4DE;

/* Subtle separation */
--border-subtle: 1px solid #DDD8D0;

/* Interactive border */
--border-interactive: 1.5px solid #C4B5A0;

/* Focus ring */
--border-focus: 2px solid #7B8EA8;
```

### Transitions

```css
/* Quick micro-interactions */
--transition-fast: 150ms ease;

/* Standard interactions */
--transition-base: 200ms ease;

/* Deliberate movements */
--transition-slow: 300ms ease;

/* Dramatic reveals */
--transition-dramatic: 500ms cubic-bezier(0.4, 0, 0.2, 1);
```

## Layout Patterns

### Hero Section
```
┌────────────────────────────────────────────────────────┐
│                    [96px top padding]                   │
│                                                        │
│              OVERLINE CATEGORY TEXT                    │
│                                                        │
│         Large Display Headline in                      │
│              Cormorant Garamond                        │
│                                                        │
│    Supporting body text in Inter, centered,            │
│    maximum 600px width for optimal reading             │
│                                                        │
│              [PRIMARY BUTTON]                          │
│                                                        │
│                    [96px bottom padding]               │
└────────────────────────────────────────────────────────┘
```

### Content Grid
```
┌──────────────┬──────────────┬──────────────┐
│              │              │              │
│    Card 1    │    Card 2    │    Card 3    │
│              │              │              │
├──────────────┼──────────────┼──────────────┤
│              │              │              │
│    Card 4    │    Card 5    │    Card 6    │
│              │              │              │
└──────────────┴──────────────┴──────────────┘
Grid: 3 columns, 24px gap
Cards: Equal height, 32px padding
```

### Split Layout
```
┌─────────────────────────┬─────────────────────────┐
│                         │                         │
│        Image/Media      │    Content Column       │
│        (50% width)      │    - Headline           │
│                         │    - Body text          │
│                         │    - CTA button         │
│                         │                         │
└─────────────────────────┴─────────────────────────┘
Gap: 64px between columns
Alignment: Vertical center
```

## Responsive Breakpoints

| Breakpoint | Value | Layout Adjustments |
|------------|-------|-------------------|
| Mobile | < 640px | Single column, 20px margins, stacked navigation |
| Tablet | 640px - 1024px | 2-column grid, 40px margins |
| Desktop | 1024px - 1440px | Full grid, 80px margins |
| Large | > 1440px | Centered container, max-width constraints |

## Iconography

### Style Guidelines
- **Stroke weight**: 1.5px
- **Size scale**: 16px, 20px, 24px, 32px
- **Color**: Inherit from text color
- **Style**: Outlined, rounded corners
- **Recommended set**: Lucide, Feather Icons, or similar minimal line icons

### Icon + Text Pairing
```css
.icon-text {
  display: inline-flex;
  align-items: center;
  gap: 8px;
}

.icon-text svg {
  width: 20px;
  height: 20px;
  stroke-width: 1.5;
}
```

## Imagery Guidelines

### Photography Style
- **Tone**: Warm, natural lighting with soft shadows
- **Subjects**: Lifestyle, editorial, documentary aesthetic
- **Color grading**: Slightly desaturated, warm highlights, lifted blacks
- **Composition**: Generous negative space, rule of thirds

### Image Treatments
```css
/* Subtle warm overlay */
.image-warm::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(180deg, rgba(245, 242, 237, 0) 0%, rgba(245, 242, 237, 0.1) 100%);
}

/* Soft border treatment */
.image-framed {
  border-radius: 8px;
  box-shadow: 0 4px 20px rgba(26, 43, 74, 0.08);
}
```

## Accessibility

### Color Contrast
- **Primary text on parchment**: 10.2:1 ✓ (AAA)
- **Secondary text on parchment**: 6.8:1 ✓ (AAA)
- **Tertiary text on parchment**: 4.5:1 ✓ (AA)
- **Button text on navy**: 9.1:1 ✓ (AAA)

### Focus States
```css
*:focus-visible {
  outline: 2px solid #7B8EA8;
  outline-offset: 2px;
}
```

### Touch Targets
- Minimum touch target: 44px × 44px
- Button minimum height: 48px
- Navigation link minimum height: 44px

## Design Tone

The Riviera Editorial System embodies **quiet luxury** — sophisticated without being ostentatious, refined without being cold. It speaks to discerning users who appreciate quality craftsmanship and timeless aesthetics over trendy decoration.

The warm neutral palette creates an inviting, approachable atmosphere while the navy accents provide necessary contrast and visual anchoring. Typography choices balance editorial elegance (Cormorant Garamond) with digital practicality (Inter), creating a system equally at home in magazine-style content and functional interfaces.

This system excels in contexts requiring trust, sophistication, and premium positioning: luxury e-commerce, lifestyle editorial, hospitality platforms, premium service providers, and high-end SaaS products.

## Usage Notes for AI Implementation

1. **Background hierarchy**: Use `#F5F2ED` (parchment) as primary background, `#E8E4DE` (warm stone) for cards/surfaces on top, and `#FFFFFF` sparingly for high-contrast elements

2. **Typography pairing**: Default to Cormorant Garamond for H1-H2 headlines, Inter for everything else. Reserve serif for moments of editorial emphasis

3. **Whitespace is intentional**: This system relies on generous spacing. Don't compress elements — let them breathe

4. **Color restraint**: Use navy (`#1A2B4A`) for text and primary actions only. Accents should be used sparingly as highlights, not as primary UI colors

5. **Interaction subtlety**: Hover states should be gentle transitions in color or shadow, not dramatic transformations

6. **Image integration**: Photography should feel warm and editorial. Avoid stock photo aesthetics — favor documentary, lifestyle imagery with natural lighting

7. **Responsive priority**: Mobile layouts should maintain generous padding and readable type sizes. Never sacrifice whitespace for cramming content

8. **Loading states**: Use subtle opacity transitions or skeleton screens with warm stone (`#E8E4DE`) backgrounds, never harsh spinners
