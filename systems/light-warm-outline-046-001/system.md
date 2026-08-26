---
id: light-warm-outline-046
title: Buttermilk Outline System
description: A warm two-mode system where marketing surfaces sit on butter cream with heavy ink-outlined cards and product surfaces switch to warm gray chrome with soft tonal panels, sharing one ink and one serif.
tags: [light, warm, playful, cards, serif, modern]
colors: ["#FFFFED", "#F6F6E5", "#1A1A1A", "#ECD8FC", "#EE7556"]
created: 2026-08-26
---

# Buttermilk Outline System

A warm, faintly yellow system that runs in two surface modes from a single palette. **Marketing mode** sits on butter cream, gives cards a heavy near-black outline, and admits hand-drawn illustration in coral, amber, and blush. **Product mode** switches the ground to warm gray chrome with a near-white content panel, drops the outline to a soft warm border, and retires the illustration accents entirely in favor of tiny category markers. Both modes share the same ink, the same serif reserved for titles, the same sans for everything else, and the same generous radii. Suited to products that need a playful front door and a calm workspace behind it without looking like two different companies.

## Color Palette

**Page Surface:** `#FFFFED` — the marketing ground, a pale butter cream with an unmistakable yellow cast. In product mode the ground becomes `#F5F4F1`; both are grounds, and the mode determines which one is in play.

**Primary Colors:**
- Ink `#1A1A1A` — all display type, headings, labels, the solid marketing button fill, and the 2px card outline in marketing mode. A near-black, never pure `#000000`.
- Ink Secondary `#4D4A43` — supporting lines in product mode, warmer than the primary ink.
- Muted `#5C5C56` — body copy on marketing surfaces and secondary metadata everywhere. A warm gray with a green cast that ties it to the butter ground.
- Faint `#A6A4A0` — placeholder text, timestamps, disabled labels.

**Neutral Colors — marketing mode:**
- Butter `#FFFFED` — page ground.
- Bone `#F6F6E5` — card fill, one half-step deeper than the ground. The only card fill in this mode.

**Neutral Colors — product mode:**
- Chrome `#F5F4F1` — app ground, sidebar, and title bar.
- Paper `#FCFCFB` — the content panel and any input field. The near-white that content sits on.
- Tan `#F0EBE2` — raised and selected surfaces: the detail rail card, hovered and selected list rows.
- Border `#EEEBE4` — the 2px separator between chrome and panel, and the fill for an active navigation item.

**Accent/State Colors:**
- Lilac `#ECD8FC` — plan and tier badges only, with Ink on top. The only chromatic fill permitted in product mode.
- Coral `#EE7556`, Amber `#F3AD5A`, Blush `#F5BFEF` — illustration only, in marketing mode only. Never a fill, a button, a border, or a text color anywhere in the interface.
- Marker Red `#C3291C` and Marker Blue `#4599DF` — 4px category bars on list rows, and nothing else. They carry a user's own color assignment, not a system state.
- Focus Ring `#1A1A1A` at 2px offset 2px, identical in both modes.

## Typography

**Display & Headings:** a high-contrast serif with sharp wedge serifs and small teardrop terminals, used only at display sizes. Google Fonts equivalent: `Instrument Serif`, weight 400 plus 400 italic. Fallback: `'Instrument Serif', 'Times New Roman', Georgia, serif`.

**Body & UI:** a geometric sans with a high x-height, generous apertures, and rounded terminals, for every other piece of type in both modes. Google Fonts equivalent: `DM Sans`, weights 400/500/700. Fallback: `'DM Sans', 'Inter', -apple-system, sans-serif`.

**Type Scale:**
- Marketing headline (serif) — 46px / 400 / 1.10 / 0
- Screen title (serif) — 34px / 400 / 1.15 / 0
- Object title (serif) — 28px / 400 / 1.20 / 0
- Marketing body (sans) — 18px / 400 / 1.50 / 0, set in Muted
- Section label (sans) — 13px / 700 / 1.2 / 0.08em, uppercase, set in Muted
- Row title (sans) — 17px / 500 / 1.40 / 0
- Navigation label (sans) — 16px / 500 / 1.40 / 0
- Body (sans) — 15px / 400 / 1.55 / 0
- Button label (sans) — 15px / 700 / 1.20 / 0
- Metadata (sans) — 14px / 400 / 1.45 / 0, set in Muted or Faint
- Badge (sans) — 13px / 700 / 1.2 / 0

