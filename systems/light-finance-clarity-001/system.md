---
id: light-finance-clarity-001
title: Evergreen Ledger
description: Clean, trustworthy light interface with emerald green accents, progress indicators, and organized card-based layouts for financial clarity
tags: [light, minimal, professional, card-based, mobile-first, data-visualization]
colors: ["#1A1A1A", "#C4203C", "#1E7D4D", "#F7F7F7", "#FFFFFF"]
created: 2026-01-12
---

# Evergreen Ledger

A clean, trustworthy design system emphasizing financial clarity through organized card-based layouts, emerald green accents for positive states and progress, and a warm crimson gradient header that grounds the interface. The system balances professional restraint with approachable softness, using generous white space, clear typographic hierarchy, and intuitive progress visualizations to make complex financial data feel manageable.

## Color Palette

**Primary Colors:**
- Header Gradient Start: #C4203C — Rich crimson, used as primary brand anchor in header
- Header Gradient End: #8B1A2E — Deeper burgundy for gradient depth
- Action Green: #1E7D4D — Emerald green for toggles, progress bars, positive states, and confirmations

**Neutral Colors:**
- Background: #F7F7F7 — Warm light gray, primary canvas
- Surface/Cards: #FFFFFF — Pure white for elevated cards and content areas
- Text Primary: #1A1A1A — Near-black for maximum readability on headings and amounts
- Text Secondary: #5C5C5C — Medium-dark gray for body text and descriptions
- Text Tertiary: #8A8A8A — Medium gray for labels, timestamps, and metadata
- Text Muted: #ABABAB — Light gray for disabled states and subtle hints
- Borders: #E8E8E8 — Subtle warm gray for card borders and dividers
- Dividers: #F0F0F0 — Very light gray for section separators within cards

**Accent/Category Colors:**
- Wants Category: #F5E6A3 — Soft yellow for discretionary spending icons
- Needs Category: #C8E6C9 — Soft green for essential expenses icons
- Savings Category: #B3E5FC — Soft blue for savings goals icons
- Alert/Review Border: #C4203C — Crimson for attention-requiring card borders

**Progress Bar Colors:**
- Progress Fill (Great/Good): #1E7D4D — Emerald green
- Progress Track: #E0E0E0 — Light gray unfilled track
- Progress Track Alt: #D0D0D0 — Slightly darker for utilization context

**State Colors:**
- Success/Good: #1E7D4D — Emerald green
- Warning: #F5A623 — Amber orange
- Error/Poor: #C4203C — Crimson red
- Pending: #8A8A8A — Gray for pending states
- Toggle Off: #D1D1D1 — Muted gray for inactive toggles

**Badge Colors:**
- Good Badge Background: #1E7D4D
- Good Badge Text: #FFFFFF
- Rating Badge Background: #F5A623 — Orange/amber for letter grades
- Rating Badge Text: #FFFFFF

## Typography

**Font Families:**
- Primary: SF Pro Display / -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
- Secondary: SF Pro Text for body and smaller text
- Fallback: System UI stack for cross-platform consistency

**Type Scale:**
- Page Title: 28px, 700 weight, line-height 1.2, letter-spacing -0.5px — "Card Usage"
- Page Subtitle: 17px, 600 weight, line-height 1.3 — "Customize Dashboard"
- Section Header: 18px, 700 weight, line-height 1.3 — "Instant Insights", "Dashboard Cards"
- Card Title: 16px, 600 weight, line-height 1.3 — "Summary"
- Body Large: 15px, 400 weight, line-height 1.5 — Descriptive paragraphs
- Card Label: 15px, 400 weight, line-height 1.4 — Item names in settings lists
- Data Label: 13px, 400 weight, line-height 1.2 — "Total Balance", "Total Limit"
- Data Value Large: 20px, 700 weight, line-height 1.2 — "$12,575", "$59,100"
- Data Value Medium: 17px, 600 weight, line-height 1.2 — "$8,335 Balance"
- Percentage Large: 18px, 600 weight, line-height 1.2 — "21%", "28%"
- Category Label: 13px, 600 weight, line-height 1.2, letter-spacing 0.5px, uppercase — "MY WATCHLIST", "USAGE BY ACCOUNT"
- Status Label: 12px, 600 weight, line-height 1.2, uppercase — "CURRENT STATUS"
- Amount Small: 14px, 400 weight, line-height 1.3 — "$0"
- Caption: 12px, 400 weight, line-height 1.4 — "this month", "as of 3 days ago"
- Tab Label: 10px, 500 weight, line-height 1.2 — Bottom navigation labels
- Scale Labels: 12px, 400 weight — "Great", "Good", "Fair", "Poor"

**Hierarchy Rules:**
- Section headers use all-caps with letter-spacing: 0.5px for category labels
- Primary amounts are bold (700), secondary supporting text is regular (400)
- High contrast (near-black on white) for all critical financial data
- Bold inline text for emphasis within sentences: "You have **3 open credit card accounts**"
- Percentage values right-aligned in data rows

