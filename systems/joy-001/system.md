# Joy Design System

A comprehensive design system for use in AI-assisted design.
## Core Design Principles

1. **Approachable Warmth** - Design should feel friendly and supportive, never clinical or intimidating
2. **Clean Simplicity** - Information hierarchy is clear, layouts are uncluttered
3. **Soft Modernism** - Contemporary design with rounded edges and gentle curves
4. **Trust Through Professionalism** - Polish and attention to detail convey expertise
5. **Accessible Optimism** - Visual tone is positive without being overly saccharine

-----

## Color Palette

### Primary Colors

**Warm Coral/Peach**

- Primary: `#FF8B7B` (approx)
- Use for: Primary CTAs, key highlights, brand moments
- Represents: Warmth, care, human connection

**Soft Teal/Turquoise**

- Primary: `#5ECEC6` (approx)
- Use for: Secondary actions, accents, informational elements
- Represents: Calm, trust, support

**Navy/Deep Blue**

- Primary: `#2B3F5C` (approx)
- Use for: Headers, body text, professional elements
- Represents: Trust, expertise, reliability

### Secondary Colors

**Cream/Warm White**

- Background: `#FFF9F5` (approx)
- Use for: Main backgrounds, cards, sections
- Creates: Warmth and softness compared to stark white

**Soft Pink**

- Accent: `#FFD4CF` (approx)
- Use for: Subtle backgrounds, highlights, gentle emphasis

**Light Teal**

- Accent: `#E5F7F6` (approx)
- Use for: Alternative section backgrounds, cards

### Neutral Colors

- **Pure White:** `#FFFFFF` - Cards, overlays
- **Light Gray:** `#F5F5F5` - Subtle backgrounds
- **Mid Gray:** `#8B8B8B` - Secondary text
- **Dark Gray:** `#3A3A3A` - Body text
- **Black:** `#000000` - Sparingly for emphasis

### Usage Guidelines

- **Backgrounds:** Primarily use cream/warm white for warmth
- **Text:** Navy for headings, dark gray for body text
- **CTAs:** Warm coral for primary, soft teal for secondary
- **Accents:** Use soft pink and light teal for visual interest
- **Contrast:** Maintain WCAG AA standards minimum

-----

## Typography

### Font Families

**Primary Font:** Sans-serif, likely similar to:

- **Circular** or **Inter** or **DM Sans**
- Clean, modern, highly readable
- Slightly rounded characteristics for warmth

**Secondary Font:** Same family or similar sans-serif

- Consistent brand voice across all text

### Type Scale

```
H1: 48-56px / 3-3.5rem
    Line Height: 1.1-1.2
    Weight: 700 (Bold)
    Use: Hero headlines, page titles

H2: 36-42px / 2.25-2.625rem
    Line Height: 1.2
    Weight: 700 (Bold)
    Use: Section headers, major features

H3: 28-32px / 1.75-2rem
    Line Height: 1.3
    Weight: 600 (Semi-bold)
    Use: Subsection headers, card titles

H4: 20-24px / 1.25-1.5rem
    Line Height: 1.4
    Weight: 600 (Semi-bold)
    Use: Component headers, list titles

Body Large: 18-20px / 1.125-1.25rem
    Line Height: 1.6
    Weight: 400 (Regular)
    Use: Hero subtext, important body copy

Body: 16px / 1rem
    Line Height: 1.6
    Weight: 400 (Regular)
    Use: Standard body text, descriptions

Body Small: 14px / 0.875rem
    Line Height: 1.5
    Weight: 400 (Regular)
    Use: Captions, metadata, secondary info

Button Text: 16-18px / 1-1.125rem
    Weight: 600 (Semi-bold)
    Letter Spacing: 0.02em
```

### Typography Guidelines

- **Hierarchy:** Clear size differentiation between levels
- **Readability:** Never compromise on legibility
- **Line Length:** Max 65-75 characters for body text
- **Alignment:** Left-aligned for body text, centered for headers when appropriate
- **Weight Contrast:** Use weight to create visual hierarchy

-----

## Spacing System

Use an 8px base unit system for consistency:

```
XXS: 4px   (0.25rem)
XS:  8px   (0.5rem)
S:   16px  (1rem)
M:   24px  (1.5rem)
L:   32px  (2rem)
XL:  48px  (3rem)
XXL: 64px  (4rem)
XXXL: 96px (6rem)
```

### Spacing Applications

- **Component Padding:** 16-32px (S-L)
- **Section Spacing:** 64-96px (XXL-XXXL)
- **Card Padding:** 24-32px (M-L)
- **Element Margins:** 8-24px (XS-M)
- **Gutter Width:** 16-24px (S-M)

-----

## Layout & Grid

### Grid System

- **Columns:** 12-column responsive grid
- **Max Width:** 1200-1280px for main content
- **Breakpoints:**
  - Mobile: 320-767px
  - Tablet: 768-1023px
  - Desktop: 1024px+
  - Wide: 1440px+

