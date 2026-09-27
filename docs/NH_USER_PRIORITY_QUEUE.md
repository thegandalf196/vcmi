# User-priority queue

User-established priority, 2026-09-24: persist newly assigned tasks here and
resolve them before resuming ordinary New Horizons implementation. Read this
file on every work resumption. Do not remove unfinished entries or equate an
implementation with a verified fix in the user's playable version.

Statuses: Open; In progress; Implemented (verification pending); Verified
(delivery pending); Resolved. Record blockers explicitly. Preserve resolved
entries and their validation/delivery evidence.

This is a task register, not a replacement for the canonical DOCX or Pending
Changes. Existing ordinary backlog remains in the completion audit and other
registers; it is not cancelled by this new queue.

## UP-001 — Tower construction-screen layout

Status: Implemented (visual verification pending); playable delivery pending.

2026-09-26 source delivery: commit `4a03aae52` isolates the Tower-only opaque
leather replacement and per-card responsive frames, together with its source
wiring regression. Independent review confirmed child ownership, paint order,
five-row bounds, non-Tower isolation and unchanged building interactions. The
focused Tower and recruitment-category checks pass. Windows CI and actual
rendered inspection remain pending; this is not yet visual acceptance.

2026-09-24 checkpoint: existing dirty `CHallInterface` source replaces the baked
vanilla card area with opaque leather and attaches an individual background to
each relocated card. Independent source review found correct ownership, paint
order, and row bounds (last row ends at y543, leather ends552, footer begins556).
Added a source wiring guard; both tests in
`tools.tests.test_new_horizons_tower_building_progression` pass, as does
`client/tests/check-new-horizons-recruitment-category-ui.py`. These checks do not
prove rendered appearance. The launcher still resolves snapshot `29d9a6c6d3d2c9a42beff9d20921c7e6af320ef910e22d8dfdfcb63000b9d12f`;
no promotion or visual acceptance has occurred in this checkpoint.

Reported screenshot: Village Hall, Tower, day 2. The Marketplace / Mage Guild /
Arcane Reservoir row has a broad black strip and a shared-looking frame. The
bottom Mage Tower / Library / Golden Pavilion / Cloud Temple row likewise has
black gaps and missing individual card framing. Adjacent rows demonstrate the
intended leather-backed spacing and individually framed cards.

Requirements:
- Correct the card layout/background rendering; preserve the established
  leather, red, and gold visual style without black filler strips.
- Check all Tower building states and rows, not only the pictured purchase state.
- Confirm the previously requested Genie/Magi dwelling ordering and Library
  placement remain correct; do not undo the intended swap to fix presentation.
- Preserve build selection, affordability, prerequisites, and right-click help.

Acceptance: inspect the responsible source and reproduce/verify the visual
result through an authorized method; record candidate identity and delivery.
No GUI/input automation permission is inferred from this report.

Reference supplied in conversation: Image #1, temporary attachment
`/tmp/codex-clipboard-IMr9VX.png`. The written observations above must remain
usable if the temporary attachment disappears.

## Queue intake and ordering

### UP-017 — Activate No Quarter and integrate its perk art

Status: Source implemented; native and playable verification pending, assigned
2026-09-27.

2026-09-27 source checkpoint: canonical No Quarter is active with its Expert
gate. Every qualifying physical melee hit evaluates each surviving hostile
primary or collateral target against a strict post-damage 25% threshold,
including retaliation, Cleave and pre-emptive strikes while excluding ranged,
spell-like and Time Stopped targets. A tagged round blocker suppresses even
unlimited retaliation before the immediate counter check; an explicit saved
activation lifetime keeps the non-stacking -2 Morale penalty through the end of
the target's next accepted activation, including when applied to the currently
active unit. Phantom integrity supplies its own maximum. Authoritative runtime,
Battle AI preview/replay, packet/downsave guards, focused runtime/AI tests and
purpose-made four-state provisional art are present. All 140 New Horizons
Python tests, module regeneration, JSON/CSV parsing, the 71-icon active-perk
provenance/uniqueness guard and whitespace checks pass; two independent Astra
reviews found no remaining material source blocker after the first review's
five findings were corrected. Native compilation/tests, playable delivery and
in-game visual approval remain pending.

Implement the canonical Expert Offense perk end to end: when a melee attack
leaves a surviving enemy stack strictly below 25% of its maximum HP, that stack
loses every remaining retaliation for the current round and suffers -2 Morale
through the end of its next activation. Exact 25% does not trigger. The
authoritative effect must suppress even unlimited retaliation, become visible
before any immediate retaliation check, expire correctly at the new round / end
of the affected stack's next accepted activation, and avoid duplicate stacking
when refreshed.

Acceptance: authoritative runtime and Battle AI apply the same actual-health
threshold and transient effects without mutating live state during hypothetical
evaluation; focused native tests cover the strict threshold, immediate
retaliation suppression, unlimited retaliation, round reset, Morale lifetime,
refresh, exclusions, save/packet behavior where applicable, and AI parity.
Activate the existing perk catalogue entry, regenerate/check the module, bind
purpose-made HoMM3-style provisional art, retain source prompt/provenance and
runtime hashes, and pass active-perk data/art guards. Playable delivery and
in-game visual review remain separate gates.

### UP-016 — Activate Cleave and integrate its perk art

Status: Source implemented; native and playable verification pending, assigned
2026-09-27.

2026-09-27 source checkpoint: canonical Cleave is active with its Advanced gate.
Authoritative combat selects from the destroyed stack's adjacent living enemies
by current aggregate HP, lowest occupied hex and unit ID, then resolves one
50%-damage physical follow-up before any surviving retaliation. Its saved
per-activation expenditure resets only on genuine activations; continuations
preserve it, and old serializers reject lossy state. Battle AI scores and replays
the same follow-up without mutating the live battle, including post-Cleave
retaliation recalculation and clone/rebirth distinctions. Purpose-made
HoMM3-style source art, four runtime states, prompt/provenance and hashes are
retained and bound as Provisional. Focused runtime, AI and compatibility tests
are registered. All 137 New Horizons Python tests, module regeneration, the
68-icon art/uniqueness guard, JSON/Lua syntax and whitespace checks pass; an
independent Astra review found no remaining production blocker. Native CI and
playable/in-game visual verification remain pending.

Implement the canonical Advanced Offense perk end to end. After an ordinary
physical melee attack destroys an enemy stack, the attacker automatically
strikes one living hostile stack adjacent to the destroyed stack for 50% normal
damage. Choose the candidate with the highest current aggregate HP; break ties
by the lowest occupied battlefield hex and then unit ID. Cleave triggers at most
once per genuine creature activation, does not trigger itself, and is not a
ranged, retaliation, Brace/pre-emptive, or spell-like attack. Same-activation
continuations preserve expenditure; a genuinely new activation resets it.

