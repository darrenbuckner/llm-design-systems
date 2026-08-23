# Contributing

## The most useful contribution

**Report a system that doesn't reproduce.** Hand a `system.md` to your agent, build something with it, and if the result doesn't look like the preview, open an issue saying which system and what drifted. A spec that reads well but implements badly is the failure mode that matters here, and it's hard to catch without people building real things.

Include the system ID, the agent you used, and what came out wrong.

## Corrections

Wrong hex, missing state, contradictory rule, a spec that says one thing and the preview shows another — open an issue or a PR. Small fixes don't need discussion first.

## Proposing a new system

Systems are extracted from real interfaces and then anonymized, and that pipeline runs upstream of this repo — so new systems aren't merged here directly. Open an issue describing the aesthetic you want covered and what's missing from the current 111. Gaps in coverage are genuinely useful to know about.

If you're proposing one from a specific interface, describe the visual grammar rather than linking the product. What matters is the palette relationships, type rules, and component geometry, not the brand.

## Things that will be declined

- Systems containing brand names, real product names, logos, or identifying copy. Everything here is anonymized, without exception.
- Additions that are minor variations on an existing system. 111 systems is already enough that the marginal near-duplicate makes the library harder to search, not richer.
- Tag proposals that duplicate an existing canonical tag. Check `tag-vocabulary.json` first — if a genuinely new concept recurs across several systems, propose adding it to `canonical` rather than introducing a variant.

## Sync

`systems/`, `index.md`, and `tag-vocabulary.json` are synced automatically from the published library. Edits to those files land upstream first, so a PR against them will be overwritten on the next sync. Issues and PRs are still the right way to raise them — they just get applied at the source and flow back down.

`README.md`, `CONTRIBUTING.md`, and `skills/` are maintained here directly.
