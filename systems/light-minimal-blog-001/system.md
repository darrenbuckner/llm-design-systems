---
id: light-minimal-blog-001
title: Parchment Editorial System
tags: [light, minimal, editorial, cards, modern, long-form]
colors: ["#FFFFFF", "#F5F5F5", "#8B5CF6", "#333333", "#666666"]
created: 2026-01-23
---

# Parchment Editorial System

A white-ground reading system built on a three-step grey text ladder, where a single violet marks every link and action and nothing else in the interface carries color. Restrained, shadowless, and built around a long reading measure. Suited to blogs, documentation, newsletters, personal sites, and any long-form surface where the writing is the product.

## Color Palette

**Page Surface:** `#FFFFFF` — pure white, the ground for every screen. This is one of the few systems where a pure white ground is correct rather than lazy: with no shadows and a single accent, the page needs the maximum available contrast for its text ladder to read.

**Primary Colors:**
- Violet `#8B5CF6` — the only accent. Links, primary button fill, active navigation, and the focus ring. It appears in prose as a link and nowhere else in prose.
- Violet Deep `#7C3AED` — hover and active state for every Violet fill or link. Never a resting color.

**Neutral Colors:**
- Surface `#F5F5F5` — the secondary surface: pull quotes, code blocks, sample cards, and tag fills. The only fill besides white.
- Hairline `#E5E5E5` — the border on every card, input, and divider. One weight, one color.

**Text — the three-step ladder:**
- Primary `#333333` — body copy and headings. A soft near-black; pure black against pure white is too harsh for sustained reading, and that softening is a deliberate reading-comfort decision.
- Secondary `#666666` — bylines, captions, descriptions, tag labels.
- Tertiary `#999999` — timestamps, metadata, placeholder text, and any line the reader can safely skip.

**Accent/State Colors:**
- Warm `#E8D5C4` — a muted sand used only as an illustration or thumbnail placeholder tone. Never a fill, a border, or type.
- Error `#B3352B` — message text and a 1px border on the offending input.
- Focus Ring `#8B5CF6` at 2px offset 2px.

## Typography

**Display & Headings:** a single humanist sans across the whole interface, differentiated by weight and size. Google Fonts equivalent: `Inter`, weights 400/500/600/700. Fallback: `'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif`. The system deliberately reads in a sans rather than a serif — it is built for screen-native writing, not for imitating print.

**Code:** a monospaced face for inline code and code blocks. Google Fonts equivalent: `JetBrains Mono`, weight 400. Fallback: `'JetBrains Mono', 'SF Mono', Monaco, monospace`.

**Type Scale:**
- Post title — 40px / 700 / 1.20 / -0.02em
- Section heading — 28px / 600 / 1.30 / -0.01em
- Subheading — 20px / 600 / 1.40 / 0
- Lead paragraph — 20px / 400 / 1.65 / 0
- Body — 17px / 400 / 1.75 / 0
- Inline code (mono) — 15px / 400 / 1.60 / 0
- Button and input — 16px / 500 / 1.00 / 0
- Byline and caption — 15px / 400 / 1.50 / 0, set in Secondary
- Timestamp and tag — 14px / 400 / 1.40 / 0, set in Tertiary

**Hierarchy Rules:** Body copy runs at 17px with a 1.75 line-height — both larger and looser than a typical interface, because this system is read continuously rather than scanned. The measure is capped at 68 characters. Hierarchy is weight and size against a fixed three-step grey ladder; color is never used for emphasis, because violet already means "this is a link" and a violet heading would invite a click. Bold inside body copy is 600 in Primary, never a color change. Nothing is italic except a genuine citation.

## Spacing System

**Base Unit:** 4px.

**Scale:** 4, 8, 12, 16, 24, 32, 48, 64, 96.

**Common Patterns:**
- Page gutter 24px; reading measure capped at 680px, index and listing views at 1120px.
- Paragraph to paragraph: 24px.
- Heading to its first paragraph: 12px. Paragraph to the next heading: 48px — the asymmetry is what binds a heading to the text beneath it.
- Section to section: 64px.
- Card padding 24px. Card to card: 24px.
- Button padding 12px 20px. Input padding 12px 16px, 12px between stacked fields.
- Pull quote and code block: 24px padding, 32px above and below.

**Gutter ownership:** one element owns the horizontal gutter and nothing else sets horizontal padding on it. Vertical rhythm uses longhand `padding-top` / `padding-bottom` rather than a `padding: 64px 0` shorthand on that element, which would win on source order and zero the gutter.

## Component Styles

### Buttons

**Primary** — fill `#8B5CF6`, label `#FFFFFF` at 16px/500, 6px radius, padding 12px 20px, no border, no shadow. Hover: fill `#7C3AED`.

