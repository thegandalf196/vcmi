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

This list is known gaps, not an exhaustive replacement for the scriptures. Keep
the full implementation goal active until a requirement-by-requirement audit
proves completion. See `NH_BUILD_HANDOFF.md` for the current test failures and
the exact playable snapshot boundary.
