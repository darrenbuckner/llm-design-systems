# Canvas Brutalist Design System

## Visual Style

Brutalist minimalism - pure white (#FFFFFF) background, pure black (#000000) text, maximum contrast. No grays, no accent colors, no gradients.

## Typography

**Typeface:**

- Sans-serif (Inter, Suisse Int’l, ABC Favorit, or similar modern grotesque)
- Section labels: lowercase monospace
- Body text: clean sans-serif, line-height 1.5-1.6
- No heavy bolds - use medium/regular weight only

**Hierarchy:**

- Section headers: lowercase monospace (~12-14px)
- Main headlines: ~32-36px
- Body text: ~14-16px
- Clear size scale, generous line spacing

## Color Palette

- Background: Pure white (#FFFFFF)
- Text: Pure black (#000000)
- Borders/dividers: Black 1px lines
- No grays, no color accents, no transparency effects

## Layout Systems

### Single Column (Mobile/Narrow)

- Flush left alignment
- Generous padding (20-24px sides)
- 40-60px vertical spacing between sections
- Comfortable reading width, never full-width text blocks
- Thin black horizontal rules (1px) as section dividers

### Multi-Column Grids (Desktop/Wide)

- 12-column grid system with generous gutters (24-32px)
- Common patterns:
  - **2-column:** 50/50 split or 60/40 for content/sidebar (e.g., 8-col + 4-col)
  - **3-column:** Equal thirds for card layouts or feature grids (4-4-4)
  - **4-column:** For galleries, team members, dense information (3-3-3-3)
- Maintain alignment to grid even with asymmetric layouts
- Column content flush left within each column
- Vertical rhythm maintained across columns (aligned baselines when possible)

### Grid Principles

- White space is structural, not decorative
- Gutters never less than 24px
- Grid lines invisible but structure is evident
- Asymmetric layouts allowed but intentional (2:1, 3:2 ratios)
- Never crowd columns - breathing room essential

### Responsive Behavior

- **Desktop:** Multi-column grids as designed
- **Tablet:** Reduce to 2-column or single column
- **Mobile:** Always single column
- Breakpoints feel natural, not arbitrary

## Spacing Scale

Consistent spacing units based on 8px grid:

- **XS:** 8px
- **S:** 16px
- **M:** 24px
- **L:** 32px
- **XL:** 40px
- **XXL:** 48-64px
- **Section gaps:** 60-80px

## Components

### Buttons

- Outline style only - thin black border (1-2px)
- Rounded corners (~24px radius)
- Text-only interior, no fill
- No shadows, completely flat
- Generous padding (12-16px vertical, 24-32px horizontal)
- Hover: subtle inverse (black background, white text) or slight border weight increase

### Cards/Tiles

- White background (same as page) or thin black border (1px)
- No shadows, no elevation, no depth
- Internal padding: 24-32px
- Cards align to grid columns
- Consistent card heights within rows when possible

### Navigation/Headers

- Can span full width or follow grid
- Horizontal divider (1px black) to separate from content
- Left-aligned logo/branding, right-aligned actions/links
- Generous padding (20-24px vertical)

### Sections

- Full-width thin black dividers (1px) between major sections
- Section titles can be full-width or column-constrained
- Content within sections follows grid system

### Lists/Tables

- Use grid columns for multi-column data
- Thin black borders (1px) for table cells
- Generous cell padding (16-20px)
- No alternating row colors - use spacing for clarity

### Forms

- Input fields: black border (1px), no fill or transparent
- Labels: above inputs, lowercase monospace optional
- No placeholder text styling - keep minimal
- Focus states: subtle border weight increase or inverse

### Icons

- Minimal and geometric
- Line-based, not filled
- Consistent stroke width (1-2px)
- Scale appropriately to context

## Layout Patterns

### Two-Column Content + Sidebar

```
[8 columns: main content] [4 columns: sidebar/meta]
```

- Main content: flush left, comfortable reading width
- Sidebar: supplementary info, smaller text acceptable
- Maintain vertical rhythm between columns

### Three-Column Feature Grid

```
[4 cols] [4 cols] [4 cols]
```

- Equal weight features or cards
- Aligned tops
- Consistent internal structure
- Generous gutters (24-32px)

### Asymmetric Layout

```
[5 columns: primary] [7 columns: detail/visual]
```

- Intentional imbalance creates focus
- Both columns maintain internal spacing rules
- Can flip ratio based on content priority

### Gallery/Team Grid

```
[3] [3] [3] [3]
[3] [3] [3] [3]
```

- Uniform tiles
- Consistent gutters (24-32px)
- Can be 2, 3, or 4 columns based on screen size
- Maintains grid alignment

## Content Density Rules

- **Sparse layouts:** Large hero sections, landing pages - let content breathe
- **Dense layouts:** Dashboards, data tables - grid keeps it organized
- Never sacrifice readability for density
- White space is functional, not wasted space
- One key message per screen/section when possible

## Alignment Principles

- **Text:** Flush left within containers (never centered paragraphs)
- **Headings:** Can be centered for impact, but keep rare
- **Grid items:** Top-aligned unless intentionally centered
- **Baseline grid:** Maintain when possible across columns
- **Overall page:** Content typically left-aligned or follows grid

## Design Principles

1. **Radical simplicity** - No decorative elements whatsoever
1. **Information hierarchy through scale and space** - Not color or weight
1. **Confidence through restraint** - The absence of styling is the style
1. **Readability first** - High contrast, generous spacing, optimal line length
1. **Grid creates order** - Structure through layout, not ornament
1. **Clarity through light** - Clean, open, uncluttered canvas for content
1. **Tech-forward** - Monospace touches, lowercase conventions signal precision and craft

## What NOT to Do

- ❌ No drop shadows or elevation effects
- ❌ No gradients or color transitions
- ❌ No rounded content blocks (buttons are exception)
- ❌ No gray tones or muted colors
- ❌ No centered body text paragraphs
- ❌ No decorative elements or flourishes
- ❌ No background textures or patterns
- ❌ No multiple accent colors
- ❌ No cramped spacing or tight gutters
- ❌ No heavy bold weights everywhere

## Tone & Voice

Confident, direct, pristine clarity. Designer/architect culture. This design says: “We value clarity and precision. Clean lines, clear thinking.”

-----

## AI Prompting Templates

### For Web Design (HTML/React):

```
Create a [page type] using Canvas brutalist aesthetic:

Style:
- Pure white background (#FFFFFF), black text (#000000)
- Monospace lowercase section headers
- Clean sans-serif body text, line-height 1.5-1.6
- Thin black borders/dividers (1px)
- Outline buttons with ~24px rounded corners
- No shadows, gradients, or grays

Layout:
- [Specify: single column OR multi-column grid]
- [If grid: "12-column grid with 24-32px gutters"]
- [Specify column distribution: "8-col main + 4-col sidebar" or "3 equal columns"]
- Generous spacing: 40-60px between sections
- 20-24px side padding

Responsive:
- Desktop: [X] columns
- Tablet: [Y] columns
- Mobile: Single column

Use Tailwind core utilities only (no custom classes).
```

### For Presentations (PPTX):

```
Design a [presentation type] with Canvas brutalist aesthetic:

- White slides (#FFFFFF), black text (#000000) throughout
- Minimal sans-serif typography
- Monospace lowercase section headers
- One key message per slide
- Thin line dividers only (1px black)
- No gradients, shadows, or transitions
- Generous spacing, never cramped
- Outline-style elements if needed
- [Specify slides needed and key content]
```

### For Documents (DOCX):

```
Format this [document type] in Canvas brutalist style:

- High contrast, clean typography
- Monospace headers in lowercase (optional)
- Generous line spacing (1.5-1.6)
- Minimal formatting, maximum readability
- Use spacing for hierarchy, not excessive bold
- Simple tables with clear borders
- No colors, no grays
- [Specify content and structure]
```

### For Complex Layouts:

```
Create a [page/interface] using Canvas brutalist aesthetic with [2/3/4]-column grid:

Layout:
- 12-column grid, 24-32px gutters
- [Specify: "60/40 split" or "3 equal columns" or "asymmetric 5-7"]
- Maintain 40-60px section spacing
- Align elements to grid
- [Desktop/Tablet/Mobile behavior]

Style:
- Pure white background, black text
- Thin black borders/dividers (1px)
- No shadows or gradients
- Monospace lowercase section headers
- Generous padding within grid items
- Outline buttons only

Content:
- [Specify sections and content needs]
```

-----

## Quick Review Checklist

Before finalizing any design:

- ☐ Is it pure white/black (no grays or colors)?
- ☐ Are headers in lowercase monospace?
- ☐ Is spacing generous (40-60px between sections)?
- ☐ Are buttons outline-only with rounded corners?
- ☐ Is everything flat (no shadows, no gradients)?
- ☐ If multi-column: Are gutters 24px minimum?
- ☐ If multi-column: Does it collapse logically on mobile?
- ☐ Is text flush left (not centered)?
- ☐ Are dividers thin (1px) black lines?
- ☐ Does it feel confident and minimal?
- ☐ Is the grid structure evident but invisible?
- ☐ Is white space used structurally?
- ☐ Does it feel clean and open (not stark or harsh)?

-----

## Implementation Notes

### For HTML/CSS:

- Use `background: #fff; color: #000;`
- Border: `border: 1px solid #000;`
- Grid: CSS Grid or Flexbox with explicit gap values
- Buttons: `border: 1px solid #000; border-radius: 24px; background: transparent;`
- Hover (optional): `background: #000; color: #fff;`

### For Tailwind:

- `bg-white text-black`
- `border border-black`
- `rounded-3xl` for buttons
- `gap-6` or `gap-8` for grid gutters
- `space-y-12` or `space-y-16` for section spacing
- `hover:bg-black hover:text-white` for button hovers

### For Design Tools (Figma/Sketch):

- Background: #FFFFFF
- Text: #000000
- Use 8px grid
- Set up 12-column layout grid with 24-32px gutters
- Create component styles for buttons, cards, headers
- Use auto-layout with generous spacing

-----

## When to Use Canvas vs Block

**Use Canvas Brutalist when:**

- You want a cleaner, lighter, more open feel
- The content is dense and needs maximum clarity
- Printing or PDF output is primary use case
- Target audience expects traditional document aesthetics
- Long-form reading is the primary use case
- You want to feel more “architectural” and “design studio”

**Use Block Brutalist when:**

- You want a more dramatic, tech-forward aesthetic
- The platform is digital-first (web apps, developer tools)
- You want to signal innovation and cutting-edge work
- Reducing eye strain in dark environments is important
- You want to feel more “builder” and “hacker culture”

**Both work for:**

- Technical documentation
- Product marketing
- Portfolio sites
- SaaS platforms
- Editorial content

-----

## Design Philosophy

Canvas represents the same brutalist principles as Block, but inverted for light. It’s not just “light mode” - it’s a deliberate aesthetic choice that communicates:

- Precision and clarity
- Architectural thinking
- Designer/creative culture
- Confidence that doesn’t need darkness to be sophisticated
- Openness and accessibility

The design says: “We value substance and clarity. Clean canvas, clear purpose.”

Like a blank page waiting for purposeful content, Canvas provides structure without interference. The white space isn’t empty - it’s intentional, functional, and part of the design language.