Acceptance: authoritative runtime and Battle AI use the same eligibility and
target-selection rules; hypothetical replay includes the follow-up state and
score without mutating the live battle; save/packet compatibility preserves the
activation expenditure; focused native tests cover trigger, 50% damage,
deterministic targeting, exclusions, non-recursion, and activation reset. Bind
purpose-made HoMM3-style provisional art, retain source prompt/provenance and
runtime hashes, regenerate/check content, and pass active-perk data/art guards.
Playable delivery and in-game visual review remain separate gates.

### UP-015 — Activate Encirclement and integrate its perk art

Status: Source implemented; native and playable verification pending, assigned
2026-09-27.

The canonical Basic Offense perk is “Flank! gains +7% damage per additional
distinct attack side instead of +4%.” Activate its existing catalog definition,
preserve its `requires: basic` gate and exact text, and bind purpose-made,
role-appropriate art. The additional-side coefficient must become +7% for an
eligible Encirclement holder; the first-side/base Flank formula and non-Flank
attacks remain unchanged. Keep authoritative battle damage and AI evaluation in
sync, and verify the effect across save/load and applicable battle cases.

2026-09-27 content/UI checkpoint: the config entry and regenerated module are
active, the client icon binding points to its purpose-made four-state runtime
descriptor, and the source/runtime hash guard and active-perk data tests pass.
Original prompt, source master, reductions, comparison and runtime provenance
are retained under `assets/new-horizons/art-source/encirclement-v1/`; the art is
provisional, with no in-game review or user-final approval recorded. Runtime
logic, focused native scenarios, and playable delivery remain open; this
checkpoint does not claim the gameplay effect is implemented or verified.

2026-09-27 runtime/AI checkpoint: authoritative damage and Battle AI now share
one saved-snapshot-aware additional-side resolver: ordinary Flank retains 4%,
while an eligible Encirclement holder receives 7%. The first-side formula is
unchanged. AI valuation counts distinct sides from currently contacting ready
melee stacks without mutating authoritative state. Focused source coverage now
compares identical additional-side damage before/after selection, preserves
repeated-side damage, exercises a multi-hex contact mask, transports the mask
through client-pack and serializer roundtrips, and makes the AI choose a weaker
base target only when the multi-side opportunity reverses the comparison.
Static/data/art checks and independent source review pass; native execution is
assigned to GitHub CI. Saved perk catalogs remain authoritative: an older hero
whose snapshot still marks Encirclement planned is not silently rewritten, so
the perk becomes offerable in newly initialized New Horizons games.

Acceptance: focused native tests establish +7% per additional distinct side
only for the eligible holder, unchanged first-side damage and no change to
non-Flank attacks; verify AI estimates and save/load identity; regenerate/check
the module and pass active-perk art/data guards. Separately record in-game art/UI
review and the delivered build identity before closing visual/playable work.

### UP-014 — Fixed-school Mage Guild spell generation

Status: Implemented (verification pending), assigned 2026-09-25.

2026-09-26 source delivery: commit `deacc31af` defines the exact nine canonical
preferred-school pairs and 5/4/2/2/2 slot profile. Generation chooses distinct
non-preferred schools, prevents duplicate spell IDs, leaves unavailable slots
empty, and admits only eligible ordinary combat spells. Authored spells cannot
bypass the roster, map bans, school slots, or common-spell eligibility. New
Horizons stores no hidden replacement reserve: client Spell Research is absent
and the server rejects it before mutation, while marker-absent legacy rules keep
their historical path. Visible counts and assigned schools serialize with old
defaults and downsave protection. Forty-eight focused data/source checks,
module regeneration and independent review pass. Native CI and playable
delivery remain pending.

2026-09-26 static-validation checkpoint: ordinary random selection now draws
uniformly from every currently eligible spell in the required school/level,
rather than filtering multi-school spells to preserve a later slot. This honors
the equal-chance rule; uniqueness can consequently leave a later overlapping
school slot empty. All 129 New Horizons Python checks and module-regeneration
check pass. Native compilation/tests remain assigned to GitHub CI.

Replace the canonical DOCX guild-generation rule and implement it: each faction
has two equal preferred schools. Levels I/II contain one spell from each preferred
school plus 3/2 spells from distinct non-preferred schools respectively. Levels
III/IV/V contain exactly one spell from each preferred school. Totals 5/4/2/2/2.
Select non-preferred schools uniformly without replacement, then eligible spells
uniformly within each school/level; no faction spell weights or duplicates.
If a required school has no eligible spell at that level, leave that slot empty;
never substitute a spell from another school.
Update New Horizons.docx directly, not only Pending Changes. Preserve roster/map
eligibility, determinism, and non-NH gameplay. Verify rules and generation with
focused tests; distinguish source completion from playable delivery.

### UP-013 — Complete missing Mage Guild levels and artwork

Status: In progress; user explicitly requested creation, 2026-09-24.

2026-09-25 delivery request: promote the supplied Mage Guild integration for the
normal play script. Prepare an art-only successor of the currently selected
snapshot, preserving its engine and unrelated rules; validate before promotion.

Superseded immediately by the user's explicit request to build EVERYTHING
committed. Build clean detached commit `42860ed29`, excluding dirty source;
validate and promote that complete build. The art-only candidate was not promoted.

Delivery completed: clean detached `42860ed29` built vcmiclient and vcmitest
(RelWithDebInfo, 12 jobs). Five asset tests and three focused native tests passed.
Frozen candidate `e2bd99692994bab59ae36553ff23b9f2de73c3c2b1c958582bd3b631a24aee95`
initialized All for One headlessly and completed seven full AI days before the
intentional 15-second timeout; no reported errors in the smoke log. Promoted
that complete committed build, not the earlier art-only candidate. Normal play
script resolves the new snapshot. Uncommitted source remains excluded; graphical
appearance awaits user acceptance. Previous snapshot retained for rollback.

2026-09-25 supplied-art integration: imported all 92 runtime files (80 PNGs
byte-identical to the three retained archives), normalized descriptor basepath
separators, adopted Castle V, Fortress IV/V and the complete Stronghold guild/
Valhalla ridge swap. Preserved NH costs, prerequisites and five spell rows.
Local vcmiclient/vcmitest build passed; five supplied-asset tests and three
focused native tests passed (guild construction/bindings, guild acquisition,
Tower Library growth). Independent review found no integration blockers.
The broader building fixture still has two unrelated mana expectation failures;
those changes are not part of this delivery. No graphical acceptance claimed.
Committed as `42860ed29` and pushed to `origin/definitive-mvp`. The existing
launcher snapshot was not promoted: the development build also contains
unrelated unfinished work. Supplied guild content is integrated in the local
development build; normal-launcher delivery and visual acceptance remain pending.

2026-09-25 user reprioritization: work only on integrating the three supplied
Mage Guild ZIP packages, retain their source folder in the repository, build
locally, test, commit and push. These supplied designs supersede the generated
drafts below. Preserve Castle's animation, Fortress v8's synchronized flames,
and the Stronghold guild/Valhalla ridge swap. Keep NH costs, prerequisites and
five-level spell access. Additional already-solid changes may be committed, but
unfinished unrelated work must not be swept into this delivery.