**Ghost** — transparent fill, 1px `#8B5CF6` border, label `#8B5CF6`, same radius and padding. Hover: fill `#8B5CF6`, label `#FFFFFF`. The pair is deliberately the only two button styles — there is no neutral or grey button, because a reading interface should present at most one or two actions at a time.

### Cards

Fill `#F5F5F5`, 1px `#E5E5E5` border, 8px radius, 24px padding, **no shadow**. Used for post previews in an index, related-reading blocks, and sample content. Hover on an interactive card darkens the border to `#D5D5D5`; nothing lifts or moves.

### Post Preview

A card containing an optional thumbnail in the Warm placeholder tone, then a 20px/600 title in Primary, then a 15px description in Secondary capped at two lines, then a 14px timestamp in Tertiary. The title is the only link target in the card.

### Input Fields

Fill `#FFFFFF`, 1px `#E5E5E5` border, 6px radius, padding 12px 16px, 16px in Primary. Placeholder in Tertiary. Focus: border `#8B5CF6` plus a 2px violet ring at 2px offset. Invalid: 1px `#B3352B` border with the message beneath at 14px in the same red.

### Links

Violet with no underline at rest inside navigation and metadata; **underlined at rest inside body copy**, because an unmarked color change is not sufficient signal in a long passage. Hover: `#7C3AED`, underline persists. Visited links are not styled differently — the system has one link color.

### Pull Quotes and Code Blocks

Fill `#F5F5F5`, no border, 8px radius, 24px padding, 32px of clearance above and below. A pull quote is 20px/400 in Primary with a 15px attribution in Secondary beneath. A code block is 15px monospaced in Primary and scrolls horizontally within its own box rather than widening the page.

### Tags

Fill `#F5F5F5`, no border, 6px radius, padding 6px 12px, 14px/400 in Secondary. As a filter, the selected state fills `#8B5CF6` with white type.

### Dividers

1px `#E5E5E5` at the reading measure, not the full page width. A rule that runs wider than the text it separates reads as a section break rather than a paragraph break.

## Layout Principles

A single centered column. Reading views cap at 680px; index and listing views widen to 1120px with a two- or three-across card grid that collapses to one column below 600px. The header is a simple wordmark-left, links-right bar with no fill and no border, and it does not become sticky — a fixed bar steals vertical space from the thing the reader came for. Images inside a post run to the reading measure rather than full-bleed, keeping the white ground as continuous margin. Below 600px the gutter holds at 24px and body copy drops to 16px/1.7.

## Visual Effects

No shadows anywhere. Separation is the 1px hairline plus the step from `#FFFFFF` to `#F5F5F5`. Radii: 8px on cards, quotes, and code blocks; 6px on buttons, inputs, and tags. Borders are always 1px `#E5E5E5`. No gradients, no glass, no texture, no blur. Transitions are 150ms ease on background-color, border-color, and color only.

## Design Tone

Quiet and unfussy, with just enough personality to not read as a template. The violet is the single note of character in an otherwise neutral page, and holding it to links and actions is what keeps a long article feeling like writing rather than an interface. It gets out of the way.

## Usage Notes for AI Implementation

1. **Violet means "clickable" and nothing else.** Links, buttons, active navigation, focus rings. A violet heading or a violet accent bar invites a click that is not there and destroys the one signal the system has.

2. **Body text is `#333333`, not black.** Pure black on pure white is harsh over a long read. The soft near-black is a reading-comfort decision, not an accident, and it anchors the three-step grey ladder.

3. **Keep body at 17px / 1.75 with a 68-character measure.** All three numbers are set for continuous reading rather than scanning. Tightening any of them to fit more above the fold makes the system worse at its only job.

4. **Body links are underlined at rest.** Color alone is not enough signal inside a paragraph. Navigation and metadata links may drop the underline; prose links may not.

5. **The heading gap is asymmetric.** 12px above the text a heading introduces, 48px below the text it follows. Equalizing them detaches every heading from its section.

6. **No shadows and only two fills.** White and `#F5F5F5`, separated by a 1px hairline. A shadow on a `#F5F5F5` card is nearly invisible on white anyway, so reaching for one means the tonal step is being used wrong.

7. **There are only two buttons.** Violet fill and violet ghost. Adding a neutral grey button gives a reading interface three competing actions, which is two too many.

8. **The warm sand tone is a placeholder only.** `#E8D5C4` stands in for imagery. It is never a fill, a border, a tag, or type — it exists so an image-less card is not an empty grey box.

9. **Dividers run to the measure, not the page.** A full-width rule under a 680px column reads as a section break and cuts the article into pieces.

10. **The header does not stick.** A fixed bar permanently occupies the top of a reading view. If persistent navigation is genuinely required, use a compact bar that hides on scroll down and returns on scroll up.
