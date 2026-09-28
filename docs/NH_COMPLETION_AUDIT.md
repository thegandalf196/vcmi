# New Horizons completion audit

> Historical inventory snapshot. Its 2026-09-24 perk counts and per-Skill rows
> are stale and must not be used as current Phase 1 coverage. The maintained
> working-tree ledger is [NH_FUNCTIONAL_COMPLETION_MATRIX.md](NH_FUNCTIONAL_COMPLETION_MATRIX.md),
> which currently records 95 active / 215 planned perks. Keep this audit for
> its earlier evidence and unfinished-item history until its whole scope can
> be reconciled, rather than updating one number and implying the rest is live.

## Status and evidence standard

Catalogue refreshed 2026-09-24; initial evidence inventory 2026-09-22. This is not a completed scripture audit
or release acceptance. Authority remains `design-sources/New Horizons.md`;
the completed legacy dispositions are retained in `NH_OVERRIDE_MIGRATION.md`,
and temporary amendments belong in Pending Changes before canonical integration.
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

### Historical DOCX catalogue-validation checkpoint

The earlier 26-failure/hash-mismatch checkpoint is superseded. The current
then-canonical DOCX SHA-256 was
`7fd38c3b12386e62f511d66bfbd1ea615f301d1e2bdf57a9c70b831ff3ff81e4`;
the registry and generated module identify that source, all 129 New Horizons
Python data checks pass, and module regeneration is clean. This establishes
catalogue/source consistency only, not native runtime or playable acceptance.

### Metamagic reconciliation at the DOCX checkpoint

Pending Changes is empty because the accepted consume-on-use Metamagic,
Arcane Acquisition, Formula Reserve, Spell Buffer, and automatic Grand
Metamagic rules were integrated into the DOCX and carried into the canonical
Markdown. Implement and test
the definitions there; historical traces below are evidence of earlier states,
not alternative authority. Current runtime and delivery evidence remains tracked
under UP-003 in the user-priority queue.

The older manual-Grand and grant-time-counting source trace is superseded by the
consume-on-use canonical decision and subsequent UP-003 implementation work. Do
not restore those rejected transitions from this historical audit. Review the
current source, AI projection, replicated state, and focused transition tests
together before changing status from implementation to verified delivery.

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