2026-09-24 art checkpoint: confirmed five placeholder levels (Castle V,
Stronghold IV/V, Fortress IV/V). Generated five original provisional masters
with the HoMM3 Art skill and built-in image generator, retained with exact prompts
and reference provenance in `assets/new-horizons/art-source/mage-guild-levels-v1/`.
Decoded-alpha inspection confirms transparency in all five. Runtime exports,
hall cards, selection masks, bindings, native-size/placement checks, functional
validation and delivery remain unfinished. No original purchaser pixels were
copied into the repository; no GUI or promotion occurred. This is art progress,
not completion of the full building upgrade.

2026-09-24 integration checkpoint: generated five matching wide hall paintings;
source now binds town sprites, alpha-derived selection areas, indexed cyan-key
gold borders, 150×70 hall cards and 58×64 campaign thumbnails for all five levels.
Unique composed hall descriptors preserve all 44 original frame references except
the new guild levels. Root inspected the native-size comparison sheet. Independent
review caught missing town-to-hall-sheet bindings and stale/skip-on-missing test
assumptions; these were fixed. All eight focused art/configuration/Tower tests
pass without skips, module regeneration check passes, and diff whitespace check
passes. Art remains Provisional. These are source/raster checks, not an actual
construction/access journey or town-screen visual acceptance. No native build,
GUI, commit, snapshot promotion or playable delivery occurred in this checkpoint.

Inventory faction/level gaps, then create faction-appropriate missing Mage Guild
building artwork using the HoMM3 art skill, including provisional drafts.
Integrate the required town, construction-screen, and Mage Guild UI assets;
verify build/upgrade prerequisites and level I–V access. Do not mistake enabling
level V in configuration for complete art or reuse a lower-level building while
claiming the new artwork is done. Preserve original assets read-only, record
provenance and runtime bindings, and keep art Provisional until approved.

Acceptance: exact missing-level inventory, generated originals and required
exports/bindings, functional construction/access tests, authorized visual review,
and identified playable delivery. No new GUI/input permission is inferred.

The user additionally placed every item from the assistant's omitted-task list
in this priority queue. The entries below are not claims that source work is
absent: reconcile existing changes and tests before implementing or repeating
anything. All are Open until current evidence establishes their actual status.
UP-001 and UP-002 remain the initial two screenshot reports; the remaining
entries are also priority work, ahead of the ordinary backlog. Dependencies
may determine execution order; explicitly record any blocker or reprioritization.

## UP-003 — Revised Metamagic and Grand Metamagic

Status: In progress; core runtime aligned, focused persistence/projection and
playable verification remain.

2026-09-27 duration-lifecycle checkpoint: successful Windows run `36291243926`
built the client at `eb6aa28c5`, including the Spell Buffer/Grand-expiry and
Fire Wall duration corrections. Static perk/module guards remain clean. Added
focused native coverage for an Echoed Duration Fire Wall surviving a complete
world save/load with four rounds remaining, expiring after exactly four round
boundaries, and aging through an isolated hypothetical Battle AI model without
mutating the live obstacle. These new native cases await the next CI execution;
no playable or rendered acceptance is claimed. A read-only AI integration trace
found no separate projected-Mana defect: hypothetical spell evaluation neither
stores nor spends caster Mana, and every real continuation decision is rebuilt
from the newly authoritative post-cast state, which already contains Formula
Reserve or Spell Buffer rewards.

2026-09-27 canonical completeness audit: the current runtime and focused tests
cover the core lifecycle, all ten active perk identities, Grand continuation,
Formula Reserve, Arcane Acquisition, save/load, logs and AI projection. Two
active-rule contradictions remain in the committed source and are now isolated
for the next checkpoint. Spell Buffer only recognizes an unused initial offer,
although the canonical wording also includes Grand Metamagic's unused further
Spell Action. New Horizons Fire Wall stores a fixed three-round obstacle without
passing its eligible follow-up duration through Echoed Duration. The source fix
and focused regressions are prepared locally: either pending Metamagic grant
qualifies for the once-per-combat round-expiry Buffer reward, and Fire Wall uses
the shared duration adjustment while legacy obstacle behavior stays unchanged.
Retired Spell Echo and Countersequence references are retained deliberately for
old-save migration/compatibility; they are not restored to the active perk pool.
The module drift check, ten perk-data tests, client Metamagic source guard,
whitespace check and independent Astra review pass. Native compilation/execution
and playable delivery remain pending.

2026-09-26 persistence/projection checkpoint: focused coverage now transports
the saved Arcane Acquisition provenance on a Focus Magic enchantment through
the detached `BattleStart` descriptor wire path and verifies the restored side,
value, duration and perk flag. Battle AI projection separately resolves a
single ranged strike from zero to exactly two marks, then a second strike from
two to the three-mark cap with the increased projected damage, while leaving
the authoritative battle untouched. Production already shares the saved
parameters and the same combat-event script between authoritative and
hypothetical resolution. Native compilation/execution and playable delivery
remain pending; this checkpoint is not runtime acceptance.

2026-09-26 decline-retirement checkpoint: current New Horizons battles no longer
accept an explicit Metamagic decline/end command. The compatibility bit remains
decodable, but the authoritative request processor and replicated-state visitor
reject it without changing the pending sequence or paying Formula Reserve.
Unused opportunities now close only at their canonical round/combat boundary.
The main fixture installs Basic/Advanced/Expert prerequisite perks in tier order
and no longer treats retired Countersequence as selectable current content. A new
integration regression transports a live third-use Grand continuation through the
real BattleStart serialization path, consumes it after reload, and verifies three
uses, cleared state, no recursive action, exactly one Formula Reserve Normal-Mana
payment, and unchanged Buffer. The two client source guards, all 129 New Horizons
Python data checks, and diff whitespace validation pass. Native compilation and
focused runtime execution are intentionally deferred to GitHub CI under the
user's no-local-build instruction. Arcane Acquisition effect persistence and
perk-aware AI projection remain the next focused gaps; the misleading three-row
action counter presentation is owned by UP-004.

Independent review caught two Warcasting regressions that selected Expert Grand
Metamagic without the required Basic and Advanced fixture perks. Both now install
Arcane Acquisition, Echoed Duration, then Grand Metamagic in canonical tier order;
the reviewer verified the correction and reported no remaining blocking,
correctness, or compile-risk finding in this bounded checkpoint.

2026-09-26 canonical/runtime checkpoint: the approved consume-on-use sequence,
Formula Reserve, Spell Buffer, automatic Grand Metamagic, five-round combined
Spell Lock duration and per-target Arcane Acquisition rules are now integrated
into the canonical DOCX. The document passed ZIP integrity and a complete
188-page render with affected-page visual inspection. Arcane Acquisition source
captures eligible Focus Magic provenance and rechecks every damaged target;
legacy Countersequence state and saved perk snapshots remain distinct. Focused
native CI verification and playable delivery remain pending.