**Hierarchy Rules:** The serif is reserved for exactly three things — the marketing headline, the screen title, and the name of the single object currently in focus. It never sets a list row, a navigation label, a button, or body copy, which is why the interface can stay dense while still feeling authored. Sans handles everything else at 400/500/700, with 500 doing most of the work in the product UI. The uppercase letterspaced section label is the only all-caps type in the system and appears only above a grouped list. Body copy on marketing surfaces is Muted rather than Ink and is centered inside the card; everything in product mode is left-aligned and Ink.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80.

**Common Patterns:**
- Marketing card: 48px padding, centered contents, roughly 520px wide, vertically centered in the viewport.
- Marketing stack: check glyph, 32px, headline, 24px, body, 40px, button.
- Product chrome: 12px of chrome visible around the content panel on the top and right, with the sidebar occupying the left.
- Sidebar: 208px wide, 12px horizontal padding, nav rows 40px tall with 12px between icon and label, 4px between rows.
- Content panel: 32px padding, 24px between the title row and the first content block.
- List rows: 64px tall, 16px internal padding, 8px between rows, 12px between the marker bar and the avatar.
- Detail rail: 320px wide, 24px card padding, 24px gap from the content column.
- Grouped list: 12px between the section label and its first row, 32px between groups.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm is applied with `padding-top` and `padding-bottom` longhand, never a `padding: 56px 0` shorthand, because a shorthand on a class sharing that element wins on source order and silently zeroes the gutter, flushing content to the viewport edge on mobile.

## Component Styles

### Cards — Marketing Mode

Fill `#F6F6E5` on the Butter ground, **2px `#1A1A1A` outline**, 24px radius, 48px padding, no shadow. The heavy ink outline is the signature of this mode and the reason the card reads as drawn rather than rendered. Contents center: a 56px circled check glyph in Ink at 2px stroke, the serif headline, two lines of Muted body, then a full-width button.

### Cards — Product Mode

Fill `#F0EBE2`, **no border**, 20px radius, 24px padding, no shadow. Product cards never take the ink outline — the tonal step from Paper to Tan is the whole separation mechanism. Contents left-align: serif object title, Muted metadata line, then a single button.

### Buttons

**Solid (marketing)** — fill `#1A1A1A`, label `#FFFFFF` at 15px/700, 8px radius, 18px 24px padding, full width of the card. Hover: `#302D36`. The only place a solid dark button appears.

**Quiet (product)** — fill `#FCFCFB`, 1px `#EEEBE4` border, label `#1A1A1A`, 10px radius, 12px 20px padding, optional 18px leading icon. Hover: fill `#F0EBE2`. This is the default button inside the app; product mode has no dark button at all.

**Ghost** — no fill, no border, label `#4D4A43`, 10px radius. Hover: fill `#EEEBE4`. Used for header actions and overflow controls.

### Navigation

A 208px sidebar on the Chrome ground with no right border — the content panel's own border provides the edge. Rows are a 20px line icon at 1.75px stroke plus a 16px/500 label, 40px tall, 10px radius. Resting label Ink, icon Ink Secondary. Hover: fill `#EEEBE4` at 50%. Active: fill `#EEEBE4` with icon promoted to Ink. No left accent bar, no bold weight change, no color. A hairline `#EEEBE4` divider separates the primary group from the account group pinned to the bottom.

### Content Panel

Fill `#FCFCFB`, 2px `#EEEBE4` border, 24px radius, inset 12px from the top and right edges of the Chrome ground so the chrome frames it on those sides. This inset frame is what makes product mode read as an application rather than a page.

### List Rows

Fill `#F1EDE4` when active or hovered, transparent at rest, 12px radius, 64px tall. A 4px full-height marker bar in Marker Red or Marker Blue sits flush at the left inside edge, then a 36px circular avatar, then a 17px/500 title with a 14px Muted metadata line beneath. Rows carry no border and no divider; the 8px gap and the fill do the separating.

### Section Labels

A 20px line icon, then 13px/700 uppercase at 0.08em letterspacing in Muted, with the group's pagination and refresh controls pushed right as ghost buttons. Sits above a group of list rows with no rule beneath it.

### Inputs

Fill `#FCFCFB`, 1px `#EEEBE4` border, fully rounded (`border-radius: 999px`) for search and prompt fields, 10px radius for multi-line fields. 16px/400 text, placeholder in Faint, 16px 24px padding. Focus: border `#1A1A1A` plus a 2px Ink ring at 2px offset.