Read-only native probes now load all three captured states successfully, with
the same gameplay-mod set as the capture (the normal native-test preset adds
`vcmi-test` and correctly fails the save's mod-compatibility check). Gretchin's
fresh ordinary path cannot reach the destination; fresh NK2 projection includes
the required battle at the intervening garrison, both with and without town-chain
planning. This differs from the original executing route, which omitted that
garrison milestone. Neither Tiva destination has an ordinary route or a fresh
single-hero NK2 projected route in its respective captured state. These probes
do not yet reconstruct the original multi-hero planning state or prove why its
route survived into execution. Next compare plan creation, task retention, and
state changes before execution; do not treat a fresh projection as reproduction
of the defective original plan. Temporary probe code was removed after use.

### Stationary army-change route invalidation — 2026-09-24

Army-change client notifications reached an empty `garrisonsChanged` callback,
so NK2 could reuse projected routes after a stationary hero's army changed.
A corridor regression failed before the fix: strengthening the hero still left
the guarded destination unavailable at the next planning update. The callback
now marks projected paths stale; it performs no immediate path search or polling.
The regression covers both strengthening and weakening without movement and
requires the battle milestone on the stronger army's projected route.
The client and native tests build successfully; all 19 movement-failure and
chain-reconstruction tests pass with both New Horizons and original-content
presets. Independent review found no blocking issue in this bounded callback
fix. No graphical acceptance or playable-snapshot promotion was performed.

Further exact-save probes included all allied heroes and warmed the threat and
town-distance analysis before own pathfinding. They still did not reproduce the
original invalid plans. Tiva's destinations were assigned to other heroes in the
fresh projection. Do not claim this invalidation fix resolves those match failures.

An additional corridor experiment exposed a separate enemy-projection defect:
danger evaluation ignores its visitor argument and treats armies friendly to the
AI player as harmless even when projecting an enemy's movement. Strengthening
our stationary blocking hero therefore did not remove an enemy threat beyond it,
even after explicitly rebuilding the hitmap. Threat-cache invalidation alone
does not solve this. A proposed hitmap reset was removed from this checkpoint;
fix the evaluation perspective and add the enemy-corridor regression separately.

### Enemy route threat perspective — 2026-09-24

The follow-up carries the visiting hero's owner through tile danger evaluation,
including the encountered object, its visited town, ordinary guards, and guards
at a known subterranean-gate exit. Calls without a visiting hero retain the AI
player's perspective. Neutral visitors do not inherit the AI player's alliances.
Army-change notifications also mark enemy-threat and town-ownership data stale;
the paired invalidation is necessary because threat rebuilding clears both
fields in the shared tile records. These callbacks set flags only; calculations
remain deferred to the next normal AI state update.

The restored enemy-corridor regression checks that a weak defender permits the
projected enemy route while a much stronger stationary defender blocks it after
refresh. It also covers both visitor perspectives, the unchanged object-only
API, neutral/allied visitors, and the two cache invalidation flags. This is
separate from the original captured-match path discrepancies.
The client/test build passed, followed by 57 targeted movement, pathfinding,
defence, and escape tests in each of the New Horizons and original-content
presets. The enemy-corridor test that previously failed now passes.

A bounded 25-second private-profile headless All for One run completed 39 AI
turns (mean 473 ms; maximum 2,881 ms). The log contains no crash or assertion
report before the intentional timeout. However, the same three captured route
failures remain: Gretchin targeting (55, 57, 0), and Tiva targeting (44, 25, 1)
and (47, 23, 1). This validates neither a fix for those routes nor resolution of
the reported long-turn problem. Continue tracing the original projected paths
against execution state; do not substitute this threat fix for that diagnosis.
The playable snapshot was not promoted or changed by this checkpoint.

### Captured route failures: allied occupancy diagnosis — 2026-09-24

Both captured Tiva failures were isolated with a read-only save load and
in-memory relocation of one allied hero at a time. In the first capture,
moving Brissa away from her blocking position made Tiva's destination reachable;
moving Aenain did not. In the second, moving Aenain made the destination
reachable; moving Brissa did not. Restoring each ally and invalidating only the
ordinary path cache separated the cases. No saved game was overwritten.

The production log shows another hero finishing movement immediately before
Tiva executes a previously selected task, with no intervening planning pass.
`makeTurn` retains the batch of selected tasks across successful movement;
copied `ExecuteHeroChain` paths do not automatically change when the pathfinder
is invalidated. A synthetic corridor test now covers initial reachability,
loss of ordinary and freshly projected reachability after allied occupancy,
and restored reachability when the ally moves aside. This establishes the
occupancy cause for the two Tiva captures, not a completed scheduling fix.
The native test build and all nine movement-failure tests pass in both the New
Horizons and original-content presets. Temporary save-loading probes were
removed and the normal test bootstrap restored before these runs.

The follow-up adds a first-step preflight for queued ordinary movement after an
earlier successful task has invalidated projected paths. It reuses the ordinary
path cache rather than rebuilding projected routes for each move. If the first
move is unavailable, the batch is discarded for the next normal planning pass
without locking that hero. Recovery is limited to once per hero per turn; a
repeat falls through to the existing bounded failure handling. Composition
checks only its first executable task, and special-action-first chains are not
predicted, since those actions may themselves establish the route. This does not
validate every future step of a multi-action chain. The separate Gretchin
post-purchase missing-battle-milestone case remains unresolved.

Validation of the queued-route recovery: client/test build passed and 60 targeted
tests passed in each ruleset, including composition execution and the blocked
first-step preflight. A 30-second private headless run with the same map and
seed completed 45 AI turns (mean 571 ms, maximum 3,135 ms). On the formerly
failing Tiva turn, the new preflight triggered, the next planning pass selected
the reachable Star Axis at (56, 3, 1), and Tiva moved during that same turn.
No Tiva route failure was logged through day 15; the changed decisions mean this
is not an identical replay of the later failure. Gretchin's post-purchase route
failure persisted. No crash, assertion or maximum-pass warning was logged before
the intentional timeout. This bounded run does not establish resolution of all
long-turn cases. The candidate remains unpromoted.

### Recruitment-route diagnostic checkpoint — 2026-09-24

A new private save captured the state immediately before the failing Gretchin
chain, not merely after recruitment. Fresh pathfinding from that state reproduces
the discrepancy: the base-army path includes a battle at (44, 60, 0), while the
town-recruitment path to (55, 57, 0) includes the purchase at (34, 59, 0) but no
battle milestone. The garrison is already visible before movement. After the
purchase, fresh pathfinding includes the battle again. Thus neither newly
revealed fog nor merely a copied task becoming stale explains this case.

The synthetic corridor suite now also combines town recruitment with a neutral
garrison, in addition to the existing enemy-hero case. That fixture passes and
does **not** reproduce the captured map's missing milestone. The saved pre-chain
state is the stronger reproducer for tracing combined-army node propagation and
route alternatives. No speculative runtime fix has been applied for this case.
Temporary save-capture and save-loading hooks were removed after diagnosis;
the normal client/test build passed and all ten movement-failure tests passed
in both rulesets. The playable snapshot remains unchanged.

### Recruitment-route battle-node correction — 2026-09-24

The pre-purchase reproducer isolated a committed ordinary node left behind when
the destination rule substituted a battle-aware node. The final hero-chain pass
could expand the obsolete node, omitting the required garrison battle. Merely
locking that node also left it eligible for dominance comparisons and suppressed
the legitimate recruitment route in this reproducer.

The replaced node is now invalidated with `UNKNOWN` action while retaining its
cost and remaining unlocked for a cheaper future approach. It can no longer seed
final expansion or dominate its battle-aware replacement. Re-running the exact
captured state now produces both the base route and the combined recruitment
route with the required battle at (44, 60, 0). A native regression checks node
invalidation, preservation of the battle-aware node, and cheaper-route reuse.

The clean client/test build passed; all 62 targeted AI movement, pathfinding,
defence, escape and composition tests passed in both rulesets. Temporary save
loading and tracing hooks were removed. A 30-second private headless All for One
run completed 43 player turns and reached day 15: mean completed turn 597 ms,
maximum 3255 ms. No route-execution failure or crash was observed in that bounded
run. Node-allocation-limit warnings remain and need separate investigation;
this is not evidence of complete AI or performance acceptance. The playable
snapshot was not promoted.

### Bounded path-storage diagnosis — 2026-09-24

A temporary first-rejection-per-pass probe in a private 30-second headless run
recorded 17 saturated tile samples. All reached the configured 16-slot cap;
none contained the used-daily-adventure-spell flag. Samples held 8–13 combined
actor states, 0–3 uncommitted nodes, and 0–7 invalidated committed nodes. Some
were entirely committed, with no invalidated nodes. Thus neither a system memory
allocation failure nor daily spell-state duplication explains these samples,
and reclaiming unused nodes alone cannot eliminate the limit.

The run completed 42 turns (mean 554 ms, maximum 3360 ms) and began day 15.
This is bounded diagnostic evidence, not an assertion that all important routes
survive the cap. Preserve the current memory bound. Any future admission or
reclamation change must preserve queue/predecessor pointer identity, cheaper
re-relaxation, required battle actions and deterministic route selection; simply
increasing capacity or recycling `UNKNOWN` nodes is not yet justified. The
temporary probe was removed; no playable promotion was made.

### Logistics Pathfinding perk — 2026-09-24

Pathfinding is now active in the canonical and curated perk registries. The
shared movement calculation halves the difficult-terrain surcharge only:
non-native terrain uses 1.20 rather than 1.40, and desert uses 1.40 rather than
1.80. Native terrain and ordinary water are unchanged. Roads and special travel
still apply before the single final ceiling. The perk is evaluated once when
constructing turn information, not by scanning the registry for every tile.

Replicated perk choices invalidate cached paths lazily. The AI invalidation
callback now invalidates projected hero chains as well as ordinary paths.
Native tests cover multiplier combinations, authoritative movement matching
the displayed route, deactivation after losing the required rank, and AI route
cost refresh while the hero remains stationary. The 57-test movement/perk/AI
selection passed under New Horizons; legacy passed 43 applicable tests and
skipped 14 NH-only cases. Fourteen skill/perk data tests and client invalidation
source checks passed. Client and native test builds passed.

A 30-second private headless match completed 44 player turns and reached day 15
(mean 589 ms, maximum 3233 ms). This narrow run showed no gross turn-time
regression, not exhaustive performance acceptance. Dedicated Pathfinding art
is still Not done and graphical acceptance remains pending. The playable
snapshot is unchanged; existing saves retain their saved perk registry.

### Logistics Navigation perk — 2026-09-24

Navigation is active in the canonical and curated registries. It adds 25
percentage points to sea Movement's base modifier without changing land capacity
or refilling current Movement. Normal embarkation/disembarkation preserves half
the remaining allowance, converted to the destination layer's daily capacity.
With free boarding, the shared step charge is halved instead. Integer charges
round up. Projected sailing nodes retain their source layer so disembarkation is
not mistaken for Water Walk landing while the real hero is still on land.

Validation: client and native-test build passed; 59 targeted New Horizons tests
passed, including capacity, inactive-rank, free-boarding, and boarding
preview/executor checks. Original-mode compatibility passed 50 tests with 16
New Horizons-only skips. Fourteen skill/perk data checks and module consistency
passed. These are native checks, not graphical or exhaustive sea-route AI
acceptance. Dedicated art remains Not done; the playable snapshot is unchanged.

### Logistics Scouting perk — 2026-09-24

Scouting is active in the canonical and curated registries and adds five to
adventure-map sight radius while its Logistics rank is active. The authoritative
perk-choice path compares sight before/after selection and emits the existing
fog-reveal packet immediately when radius grows. The regular movement reveal
path also uses this radius; the existing AI tile-reveal callback learns newly
visible objects. No periodic map scan is introduced.

Client/test build passed, as did 28 targeted native movement, perk and AI movement
tests, 14 skill/perk data tests, and module consistency. The new vertical-slice
test verifies immediate reveal without movement, persistence through save/load,
and loss of the radius bonus when Logistics is disabled without erasing explored
terrain. Graphical acceptance and dedicated artwork remain pending; the playable
snapshot has not changed.

### Physical reduction prerequisite for Arcane Ballistics

The canonical specification requires independent physical reductions to multiply
and their combined reduction to cap at 80%. The previous calculator added some
Order/Bulwark/general contributions and had no aggregate PDR cap. The source now
adds an explicit saved `physicalDamageReductionCapPercent` setting (80 for new
worlds, absent means historical behavior), runtime/schema validation, and a
separate physical-only damage stage shared by authoritative attacks and AI.
Contributions to the same generic bonus source/source ID retain `totalValue()`;
distinct sources, Armorer, Battlecraft Defend, Bulwark and defensive Orders
multiply. Petrification, Creature Defense, outgoing penalties and Phantom Army
remain outside the stage. Cross-source-ID percentage modifiers are not supported
by the curated grouping contract; the original path is retained for snapshots
without the setting.

Native regression cases now cover independent versus same-source contributions,
the cap, petrification remaining separate, and historical behavior. Native
validation is **pending**: the incremental `vcmitest` build remains running.
The new shared-header payload triggered a broad rebuild; it must finish before
any test executable is launched. **29 offline content checks pass**, module
metadata is synchronized, and independent source review found no blocking issue.
This is the prerequisite foundation, not completed Arcane Ballistics: its perk
catalog migration, three-mark penetration, previews and native proof remain.
No playable promotion or canonical DOCX edit was performed.

### Remaining implementation

- Implement the accepted ordered Skill/perk progression across every teaching
  source. Seventeen Skills currently have no active Basic perk; activating a
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

### September 24 — primary growth and Buffer Mana verification

The native test target builds successfully. A private-profile headless run passed
all 43 tests in `NewHorizonsPrimaryProfileTest`, `NewHorizonsPrimaryGrowthTest`,
`NewHorizonsHeroRulesTest`, `NewHorizonsVersionThreeHeroGrowthTest`, and
`SpellPointCapacityTest`, plus `NewHorizonsInstalledSkillGrowthTest` and the
three `NewHorizonsCanonicalClassGrowthTest` level cases. This covers version-3 profile validation, independent
percentile boundaries, canonical installed data, authoritative level-up gains,
and combat Buffer grants preserving normal Mana and temporary-buffer provenance.
The 12 Python hero-data tests and generated-module consistency check also pass.
The integrated source is commit `b8220475d`. The planned Wisdom perk Deep
Knowledge still lacks its specified +10-percentage-point Knowledge-growth
modifier; the base version-3 growth system must not be mistaken for completion
of that perk.

The development-screen explanation now derives bonus opportunities from the
hero's growth view. The client build succeeds, including the Tower construction
background correction; recruitment-category and Overcharge source checks pass.
Graphical verification remains pending. Added coverage verifies all five scoped
skill IDs at Basic/Advanced/Expert, nontrivial growth-roll continuation after
randomizer serialization, and all eighteen classes at levels 1, 2 and 20 with
game-state reload. The revised Metamagic perks are not verified end to end.
No playable snapshot was promoted by this check.

A subsequent private-profile run also passes all 28 tests in
`NewHorizonsHeroGrowthTest` and `NewHorizonsVersionTwoHeroGrowthTest`, covering
legacy/version-2 growth, authoritative gain reporting, game/campaign round trips,
scaled spell calculations, and ordinary Mana-cost interactions.

### September 24 — skill combat-status metadata

Optional `combatStatus` skill metadata now selects a typed read-only provider
and registers a localized description. Metamagic declares its existing combat-use
counter as the first provider; this does not introduce an action pool or new
gameplay state. Five native skill tests pass (omission, translation, schema,
malformed loader input, and existing icons), as do six Python skill-data checks
and generated-module consistency. The schema unit test intentionally isolates
metadata from mod image-filesystem validation. Generic client rows now consume
skill metadata, retain exhausted-use readback, and derive panel placement from
visible height. Ward and Warcasting use the same renderer. Focused Warcasting
and Metamagic UI source guards pass; independent source review found no material
issues. The combined client/test build passes after correcting missing
renderer/font includes. The integrated run passes all 48 focused native tests
(the 43 growth/Buffer tests plus five skill tests), 18 Python hero/skill-data
tests, module consistency, and both focused UI source guards. Compact mode
retains the existing stack/hero overlay behavior; both
layout modes, sticky panels on/off, and simultaneous statuses still require
graphical acceptance. These checks do not establish UI completion or promotion.

The existing 43 `NewHorizonsMetamagicTest` cases and eight
`HeroSpellAllowanceTransition` cases also pass as a pre-change regression
baseline. They are **not** acceptance of the newly approved perks: several
explicitly assert manual Grand activation, Countersequence, and Spell Echo in
place of Spell Buffer. Those expectations must be replaced with the canonical
pool and Pending Changes decisions during the coordinated runtime/AI migration.

Migration hazard found in the next-perk trace: the current retired-perk migration
unconditionally maps `metamagic.spellBuffer` to `metamagic.spellEcho`. Reviving
Spell Buffer requires snapshot-aware migration so current selections are not
silently rewritten to the removed perk. Round expiry clears sequence state in
`BattleInfo::nextRound`; rewards must resolve before that clear. The approved
Spell Buffer reward is specifically unused-action expiry at round end, not
voluntary decline. Formula Reserve must handle completed qualifying sequences
when the Grand continuation is cast, declined, or expires, without double pay.
Also inspect combat-end sequence finalization rather than assuming a next round
always occurs. Update human and AI Grand paths together; a protocol flag must
not remain a player-controlled way to activate Grand on an earlier sequence.

This list is known gaps, not an exhaustive replacement for the scriptures. Keep
the full implementation goal active until a requirement-by-requirement audit
proves completion. See `NH_BUILD_HANDOFF.md` for the current test failures and
the exact playable snapshot boundary.

### Metamagic migration preparation

The retired Spell Buffer migration is now restricted to the historical
`d0aa9c0017967e85120b4e63e04df3d58441d606ce9c496d29117515330654ce`
source snapshot with schema/ruleset version 1. Selections are renamed only when
the matching historical definition is migrated. New/unknown snapshots retain
their own Spell Buffer definitions; orphan selections remain invalid. JSON and
binary regressions cover these boundaries. The test target builds successfully
and all 18 `NewHorizonsPerkState` tests pass headlessly. This does not activate
the new perk: its runtime expiry reward remains
unimplemented. The catalog must carry its reconciled source identity before
reviving the ID; the source hash is not an independent catalog revision.

The automatic Grand integration trace confirms that activation belongs to the
accepted first follow-up of the third used sequence (pre-cast use count 2), with
Expert rank, the perk, and no previous Grand activation. Remove manual client
toggles and AI false/true alternatives together. The accepted-cast packet may
retain a server-derived outcome marker, but the request flag must no longer
authorize activation. Share the predicate and transition across execution and
AI projections; preserve already-pending legacy continuations. Formula Reserve
must use the derived outcome rather than the old player-choice flag. This is an
implementation contract, not evidence that automatic Grand already works.

### Automatic Grand integration

The shared transition now derives automatic third-used-sequence activation and
rejects a mismatched accepted-cast outcome atomically. Server requests with the
retired manual Grand flag are rejected; accepted packets carry the calculated
outcome. Both client toggles and their mode state are removed. AI candidates use
the same predicate, without requesting Grand or duplicating ordinary/Grand
variants. The old pre-cast continuation-score duplication is removed: a granted
continuation is evaluated against the actual post-cast battlefield on the next
AI decision. No deeper sequence-search optimality is claimed.

Tests now include three successive used sequences, an invalid third follow-up,
a forged manual request, no charge for the Grand continuation, a previously
granted legacy continuation, a typed-ledger AI third-use request, and hypothetical
transitions that leave real state untouched. The independent source review found
no remaining material issue after correcting the Formula Reserve fixture to
avoid spending its existing once-combat refund during setup. The combined
`vcmiclient`/`vcmitest` build passes. All 109 focused native tests pass across the
action ledger, shared spell transition, Metamagic, Warcasting, action/packet
serialization, and the three Metamagic AI cases. The remaining 33 magic-AI
regressions also pass (142 native tests total across these two runs). Focused
client guards and module consistency pass; no graphical acceptance or playable
promotion is claimed. Full Formula Reserve per-sequence rewards, Spell Buffer
expiry rewards, and Arcane Acquisition remain separate unimplemented revisions;
this slice does not claim that the full Metamagic pool is complete.

The focused Grand description test and module consistency check pass. The full
perk-data comparison still reports 26 failures: 25 skill-pool comparisons against
the newly supplied DOCX and the unreconciled source hash. These remain real
catalog migration gaps, not evidence to change the document or blindly refresh
its hash. They prevent a full-design completion claim.

Next reward implementation boundaries are explicit events, not polling:
resolve round expiry before `BattleNextRound` clears the sequence; resolve a
qualifying pending sequence before battle-result cleanup; final accepted extra
casts and voluntary decline already have replicated refund paths. Formula
Reserve must pay once per qualifying closure, not once per combat. Spell Buffer
must pay only on round expiry and needs a serialized once-combat flag. Ordinary
restoration and Buffer grants must remain distinct typed mana mutations. Granted
Buffer must not be added to combat-only `temporaryBufferRemaining`, which is
removed at battle cleanup. Validate closure reason and sequence/grant identity
before closing so duplicate resolution cannot grant resources twice. AI
hypothetical action state must follow the same eligibility/expiry semantics;
its current no-op mana spending is not evidence of mana-pool forecasting.

### Revised Metamagic reward catalog boundary

The live perk catalog now uses revision 2, while the parser and schema retain
revision 1 support. This separates the newly approved Spell Buffer reward from
the historical revision-1 migration of an identically named, different perk to
Spell Echo. Native regression coverage now explicitly includes revision-1
nonhistorical hashes, revision-2 snapshots with all known hash categories, and
subsequent reloads of already migrated Spell Echo selections. These new native
assertions await the next build/run; do not count source additions as passes.

The focused Python schema and revised reward-description checks pass, as do the
generic combat-status and optional-Metamagic client guards and generated-module
consistency. Independent catalog review found no correctness defect and prompted
the additional historical reload coverage above. The full DOCX/catalog comparison
still fails on 26 unresolved provenance/content comparisons. The source hash has
not been refreshed to disguise those gaps. Spell Buffer's generic neutral icon
is explicitly **Not done**, not final or purpose-made provisional art.

Reward runtime source is now implemented: Formula Reserve settles on accepted
final casts, decline of a qualifying continuation, round expiry, and combat end;
Spell Buffer settles only on unused-offer round expiry. A new serialized
once-combat Buffer flag rejects lossy older writes. Tests cover repeated
sequences, capped recovery, expiry versus decline/end, permanent versus temporary
Buffer cleanup, and serialization. Round and combat-end logs report the actual
reward amounts; the round callback refreshes cached hero Spell Point cards.
Independent production review found no correctness defect. The combined native
client/test build has started; these new native cases have **not yet run**.
Arcane Acquisition, remaining catalog reconciliation, canonical DOCX integration,
graphical acceptance, and playable promotion remain outstanding.

### Focus Magic prerequisite for Arcane Acquisition

Read-only mapping against the current DOCX confirms Focus Magic and Arcane
Breach have no runtime definitions. Arcane Acquisition therefore cannot be
completed merely by replacing the Countersequence catalog entry. The Sorcery
level-3 spell costs 11 Mana, enchants one friendly ranged-capable stack for three
rounds, and adds a mark after each damaging ranged creature attack. Marks cap
at three, last two rounds, refresh together when another mark is applied, and
are dispellable. Each mark gives subsequent friendly ranged attacks Creature
Defense penetration of `min(20%, 10% + 0.05% * SP)`; melee gains nothing and the
new mark cannot benefit the attack that applies it.

Required integration includes the spell definition, authoritative post-attack
mark mutation, damage calculation, save state, expiry/Dispel, AI projected
attacks and spell valuation, visible enchantment/mark duration and count, and
attack-preview penetration. Arcane Ballistics additionally depends on three
marks and Physical Damage Reduction penetration. Existing accepted-cast
Metamagic provenance can qualify Arcane Acquisition without adding a hero UI
field. Countersequence's saved fields require compatible reading, not blind
deletion. The phrase "first enemy stack" needs clarification on once-per-
enchantment versus every unmarked target; a question has been raised. The base
spell and mark prerequisites do not depend on that answer.

Implementation seams inspected: `AFTER_ATTACK` combat-event triggers execute
after the attack packet and expose actual per-target damage; `SetStackEffect`
provides saved, replicated timed bonuses. Do not simply label hostile marks with
the positive Focus Magic spell as their source: `scripts/spells/dispel.lua`
classifies selective removal by the source spell's positiveness. Arcane Breach
needs a correctly negative effect identity (or an equally explicit generic
polarity mechanism), so friendly cleansing and hostile buff removal stay legal.
`Bonus::bonusOwner` is not serialized and cannot retain mark beneficiary side.
Target-aware penetration must flow through the shared damage callback/Lua
calculator, and projected post-hit mark application plus damage-cache validity
must be handled explicitly for the AI. Existing bonus updates only extend
duration; they do not replace an aggregate mark count or payload.

### Metamagic rewards native validation checkpoint

The combined `vcmiclient`/`vcmitest` build completed successfully. The initial
native run passed 85 of 91 cases and exposed six fixture defects: mutually
exclusive Advanced perks selected together, a Normal baseline captured before
paying for the triggering spell, and an unsupported empty-buffer assumption
after a serializer exception. Legal perk combinations now have separate cases;
the zero-gain Buffer test fills its pool after the cast. No runtime rule was
weakened to satisfy these tests.

After rebuilding the corrected test file, all **93** reward, perk rules/state,
serialization, and Spell Point capacity tests pass. All **99** shared action,
Warcasting, Magic Arrow action, and magic-AI regressions also pass: **192 native
tests total** in two isolated headless runs. Client Metamagic and Warcasting
guards, generated-module consistency, and `git diff --check` pass. This
supersedes the earlier pending-build/reward-test status above. No graphical
acceptance or playable promotion is claimed; the full DOCX/catalog comparison
and the missing Focus Magic/Arcane Acquisition work remain unresolved.

### Arcane Breach identity and formula foundation

The registered `new-horizons:arcaneBreach` identity is now negative, special,
nonpersistent and absent from both hero-spell rosters. It has no cast effect;
this is the status source needed by selective Dispel, not a playable Focus
Magic spell. Its unrelated borrowed icon frames are explicitly **Not done**
in the asset register. All 26 offline content checks and generated-module
consistency pass. A native loader/learning-exclusion case has been added.

`NewHorizonsSorcery` now defines the canonical spell/mark durations, cap and
per-mark penetration formula in basis points. The new test covers fractional
values, every documented Spell Power example, the cap boundary, negative input
and integer overflow. The native rebuild completed and all **11** Sorcery and
spell-roster-context tests pass, including the new formula and loaded identity
cases. The formula is not yet wired into damage calculation.

Additional AI inspection confirms that `CUnitState::acquireState()` borrows
its source's unit/bonus pointers. A child hypothetical battle used for marks
between shots must therefore remain owned by the returned attack possibility;
copying health alone cannot preserve its bonus state. Selected attack replay
already carries per-strike hits in `fortuneStrikes`; extend that shared strike
aftermath rather than inventing a second independent hit history. Future
exchange attacks also need post-hit mark application, never during read-only
`evaluateOnly` target probes. The original-damage cache must retain its
pre-effect baseline while current marked damage is recalculated.

Lua combat scripts can issue the same `SetStackEffect` mutations against
`HypotheticBattle`, but AI does not dispatch combat triggers automatically.
Use an explicit deterministic mark-only bridge, not blanket replay of all
scripts (some can cast, damage, heal, animate or log). Live Focus Magic,
post-hit marks, damage integration, AI valuation, status UI and Arcane
Acquisition remain unfinished; no promotion is claimed by this checkpoint.

### Focus Magic scripted mark mutation checkpoint

Registered spell-effect and combat-event scripts now implement friendly
shooter-capable target filtering, a three-round captured-strength enchantment,
and post-hit Arcane Breach mutation. The spell effect is not yet attached to a
live Focus Magic spell definition/roster entry. The mark handler accepts only
positive-damage ranged hits on living hostiles, checks the current controller
against the captured beneficiary side, and refreshes existing marks before
adding another below the three-mark cap. Each mark retains its own potency.
Marks deliberately omit a shared stacking key: that key would collapse the
visible bonus list to one entry and defeat cap accounting.

Native Lua bindings expose current controlling side and copied combat-trigger
JSON parameters. The cast-side penetration binding applies Warcasting only to
the Spell Power component before the cap, not to the fixed base. The bindings
compile. All **15** focused native cases pass (Sorcery formula, loaded roster
identity, original combat-event dispatch and three new direct-script cases).
The direct-script cases exercise actual Lua/bonus packets, but supply hit
payloads themselves: this is not yet proof of full Focus Magic casting,
damage penetration, per-shot AI projection, expiry/Dispel interaction or UI.
The final fixture cleanup rebuilt successfully: all 15 cases pass again, and
the original combat-event test also passes separately under the legacy profile
(not skipped). No native process remains active and no playable promotion was
performed. The next integration must add the spell definition and cast tests,
shared penetration consumption, AI per-strike projection/cache handling and
player-visible status/preview/log feedback before claiming Focus Magic complete.

### Focus Magic damage and AI integration — validation pending

The working source now feeds captured Arcane Breach penetration into the shared
physical-ranged damage calculation, without changing the creature's actual
Defense. Candidate attacks retain a private hypothetical battle and apply the
same mark script between shots; selected exchange projections replay those marks
into their own model. The damage cache remembers marked targets so removing or
expiring marks cannot revive an older cached penetration premium. New native
regressions cover multi-shot isolation and expiry, alongside shared damage tests.
These additions are not yet validated: the integration build has started, and
the actual spell-cast fixture is still being completed. No playable promotion or
full Focus Magic completion is claimed.

The definition now has five registered native cast tests and a separate AI
decision test for choosing a friendly shooter. The private test maps opt into
Focus Magic without activating its production roster row. All **27** offline
content checks pass, and module metadata synchronization passes. The first native
integration build found a missing `GameSettings.h` include in the combat-event
fixture; after correction that compilation unit passed and the remaining build
continued. Native behavioral results are still pending. Independent source
review found no concrete lifetime/mark-replay regression, but is not a substitute
for those tests or graphical acceptance.

The native integration and cast-fixture follow-up builds succeeded. The first
focused run executed 28 cases: **20 passed, 6 failed, 2 skipped**. Scripted marks
were ignored because Lua returns JSON numbers as floats while the damage bridge
required integer storage; the bridge and UI now compare exact numeric side
values instead (not a truncating conversion). Two AI tests accidentally selected
the identifier API's boolean overload through a C-string argument; explicit
string arguments correct that lookup. These fixes await rebuild/retest. Valid
Focus Magic casts and the AI choice also failed and remain under diagnosis.
The creature status tooltips and ranged preview now have source implementations,
but client compilation and rendered acceptance are still pending. No promotion.

After rebuilding, the scripted-mark damage assertions no longer reported a
failure, but the run terminated in the now-unskipped AI projection test. A
single-test debugger run located a dangling temporary bonus-list iteration in
the shared damage callback. The callback and AI mark-detection helper now retain
the returned shared list before iterating; this correction is not yet retested.
Cast preflight still rejects valid targets with no `ProblemImpl` text, so scoped
script-error diagnostics are being added rather than weakening cast validation.

Static tracing then found a script-identity collision: both the enchantment spell
effect and its combat trigger used `core:focusMagic`, while script identities
share a registry. The spell loader rejects a combat-trigger entry as a spell
effect, leaving no applicable effect and no target problem text. The enchantment
registration is being separated as `core:focusMagicEnchantment`; the existing
combat trigger remains `core:focusMagic`. Native kind/distinct-ID assertions and
a new validation run must confirm the correction.

After the distinct script registration and bonus-list lifetime fixes rebuilt,
the focused native run completed without crashes or skips: **27 of 28 passed**.
This includes mark damage, mark expiry, multi-shot projection, AI selection of
Focus Magic, ordinary accepted casts and Warcasting. The remaining recast test
attempts a second Hero spell in the same round; its fixture must advance the
round rather than bypass the action rule. Separately, **25 Focus Fire, Sylvan
Luck and Hero Command AI regressions passed**. Client compilation, remaining
full attack/Dispel/log tests, and graphical acceptance are still outstanding.

The corrected recast fixture rebuilt and the full focused set now passes:
**28 native tests, no skips**. These results validate the loaded spell/effect
identities, fixed-duration recasting across rounds, captured potency, Warcasting,
scripted mark penetration, expiry and per-shot AI projection/selection. They do
not yet prove full authoritative multi-shot event dispatch, selective Dispel,
battle-log presentation or rendered UI. The logging work is resuming and the
client UI build is next; the playable snapshot remains unchanged.

The client build passed. The authoritative Grand Elf double-shot test now proves
that the first hit receives no premature penetration, the second benefits from
the first mark, and Selective Dispel removes the negative marks while preserving
a positive enchantment. Localized combat logs report actual combined penetration,
including mixed-potency capped refreshes; hypothetical AI evaluation does not
perform logging or the extra log-only bonus reads. The CMake curated-translation
guard now includes the new combat text source.

Focus Magic is enabled in the canonical new-world roster (Sorcery level 3,
11 Spell Points at every rank). Cast and AI fixtures use that installed entry
rather than injecting it; a separate context test verifies older saved rosters
do not silently gain it. The roster fixture baseline is now 71 entries.
After rebuilding, **77 native tests from 12 suites passed with no skips**,
covering Focus Magic, logs, authoritative Dispel, AI projections/selection,
roster contexts/consumers, magic-state serialization, Focus Fire, Sylvan Luck,
and Hero Commands. **28 content tests** and the module metadata check passed.
These are source/native integration results, not graphical acceptance or a
playable promotion. Purpose-made Focus Magic/Arcane Breach art and their
remaining perk interactions are still unfinished; the published playable
snapshot has not changed.