2026-09-26 Arcane Acquisition checkpoint: Focus Magic now snapshots both the
eligible Metamagic-follow-up provenance and the active perk on its serialized
effect. Every damaged living enemy target is rechecked when hit: an unmarked
target receives two marks, an already marked target receives one, and the
three-mark cap remains. The Lua combat-event schema accepts the optional saved
provenance field; older effects without it retain ordinary one-mark behavior.
Focused native coverage is present but awaits GitHub CI.

2026-09-24 reconciliation: 53 authoritative Metamagic/state tests and ten shared
`HeroSpellAllowanceTransition` tests passed in the private NH profile, no skips.
Independent source review found the consume-on-additional-cast, automatic Grand,
Spell Buffer expiry, and Formula Reserve closure behavior consistent with the
accepted Pending Changes amendment. However, Echoed Duration changes the normal
mechanics duration while Focus Magic, Phantom Army, and Spell Lock scripts derive
their own durations. The existing Slow getter test misses this applied-effect
gap. A shared duration-adjustment hook and real Focus Magic follow-up regression
are integrated in source: `Mechanics::adjustEffectDuration` defaults to identity;
BaseMechanics preserves direct-hero Echoed Duration eligibility and saturates the
increment. Explicit ordinary duration overrides remain unchanged. Focus Magic
adjusts its fixed base once. Added the actual server-cast 3-to-4-round regression
and explicit-override/saturation assertions. Independent review found no concrete
defect. Native rebuild session 70162 completed successfully. All 70 tests in
`FocusMagicSpellTest.*`, `NewHorizonsMetamagicTest.*`,
`NewHorizonsMetamagicStateTest.*`, and `HeroSpellAllowanceTransition.*` passed
without skips in the private NH profile (14,118 ms), including the applied
Focus Magic duration regression and override/saturation assertions. Other
scripted duration/cap interactions remain to audit. Matching client rebuild
session 99069 also exited successfully; no GUI run or promotion occurred.
The original Phantom Army gap spanned its script, `BattleInfo::addUnit`,
`CUnitState::initializePhantomProfile`, state loading, and the outcome log;
all had assumed exactly two rounds. These paths are now coordinated for the
extension. Spell Lock separately caps ordinary duration at three and its
Spellbinder extension at four; reconcile the Echoed Duration interaction explicitly.
The existing nine `NewHorizonsPhantomArmyTest.*` tests pass without skips
(2,450 ms). They cover the current two-round behavior, not an Echoed Duration
additional cast. Keep that distinction when adding the extended-lifespan,
save/load, malformed-profile, expiry, and actual-duration log regressions.
Read-only implementation review: retain the ordinary base duration of two;
apply `adjustEffectDuration` in Phantom Army's authoritative script and accept
only the supported two/three-round initial profiles in both allocators. Existing
remaining-round serialization can preserve three without a new field; keep all
integrity/alive/provenance checks and reject counters above three. Record the
granted duration from the ADD packet for the outcome log instead of printing
the base constant. Those source changes are now integrated and independent
review found no concrete defect. Added actual additional-cast lifespan,
three-round saved-state, invalid initial/remaining duration, and accurate
three-round log regressions. Root added the test's required BattleProcessor
include. Native rebuild session 41993 and its follow-up incremental check exited
successfully. All 83 tests across Phantom Army, Focus Magic, Metamagic/state,
shared action transitions, and the two selected Tower tests passed without skips
(16,963 ms). This includes the new lifespan/save-state/invalid-bound/log tests.
The matching client rebuild (session 36518) exited successfully; no promotion
or GUI run occurred. Read-only DOCX text review confirms Echoed Duration says
temporary effects gain one round, whereas Spellbinder explicitly caps Spell Lock
at four. The user subsequently approved five rounds when both perks apply;
the clarification is recorded in Pending Changes. Apply Spellbinder's ordinary
cap first, then Echoed Duration once. Script integration and an actual applied
Spell Lock regression remain required. No canonical document edits or layout
verification occurred.
Canonical DOCX migration and playable delivery are still outstanding.

Check the latest canonical document and accepted amendments against Metamagic's
action/use lifecycle and Grand Metamagic. Reconcile affected perks, descriptions,
AI decisions, and runtime behavior. Do not revive rejected manual-activation or
action-carryover proposals. Resolve chronology from evidence rather than treating
every historical proposal as simultaneously active.

Acceptance: a traceable requirements-to-code comparison, lifecycle regression
tests (including unused actions and round boundaries), correct text/AI behavior,
and identified playable delivery.

## UP-004 — Generic hero combat-resource panel

Status: Source implemented; native client/loader checks passed; visual and
playable verification pending.

2026-09-27 evidence reconciliation: the generic renderer and typed provider
loader are ancestors of successful Windows client build `36291243926` at
`eb6aa28c5`. The five focused `CSkill` combat-status loader cases passed in the
recorded native integration run; current Metamagic/Warcasting UI guards, module
regeneration, and whitespace checks also pass. No further speculative product
change is justified before rendered inspection. Remaining acceptance is a
screenshot/input matrix covering sticky and non-sticky panels, compact/outside
placement, short viewports, simultaneous statuses, maximum values, z-order,
hover and right-click help.

2026-09-26 provider-extensibility checkpoint: the compact hero battle panel now
renders a variable list of generic icon/label/value/tooltip entries above the
separate Hero, Order and Spell Action counts. Metamagic contributes its
authoritative remaining/maximum uses through typed skill metadata. Bloodrage is
the second canonical Faction Skill consumer of the same path and contributes
its authoritative current creature-damage bonus and rank cap; this does not
create or mutate a second currency. Skills without provider metadata or a
learned rank reserve no row. Counterspell and Warcasting also use the generic
renderer as non-Faction-Skill state entries. Provider parsing rejects unknown or
malformed metadata, and dynamic panel height drives stack-panel placement.
Focused source/schema/data checks pass. The generated module, C++ loader tests,
native client build, rendered layout and playable delivery still require the
next isolated integration/CI checkpoint; do not mark this resolved from source
guards alone.

2026-09-24 source checks: the Metamagic prompt and Warcasting status guards both
pass. `BattleWindow::refreshHeroBattleStatus` collects generic `CombatStatusEntry`
records separately from action counts. Rendered layout and complete provider
behavior remain verification work; a passing source guard is not closure.

Display Metamagic points through a reusable combat-resource presentation, not a
hardcoded Metamagic-only field beneath Actions. Keep Hero Actions, Spell Actions,
and Order Actions distinct. Support another defined resource through the same
interface without inventing a new gameplay resource. Respect leather background,
red/gold framing, readable spacing, icons, and explanations.

Acceptance: inspect provider/state wiring, validate resource/action updates and
absent-resource behavior, verify layout through an authorized method, and identify
the playable version containing it.

## UP-005 — Skill/perk progression across acquisition paths