## Spacing System

**Base Unit:** 4px
**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64

**Common Patterns:**
- Page horizontal padding: 16px
- Card internal padding: 20px (large cards), 16px (compact cards)
- Card gap (between cards): 12px
- Section spacing (between groups): 24px
- Section header margin-bottom: 16px
- List item vertical padding: 16px
- List item horizontal padding: 20px
- Icon to text spacing: 12px
- Data row spacing: 16px between label and value stacks
- Progress bar height: 8px
- Progress bar margin: 12px vertical
- Bottom navigation height: 64px + safe area
- Back arrow top padding: 16px

**Grid System:**
- 2-column grid for watchlist cards on mobile
- 3-column layout for data values (Balance | Limit | Usage)
- Gap between grid items: 12px
- Full-width cards for list items and detailed views
- 16px horizontal page margins

## Component Styles

### Toggle Switch
- Track width: 51px
- Track height: 31px
- Thumb diameter: 27px
- Active state: #1E7D4D background, white thumb
- Inactive state: #D1D1D1 background, white thumb
- Border radius: 16px (fully rounded)
- Transition: 200ms ease-out

### Progress Bar (Horizontal)
- Height: 8px
- Border radius: 4px (fully rounded)
- Track color: #E0E0E0
- Fill color: #1E7D4D (for good/great states)
- Fill animation: 300ms ease-out on load

### Utilization Scale Bar
- Height: 8px
- Border radius: 4px
- Segmented background showing ranges
- Active segment: #1E7D4D
- Inactive segments: Gradient from #E0E0E0 to #D0D0D0
- Scale labels below: "Great", "Good", "Fair", "Poor"
- Label spacing: Evenly distributed, 12px below bar

### Rating Badge (Circular)
- Diameter: 32px
- Background: #F5A623 (amber/orange)
- Text: White, 16px, 700 weight
- Border radius: 50%
- Used for letter grades (A, B, C, etc.)

### Status Badge (Pill)
- Padding: 6px 16px
- Background: #1E7D4D (for "Good")
- Text: White, 13px, 600 weight
- Border radius: 16px (fully rounded)

### Cards (Overview Style)
- Background: #FFFFFF
- Border: none (shadow-based elevation)
- Border radius: 16px
- Shadow: 0 2px 8px rgba(0,0,0,0.06)
- Padding: 20px
- Contains: Title, description, data grid, progress visualization

### Cards (List Item Style)
- Background: #FFFFFF
- Border: none
- Border radius: 12px
- Shadow: 0 1px 3px rgba(0,0,0,0.05)
- Padding: 16px 20px
- Separator: 1px solid #F0F0F0 between items within same card

### Cards (Account Row Style)
- Background: #FFFFFF
- Border radius: 12px (on container)
- Internal rows separated by 1px #F0F0F0 divider
- Row padding: 16px 20px
- Icon: 40px × 40px, #F5F5F5 background, rounded 8px
- Progress bar inline below account name

### Cards (Watchlist Style)
- Background: #FFFFFF
- Border: none (shadow-based elevation)
- Border radius: 12px
- Shadow: 0 1px 3px rgba(0,0,0,0.08)
- Padding: 16px
- Icon container: 40px × 40px, rounded to 20px
- Icon background colors: Category-specific pastels
- More menu: Three-dot icon, top-right

### Transaction Row
- Background: #FFFFFF
- Avatar: 40px × 40px circle with category icon or merchant initial
- Primary text: 15px, 600 weight (merchant name)
- Secondary text: 13px, 400 weight, #8A8A8A (date | status)
- Amount: 15px, 600 weight, right-aligned
- Vertical padding: 14px

### Alert Card
- Background: #FFFFFF
- Border: 2px solid #C4203C
- Border radius: 12px
- Icon container: 40px × 40px, #E3F2FD background, rounded 8px
- Chevron: #666666, right-aligned
- Padding: 16px

### Summary Card
- Background: #FFFFFF
- Border radius: 16px
- Shadow: 0 2px 8px rgba(0,0,0,0.06)
- Header: Icon + Title + Status Badge (right-aligned)
- Content: Status indicator dot + Label + Description
- Status dot: 8px diameter, #1E7D4D for good status
- Padding: 20px

### Bottom Navigation
- Background: #FFFFFF
- Height: 64px (excluding safe area)
- Active icon/text: #C4203C
- Inactive icon/text: #1A1A1A
- Icon size: 24px
- Label size: 10px
- Item spacing: Equal distribution across 5 items
- Border-top: 1px solid #E8E8E8

### Header Bar (Gradient)
- Background: Linear gradient 180deg from #C4203C to #8B1A2E
- Height: 96px (including status bar area)
- Text color: #FFFFFF
- Icon color: #FFFFFF (settings gear, notification bell)
- Date display: 17px, 500 weight, centered

### Header Bar (Simple)
- Background: #FFFFFF or #F7F7F7
- Back arrow: 24px, #1A1A1A
- Title area below back arrow
- Rating badge inline with "Rating" label

