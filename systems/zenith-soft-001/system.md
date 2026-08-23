# Zenith Soft Design System

## Visual Style

Empathetic minimalism - soft neutral background (warm off-white #F5F3F0 or cool light gray #F0F0F2), deep black text (#000000 or #1A1A1A), gentle contrast. Calming, centered, human-focused aesthetic.

## Typography

**Typeface:**

- Serif for body text and headlines (Georgia, Crimson Text, Lora, or similar elegant serif)
- Sans-serif for UI elements and labels (SF Pro, Inter, or system fonts)
- Body text: serif, line-height 1.6-1.8 (extra generous for readability)
- UI elements: clean sans-serif

**Hierarchy:**

- Greetings/small headers: Sans-serif, regular weight (~14-16px)
- Main body/quotes: Serif, regular weight (~18-22px)
- Headlines: Serif, medium weight (~28-36px)
- Button text: Sans-serif, medium weight (~16-18px)
- Generous line spacing for calm, unhurried reading

## Color Palette

- Background: Warm off-white (#F5F3F0) or cool light gray (#F0F0F2)
- Text: Deep black (#000000) or near-black (#1A1A1A)
- Borders: Thin black lines (1px) - subtle, not harsh
- Accents: None needed - relies on typography and space
- Optional: Very subtle warm tones for backgrounds (beige, cream)

## Layout Systems

### Single Column (Primary Pattern)

- Center-aligned content (this is the key difference from Canvas/Block)
- Maximum content width: 600-700px for optimal readability
- Generous side margins that grow with viewport
- 50-70px vertical spacing between sections
- Content feels like it’s floating in calm space

### Multi-Column (Rare, Secondary)

- Use sparingly - only for structured data or feature comparisons
- When used: 2-3 columns maximum
- Maintain centered overall layout
- Column content can be center-aligned within columns
- Generous gutters (32-40px)

### Layout Principles

- **Center stage**: Content centered horizontally on page
- **Vertical flow**: Single column reading experience
- **Breathing room**: Wide margins create sense of calm
- **No crowding**: Never push content to edges
- **Symmetry**: Balanced, harmonious composition

### Responsive Behavior

- **Desktop:** Centered column with wide side margins
- **Tablet:** Slightly narrower margins, same centered approach
- **Mobile:** Reduced side padding (20-24px) but maintain centered feel

## Spacing Scale

Generous spacing units based on 8px grid:

- **S:** 16px
- **M:** 24px
- **L:** 32px
- **XL:** 48px
- **XXL:** 64px
- **Section gaps:** 70-90px
- **Paragraph spacing:** 24-32px (more than typical)

## Components

### Buttons

- Pill shape - fully rounded ends (border-radius: 999px or 50%)
- Outline style with thin black border (1-2px)
- White/off-white background (same as page or slightly different)
- No fill color, clean and minimal
- Generous padding (14-18px vertical, 32-48px horizontal)
- Full-width on mobile, auto-width on desktop
- Center-aligned text
- Hover: subtle background shift or slight shadow (very soft)
- Stacked vertically with consistent spacing (16-20px between)

### Cards (Minimal Use)

- Subtle background if needed (slightly different shade of off-white)
- Rounded corners (16-24px) - soft, not sharp
- Thin border (1px) optional
- Internal padding: 32-40px
- Center-aligned content within cards
- Avoid harsh edges or stark contrasts

### Headers/Navigation

- Minimal and unobtrusive
- Logo/branding left-aligned
- Menu/actions right-aligned or center-aligned
- Thin bottom border (1px) optional
- Ample padding (20-24px vertical)
- Can use sans-serif for navigation items

### Greetings/Micro-copy

- Small, friendly sans-serif text
- “Hi, [Name]!” pattern - personal and warm
- Positioned above main content
- Can be center-aligned or left-aligned within centered container

### Content Blocks

- Main message/quote: Large serif text, center-aligned
- Generous padding around text blocks
- Line length optimized for readability (45-75 characters)
- Paragraph breaks for breathing room

### Icons (Minimal Use)

- Simple, line-based when needed
- Geometric but soft (rounded line ends)
- Used sparingly - let typography lead
- Brand icon can have more detail/personality

## Content Patterns

### Welcome/Daily Message Pattern

```
[Greeting: "Hi, Name!"]

[Main message/quote: Large serif, center-aligned, 
generous line height, comfortable reading width]

[Action buttons: Stacked, pill-shaped, equal width]
```

### Feature/Section Pattern

```
[Section title: Serif, centered]

[Description: Serif, centered, comfortable width]

[Optional CTA: Pill button, centered]
```

### List Pattern (when needed)

```
[Section title]

[Items stacked vertically with generous spacing]
[Each item can be a pill button or simple text]
```

## Content Density Rules

- **Always generous** - never cramped
- **One primary message** per screen
- **Limited choices** - 2-4 options maximum per screen
- **White space is calming** - embrace emptiness
- **Slow down the user** - unhurried, contemplative pace

## Alignment Principles

- **Primary content:** Center-aligned
- **Paragraphs:** Center-aligned (exception to typical left-align rule)
- **Buttons:** Center-aligned, full or auto width
- **Navigation:** Left/right alignment acceptable
- **Overall composition:** Symmetrical and balanced

## Design Principles

1. **Empathetic design** - Feels like a friend, not a tool
1. **Calm and unhurried** - No urgency, no pressure
1. **Centered focus** - One thing at a time
1. **Generous spacing** - Room to breathe and think
1. **Serif warmth** - Human, approachable, thoughtful
1. **Soft edges** - Pill buttons, rounded corners, gentle borders
1. **Minimal choices** - Reduce cognitive load

## What NOT to Do

- ❌ No harsh angles or sharp corners on interactive elements
- ❌ No bright or saturated colors
- ❌ No high-contrast stark designs
- ❌ No cluttered layouts or dense information
- ❌ No aggressive CTAs or urgent language
- ❌ No multiple columns of body text
- ❌ No left-aligned paragraphs (center them)
- ❌ No small margins - always generous
- ❌ No cold, technical aesthetics

## Tone & Voice

Warm, empathetic, personal. Like a thoughtful friend or gentle coach. Uses “you” and “your” frequently. Speaks to the inner self. Encouraging without being pushy. Contemplative, not urgent.

-----

## AI Prompting Templates

### For Web Design (HTML/React):

```
Create a [page type] using Zenith Soft aesthetic:

Style:
- Warm off-white background (#F5F3F0), deep black text (#1A1A1A)
- Serif typography for main content (Georgia, Crimson, Lora)
- Sans-serif for UI elements and small labels
- Line-height 1.6-1.8 for body text
- Pill-shaped buttons (fully rounded, border-radius: 999px)
- Thin borders (1px black)

Layout:
- Center-aligned single column
- Maximum content width: 600-700px
- Wide side margins that grow with viewport
- 50-70px vertical spacing between sections
- Content centered on page

Components:
- Buttons stacked vertically, full or auto width
- Center-aligned text in main content areas
- Generous padding everywhere (never cramped)
- Soft, rounded corners (16-24px) where needed

Tone:
- Warm, personal greeting ("Hi, [Name]!")
- Empathetic, unhurried copy
- One primary message per screen
```

### For Mobile Apps:

```
Design a [screen type] with Zenith Soft aesthetic:

- Warm neutral background (#F5F3F0)
- Serif for main message/content
- Sans-serif for buttons and small labels
- Center-aligned layout
- Generous vertical spacing (50-70px sections)
- Pill buttons stacked vertically (16-20px apart)
- Personal greeting at top
- Maximum 2-4 action options per screen
- Calm, contemplative pace
```

### For Content/Editorial:

```
Format this [content type] in Zenith Soft style:

- Serif typography (Georgia, Crimson, or Lora)
- Center-aligned text
- Line-height 1.7-1.8
- Generous paragraph spacing (24-32px)
- Maximum 600px reading width
- Warm off-white background
- Deep black text for optimal readability
- Personal, empathetic tone
- One key message or theme per section
```

### For Wellness/Reflection Apps:

```
Create a [feature screen] using Zenith Soft aesthetic:

Style:
- Warm, calming color palette (off-white backgrounds)
- Serif for quotes, messages, reflections
- Sans-serif for navigation and buttons
- Pill-shaped buttons (fully rounded)
- Generous spacing throughout

Layout:
- Center-aligned single column
- 600-700px max content width
- Wide margins for breathing room
- 70-90px between major sections

Content:
- Personal greeting ("Hi, [Name]!")
- One primary message or prompt
- 2-4 action options maximum
- Encouraging, non-urgent tone
- Room for reflection and pause
```

-----

## Quick Review Checklist

Before finalizing any design:

- ☐ Is background a warm/soft neutral (not stark white)?
- ☐ Is main content in serif typeface?
- ☐ Are buttons pill-shaped (fully rounded)?
- ☐ Is content center-aligned?
- ☐ Is there generous spacing (50-70px+ between sections)?
- ☐ Is the max content width 600-700px?
- ☐ Are there 2-4 options maximum per screen?
- ☐ Is the tone warm and personal?
- ☐ Does it feel calm and unhurried?
- ☐ Are there wide side margins?
- ☐ Is line-height generous (1.6-1.8)?
- ☐ Does it feel empathetic, not mechanical?

-----

## Implementation Notes

### For HTML/CSS:

```css
body {
  background: #F5F3F0;
  color: #1A1A1A;
  font-family: Georgia, 'Crimson Text', serif;
  line-height: 1.7;
}

.container {
  max-width: 650px;
  margin: 0 auto;
  padding: 0 24px;
  text-align: center;
}

.button {
  border: 1px solid #000;
  border-radius: 999px;
  background: transparent;
  padding: 16px 40px;
  font-family: -apple-system, sans-serif;
  display: block;
  width: 100%;
  max-width: 400px;
  margin: 16px auto;
}

h1, h2, .message {
  font-family: Georgia, serif;
  text-align: center;
  max-width: 600px;
  margin: 0 auto;
}

.greeting {
  font-family: -apple-system, sans-serif;
  font-size: 15px;
  text-align: center;
  margin-bottom: 48px;
}
```

### For Tailwind:

```
Container: max-w-2xl mx-auto px-6 text-center
Background: bg-stone-50 or bg-gray-50
Text: text-gray-900
Buttons: rounded-full border border-black px-10 py-4 w-full
Spacing: space-y-16 or space-y-20 for sections
Typography: Font family requires custom config for serif
```

### For React Native / Mobile:

```jsx
<View style={{
  flex: 1,
  backgroundColor: '#F5F3F0',
  paddingHorizontal: 24,
  alignItems: 'center'
}}>
  <Text style={{
    fontFamily: 'Georgia',
    fontSize: 20,
    lineHeight: 32,
    textAlign: 'center',
    maxWidth: 600
  }}>
    Content here
  </Text>
  
  <TouchableOpacity style={{
    borderRadius: 999,
    borderWidth: 1,
    borderColor: '#000',
    paddingVertical: 16,
    paddingHorizontal: 40,
    marginTop: 16,
    width: '100%'
  }}>
    <Text style={{
      fontFamily: 'System',
      textAlign: 'center'
    }}>
      Button Text
    </Text>
  </TouchableOpacity>
</View>
```

### For Design Tools (Figma/Sketch):

- Background: #F5F3F0 (warm) or #F0F0F2 (cool)
- Text: #1A1A1A
- Set up center-aligned artboard constraint
- Max content frame: 650px wide
- Use Georgia or similar serif for body text
- Buttons: Shape with 999px or 50% border radius
- Create component library with consistent spacing
- Set up 8px grid
- Use auto-layout with center alignment

-----

## When to Use Zenith Soft

**Use Zenith Soft when:**

- Building wellness, meditation, or mental health apps
- Creating journaling or reflection tools
- Designing coaching or personal development platforms
- Need to convey empathy and warmth
- Content is contemplative or philosophical
- Reducing anxiety and urgency is important
- One primary action per screen is sufficient
- Building for mindfulness or intentional living

**Don’t use Zenith Soft when:**

- Need to display dense data or dashboards
- Multiple actions/choices required per screen
- Building technical or developer tools
- Speed and efficiency are primary goals
- Professional/corporate aesthetic is required
- Content is action-oriented rather than reflective

**Similar to:**

- Calm, Headspace, Day One (journaling apps)
- Wellness and mental health platforms
- Personal development tools
- Mindfulness applications

-----

## Design Philosophy

Zenith Soft represents a human-centered, empathetic approach to digital design. Unlike the confident, builder-focused aesthetics of Block and Canvas, Zenith prioritizes emotional connection and inner reflection.

Key philosophical differences:

- **Centered vs. Flush Left**: Centering creates intimacy and focus
- **Serif vs. Sans-Serif**: Serif brings warmth and humanity
- **Soft vs. Sharp**: Pill buttons and rounded corners feel gentle
- **Space as Calm**: Generous spacing slows the user down intentionally
- **Few Choices**: Reduced cognitive load through simplicity

The design says: “Take your time. We’re here to support you, not rush you. Your inner world matters.”

This isn’t minimalism for aesthetics—it’s minimalism for mental space. Every design choice reduces anxiety and creates room for reflection.