Status: Implemented (native verification pending); playable delivery pending.

2026-09-27 Master Gate catalogue checkpoint: the canonical Expert Demonic
Gating perk is now implemented in source rather than merely activated to conceal
a progression gap. The first successfully opened Gate per side and combat
preserves the gating stack's existing Creature Activation; rejected actions and
post-movement Mobile Gate failures do not spend the perk. The continuation does
not begin another activation, expire activation-scoped state, roll Morale, or
advance the queue, and authoritative and Battle AI hypothetical lifecycles use
the same rule. The spent flag and Mobile Gate transition are versioned for
save/network transport with old-load defaults and downsave protection. Focused
regular, Mobile, failure, second-Gate, serialization and AI-projection tests are
present. Static/data/art checks and independent source review pass; native CI,
playable delivery and runtime acceptance remain pending.

2026-09-26 completion checkpoint: the one-per-tier cardinality question is
resolved. The user retained the existing runtime, and the canonical detailed
rule assigns exactly one perk slot to each of Basic, Advanced and Expert; the
older queue wording claiming an open conflict was stale. Ordinary generated
offers, human replies and the authoritative rank application now all enforce
Basic Skill → Basic perk → Advanced Skill → Advanced perk → Expert Skill →
Expert perk. Explicit external rewards retain the canonical exception and may
advance an eligible Skill without the preceding perk, after which offers resume
at the earliest missing perk tier. Teacher rewards now recheck current class
weight and faction ownership even for an already-owned Skill, closing the Thane
/ Wisdom advancement bypass while preserving negative adjustments and full-bar
advancement of eligible existing Skills. Focused source/tests are present;
native compilation and execution are assigned to GitHub CI, and no playable
delivery or runtime acceptance is claimed yet.

The strict gate deliberately exposes the still-incomplete perk catalogue:
Skills without an active Basic perk cannot advance ordinarily, and Skills with
no active Advanced perk cannot reach Expert through ordinary progression. Do
not reactivate inert/planned perks to hide that gap; finish their mechanics and
tests under the implementation backlog before claiming complete playable Skill
progression. Exceptional eligible rewards remain available as specified.

2026-09-26 source checkpoint: ordinary Skill advancement now requires the
preceding perk tier, ordinary human and AI level-up paths share the gate, and an
exceptional external rank grant preserves the rank while subsequent perk offers
fill Basic, Advanced and Expert tiers in order. Focused regressions were added.
The earlier interpretation that the DOCX permitted multiple perks from an
already eligible tier was superseded by the user's explicit decision to retain
the one-per-tier runtime and by the detailed canonical one-slot-per-tier rule.
CI must still verify the compiled paths before this item advances to delivery.

Latest decision, 2026-09-24: user answered **Keep the DOCX exception**. Preserve
exceptional external skill-rank advancement without an earlier perk. Do not
implement the older strict-everywhere rule below. Ordinary progression and perk
offer order still require audit against the actual DOCX; this answer does not
authorize arbitrary perk grants or skipping the document's perk-choice order.

2026-09-24 validation checkpoint: all 36 existing tests across
`NewHorizonsPerkState.*`, `NewHorizonsPerkVerticalSliceTest.*`,
`NewHorizonsRewardSkillFilterTest.*`, and `NewHorizonsFactionSkillQueryTest.*`
passed without skips (6,843 ms). This proves existing behavior, not the requested
strict sequence: one existing expectation permits the identified bypass.
Implementation of new prerequisite gates is held pending the user's answer to
the explicit DOCX-exception versus strict-sequence question. No progression
product edits were made at this checkpoint.

2026-09-24 read-only audit found missing prerequisite gates in
`PerkState::prepareOffer`/`select`, ordinary skill-rank offers in `MapQueries`,
and direct secondary-skill reward advancement. An existing Expert Havoc test
even permits later-tier offers with only the Basic perk selected. Add regression
coverage for missing prior perks and external teachers, not just ordinary
level-ups. The accepted ordered-progression amendment is still in legacy
Overrides; its conflict with the DOCX external-advancement exception remains
tracked in the migration register. Integrate the accepted decision through
Pending Changes and the canonical document, without declaring migration complete.
Root verified the Thane/Wisdom identity: Thane uses `core:alchemist`, renamed
Battle Mage, whose Wisdom weight is zero. `core:battlemage` is instead renamed
Shaman and has positive Wisdom weight. The latter does not justify teaching
Wisdom to Thane. Preserve and run the existing teacher rejection regressions;
do not confuse legacy identifiers with New Horizons display names.

Apply the ordinary progression rules from the canonical document while retaining
its external-advancement exception, as the user explicitly confirmed. Earlier
strict-everywhere proposals and the historical audit above do not authorize
removing that exception. Audit ordinary level-ups and exceptional grants
separately, preserving class eligibility restrictions in both. Resolve any
remaining perk-cardinality ambiguity from the canonical text or explicit review.

Acceptance: tests covering progression and exceptional grants, correct offers
and class eligibility, no lost choices, and identified playable delivery.

## UP-006 — Browse all perks from a skill

Status: Implemented (visual/input verification pending); playable delivery pending.

2026-09-26 reconciliation: the implementation is already committed and pushed.
The complete saved perk catalogue is grouped by tier with icon, name and learned
state; skill left-click opens it, perk right-click shares the normal perk-help
formatter, and legacy skill help remains the fallback. The focused browser guard
passes in the current tree. No new product edit is warranted without rendered
input evidence; this is not yet visual acceptance.

2026-09-24 source reconciliation: `CHeroWindow` already routes skill left-clicks
to `NewHorizonsPerkBrowser` using the saved perk catalogue, retaining ordinary
skill help as fallback. The browser groups all saved perks by rank, shows icon,
name and learned status, and uses `newHorizonsPerkHelp::format` for right-click
explanations. `client/tests/check-new-horizons-perk-browser.py` passes. Runtime
input/visual acceptance and playable-version confirmation remain unverified;
do not reimplement this browser merely because this queue entry is open.

Left-clicking a skill opens its perk collection with names and icons.
Right-clicking each perk displays the same explanation as directly right-clicking
that perk on the hero UI. Include unlearned perks with clear status and preserve
ordinary skill help. Use the established visual style.

Acceptance: correct complete perk pool, shared description behavior, usable
layout/input, and identified playable delivery.

## UP-007 — Complete Tower dwelling and Library swap

Status: Implemented (visual/runtime journey pending); playable delivery pending.

2026-09-26 reconciliation: committed configuration and focused tests cover the
Genie/Magi dwelling identities, row order, costs, prerequisites, recruitment and
Library growth/position requirements. The two Tower progression source tests and
the recruitment-category guard pass in the current tree; the recorded native
Library and melee-penalty regressions also passed. A real construction/recruitment
journey and construction-screen acceptance remain required before resolution.

