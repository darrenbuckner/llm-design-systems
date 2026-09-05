---
id: light-bevel-messenger-053
title: Bevel Messenger System
description: A skeuomorphic desktop-chrome system built from tan dialog faces, glossy blue title bars, and two-pixel bevels that draw depth without a single blur.
tags: [light, retro, warm, gradient, skeuomorphic, forms, productivity]
colors: ["#ECE9D7", "#015BEE", "#FFFFFF", "#C41200", "#ACA899"]
created: 2026-09-04
---

# Bevel Messenger System

Bevel Messenger System is a skeuomorphic desktop-chrome language built from tan dialog faces, glossy blue title bars, and two-pixel bevels that draw depth without a single blur. Nothing is rounded and nothing floats: raised surfaces take a white top-left edge and a grey bottom-right, sunken wells invert exactly the same two pixels, and every level of hierarchy is communicated by which direction the light falls. It is built for dense utility interfaces — message clients, contact lists, form panels, tool palettes — where the chrome is meant to be read as physical hardware rather than as a surface that gets out of the way.

The system's defining split is that chrome and content use different type entirely. Every control, label, menu, and tab is set in an 11px humanist sans; every word a person actually reads is set in a 16px serif on white. The two never mix, and collapsing them into one family is the single fastest way to destroy the aesthetic.

## Color Palette

**Page Surface:** `#ECE9D7` — the dialog face. Every window body, toolbar, panel, tab strip, and status bar sits on this warm tan. It is the ground, not an accent.

**Primary Colors:**
- Caption Deep `#0231D4` — the top stop of the active title bar gradient and the resting fill of primary buttons
- Caption Mid `#015BEE` — the dominant blue; the middle two-thirds of the caption gradient
- Caption Light `#2A80F8` — the lower stop, where the gradient lifts back toward the glass highlight
- Caption Sheen `#7BB0F7` — a single-pixel highlight line inset one pixel below the top of the title bar
- Caption Inactive `#7E9CE8` — the flat, desaturated title bar of an unfocused window
- Caption Ink `#FFFFFF` — title text, always bold, always with a one-pixel `rgba(0,0,0,0.35)` offset shadow

**Neutral Colors:**
- Content Well `#FFFFFF` — the inside of every sunken field, transcript area, and list body
- Chrome Tint `#F5F2E1` — the upper band of a toolbar and the hover fill of a flat button
- Sheen `#FFFCEA` — the one-pixel highlight along the top edge of any raised band
- Bevel Light `#FFFFFF` — top and left edge of a raised element; bottom and right of a sunken one
- Bevel Shadow `#ACA899` — bottom and right edge of a raised element; top and left of a sunken one
- Bevel Dark `#716F64` — the outer ring on a heavily raised control, used only on the action-bar buttons
- Etch Groove `#C9C7BB` — the dark half of a one-pixel etched divider, paired with `#FFFFFF` below it
- Field Border `#7F9DB9` — the cool blue-grey hairline around a sunken white well
- Ink `#000000` — all primary text, chrome and content alike
- Ink Muted `#545454` — secondary labels, timestamps, disabled-adjacent metadata
- Ink Disabled `#ACA899` — greyed menu items and inactive button labels

**Accent/State Colors:**
- Speaker A / Alert `#C41200` — the first participant's name, error text, destructive labels
- Speaker B / Info `#0135DB` — the second participant's name, informational badges
- Hyperlink `#0000EE` — always underlined, never restyled
- Success `#2F6B12` — sent confirmations, online indicators
- Warning `#8A6100` — away states, unsaved changes
- Selection Fill `#316AC5` with `#FFFFFF` ink — the highlight on a selected list row or open menu item

## Typography

**Display & Headings:** Tahoma, 11px, weight 700 — the same face and size as body chrome, distinguished only by weight. This system has no display type.