### Layout Patterns

**Hero Sections:**

- Full-width backgrounds with contained content
- Asymmetric layouts with image/illustration on one side
- Generous vertical padding (80-120px)
- Content typically left-aligned or centered

**Content Sections:**

- Alternating layouts (left-right, right-left)
- Balanced white space
- Clear visual separation between sections
- Background color changes for distinction

**Card Layouts:**

- Equal-height cards in grid patterns
- 2-4 columns depending on viewport
- Consistent internal padding
- Subtle shadows or borders

-----

## Components

### Buttons

**Primary Button**

- Background: Warm coral (`#FF8B7B`)
- Text: White
- Border Radius: 24-32px (pill shape)
- Padding: 14px 32px
- Font Weight: 600
- Hover: Slightly darker shade (10-15%)
- Shadow: Subtle `0 2px 8px rgba(0,0,0,0.1)`

**Secondary Button**

- Background: Soft teal (`#5ECEC6`)
- Text: White or Navy
- Border Radius: 24-32px (pill shape)
- Padding: 14px 32px
- Font Weight: 600
- Hover: Slightly darker shade

**Outline Button**

- Background: Transparent
- Border: 2px solid Navy or Coral
- Text: Navy or Coral
- Border Radius: 24-32px
- Padding: 12px 30px
- Hover: Fill with color, white text

### Cards

**Standard Card**

- Background: White or Cream
- Border Radius: 16-24px
- Padding: 24-32px
- Shadow: `0 4px 16px rgba(0,0,0,0.08)`
- Border: None or 1px subtle border

**Feature Card**

- Larger padding (32-48px)
- Icon or illustration at top
- Title + description + optional CTA
- Centered or left-aligned content
- Hover: Lift effect with increased shadow

### Icons

**Style:**

- Line-based or minimal filled
- Rounded ends (not sharp)
- Consistent stroke width (1.5-2px)
- Sized at 20px, 24px, 32px, 48px

**Usage:**

- Pair with text for clarity
- Use color strategically (coral/teal for emphasis)
- Maintain consistent visual weight

### Forms

**Input Fields**

- Border Radius: 8-12px
- Border: 1px solid light gray
- Padding: 12px 16px
- Font Size: 16px
- Focus State: Border color changes to coral/teal, subtle shadow
- Background: White or very light cream

**Labels**

- Position: Above input
- Font Size: 14px
- Weight: 600
- Color: Navy or dark gray
- Spacing: 8px below label

### Navigation

**Header Navigation**

- Clean horizontal layout
- Logo left, menu items right
- Transparent or white background
- Sticky positioning common
- Mobile: Hamburger menu

**Menu Items**

- Font Size: 16px
- Weight: 500-600
- Color: Navy
- Hover: Color change to coral
- Spacing: 24-32px between items

-----

## Visual Elements

### Imagery

**Photography:**

- Warm, natural lighting
- Real parents and children (not overly staged)
- Diverse representation
- Soft focus or slight blur acceptable
- Color grading: Warm tones, slightly desaturated

**Illustrations:**

- Soft, organic shapes
- Minimal detail, modern style
- Color palette matches brand colors
- Used as accents and decorative elements
- Avoid sharp angles

### Shapes & Patterns

**Rounded Elements:**

- Border Radius: 8px (small), 16px (medium), 24px+ (large)
- Pill shapes for buttons and badges
- Organic, flowing shapes in backgrounds

**Background Patterns:**

- Subtle textures or gradients
- Organic blobs or waves
- Light overlays for depth
- Never overwhelming or distracting

### Shadows & Depth

**Subtle Elevation:**

```css
Level 1: 0 2px 8px rgba(0,0,0,0.06)
Level 2: 0 4px 16px rgba(0,0,0,0.08)
Level 3: 0 8px 24px rgba(0,0,0,0.12)
```

**Usage:**

- Cards and modals: Level 1-2
- Floating elements: Level 2-3
- Keep shadows soft and diffused

-----

## Motion & Animation

### Principles

- **Ease Timing:** ease-out or ease-in-out
- **Duration:** 200-400ms for most transitions
- **Subtle:** Never jarring or attention-grabbing
- **Purposeful:** Enhance understanding, don’t decorate

### Common Animations

**Hover States:**

- Scale: 1.02-1.05
- Shadow increase
- Color shifts
- Duration: 200ms

**Page Transitions:**

- Fade in/out: 300ms
- Slide animations: 400ms
- Stagger child elements: 50-100ms delay

**Loading States:**

- Skeleton screens
- Pulsing animations
- Progress indicators in brand colors

-----

## Accessibility Standards

### Minimum Requirements

- **Color Contrast:** WCAG AA (4.5:1 for normal text, 3:1 for large text)
- **Focus States:** Clear visible indicators (outline or shadow)
- **Touch Targets:** Minimum 44x44px
- **Alt Text:** All images require descriptive alt text
- **Keyboard Navigation:** Full site accessible via keyboard
- **Screen Readers:** Semantic HTML, ARIA labels where needed