### Badges

Fill `#ECD8FC`, label `#1A1A1A` at 13px/700, pill radius, 4px 12px padding. Tier and plan only. Never a count, never a status, never any other color.

### Tabs

16px/500 labels in Muted with 24px between them, the active tab in Ink with a 2px Ink underline sitting on a full-width 1px `#EEEBE4` rule. No pill, no fill, no capsule.

### Illustration

Loose hand-drawn line work in Ink at 2.5px stroke with flat fills in Coral, Amber, and Blush, positioned to overlap and break the edge of a marketing card rather than sit inside it or beside it. The overlap is what makes the card read as drawn, so the illustration is anchored to the card's own bounding box, not to the section. Background line work is the same drawing at 3% opacity, scaled up and bled off two edges of the viewport. Illustration never appears in product mode.

## Layout Principles

Marketing mode is a single centered card in an otherwise empty viewport, with the wordmark at top center and illustration breaking the card's top-right corner. Nothing scrolls; the composition is meant to be seen whole.

Product mode is a fixed 208px sidebar, a fluid content column, and a 320px detail rail that appears only when an object is selected and collapses below 1200px, pushing the object's card to the top of the content column instead. The content panel is inset from the chrome on the top and right but runs flush to the bottom. Below 900px the sidebar becomes an off-canvas drawer and the content panel loses its inset, running full-bleed with the border removed.

## Visual Effects

No shadows in either mode. Radii are large and consistent: 24px on the marketing card and content panel, 20px on product cards, 12px on list rows, 10px on nav rows and quiet buttons, 8px on the solid button, 999px on badges and search fields. Border weight is the mode tell — 2px `#1A1A1A` in marketing, 2px `#EEEBE4` or none in product, with 1px `#EEEBE4` on small controls. No gradients, no glass, no texture, no blur. Transitions are 140ms ease on background-color, border-color, and color only.

## Design Tone

Warm and slightly handmade without being twee. The butter ground and the drawn ink outline give the marketing surface a sticker-like friendliness, while the product surface trades that for a quiet warm gray calm that can hold a dense list all day. The serif appearing on object titles inside an otherwise plain interface is what keeps the two halves recognizably the same product.

## Usage Notes for AI Implementation

1. **Pick a mode and stay in it.** Butter ground plus ink-outlined cards, or Chrome ground plus soft-bordered panels. Mixing them — an ink-outlined card inside the app, a warm gray panel on the marketing page — is the fastest way to lose the system. The palette is shared; the border weight and the ground are not.

2. **The 2px ink outline is marketing-only.** It is the single most recognizable thing about the front door and the single most wrong thing to put in the product UI, where separation comes from the Paper-to-Tan tonal step instead.

3. **The serif is for three things only:** the marketing headline, the screen title, and the name of the object currently in focus. Setting a list row, nav label, or button in the serif immediately makes the interface look like a magazine instead of a tool.

4. **Illustration colors never touch the UI.** Coral, amber, and blush exist inside the drawing and nowhere else — not as a button, a badge, a border, a chart series, or a link. If a marketing surface needs a colored element that is not illustration, it does not get one.

5. **Product mode has no dark button.** The solid `#1A1A1A` button belongs to the marketing card. Inside the app the primary action is the quiet Paper button with a hairline border, which is why the lilac badge and the marker bars read as the only color.

6. **Marker bars carry user color, not system state.** Red and blue on a list row mean "this belongs to that calendar or category," never error or info. Do not add a green success bar or reuse them for validation.

7. **No shadows anywhere, in either mode.** Elevation is expressed by the ink outline in marketing and by the tonal ladder in product. Adding a shadow to the content panel or a product card flattens both modes at once.

8. **Keep the panel inset asymmetric.** The content panel is inset from the top and right of the chrome and runs flush to the bottom. Insetting it evenly on all four sides makes it look like a floating modal rather than an application surface.

9. **One lilac badge per screen.** Tier only, top of the sidebar, next to the wordmark. A second lilac element anywhere breaks the rule that product mode carries exactly one chromatic fill.

10. **Anchor the illustration to the card, not the section.** It must overlap and break the card's corner. Positioning it against the section instead leaves it floating in empty ground beside the card, which loses the drawn, stuck-on quality entirely.
