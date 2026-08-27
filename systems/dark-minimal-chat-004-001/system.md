---
id: dark-minimal-chat-004-001
title: Void Platform Design System
tags: [dark, minimal, technical, chat, high-contrast, mono]
colors: ["#000000", "#1a1a1a", "#2a2a2a", "#00ff88", "#ffffff"]
created: 2026-01-21
---

# Void Platform Design System

A pure-black conversational interface built as a four-step grey ladder, where every surface is a lift in value rather than a change in hue and the only color in the entire system is a single signal green on a 8px status dot. Monospaced throughout for message content, sans for chrome. Suited to developer tools, AI chat interfaces, terminals with a UI layer, logs, and anything where the content is text the user reads closely at length.

## Color Palette

**Page Surface:** `#000000` — pure black, the ground for the entire interface. Not a near-black: the ladder above it is tightly spaced, so it needs the floor to be as low as possible to keep four steps distinguishable.

**Neutral Colors — the ladder:**
The system's entire structural vocabulary, in order of elevation. Each step is a container nested inside the one below it.
- Step 0 `#000000` — page ground
- Step 1 `#1a1a1a` — message bubbles, tags, swatch cards. The surface content sits on.
- Step 2 `#2a2a2a` — inputs and default buttons. The surface the user *operates*.
- Step 3 `#333333` — borders, dividers, and the primary button fill
- Step 4 `#4a4a4a` — the highest lift; hover states and selected rows

Step 2 being reserved for interactive surfaces is the rule that makes the interface readable: if it is lighter than a message bubble, you can click or type in it.

**Text Colors:**
- Primary `#ffffff` — message content, headings, input values, button labels.
- Secondary `#cccccc` — supporting lines, tag labels, sender names.
- Muted `#666666` — timestamps, placeholder text, disabled labels, metadata. On pure black this is the floor for legible text; nothing dimmer is used.

**Accent/State Colors:**
- Signal `#00ff88` — the only chromatic value in the system. Used exclusively as an 8px round status dot for online, connected, or streaming. Never type, never a fill, never a border.
- Error `#ff5f56` — message text and a 1px border on the offending input.
- Focus Ring `#ffffff` at 2px offset 2px — white rather than Signal, so focus never reads as a status.

## Typography

**Display & Headings:** a neutral sans for interface chrome — headings, buttons, labels, tags, and navigation. Google Fonts equivalent: `Inter`, weights 400/500/600. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`.

**Message & Code:** a monospaced face for all message content, code, timestamps, and any value the user might copy. Google Fonts equivalent: `JetBrains Mono`, weights 400/500. Fallback: `'JetBrains Mono', 'SF Mono', Monaco, 'Cascadia Code', monospace`.

**Type Scale:**
- Page title (sans) — 28px / 600 / 1.25 / -0.01em
- Section heading (sans) — 20px / 600 / 1.35 / 0
- Message body (mono) — 15px / 400 / 1.65 / 0
- Input (mono) — 14px / 400 / 1.50 / 0
- Body (sans) — 15px / 400 / 1.60 / 0, set in Secondary
- Button and label (sans) — 14px / 500 / 1.00 / 0
- Sender name (sans) — 14px / 500 / 1.40 / 0, set in Secondary
- Tag (sans) — 12px / 500 / 1.30 / 0, set in Secondary
- Timestamp (mono) — 12px / 400 / 1.30 / 0, set in Muted

**Hierarchy Rules:** Mono carries content, sans carries chrome — if the user could plausibly copy it, it is monospaced. Message body runs at a generous 1.65 line-height because long monospaced passages on pure black tire the eye faster than proportional text on paper. There is no bold body text: emphasis inside a message is handled by the mono face itself, and bolding monospace on black smears at small sizes. Nothing is italic or all-caps.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 20, 24, 32, 48, 64.

**Common Patterns:**
- Page gutter 24px; conversation measure capped at 720px, full interface at 1120px.
- Message bubble padding 16px 20px, capped at 400px wide, with 12px between consecutive bubbles.
- 24px between speaker turns — double the within-turn gap, which is what groups a run of messages visually.
- Input padding 12px 20px. Button padding 12px 20px.
- Card and swatch padding 20px.
- Section to section: 48px.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses longhand `padding-top` / `padding-bottom` rather than a `padding: 48px 0` shorthand on that element, which would win on source order and zero the gutter.

## Component Styles

### Message Bubbles

Fill `#1a1a1a`, **8px radius**, padding 16px 20px, `max-width: 400px`, no border and no shadow. Content is 15px monospaced in Primary; a 12px monospaced timestamp in Muted sits beneath with 8px of space. Bubbles are never tinted by speaker — the sender is identified by a 14px name line above the run, not by color. An assistant bubble and a user bubble are the same fill; only alignment and the name differ.