### Best Practices

- Test with actual assistive technologies
- Ensure form errors are clearly announced
- Provide skip navigation links
- Use sufficient spacing between interactive elements
- Never rely on color alone to convey information

-----

## Content Voice & Tone

### Writing Style

**Voice Characteristics:**

- Warm and supportive
- Expert but approachable
- Conversational, not clinical
- Empathetic and understanding
- Action-oriented

**Tone Guidelines:**

- **Supportive:** “We’re here for you” attitude
- **Clear:** Avoid jargon, explain when necessary
- **Positive:** Focus on solutions and capabilities
- **Respectful:** Never patronizing or dismissive
- **Human:** Write like a caring friend with expertise

**Example Phrases:**

- ✅ “We’re awake too” (empathetic, human)
- ✅ “Expert advice 24/7” (clear value)
- ✅ “Whatever is on your mind” (open, supportive)
- ❌ “Solutions for your problems” (cold, transactional)
- ❌ “Professional consultation services” (clinical, distant)

-----

## Implementation Guidelines

### For AI Design Tools

When using this design system with AI:

1. **Start with Purpose:** Define the component or page goal first
2. **Reference Color Codes:** Use specific hex values from this system
3. **Follow Hierarchy:** Maintain clear visual hierarchy in every design
4. **Maintain Consistency:** Apply patterns consistently across designs
5. **Check Accessibility:** Verify contrast and spacing standards
6. **Consider Context:** Adapt spacing and sizing for different viewports
7. **Use Examples:** Reference Joy.co patterns when describing layouts

### Quick Reference Prompts

**For Hero Sections:**
“Create a hero section using Joy design system: warm coral CTA, cream background, asymmetric layout with illustration right, navy heading, dark gray body text, generous 96px vertical padding”

**For Cards:**
“Design feature cards using Joy system: white background, 24px border radius, 32px padding, subtle shadow level 1, coral icons, navy headings, centered content”

**For Forms:**
“Create form using Joy design: 12px border radius inputs, 16px font size, navy labels above inputs, coral focus states, warm coral submit button”

### Component Library Priorities

Build these components first:

1. Button variants (primary, secondary, outline)
2. Card components (standard, feature, pricing)
3. Form elements (input, textarea, select, checkbox)
4. Navigation (header, footer, mobile menu)
5. Hero sections (2-3 layout variants)
6. Content sections (alternating layouts)

-----

## Examples & Patterns

### Homepage Hero Pattern

```
Layout: Asymmetric 60/40 split
Left Side:
  - Navy H1 heading (48-56px)
  - Dark gray body text (18-20px)
  - Coral primary CTA button
  - Trust indicator text below
Right Side:
  - Illustration or photo montage
  - Organic shapes or flowing design
Background: Cream (#FFF9F5)
Padding: 96px vertical, contained width
```

### Feature Section Pattern

```
Layout: Centered or alternating
Background: Alternates between cream and light teal
Content:
  - Navy H2 heading (36-42px)
  - List of features with icons
  - Each feature: Icon (coral/teal) + Title + Description
  - Optional image alongside
Spacing: 64px between sections, 24px between features
```

### Pricing Card Pattern

```
Card Structure:
  - White background
  - 24px border radius
  - 32px padding
  - Subtle shadow
Content Hierarchy:
  - Small label at top ("Most Popular" - coral background)
  - Plan name (H3, navy)
  - Large price (H2, navy)
  - Billing frequency (small text, gray)
  - Feature list (checkmarks in teal)
  - Full-width CTA button at bottom
```

-----

## Dos and Don’ts

### Do:

✅ Use warm, approachable color palette  
✅ Maintain generous white space  
✅ Use rounded corners consistently  
✅ Create clear visual hierarchy  
✅ Test for accessibility  
✅ Keep navigation simple and clear  
✅ Use real, warm photography  
✅ Write in supportive, friendly voice

### Don’t:

❌ Use sharp angles or harsh design elements  
❌ Overcrowd layouts with too many elements  
❌ Use cold or clinical color schemes  
❌ Create confusing navigation  
❌ Sacrifice readability for aesthetics  
❌ Use overly formal or corporate language  
❌ Rely solely on icons without text  
❌ Forget mobile-first responsive design

-----

## Version History

**Version 1.0** - Initial design system created from Joy.co analysis  
**Date:** November 12, 2025  
**Created for:** AI-assisted design guidance

-----

## Notes for Designers

This design system is optimized for parenting and family-focused applications but can be adapted for:

- Healthcare and wellness apps
- Educational platforms
- Community-focused services
- Support and coaching services

The key is maintaining the warm, approachable aesthetic while adjusting colors and imagery to match your specific brand.

-----

**When in doubt:** Always maintain the core principles of warmth, clarity, and accessibility outlined in this system.