2026-09-24 checkpoint: both Tower building progression source/configuration
tests pass. The native Library-growth and Magi-melee-penalty tests also pass
without skips (two tests, 568 ms). Strengthened the Library native test to assert
the actual loaded Genie and Mage rows are respectively index three and four;
the strengthened assertions passed in the subsequent 83-test native run.
Cost/prerequisite checks in the Python test inspect merged authored data;
they are not an authoritative
construction/recruitment journey or visual acceptance.

Audit the Genie/Magi swap across dwelling positions, costs, upgrade costs,
prerequisites, recruitment identity, and the Library's position and requirements.
Compare against the canonical design and accepted amendments. Both families
remain Elite. Check actual content, not just labels or screen order.

Acceptance: consistent configuration and runtime building/recruitment checks,
correct construction-screen order, and identified playable delivery.

## UP-008 — Outstanding UI corrections

Status: Implemented (visual/input verification pending); playable delivery pending.

2026-09-26 reconciliation: all three product corrections are already committed
and pushed. `4293ebc0a` binds the Metamagic specialty to the native 44×44 slot;
`7a361474e` provides the Fort label/value gutter and compact bordered leather
Overcharge window; `a313d3c67` supplies the target-aware shared damage/casualty
forecast. The specialty-art, recruitment-layout and Overcharge source guards pass
in the current tree, and the two recorded native forecast regressions passed.
Current dirty `CCastleInterface` hunks belong to UP-001/UP-014, not this item.
Rendered legibility and pointer interaction remain unverified.

2026-09-24 source reconciliation: Overcharge already uses a 320x250 bordered
leather dialog, refreshes selected-target damage/kills through the shared effect
forecast on input, and keeps paint callbacks free of state refresh. Its source
guard passes. Native follow-up coverage is
`NewHorizonsDirectDamageMechanicsTest.MagicArrowOvercharge*`, including the
wounded/temporary-health casualty forecast. Both tests passed in the subsequent
eight-test AI/forecast run (2,534 ms total, no skips); neither the source guard
nor native forecasts establish rendered legibility.

- Specialty icon must fit its intended hero-screen cell, without oversized art.
- Fort stat icons/labels/values need sufficient horizontal separation, including
  long Leadership Cost labels and wide values; use the current approved bindings.
- Overcharge dialog should be approximately half the reported oversized layout,
  leather-backed and consistent with the game's frames and controls.
- Overcharge damage and estimated kills must update dynamically with the selected
  amount and target, including comparison against no Overcharge.

Acceptance: source/input checks and relevant prediction tests plus authorized
visual verification of each subitem. Record delivery separately from source work.

## UP-009 — Asset integration and comprehensive UI/art inventory

Status: Implemented (visual verification pending); playable delivery pending.

2026-09-27 Master Gate art checkpoint: the newly active perk has purpose-made
horned-gate, master-key and ready-sword art created through the HoMM3 Art
workflow. Its generated master, exact prompt, 44x44 and 32x32 reductions,
comparison sheet, hashes and deterministic four-state exporter are retained
under `master-gate-v1`; `NH_perk_master_gate` is bound to all four runtime
states. This raises the complete active-perk set to 65 without borrowing another
perk's image. Source/art uniqueness checks and independent review pass. The art
remains Provisional until in-game visual review and explicit user approval.

2026-09-27 inventory-to-runtime audit: the complete requested replacement set
was traced from retained provenance through exported assets and every known
source consumer. The twelve current Metamagic rank assets, both Metamagic
specialty bindings, hero Movement and Leadership replacements, creature/Fort
Leadership crown, creature Rank stair-step and skill-probability information
control are all installed. No missing runtime binding was found. Fort cards
reuse the crown for Leadership Cost but intentionally present Core/Elite/
Champion as text headings; the stair-step is confined to the categorized
creature window. The skill-probability information mark is code-drawn over its
four-state entry control and therefore has no raster-art provenance. Stale
register and manifest descriptions were reconciled, including the superseded
single-master Metamagic record and the crown's Fort consumer. The audit also
found that the 24-pixel descriptor hitbox could overlap adjacent fields and the
first skill row. In the New Horizons layout it now contracts to the visible
16-pixel information mark and sits exactly between those regions, while legacy
presentation retains its 24-pixel descriptor. The source guard checks the
heading width, both vertical boundaries and the horizontal panel boundary.
All seven focused static art/export/binding checks, JSON/CSV validation and an
independent source review pass. Native rendered inspection of every listed slot
and identified playable delivery remain outstanding; this is not visual
approval or final-art acceptance.

2026-09-26 exact active-perk checkpoint: all 64 currently active perks now have
named bindings to distinct normal art and complete four-state descriptors. The
active-perk completeness/uniqueness gate passes. Planned perks remain outside
this active count and must receive purpose-made art before activation.
The older inventory estimate of
16 is stale. Do not weaken the active-perk uniqueness gate or reuse unrelated
art; create and export purpose-made provisional paintings through the HoMM3 Art
skill.

2026-09-26 Arcane Acquisition art checkpoint: a purpose-made brass
astrolabe/crystal-prism painting was generated through the HoMM3 Art workflow,
verified at 44x44 and 32x32, bound as `NH_perk_arcane_acquisition`, and exported
to four runtime states. Source master, exact prompt, hashes, comparison sheet and
runtime manifest are retained under `active-perks-v5`. It remains Provisional
until an in-game review and explicit user approval.

2026-09-26 Spell Buffer art checkpoint: the retired runtime art was not reused.
A new brass-caged azure reservoir painting was created through the HoMM3 Art
workflow, verified at 44x44 and 32x32, and bound under the distinct
`NH_perk_spell_buffer_v2` family with four states. Its source master, prompt,
hashes and comparison sheet are retained in `active-perks-v5`; final approval
and in-game review remain pending.

2026-09-26 Stormcaller art checkpoint: the borrowed Havoc skill glyph was
replaced by a purpose-made copper storm-horn/lightning painting created through
the HoMM3 Art workflow. The 44x44 and 32x32 exports were inspected, and the
distinct `NH_perk_stormcaller_v2` four-state family is now bound. Provenance is
retained under `active-perks-v5`; final approval and in-game review remain
pending.

2026-09-26 Logistics art checkpoint: Pathfinding, Navigation and Scouting now
have purpose-made boot/trail, sextant/compass and spyglass/revealed-terrain art.
All three masters were created through the HoMM3 Art workflow, inspected at
44x44 and 32x32, exported to four runtime states, bound to their active IDs, and
recorded with exact prompts and hashes in `active-perks-v5`. Final approval and
in-game review remain pending.

2026-09-26 Recruitment art checkpoint: Volunteer Network, Elite Draft,
Champion's Call and Master Recruiter now have purpose-made village muster,
selected equipment, champion horn and command-ledger art. All four masters were
created through the HoMM3 Art workflow, inspected at 44x44 and 32x32, exported
to four runtime states, bound to their active IDs, and recorded with exact
prompts and hashes in `active-perks-v5`. Final approval and in-game review
remain pending.

