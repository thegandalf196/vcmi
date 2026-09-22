# New Horizons completion audit

## Status and evidence standard

Initial evidence inventory, 2026-09-22. This is not a completed scripture audit
or release acceptance. Authority remains `design-sources/New Horizons.docx`,
accepted `NEW_HORIZONS_OVERRIDES.md` entries, and subsequent user directions.
Do not infer completion from a catalogue entry, an `active` flag, artwork, or a
small passing test selection. Implementation, validation, and playable delivery
are separate states.

The earlier conversational estimate of 50–65% was not measured. Do not use it
as a release metric; the content inventory below exposes substantial unfinished
breadth. An overall percentage requires a full requirement inventory and an
explicit weighting method, neither of which has been completed.

## Measured catalogue inventory

Current working-tree `config/newHorizonsPerks.json` contains:

| Item | Active flag | Planned flag | Total |
| --- | ---: | ---: | ---: |
| Skill-rank effects | 78 | 15 | 93 across 31 skills |
| Perks | 55 | 255 | 310 |

These counts include the uncommitted Illusionist activation. They are catalogue
states, not independently verified functional counts and not counts of features
available in the promoted playable snapshot. Recompute after content changes:

```sh
jq '{skills:(.skills|length),perkStatuses:([.skills[].perks[].effect.status]|group_by(.)|map({status:.[0],count:length})),rankStatuses:([.skills[].ranks[].effect.status]|group_by(.)|map({status:.[0],count:length}))}' config/newHorizonsPerks.json
```

## Current verification and delivery boundaries

| Area | Evidence obtained | Remaining gate |
| --- | --- | --- |
| Source retention | Downloaded DOCX and retained source hash matched | Reconcile every requirement with implementation and accepted overrides |
| Content consistency | 62 selected Python content tests passed | Tests do not prove gameplay for the full catalogue |
| Phantom Army | Nine focused native cases passed, including real creation, Integrity, rounding, damage and expiry | Finish related AI regressions, full review, rebuilt client and playable delivery |
| Phantom source restrictions | Selected healing/summoning tests pass; scoped healing correction reviewed | Integrated regression pass and gameplay validation |
| Metamagic logs | 19 of 20 selected logging cases passed | Explicit legacy Clone fixture; active Phantom creation outcomes; wider interaction coverage |
| Orders logs | Activation messages exist | Actual trigger results and exact source-specific damage-prevention attribution |
| Linux launcher | Frozen/checksummed snapshot selection tested and promoted | New working-tree changes require separate build, validation and promotion |
| Full product | No full acceptance established by this checkpoint | Faction audit, complete content, AI, saves, UI, Linux/Windows and installed-asset journey |

## Known remaining breadth

- Audit and finish all remaining skill/perk and spell effects, not just their data.
- Audit every faction's heroes, buildings, creatures, recruitment and AI behavior.
- Complete fixed adventure-spell Mage Guild unlock purchases/learning flow.
- Reconcile travel spell movement rules with the independent hero movement system.
- Complete Logistics development and its effects in authoritative movement and AI.
- Extend explanatory combat logging across new mechanics, using actual resolved
  outcomes rather than hypothetical AI calculations or tooltip estimates.
- Verify save compatibility, integrated UI, and both supported release platforms.

This list is known gaps, not an exhaustive replacement for the scriptures. Keep
the full implementation goal active until a requirement-by-requirement audit
proves completion. See `NH_BUILD_HANDOFF.md` for the current test failures and
the exact playable snapshot boundary.