**Font Families:**
- Chrome: `Tahoma, Verdana, "DejaVu Sans", Geneva, sans-serif` — a humanist sans with a large x-height that stays legible at 11px
- Content: `"Times New Roman", Tinos, "Liberation Serif", Times, serif` — the transitional serif every message, note, and body paragraph is set in

**Type Scale:**
- Caption / title bar — 11px / 700 / 1.0 / `#FFFFFF` with a 1px dark offset shadow
- Menu item — 11px / 400 / 1.2 / `#000000`
- Button label — 11px / 400 / 1.2, centered under its icon
- Group header — 11px / 700 / 1.2, often with a count in `#545454` after it
- List row — 11px / 400 / 1.45
- Status text — 11px / 400 / 1.2 / `#545454`
- Content body — 16px / 400 / 1.5 serif on `#FFFFFF`
- Speaker name — 16px / 700 / 1.5 serif, in the participant's accent color, followed by a colon and a single space

**Hierarchy Rules:** Weight and color carry the entire hierarchy; size almost never does. Chrome type is fixed at 11px everywhere and is never scaled up for emphasis — a heading is bold 11px, not 14px. The 16px serif is reserved for text a person reads in sequence, and no chrome label is ever set in it. Nothing is centered except a button label under its icon and the caption text on a dialog. Sentence case throughout; no uppercase tracking, no letter-spacing adjustments at any level.

## Spacing System

**Base Unit:** 2px. Bevels are 1–2px, so every other measurement is a multiple of the bevel to keep edges aligned to the same grid.

**Scale:** 2 / 4 / 6 / 8 / 12 / 16 / 24 / 32 / 48

**Common Patterns:**
- Window body padding: 6px on all sides
- Title bar height: 26px, with 4px of inset before the caption text
- Menu bar height: 20px, items padded 4px 8px
- Toolbar height: 26px, padded 2px 4px, buttons 22px square
- Sunken field padding: 4px 6px; the field's own border sits outside that
- Gap between sibling controls: 4px; between control groups: 8px with an etched divider between
- Icon action-bar button: 52px wide on desktop, 44px minimum on touch, 4px 6px padding, icon over label with a 2px gap
- List row height: 20px, 4px 6px padding, 16px indent per tree level
- Page gutter: 16px mobile, 24px at 768px and above

## Component Styles

### Window Frame

The outermost container. `background: #ECE9D7`, a 3px blue frame in `#0231D4` on the left, right, and bottom, and `border-radius: 6px 6px 0 0` — the only rounded corners the system permits. The drop shadow is hard, never blurred: `box-shadow: 3px 3px 0 rgba(0, 0, 0, 0.25)`. An inactive window keeps the identical geometry and swaps the frame and caption to `#7E9CE8`.

### Title Bar

26px tall, `linear-gradient(180deg, #0231D4 0%, #015BEE 18%, #015BEE 72%, #2A80F8 100%)`, with a one-pixel `#7BB0F7` line inset at 2px from the top to read as glass. Caption text is 11px bold white with a 1px `rgba(0,0,0,0.35)` shadow, inset 8px. Caption buttons sit at the right: 16×14px, 2px radius, 1px `rgba(255,255,255,0.5)` inner top edge. Minimize and maximize fill `#2A62D0`, lifting to `#3A70DE` on hover; close fills a warmer `#C33B2B`, lifting to `#CB4131`. Every one of those four holds at least 4.5:1 against the white glyph — the caption button is the smallest text in the system and the easiest place to ship an unreadable one. Every caption button is a square with a glyph, never an icon font, never a circle.

### Menu Bar

20px tall, flush to the title bar with no gap, on the plain `#ECE9D7` face. Items are 11px, padded 4px 8px, with the first letter underlined for a mnemonic. Resting state has no border at all. On hover the item takes the `#316AC5` selection fill with white ink and squared corners — no radius, no transition longer than 0ms, because a menu highlight in this system snaps.

### Bevel Buttons

The core primitive. Three states, each drawn entirely with two pixels of border:

- **Raised (resting):** `background: #ECE9D7`, `border-top` and `border-left` `2px solid #FFFFFF`, `border-bottom` and `border-right` `2px solid #ACA899`, `border-radius: 0`
- **Hover:** the face lifts to `#F5F2E1`; the bevel does not change
- **Pressed:** the two border pairs swap — light moves to bottom-right, shadow to top-left — and the label shifts 1px down and 1px right, so the button visibly sinks
- **Focus:** a 1px dotted `#000000` outline inset 3px, drawn inside the bevel, never a glow or a ring
- **Disabled:** face stays `#ECE9D7`, label goes `#ACA899` with a 1px `#FFFFFF` offset shadow to read as engraved

A default button adds a 1px `#0231D4` ring outside the bevel. Buttons are 22px tall for toolbar use and 24px for dialog use, with 12px horizontal padding, and they never grow to fill their container.

### Sunken Fields & Wells

Any surface that receives input or holds scrolling content: `background: #FFFFFF`, `border: 1px solid #7F9DB9`, plus an inner `box-shadow: inset 1px 1px 0 #ACA899` to complete the recess. `border-radius: 0`. Padding is 4px 6px. On focus, the border darkens to `#0231D4` and nothing else changes — no ring, no shadow, no color wash. A transcript well is the same construction at a larger size, holding 16px serif content rather than an input.

### Toolbar Strip

A 26px band on `#ECE9D7` carrying a `#FFFCEA` one-pixel sheen along its top edge and a `#C9C7BB` hairline along its bottom. Buttons inside it are 22px square and start **flat** — no bevel at all — acquiring the raised bevel only on hover and the pressed bevel on click. This flat-until-hover behavior is what keeps a row of twelve controls from reading as twelve boxes. Groups are separated by an etched vertical groove: a 1px `#C9C7BB` line with a 1px `#FFFFFF` line immediately right of it, 16px tall, with 4px of space either side.

### Icon Action Bar

The heavy row of labelled icon buttons that anchors the bottom of a window. Each button is a 32×32 icon over an 11px centered label, 52px wide minimum, on the `#ECE9D7` face with no resting border. Hover raises it with the standard 2px bevel plus an outer 1px `#716F64` ring — the only place `Bevel Dark` appears. The primary action in the row (send, submit, commit) is distinguished by a 3px `#2F6B12` underline beneath its label, not by a colored fill.

### Tree List & Group Headers

Rows are 20px tall on `#FFFFFF` inside a sunken well. A group header is bold 11px with a 9×9px expander to its left: a 1px `#716F64` square containing a `+` or `−` glyph, not a chevron or a triangle. Children indent 16px per level with no connector lines. Selection fills the full row width with `#316AC5` and white ink; hover does nothing at all, because in this system hover is reserved for controls and selection is reserved for content.

### Tabs & Status Bar

Tabs dock to the **bottom** of a panel, not the top. Each is 20px tall with `border-radius: 0 0 4px 4px`, the raised bevel on its left, right, and bottom edges, and no top edge at all. The active tab fills `#ECE9D7` and sits 1px taller than its siblings; inactive tabs fill `#D8D5CA` and sit flush. A status bar is a 20px band with the sunken bevel inverted to shallow — 1px `#ACA899` on top, 1px `#FFFFFF` below — holding 11px `#545454` text, segmented by the same etched grooves the toolbar uses.

## Layout Principles

Everything is a rectangle inside a rectangle. Panels butt directly against each other with a 1px etched divider between them and no gap, no gutter, and no shadow separating them — negative space is not a structural device in this system, edges are. Content is left-aligned and top-aligned without exception outside of button labels.

The measure for serif content is 66–72 characters, achieved by the well's width rather than by a `max-width` on the text. Layout is fixed-position in spirit: a window has a title bar, an optional menu, an optional toolbar, one or two wells, and an action bar, in that order, top to bottom.