2026-09-26 first Demonic Gating art checkpoint: Swift Gate, Wide Gate,
Hellfire Arrival and Reinforced Gate now have purpose-made hourglass, expanded
hex-ring, radial fireblast and shielded-gate art. All four masters were created
through the HoMM3 Art workflow, inspected at 44x44 and 32x32, exported to four
runtime states, bound to their active IDs, and recorded with exact prompts and
hashes in `active-perks-v5`. Final approval and in-game review remain pending.

2026-09-26 final Demonic Gating art checkpoint: Mobile Gate, Infernal Beacon,
Reserve Discipline and Endless Legion now have purpose-made movement-trail,
beacon/banner, disciplined-mask and casualty-return art. All four masters were
created through the HoMM3 Art workflow, inspected at 44x44 and 32x32, exported
to four runtime states, bound to their active IDs, and recorded with exact
prompts and hashes in `active-perks-v5`. This closes the active-perk art gap;
final aesthetic approval and in-game review remain pending.

2026-09-26 Intelligence art checkpoint: purpose-made sapphire
mind-crystal/spellbook art was created through the HoMM3 Art workflow, inspected
at 44x44 and 32x32, and bound as the four-state `NH_perk_intelligence` family.
Source, exact prompt, hashes and comparison sheet are retained in
`active-perks-v5`; final approval and in-game review remain pending.

2026-09-26 Sorcery art checkpoint: Illusionist now uses purpose-made silver
mirror/duplicate-crystal art and Spellbinder uses a purpose-made clasped
grimoire gathering five magical streams. Both were created through the HoMM3
Art workflow, inspected at 44x44 and 32x32, exported to four runtime states,
and recorded with prompts and hashes in `active-perks-v5`. The stale duplicate
Planned Spellbinder inventory row was removed because the canonical runtime
registry marks this perk Active. Final approval and in-game review remain
pending.

Integrate the requested purpose-made icons where intended, including Metamagic,
hero Movement/Leadership, creature Leadership (simple yellow crown), creature
category (simple yellow stair-step), and skill-probability information control.
Check Fort and other consumers, not just the hero screen. Reconcile approvals
and the reported Expert Metamagic background concern rather than assuming finality.

Maintain the full UI/asset register beyond the user's examples. Unrelated borrowed
icons are Not done; purpose-made drafts are Provisional; Final needs approval
evidence. Record layout/binding defects separately. All newly created art,
including provisional art, must use the HoMM3 art skill.

Acceptance: inventory-to-runtime binding audit, provenance/approval evidence,
correct exports and placement, and identified playable delivery.

## UP-010 — Canonical-document and legacy Overrides migration

Status: Resolved (design migration); runtime implementation, verification, visual
acceptance, and playable delivery remain tracked in their owning queue entries.

2026-09-26 retirement checkpoint: every legacy entry L01–L41 has an incorporated,
reconciled, or explicitly superseded disposition in `NH_OVERRIDE_MIGRATION.md`.
Accepted missing rules were integrated into the canonical DOCX, including the
centered compact spell-option/Overcharge modal. Stale supporting documents were
reconciled with the contextual action model, strict one-per-tier perk sequence,
and version-3 twenty-point primary progression. The retired Overrides file was
then removed; it is no longer a runtime or precedence layer. The canonical DOCX
SHA-256 is
`7fd38c3b12386e62f511d66bfbd1ea615f301d1e2bdf57a9c70b831ff3ff81e4`.
ZIP integrity and a complete 191-page LibreOffice render passed; affected pages
4, 5, 6, 11, 46, 97, 99, 100, 122, 161, 172, 174, 182, 183, 186, 188, and 189
were visually inspected without clipping or overlap. This closes document
migration only; it does not claim those rules are all implemented or playable.

2026-09-26 conflict-resolution checkpoint: the user retained the existing
one-per-tier perk runtime, selected automatic Astral Nexus Normal-Spell-Point
refill, retained the House of Wisdom scroll storefront, chose Infernal Beacon's
first actionable round, and chose centered spell-option dialogs. The canonical
DOCX now records all five decisions, together with the previously approved
Normal/Buffer, Intelligence, Spellbinder's Hat, Arcane Reservoir, Magic Spring,
Demonic Reserve, Gate-footprint, Reinforced Gate and Mobile Gate semantics.
Registry/module hashes now identify DOCX SHA-256
`7fd38c3b12386e62f511d66bfbd1ea615f301d1e2bdf57a9c70b831ff3ff81e4`.
ZIP integrity passed; LibreOffice rendered all 189 pages; affected pages 6, 46,
99, 100, 161, 172 and 184 were visually inspected without clipping or overlap.
This resolves those design conflicts but does not retire Overrides: the remaining
open legacy entries still require item-by-item classification and verification.

2026-09-26 integration checkpoint: all five amendments formerly in Pending
Changes were integrated directly into the canonical DOCX and visually verified:
Spell Lock stacking, Arcane Acquisition, generic Faction-Skill status entries,
consume-on-use Metamagic with its accompanying perks, and ordinary Mage/Arch
Mage melee penalties. Pending Changes is now empty. The migration register and
perk registry hash were updated. This does not retire Overrides: unresolved
Spell Point/Intelligence, artifact, Gating and other clause-level entries remain.

2026-09-26 checkpoint: reconciled the 310-row registry to clear current DOCX
rules; corrected the source SHA-256 in both the config registry and module copy;
replaced the obsolete Countersequence entry with planned Arcane Acquisition;
and changed the focused test to retain three known Normal/Buffer Spell Point
conflicts (Intelligence, Formula Reserve and Spell Buffer) as explicit
exceptions. Deep Knowledge now follows the current DOCX level-up rule, and the
Havoc perk no longer adds an unsupported Master Chain Lightning effect. Ten
focused Python tests pass. Migration docs record the remaining Normal/Buffer,
runtime and save-identity work. Source alignment is complete;
implementation/migration verification remains open.

Audit each legacy override against the current canonical DOCX. Mark incorporated
items migrated; integrate absent intended decisions; flag conflicts; retire only
obsolete/redundant/explicitly superseded items. Retire Overrides only once every
entry is resolved. Pending Changes is the sole temporary amendment register.

Include the explicit decisions to retain the new DOCX primary-growth model and
ordinary shooter melee penalties for Magi/Arch Magi. Reconcile other approved
decisions, including spell inscription and the Normal/Buffer Spell Points model.

Acceptance: item-by-item evidence and resolved conflicts, verified document edits,
and no permanent legacy-override precedence layer. Do not confuse document
migration with implementation completion.

## UP-011 — AI turn times and leadership failures

Status: Open; prior isolated passes do not close the reported match regression.

2026-09-26 evidence refresh: the current profile still does not contain the
reported match. Its latest log loaded `Too Many Monsters`, recorded ten Nullkiller
turns between 72 and 876 ms, and contains no Leadership-limit rejection; the
newest autosave remains the unrelated September 21 `And One For All` save. The
known full-registry perk lookup, unreachable-movement rescoring and post-battle
Necromancy admission defects already have committed fixes and focused tests, but
none proves the user's 8.7/45.8-second scenario. A safe headless `--testsave`
route exists for a copied save. Faithful replay remains blocked on locating the
matching save; do not run or attribute the unrelated autosave instead.

