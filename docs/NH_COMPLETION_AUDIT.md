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
daily-cast planning changes. A focused curated selection passes 56 native cases:
canonical travel costs and rounding, water/flight landing cost parity between
pathfinder and authority, vehicle preservation, forged-layer rejection, saved
daily-cast state, action resource reservation, and canonical AI-node selection
when the planned arrival day changes, plus existing AI node-pool, army-loss and
chain-reconstruction regressions. Thirty-one selected movement/pathfinding cases
also pass with the legacy content preset. The client path-invalidation and hero
spell-routing source guards pass; these are source checks, not graphical proof.

Movement preparation now selects the movement day before layer-transition/cast
decisions, refreshes that day's movement capacity, and resolves the canonical AI
daily-state node before checking its lock. Three actual AI-route regressions
cover a low-Movement crossing after today's shared spell allowance was spent,
and fresh casts after one-day Water Walk/Fly effects expire. A separate hook test
checks that resolving tomorrow's node preserves today's settled node and does
not copy its special action. Independent source review covered the safe unused
slot fallback under full node buckets; that fallback still needs direct native
capacity-limit coverage.

This checkpoint is not promoted-playable evidence. Actual-route coverage does
not establish all multi-day travel combinations, authoritative legal landing,
protected barriers, or unchanged full-match AI performance. Movement preparation
adds a cost evaluation before normal movement charging. Keep the currently
promoted snapshot until integrated validation is complete.

A bounded headless `All for One` run found repeated authoritative rejection of
coastal Shipwreck visits: the planner represents the water-side blocking visit
with a SAIL node although the hero stays on land. The corrected shared predicate
allows only a non-transit blocking shore interaction, not boatless sailing, and
charges the source land terrain cost. The new native regression verifies path
and executor agreement, the actual visit, retained shore position and no boat;
the existing fake non-blocking coast-object rejection remains covered.
The same-seed headless rerun completed that Shipwreck interaction without the
server rejection and recorded 67 completed AI turns (maximum 3681 ms). It still
logged four AI `cannot reach` messages and node-capacity warnings; do not call
this a clean gameplay acceptance run or promote on this evidence alone.
`AIGateway::moveHeroToTile` currently returns success when its refreshed path is
empty, so these planning/execution failures need separate investigation rather
than being dismissed as successful actions.

### AI movement failure contract — 2026-09-24

An empty refreshed single-hero route previously returned success from
`AIGateway::moveHeroToTile`. It now raises the existing task-failure exception,
preventing a hero chain from continuing as though that movement completed.
A nonempty route whose next step belongs to a future day still returns pending
(`false`). Adventure-spell execution also restores its callback wait setting on
every exception path, including a failed Town Portal visit.

The client/test build passed. Fifty targeted New Horizons movement, daily-spell,
pathfinding and task-failure tests passed, plus seven legacy-mode movement and
task-failure tests. The two new live tiny-map tests verify unreachable versus
future-day behavior and unchanged hero position/movement. Independent review
found no correctness issue; direct spell callback-restoration coverage remains
missing.

A 35-second private-profile headless `All for One` run with requested seed
1284510375 completed 68 AI turns (mean 428 ms, maximum 2366 ms), then exited at
the prescribed timeout with no remaining client. There were no crash or server
validation errors. Three unavailable live routes entered task-failure handling;
the AI continued, but projected/live route disagreement and bounded node-pool
allocation warnings remain unresolved. Failure handling can lock the affected
hero for the rest of that turn. This is a correction to the execution contract,
not complete route-planning acceptance or evidence of graphical usability.
The candidate was not promoted; the existing playable snapshot is unchanged.

### Required battle-route diagnostics — 2026-09-24

Three corridor regressions now distinguish a projected route through a battle
from a currently executable route. With a wandering monster, a neutral garrison,
or an enemy hero blocking the sole corridor, ordinary pathfinding reaches the
near side but not the far target; every projected AI route retains a required
`BattleAction`. These isolated cases pass. The garrison fixture uses synthetic
visit geometry, not the installed garrison footprint. This is diagnostic
coverage, not reproduction or resolution of the `All for One` failures.
The rebuilt native test target passed all 17 movement-failure and chain
reconstruction tests in both the New Horizons and legacy presets. Independent
review found no blocking test defect; the near-side reachability assertion
was added to exclude a trivially inaccessible fixture.

The captured Gretchin failure precedes a later successful battle against an
enemy hero at the horizontal garrison before reaching the same town. The next
reproduction should include the actual garrison/hero geometry and the preceding
army purchase or exchange, rather than assuming all battle compression is broken.
ObjectGraph compression was considered and ruled out as the cause of this run:
all shipped difficulty settings disable it, and the captured log has no graph
update entries. Do not modify that inactive subsystem to claim these failures
fixed. Tiva's two route failures still need a concrete blocker diagnosis.

The corridor coverage now also enables hero-chain planning and town recruitment.
It requires an actual exchanged-army route and verifies that every returned route
still contains its enemy-hero battle milestone. This case passes too; it does not
reproduce the match failure. The captured source at (34,59,0) is the Stronghold
town, not an external creature dwelling.
All 18 movement-failure and chain-reconstruction tests pass with both the
New Horizons and original-content presets after the normal-binary rebuild.

To move beyond simplified fixtures, a bounded private headless run captured
three full game saves immediately before the three live-route failures. Each
save has a confirmed successful-write log entry. The capture hook was temporary,
limited to three saves, and removed from source; its frozen diagnostic binaries
were not promoted. The next diagnostic should load these exact states rather
than infer a stale cache or lost battle milestone from the abbreviated path log.
Private saves, paths, and diagnostic binaries are not repository deliverables.

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
  The decisive expiry occurs in the `NewTurn` state visitor, after explicit
  EndTurn reaches `TurnOrderProcessor`; the timer's last-moved-hero flag does not
  guard explicit EndTurn or every hero. Any fix must combine movement-time safe
  landing reachability, event-time turn-boundary validation, and AI landing
  execution. A server-only EndTurn rejection risks the AI's existing retry loop.
- Complete Logistics development and its effects in authoritative movement and AI.
- Extend explanatory combat logging across new mechanics, using actual resolved
  outcomes rather than hypothetical AI calculations or tooltip estimates.
- Verify save compatibility, integrated UI, and both supported release platforms.

This list is known gaps, not an exhaustive replacement for the scriptures. Keep
the full implementation goal active until a requirement-by-requirement audit
proves completion. See `NH_BUILD_HANDOFF.md` for the current test failures and
the exact playable snapshot boundary.