### Section Label
- Text: All caps, 13px, 600 weight
- Color: #1A1A1A
- Letter-spacing: 0.5px
- Margin-bottom: 16px
- Optional right action: "Edit" link in same styling

### Credit Card Icon
- Container: 40px × 40px
- Background: #F5F5F5
- Border radius: 8px
- Icon: Simple card outline, 20px, #666666

### Usage Box (Highlighted Metric)
- Border: 1px solid #E0E0E0
- Border radius: 8px
- Padding: 8px 12px
- Background: transparent
- Used to highlight key metric like "Usage 21%"

## Layout Principles

- **Max content width:** Full device width on mobile, 428px max on larger screens
- **Grid structure:** 2-column for watchlist cards, 3-column for data summaries, single column for lists
- **Responsive behavior:** Stacks to single column below 320px, maintains proportions on tablet
- **Alignment:** Left-aligned text, amounts and percentages right-aligned
- **Safe areas:** Respects iOS safe area insets for notch and home indicator
- **Vertical rhythm:** Consistent 24px between major sections, 12px between related cards
- **Data hierarchy:** Label above value pattern for financial metrics

## Visual Effects

**Border Radius:**
- Large cards: 16px
- Standard cards: 12px
- Buttons/inputs: 8px
- Toggle tracks: 16px (fully rounded)
- Progress bars: 4px (fully rounded)
- Badges (pill): 16px (fully rounded)
- Badges (circular): 50%
- Icons/Avatars: 50% (circular) or 8-10px (rounded square)

**Shadows:**
- Card elevation: 0 2px 8px rgba(0,0,0,0.06)
- Subtle elevation: 0 1px 3px rgba(0,0,0,0.05)
- No heavy shadows — light, airy feel throughout

**Borders:**
- List dividers: 1px solid #F0F0F0 (inside cards)
- Section dividers: 1px solid #E8E8E8
- Alert emphasis: 2px solid #C4203C
- Default cards: No border, shadow only
- Bottom nav: 1px solid #E8E8E8 top border
- Metric highlight box: 1px solid #E0E0E0

**Backgrounds:**
- Page background: Solid #F7F7F7
- Header: Linear gradient (dashboard) or solid white (detail pages)
- Cards: Solid white #FFFFFF
- Icon containers: #F5F5F5 or category-specific pastels at 100% opacity
- Progress track: #E0E0E0

**Status Indicators:**
- Dot indicator: 8px circle, filled with status color
- Positioned left of status label text

## Data Visualization Patterns

### Utilization Meter
- Horizontal bar showing current usage vs. total capacity
- Fill width proportional to percentage
- Color indicates health: Green for good, transitions toward red for poor
- Scale markers below: "Great" (0-10%), "Good" (10-30%), "Fair" (30-50%), "Poor" (50%+)

### Account Progress Rows
- Account name + percentage on same line
- Progress bar below name
- Balance (left) and Limit (right) below progress bar
- Compact format for scanning multiple accounts

### Summary Statistics
- 3-column layout: Balance | Limit | Usage
- Label above, value below
- Usage highlighted in bordered box when it's the key metric

## Design Tone

This system conveys trustworthiness and financial confidence through its clean, organized appearance. The warm crimson header adds brand personality on the main dashboard while detail pages use a simpler white header for focus. The emerald green accent color appears consistently across toggles, progress bars, and positive status indicators — creating a clear visual language where green equals good. 

The overall aesthetic is approachable yet professional — avoiding the coldness of pure white interfaces while maintaining the clarity essential for financial data. Card-based organization with generous padding creates clear information hierarchy, making users feel in control of their finances. Progress visualizations and percentage displays provide at-a-glance understanding of financial health.

## Usage Notes for AI Implementation

When implementing this system:

1. **Header gradients** should only appear on the main dashboard; detail/drill-down pages use simple white headers with back arrows
2. **Toggle switches** are the primary interactive pattern for settings — use the exact green (#1E7D4D) for active states
3. **Progress bars** always use the same green fill color regardless of the percentage — the scale below indicates the health interpretation
4. **Category colors** (yellow/green/blue pastels) should only appear in icon containers, never as text or borders
5. **Maintain high contrast** for all financial amounts — these are the most critical data points
6. **Alert cards** with crimson borders should be used sparingly for items requiring immediate attention
7. **Bottom navigation** should show the active state with crimson color on both icon and label
8. **List items** with drag handles indicate reorderable content
9. **Use system fonts** (SF Pro) for native feel on iOS, fall back to Inter/system-ui on other platforms
10. **Spacing is generous** — don't compress elements; the breathing room conveys trustworthiness
11. **Status badges** use pill shape with status color background and white text
12. **Rating badges** use circular shape with amber background for letter grades
13. **Data labels** are always lighter (#8A8A8A) positioned above bold values
14. **Percentage values** right-align in data rows for easy scanning
15. **Account rows** within a card use subtle dividers (#F0F0F0), not gaps between separate cards