2026-09-24 read-only checkpoint: prior timing/admission analysis is in
`NH_PERFORMANCE_EXPERIMENT.md`, including the synthetic selected-perk lookup
speedup and five Necromancy admission cases. The reported match replay remains
unverified; no corresponding save identifier is recorded. The launcher's default
profile currently contains six autosaves, newest dated September 21 and labelled
And One For All; that alone does not identify the reported September investigation
match. Do not substitute an unrelated autosave as proof. After the current native
build, rerun
`NewHorizonsMagicAITest.RepeatedMovementEvaluationWithSavedPerksIsStableAndReadOnly`
and `NewHorizonsNecromancyAdmissionAITest.*` as targeted regression evidence,
separately from the still-missing original-match reproduction.
That filter and the two Overcharge forecast tests subsequently passed together:
eight tests, no skips, 2,534 ms. This is regression evidence only, not an observed
turn time for the user's original match.

Investigate the user's latest relevant autosave and reported long AI turns,
including the 45,829 ms turn and leadership rejection. Identify the appropriate
save read-only; do not overwrite user saves/profiles. Attribute time to actual
work or stalls before changing behavior. Check illegal recruitment/transfer/
post-battle army paths and retry loops without bypassing authoritative validation.

Acceptance: evidence from the reported scenario or a faithful extracted
reproduction, focused regressions and measured before/after behavior. A short
unrelated test run is insufficient. Existing GUI/input restrictions remain.

## UP-012 — Hero redesign workbook and biography rewrite

Status: Implemented (native loading and playable verification pending). Originals
remain available for every entry that did not pass review.

2026-09-27 selective-activation checkpoint: all 144 standard heroes were matched
by identity against the purchaser-installed biography table and reviewed in
three editorial rounds. Fifty-two independently rewritten biographies passed
the final fidelity/material-improvement gate; the other 92 decisions are
explicit `null` inheritances, so New Horizons leaves their installed text
untouched. One nominally accepted near-verbatim copyedit was withheld on
provenance grounds. The generated module patch contains exactly the 52 accepted
entries and every record is leaf-only `texts.biography`; no workbook mechanics,
purchaser originals, comparison report, or workstation path enters the module.
Map-authored custom biographies retain precedence. The generator owns both the
manifest and patch drift check, module identity advances to 0.14.0, and 86
focused Python content/generator tests pass. Native content loading and playable
presentation remain unverified; this is not graphical acceptance.

2026-09-24 checkpoint: created a separate Downloads draft,
`New_Horizons_Biography_Comparison.md`, with six original/candidate comparisons
(including one recommendation to retain the original). Proposed lore additions
are explicitly labelled. The original workbook is unchanged. Source-lore review,
user evaluation, mechanical audit, and full-roster pass remain outstanding.
Independent editorial review rejected wholesale adoption: the sample introduces
another repeated apprenticeship/teacher pattern. Preserve the stronger originals;
revise only promising candidates after source-lore inspection. No biographies
have been replaced or claimed improved merely because drafts exist.

Review the hero redesign workbook's mechanical proposals against the canonical
rules without silently promoting proposals into gameplay. Produce a representative
side-by-side biography sample, then expand the rewrite if it proves better.
Preserve established lore/identity, distinguish proposed embellishments from
verified lore, vary structure and emphasis across the roster, and avoid turning
every biography into a specialty explanation ending in a quip.

Acceptance: mechanical findings with conflicts flagged, original/draft comparison,
roster-level editorial review, and user evaluation before wholesale replacement.
The source workbook is `New_Horizons_Hero_Redesign_Workbook.md` supplied from the
user's Downloads directory; do not overwrite its mechanics while editing prose.

## UP-002 — Compact hero-panel Spell Points / Buffer presentation

Status: Implemented; client build and focused native checks passed; visual
verification and playable delivery pending.

2026-09-26 source delivery: commit `c0bbb2d3e` isolates the compact hero-card
presentation, accessible-hero capacity callback, privacy boundary, right-click
explanation and focused regressions. The source guard and independent review
pass. A newer Windows preview build containing this commit is queued; the prior
successful build does not establish this commit's compile or visual acceptance.

2026-09-24 implementation checkpoint: root integrated `CompactHeroSpellPoints`
for both compact hero-card renderers. The two text lines are bounded to 30x20,
Buffer is yellow, narrow values use metric shorthand only when necessary, and
right-click retains the exact full-value explanation. Owned/accessible heroes
receive actual capacity through the callback; enemy Visions retains hidden max.
Independent source review found no concrete defect; compressed large-number
legibility still needs visual verification. The new compact-card source guard
passes. Client build session 36533 and test build session 26295 exited 0.
All seven tests in `SpellPointPresentationTest.*` plus
`SpellPointCapacityTest.OwnedAdventureHeroInfoIncludesActualCapacityAndBuffer`
passed in the private New Horizons test profile, without skips (550 ms).
No game was launched and no snapshot was promoted.

2026-09-24 diagnosis: `CHeroTooltip::init` and
`CInteractableHeroTooltip::init` in `client/widgets/MiscWidgets.cpp` each append
the cyan Buffer label below the original mana row without reserving layout space.
The detailed adventure info snapshot also hides maximum mana by default; fix
owned/accessible-hero data without exposing the maximum through enemy Visions.
The existing four native `SpellPointPresentationTest` cases pass, establishing
shared text arithmetic only, not this compact-card layout. Worker exploration
identified the renderer and permission boundary; root owns the integrated fix.

Reported screenshot: Fafner's compact adventure/town hero panel. Spell Points
shows a standalone white `80` beneath the scroll icon and a cyan `+50` pushed
below the attribute cell, into the adjoining panel area. Knowledge is 30.

Requirements:
- Fit normal maximum, total available Spell Points, and the included Buffer
  amount coherently inside the intended cell; prevent spillover into army slots.
- Use the agreed familiar total / maximum presentation with a Buffer suffix,
  and yellow text is acceptable/preferred over the current cyan treatment.
- Buffer is included in total, not added again. For the shown apparent state,
  verify actual capacity before rendering `80 / 30 +50`; do not infer runtime
  maximum solely from the screenshot's Knowledge stat.
- Keep the expanded tooltip consistent with the compact display and underlying
  Normal + Buffer arithmetic; cover zero Buffer and wider numbers as well.

Acceptance: check the actual compact-panel implementation and values, validate
layout through an authorized method, and record candidate identity/delivery.
No GUI/input automation permission is inferred from this report.

Reference supplied in conversation: Image #2, temporary attachment
`/tmp/codex-clipboard-Ktiq8v.png`. The written observations above must remain
usable if the temporary attachment disappears.
