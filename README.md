# Agent Design Systems

**112 production-grade design systems, written in Markdown that any Agent can actually implement. ** ****

AI coding tools are good at structure and bad at taste. Ask for a dashboard, and you get the same centered card on a slate-50 background every time. These systems fix that — each one is a complete, opinionated specification (palette with semantic roles, type scale, spacing, component geometry, interaction states, and the rules that keep it from collapsing into a template) that you hand to Claude, Cursor, or Codex before it writes a line of UI.

Free, MIT, no signup.

---

## 30 seconds to useful

Browse the index, pick a system, hand your agent the URL:

```bash
# see everything, one line per system
curl -s https://www.capabilitylab.ai/library/design-systems/llm-index.md \
  | grep '^## '
```

Then, in Claude Code / Cursor / Codex:

> Build the settings page using this design system:
> https://www.capabilitylab.ai/library/design-systems/systems/light-warm-editorial-041-001/system.md

That's the whole product. Everything below is convenience on top of it.

## Install as a skill

Drop `skills/design-systems/SKILL.md` into your agent's skills directory, and it will search the library, match a system to whatever mood you describe, and apply it — no URLs to copy.

```bash
git clone https://github.com/darrenbuckner/llm-design-systems
cp -r llm-design-systems/skills/design-systems ~/.claude/skills/
```

Works with any agent that reads the `SKILL.md` convention.

## What's in a system

Each `systems/{id}/system.md` is 4–8KB covering:

| | |
|---|---|
| **Color** | Every hex with its semantic role — page ground, surface tints, text at each emphasis level, borders at each weight, accent, states |
| **Typography** | Families with real Google Fonts equivalents, the full size/weight/line-height scale, and the hierarchy rules |
| **Spacing** | Base unit, scale, and the patterns that recur — gutters, section rhythm, component padding |
| **Components** | Buttons, cards, inputs, chips, lists, dividers — geometry and interaction states specified precisely |
| **Effects** | Radii by element type, elevation system or its deliberate absence, transition timing |
| **Usage notes** | The enforceable rules that keep the system from degrading when applied |

That last section is the part that matters. "Never add shadows — step the background one tone deeper instead" is worth more to a model than another hex code.

## Browsing

Every system has a live preview page showing its palette, type scale, and components rendered in its own aesthetic:

**https://www.capabilitylab.ai/library/design-systems**

The previews stay hosted rather than checked in, so this repo stays text-only and can be cloned in a second.

## Finding the right one

```bash
# pull full entries matching a mood, category, or tag
curl -s https://www.capabilitylab.ai/library/design-systems/llm-index.md \
  | awk 'BEGIN{RS="---";ORS="---\n"} /brutalist/'
```

Searching the prose beats filtering on tags — descriptions and design-tone text carry nuance that the tags flatten. Tags run through a controlled vocabulary (`tag-vocabulary.json`) to ensure consistent spelling, but they're a coarse filter, not the index.

57 light, 55 dark. Heaviest tags: `minimal` (67), `warm` (38), `professional` (26), `editorial` (23), `gradient` (22), `premium` (23).

## Where these come from

Each system is extracted from a real interface and then fully anonymized — no brand names, no product references, no identifying content. What's captured is the visual grammar: proportions, palette relationships, typographic rules, component geometry. Names and placeholder copy are invented.

The point is a library of production-grade aesthetics that already work, not a way to clone anyone's product.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Corrections to existing systems are especially welcome — if a spec doesn't reproduce cleanly when an agent implements it, that's a bug worth filing.

## Staying current

New systems get added regularly. If you'd rather not poll the repo:

**https://www.capabilitylab.ai** — an occasional email when systems land, plus what's working in AI-native building.

## License

MIT. Use them commercially, modify them, ship them. Attribution appreciated, not required.