On mobile the window frame collapses to full-bleed — the 3px blue frame and the rounded top corners drop away, the title bar spans edge to edge, and the action bar becomes a horizontally scrolling row with 44px targets. Multi-panel layouts stack to a single column; the tab strip stays docked at the bottom of whichever panel is showing. The only thing that changes on desktop is that panels sit side by side and the window regains its frame.

## Visual Effects

**Radii:** 0 everywhere, with exactly three exceptions — 6px on the top two corners of a window frame, 4px on the bottom two corners of a tab, and 2px on a caption button.

**Elevation:** there is no shadow system. Depth is drawn with two pixels of border, light against dark, and the direction of that light is the entire vocabulary: light top-left means raised, light bottom-right means sunken. The one blur-free exception is the window's own `3px 3px 0` hard offset shadow.

**Gradients:** exactly one, on the active title bar. Nothing else in the system takes a gradient — not buttons, not toolbars, not headers. The `#FFFCEA` sheen line and the `#F5F2E1` toolbar tint do the work a gradient would do elsewhere.

**Borders:** 1px for hairlines and field borders, 2px for bevels, 3px for the window frame. Nothing else exists.

**Transitions:** 0ms on everything. This interface snaps. A hover state that fades in reads as a modern web page immediately and undoes the whole system. The only permitted animation is a 100ms step on a progress indicator.

## Design Tone

Physical, dense, and unapologetically utilitarian — an interface that behaves like a machine with edges rather than a surface that gets out of the way. The warm tan face and glossy blue caption give it a domestic, slightly nostalgic warmth that keeps the density from reading as severe, and the serif content well makes the words a person actually reads feel like a letter sitting inside a tool. It is confident about being a program: every control announces itself, nothing hides until hover except the toolbar, and the hierarchy is legible from six feet away because it is drawn in light and shadow rather than in whitespace.

## Usage Notes for AI Implementation

1. **Never round anything.** Three exceptions exist and they are enumerated in Visual Effects. A `border-radius: 8px` on a card or a button is the single change that turns this system into a generic 2015 web page, and it is the mistake that will be made first.

2. **Never add a blurred shadow.** If an element needs to sit above another, give it the two-pixel raised bevel. If it needs to recede, invert the same two pixels. Reaching for `box-shadow: 0 2px 8px rgba(0,0,0,0.1)` is the second-fastest way to destroy the aesthetic.

3. **Keep the two type families strictly separated.** Chrome is 11px sans; content is 16px serif on white. Setting message text in the sans makes it look like a settings panel, and setting a button label in the serif makes it look like a Word document. There is no third face and no italic display type.

4. **Do not scale chrome type for emphasis.** A section heading is bold 11px. If something needs to be more prominent, add weight, add the selection fill, or give it a bevel — never add points.

5. **Toolbar buttons start flat, dialog buttons start raised.** This distinction is doing real work: a strip of twelve flat controls reads as one band, and twelve raised ones read as visual noise. Apply the bevel on hover for toolbars, at rest for dialogs and action bars.

6. **Set every transition to 0ms.** Snap is a property of this system, not an oversight. One 150ms ease on a hover fill is enough to make the whole page read as a modern site wearing retro colors.

7. **The tan is the ground, not an accent.** `#ECE9D7` should cover most of the visible area. If the page is mostly white with tan cards on it, the system is inverted — white belongs inside sunken wells only, and a white surface without a `#7F9DB9` border and an inset bevel is wrong.

8. **Use color to identify, not to decorate.** Red and blue mark *who is speaking* or *what state a thing is in*. There is no brand accent to sprinkle around, and a colored button fill does not exist outside the caption buttons — the primary action in an action bar is marked by a green underline under its label instead.

9. **Etched grooves separate; whitespace does not.** When two groups of controls need separation, put a 1px `#C9C7BB` line with a 1px `#FFFFFF` line beside it between them. Adding 24px of air instead produces something that looks like this system's colors applied to a different system's structure.

10. **Tabs dock to the bottom and expanders are square.** These two details read as arbitrary and are the ones that make the system recognizable. A chevron expander or a top-docked tab strip is a correct implementation of the wrong system.
