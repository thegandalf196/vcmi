# New Horizons completion audit

## Status and evidence standard

Catalogue refreshed 2026-09-24; initial evidence inventory 2026-09-22. This is not a completed scripture audit
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
| Skill-rank effects | 81 | 12 | 93 across 31 skills |
| Perks | 60 | 250 | 310 |

These counts were recomputed from the committed catalogue. They are catalogue
states, not independently verified functional counts and not counts of features
available in the promoted playable snapshot. Recompute after content changes:

```sh
jq '{skills:(.skills|length),perkStatuses:([.skills[].perks[].effect.status]|group_by(.)|map({status:.[0],count:length})),rankStatuses:([.skills[].ranks[].effect.status]|group_by(.)|map({status:.[0],count:length}))}' config/newHorizonsPerks.json
```

### Per-skill catalogue breakdown

Each row has three rank effects and ten perks. Active flags only:

| Skill | Active ranks / 3 | Active perks / 10 |
| --- | ---: | ---: |
| Offense | 3 | 4 |
| Armorer | 3 | 0 |
| Archery | 3 | 0 |
| Battlecraft | 3 | 1 |
| War Machines | 3 | 0 |
| Discipline | 3 | 1 |
| Recruitment | 3 | 4 |
| Command | 3 | 0 |
| Light Magic | 3 | 0 |
| Shadow Magic | 3 | 0 |
| Nature Magic | 3 | 0 |
| Havoc Magic | 3 | 3 |
| Sorcery Magic | 3 | 9 |
| Chaos Magic | 3 | 0 |
| Spellcraft | 0 | 0 |
| Wisdom | 3 | 1 |
| Warcasting | 3 | 4 |
| Logistics | 3 | 0 |
| Diplomacy | 0 | 0 |
| Estates | 3 | 0 |
| Learning | 3 | 0 |
| Luck | 3 | 0 |
| Divine Mandate | 0 | 0 |
| Sylvan Luck | 3 | 10 |
| Metamagic | 3 | 10 |
| Shroud of Malassa | 3 | 0 |
| Demonic Gating | 3 | 9 |
| Necromancy | 3 | 3 |
| Bloodrage | 3 | 1 |
| Bulwark of the Mire | 3 | 0 |
| Elemental Rebirth | 0 | 0 |

## Current verification and delivery boundaries

| Area | Evidence obtained | Remaining gate |
| --- | --- | --- |
| Source retention | Downloaded DOCX and retained source hash matched | Reconcile every requirement with implementation and accepted overrides |
| Content consistency | 62 selected Python content tests passed | Tests do not prove gameplay for the full catalogue |
| Phantom Army | Nine focused native cases and final combined 262-case selection passed, including related AI | Rebuilt client, runtime validation and playable delivery |
| Phantom source restrictions | Healing/summoning/Sacrifice guards and negative tests pass in combined selection; scoped healing correction reviewed | Gameplay validation and exhaustive copied-ability audit |
| Metamagic logs | Full native suite passes, including explicit legacy Clone and active Phantom creation/counterspell outcomes | Wider interaction coverage and playable delivery |
| Orders logs | Activation messages exist; actual Brace preemptive damage/casualty log tested | Remaining trigger results and exact source-specific damage-prevention attribution |
| Linux launcher | Frozen/checksummed snapshot selection tested and promoted | New working-tree changes require separate build, validation and promotion |
| Full product | No full acceptance established by this checkpoint | Faction audit, complete content, AI, saves, UI, Linux/Windows and installed-asset journey |

## Known remaining breadth

### Adventure travel integration checkpoint — 2026-09-24

The client and native test targets build with the current travel-cost and shared
daily-cast planning changes. A focused curated selection passes 29 native cases:
canonical travel costs and rounding, water/flight landing cost parity between
pathfinder and authority, vehicle preservation, forged-layer rejection, saved
daily-cast state, action resource reservation, and canonical AI-node selection
when the planned arrival day changes. Nine selected movement/Dimension Door cases
also pass with the legacy content preset. The client path-invalidation and hero
spell-routing source guards pass; these are source checks, not graphical proof.

This checkpoint is not promoted-playable evidence. In addition to the broader
gaps below, the AI rule order still needs an actual-route regression for a step
that advances the day inside `MovementCostRule`: layer-transition/cast decisions
run before that rule. Action-level next-day checks and canonical-node tests do
not establish that every such route chooses or renews the correct travel spell.
Keep the currently promoted snapshot until integrated validation is complete.

### Remaining implementation

- Implement the accepted ordered Skill/perk progression across every teaching
  source. Eighteen Skills currently have no active Basic perk; activating a
  universal rank gate without implementing their choices would strand those
  Skills at Basic. Do not mark inert perks active to conceal this dependency.
- Audit and finish all remaining skill/perk and spell effects, not just their data.
- Audit every faction's heroes, buildings, creatures, recruitment and AI behavior.
- Complete fixed adventure-spell Mage Guild unlock purchases/learning flow.
- Reconcile travel spell movement rules with the independent hero movement system.
  Current integration work covers the Fly/Water Walk cost multiplier, shared
  daily-cast route state, and event-driven client path-cache invalidation. These
  changes do not establish complete travel-spell acceptance. In particular,
  authoritative end-of-day legal landing and scenario-protected barriers remain
  open. An end-turn rejection alone is insufficient: movement must not strand a
  hero on water or an obstacle with no remaining Movement and no legal way to
  finish the day.
- Complete Logistics development and its effects in authoritative movement and AI.
- Extend explanatory combat logging across new mechanics, using actual resolved
  outcomes rather than hypothetical AI calculations or tooltip estimates.
- Verify save compatibility, integrated UI, and both supported release platforms.

This list is known gaps, not an exhaustive replacement for the scriptures. Keep
the full implementation goal active until a requirement-by-requirement audit
proves completion. See `NH_BUILD_HANDOFF.md` for the current test failures and
the exact playable snapshot boundary.