### Inputs

Fill `#2a2a2a`, 1px transparent border, **24px radius** (a full pill), padding 12px 20px, 14px monospaced in Primary. Placeholder in Muted. Focus: border `#4a4a4a`, fill unchanged, plus a 2px white ring at 2px offset. The pill radius is what distinguishes the composer from every rectangular surface around it. Invalid: 1px `#ff5f56` border.

### Buttons

**Default** — fill `#2a2a2a`, label `#ffffff` at 14px/500, 6px radius, padding 12px 20px, no border. Hover: fill `#4a4a4a`.

**Primary** — fill `#333333`, otherwise identical. The primary button is one step up the ladder rather than a different color, which is unusual and deliberate: in a reading interface a saturated button pulls the eye off the text.

**Ghost** — no fill, label `#cccccc`. Hover: fill `#1a1a1a`, label `#ffffff`.

### Status Dot

An 8px circle filled `#00ff88`, with 8px of space before the label it annotates. This is the entire chromatic budget of the system. A dot may also be `#666666` for offline, but never any other color — there is no amber warning state.

### Tags

Fill `#1a1a1a`, no border, `border-radius: 24px`, padding 6px 12px, 12px/500 in Secondary. Non-interactive at rest; a selected filter lifts the fill to `#333333`.

### Cards and Swatches

Fill `#1a1a1a`, 8px radius, 20px padding, no border. Where a card needs to be distinguished from a bubble in the same view, it takes a 1px `#333333` border rather than a different fill — the ladder is too tight to spend another step.

### Dividers

1px `#333333` at full container width. Never doubled, never inset.

## Layout Principles

A conversation column capped at 720px, centered, on a black page that runs full-bleed behind it. The composer is pinned to the bottom of the viewport with the message list scrolling above it, and the page itself never scrolls horizontally. Supporting interface — settings, model pickers, history — lives in a wider 1120px well using the same ladder. Messages are left-aligned as a column with sender names above each run; the system does not use the two-sided left/right chat convention, because right-aligned monospaced text loses the ragged edge that makes a run of messages scannable. Below 600px the conversation measure becomes the full gutter width and bubble max-width is removed.

## Visual Effects

No shadows anywhere — elevation is the ladder and nothing else. Radii: 24px pill on inputs and tags, 8px on bubbles and cards, 6px on buttons, 50% on status dots. Borders are 1px `#333333` and used sparingly, only where two surfaces on the same ladder step must be distinguished. No gradients, no glass, no texture, no blur. Transitions are 120ms ease on background-color and border-color only; a reading interface should not animate while text is arriving.

## Design Tone

Quiet, technical, and content-first. The tight grey ladder and the single green dot give it the feel of a well-configured terminal rather than a consumer chat product, and the monospaced message body signals that the text is the artifact — something to be read, copied, and trusted rather than skimmed.

## Usage Notes for AI Implementation

1. **Never tint message bubbles by speaker.** Both sides use `#1a1a1a`. The sender is identified by a name line and by alignment. Coloring the user's bubble is the single fastest way to turn this into a generic consumer chat app.

2. **Step 2 means interactive.** `#2a2a2a` is reserved for inputs and buttons. If a non-interactive surface takes Step 2, the interface loses the only cue telling the user what they can operate.

3. **Green is one 8px dot.** Signal `#00ff88` is a status indicator and nothing else — never text, never a fill, never a border, never a button. A green button here would be the brightest thing on a pure-black page by an enormous margin.

4. **Mono for content, sans for chrome.** If the user could copy it, it is monospaced. Message bodies, code, timestamps, IDs. Headings, buttons, labels, and tags are sans.

5. **The primary button is a ladder step, not a color.** `#333333`, one rung above the default button. Introducing a saturated primary pulls the eye off the text the interface exists to display.

6. **Keep message line-height at 1.65.** Long monospaced passages on pure black are harder on the eye than proportional text on paper. Tightening to 1.4 to fit more on screen makes the interface materially worse to read.

7. **No bold body text.** Bolded monospace on black smears at 15px. Emphasis inside a message is the mono face and the line break, not weight.

8. **Focus rings are white.** Signal green already means status; a green focus ring makes a focused field look connected rather than active.

9. **Double the gap between speaker turns.** 12px within a run, 24px between runs. That 2:1 ratio is what groups messages without needing a container or a divider.

10. **No shadows — the ladder is the elevation.** Five steps from `#000000` to `#4a4a4a` do all the work. A shadow on pure black is invisible anyway, so reaching for one means the ladder is being used wrong.
