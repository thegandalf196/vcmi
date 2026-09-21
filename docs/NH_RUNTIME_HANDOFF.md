# New Horizons runtime handoff

## Version1.0 scope — six features

`docs/NH_VERSION_1_0_SCOPE.md` is the user-confirmed scope: (1) deterministic/scaled
primary attributes, (2) secondary skills with three associated abilities/no wheel,
(3) six magic schools, (4) Core/Elite/Champion replacing seven-tier organization,
(5) Orders/Doctrines with shared hero budget, and (6) castellans/governors.
Runtime owns the authoritative rules, AI and save compatibility portions, not UI/art.
Castellans are now required, but recruitment/replacement, mobility, commander presence,
defense attribution and progression remain unresolved. Do not adopt a single-Hero
restriction, full caravan logistics or Siege economy by implication; do not equate
existing autonomous-garrison capacity with castellan Leadership. Preserve working
code/saves pending explicit migrations. Current command-native priority remains;
labels, historical narrow passes and scope documentation do not complete Version1.0.

## New product slice: area-spell AI current-control pruning

Root edits ready in `AI/BattleAI/SpellTargetsEvaluator.cpp` and the already registered
`test/battleAI/SpellTargetsEvaluatorTest.cpp`. Havoc Fireball/Frost Ring and Chaos
Hypnotize are already in the authored roster. Candidate harm filtering and ally/enemy
partitions now use current battle ownership versus caster color, not original side.
Also removed the equal-total-count early exit that kept a strictly inferior mixed
ally/enemy cast beside a better same-size cast. No legality, damage, save or data rules
changed. Three new source regressions cover control/restoration, caster perspective,
and positive/negative collateral dominance; `SpellTargetEvaluatorTest.*` now8 cases.
`git diff --check` PASS; compilation/native/gameplay unrun. Build/Content notified of
exact root paths and existing registration; no duplicate offer or Runtime4 mutation.
Build requested a two-path integration hold. Before integration, Runtime found that
cast20 in the two new collateral tests prunes mixed cast21 before cast22, masking
independent equal-size-comparison coverage. After the targeted release, removed
exactly those two setup lines; product unchanged, tests still8 and both paths refrozen.
Content independently corroborated the counterexample (MODEL, not native): corrected
algorithm selects22; old equal-size shortcut retains21+22. No duplicated model/audit;
`git diff --check` PASS. Content's corrected SOURCE review is PASS at
`testing/spell-target-control-current1/RESULT.md`. Build reports the exact two files
committed/pushed as `edc975615`; Windows FULL34757691605 is in progress with bounded
watch under `build/spell-ai-integration1/`. This is client/AI compilation with tests
OFF, not native8 acceptance. Await actual compiler result/defect; no next source
work requested. Command atomicity and Frontend popup roots remain unstaged.

Tester contribution `testing/command-rejection-atomicity1` reviewed and incorporated
as new root `test/server/battles/HeroCommandRejectionAtomicityTest.cpp`, preserving
its original source. Five fresh-budget invalid-request cases; strengthened fatal
setup handling, absent-battle assertion, both nonzero mana sentinels and valid-Charge
follow-up identity/budget checks. Build reports one new CMake registration applied. Filter
`*HeroCommandRejectionAtomicityTest.*`; native unrun and separate from Focus64/spell8.

## Active ordered Runtime backlog — continue independently of compile watches

1. **Teleport AI slice ready:** `SpellTargetsEvaluator.{cpp,h}` enumerates exact
   creature/location pairs through the real validator. `BattleEvaluator.cpp` now
   detects changed positions and evaluates with the hypothetical active unit.
   Three new target tests bring that suite to11; one installed-profile real-AI/server
   case is in `NewHorizonsMagicAITest.cpp`. Accepted Tester's packet-ID0 roundtrip in
   `HeroCommandTest.cpp` is separate. Existing registrations; six root files total,
   no data/save changes, diff-check PASS, native/unbounded-candidate timing unproven.
   BattleEvaluator overlaps future Runtime4 integration: merge the narrow position/
   model-unit change with its Focus condition; never overwrite either or edit the seal.
   Build reports Teleport's five original files integrated as `7b355a606`; the
   separately accepted packet test in HeroCommandTest.cpp is not part of that commit.
2. **Sacrifice source ready:** ordered creature pairs, removed-victim health costs,
   alive/ghost geometry invalidation and no attack by a sacrificed active unit.
   Target suite now13; new installed AI/model/server case and exact overlapping-corpse
   effect regression. Build supplied the script-specific explicit-source fix in
   `scripts/spells/sacrifice.lua`; no global AOE change. Content found NON_LIVING
   golem invalid as a sacrifice victim: changed ONLY that fixture to living Ogre300,
   retaining the real canBeCastAt assertion. Native unrun; source6 paths + pairedLua.
3. **Clone source ready:** `StackWithBonuses.cpp` now clears model-local backlinks
   on clone removal, matching BattleInfo's authoritative behavior. New
   `test/battleAI/HypotheticCloneTest.cpp` has3 real-Clone/hypothetical source cases:
   recast eligibility/live isolation, nested isolation, recursive/idempotent removal.
   Build owns registration. This is another future Runtime4 merge seam; preserve its
   other aging/ammo fixes and this cleanup, never overwrite the immutable seal.
   Build reports Sacrifice integrated as `d348718f4`, Teleport packet as `36280db58`,
   and clone-only cleanup/test/registration as `fb829f00c`; timed WIP was not staged.
4. **Timed source ready:** StackWithBonuses.{cpp,h}, new HypotheticTimedSpellTest.cpp
   (4 cases), HypotheticCloneTest.cpp (+1 derived-marker expiry case). Projected round
   and opening-round grace; SPELL_EFFECT/HERO_COMMAND N_TURNS value snapshots;
   nested removal captures before pointer suppression, repeated fresh queries;
   retained recipients age and pending clone ghosts flush through removal/backlinks.
   Other source/duration policies unchanged. Build owns one CPP registration;
   native unrun, diff-check PASS. Future Runtime4's FocusFireAITest.cpp181 explicitly
   expects the old unaged-spell TODO: reconcile that obsolete oracle in a successor,
   preserving the immutable seal rather than claiming its original64 are unchanged.
   Timed slice integrated as `16320fe75`, including Content's C++20 lifetime repair:
   capture retains the returned owning bonus-list pointer before range iteration.
5. **Obstacles integrated `7f2d29154`:** visible-only spell-obstacle copies, local
   ADD/reveal-only UPDATE/REMOVE, round0 TTL/infinite handling, AI invalidation.
   Four model tests plus actual ForceField model/server case; all native unrun.
6. **Remove Obstacle integrated `22d568e7e`:** BaseMechanics already normalizes
   OBSTACLE to LOCATION. Fixed actual neutral-target heuristic omission by enumerating
   visible obstacle footprints with overlap dedup/validator checks. Target suite14
   plus actual normalized-location/model/server case; native unrun.
7. **Earthquake integrated `db5b76672`:** StackWithBonuses.{cpp,h}, BattleEvaluator.cpp and new
   HypotheticWallTest.cpp4 cases. Local wall state + derived destroyed gate, geometry
   invalidation, field-battle negative, nested isolation and real last-gate Earthquake
   model/server. No new Siege resource economy. Four cases registered, native unrun.
8. **Non-timed removal integrated `9a6bd392d`:** value snapshots include all
   SPELL_EFFECT/HERO_COMMAND durations; only N_TURNS are aged. Two additional timer
   tests (suite6) cover selective removal, retained Doctrine, local identical re-add,
   replacement and parent/live isolation. Native unrun.
9. **Refresh identity integrated `d2323ebbe`:** actualizeEffect matches source/sid/type/
   subtype/valType; presence check includes valType. Two additional timer tests (suite8)
   cover Haste/Prayer broad/narrow+nested aging and distinct-value-type insertion.
   Content caught the BASE_NUMBER fixture assumption; corrected to haste().valType
   (default ADDITIVE_VALUE) before integration. Native unrun.
10. **Selector merge integrated `453cf35b0`:** pending updates merge before query filtering,
   without reusing a narrow caller cache key for the broader query. Added timer case
   (suite9) compares narrow/broad values and authoritative BattleInfo refresh. Native unrun.
11. **Merged effects integrated `3e6441005`:** canonicalize managed effects before
   update/removal/aging, preserving refreshed duration and retained value together.
   Two additional timer cases (suite11): full expiry/new generation and local ADD ->
   refresh/nested lifetime. Native unrun; query/copy cost unmeasured.
12. **Creature spell score integrated `6fc2e9829`:** BattleEvaluator.cpp and
   NewHorizonsMagicAITest.cpp1 case use current victim/summon ownership; Fireball
   preview checks enemy -> controlled ally -> restored enemy and live isolation.
   Removed units remain ghosts: no missing-victim crash claim or null-handling change.
   Optional wall fixture addition checks mechanics target legality alongside the valid
   original CSpell::canBeCast check. Earlier nonexistent-API diagnosis was withdrawn
   after verifying CSpell.h215. All new cases remain native unrun.
13. **Focus successor integrated `4596dfe1f`:** Build composed the reviewed Runtime5
   pairing and subsequent allocator/scorer/DPS/retaliation deltas. Current next gate is
   native64 plus legacy persistence4 and integrated acceptance, not another source seal.
   Windows successor FULL34769181914 at `de1bb7cd0` failed; its evidence is preserved.
   Corrected FULL34771438399 is pinned to
   `9ccd513dcfc7677fa51066d20f0bcb4cfd99a898`, adding only the two missing client
   CMake entries. Independent package acceptance is recorded in
   `build/new-horizons-linux/testing/windows-9ccd51-audit/final-summary.json`:
   player SHA256 `11984c4ade6ea0ce1469794d5867e054662b5d8b962445fda9c91b5d8739b8c2`,
   package/source/CRT/privacy PASS, release held; 87 package preflight regressions pass.
   TestsOFF and ruleset1 default: no native64/Persistence4, gameplay, restart, V2
   activation or publication claim. Build reports no remaining defined compile defect
   and no admitted native/compile-only or zero-capability Linux route. An explicit
   external verification route is required; do not retry the refused launcher.
   This is not the isolated5c repair or an unchanged retry.
   No V2 profile activation or execution is implied. The preparation record follows:
   Runtime5 retained newer movement, obstacle/wall and merged-effect behavior.
   Reconcile its obsolete general-spell-aging oracle explicitly; sealed Runtime4/reg4
   remain immutable and their original64 evidence cannot be relabeled as successor proof.
   `build/focus-fire-runtime-work5/` now contains36 source bodies. Three diverged
   production bodies were merged from current root (StackWithBonuses.cpp/h and
   BattleEvaluator.cpp); remaining24 preimages and nine new-path absences checked.
   FocusFireAITest replaces the obsolete spell-survival assertion with expiry, fixes
   SPEED to STACKS_SPEED, and extends existing renewal/nested-round assertions.
   Content four-body SOURCE PASS bound into readonly `build/focus-fire-runtime-source5`:
   identity **f31a31e4677cacb8e1ddef1d4d9a3195ce65b89865142e140bd0fb494c908bf4**,
   46members/36bodies/27current preimages/9absences. Other32 bodies remain Runtime4-exact;
   TEST declarations unchanged64, not unchanged oracle evidence. Build final pairing
   uses current-registration1/data2/Lua1 and only Frontend four-path patch **a4915f9e**
   (`research/combat-source2-on-50f07708-target-help.patch`), not a full client copy.
   Root integration is now explicit; seals remain untouched. All native/integrated
   gates remain outstanding.
14. **Single-target spell identity integrated `adb112192`:** BattleSpellMechanics.cpp preserves
   singleton CREATURE identity and reacquires it through the current battle, never
   another unit on its hex. New SpellTargetIdentityTest3 covers hex/area preservation,
   actual second-corpse Resurrection, and explicit-ghost rejection; MagicAITest1 covers
   live aim -> projected corpse reacquisition. Native unrun. Subsequent test-only
   extension checks an absent ID carrying a valid corpse hex resolves to INVALID/null
   and rejects without fallback; same three server cases, integrated `714347e46`.
   This extension remains native unrun.
15. **Projected allocation integrated `215c1bba0`:** StackWithBonuses.cpp nextUnitId skips inherited
   live/ghost identities and bounds signed IDs. Added HypotheticCloneTest1 (suite5) covers
   parent clone, child reservation/recast, grandchild ghost reservation and isolation.
   This changes a Runtime5 root preimage: Build must explicitly compose the reviewed
   nextUnitId follow-up with Focus, not overwrite it with the frozen whole CPP. Native unrun.
16. **Single-creature AI identity integrated `a540266e6`:** SpellTargetsEvaluator.cpp/h now emits
   exact validated unit destinations for CREATURE, retaining hex-only neutral LOCATION
   sampling. Added target-suite case (15 total) for two identities sharing a hex and
   rejection of a third; extended the projected Resurrection case to assert the actual
   enumerated model-unit candidate. Build must compose its MagicAITest delta with
   targetidentity successor2. Native unrun; no registration changes.
17. **Temporary-unit scorer integrated `a8b88100f`:** hero-spell health scoring used +/-1
   values as booleans, skipping enemy temporary-unit damage as friendly temporary healing.
   Converted flags to bool/equality. MagicAITest1 uses actual attemptCastingSpell with
   weak regular vs valuable summoned elemental: computed strict DPS difference, verified
   unavailable follow-up attacks/movement, exact selected target, regular-marker control,
   and live isolation. Initial spells cleared; postcast flags asserted. Source reviewed;
   native execution outstanding. Explicit post-Focus composition required; seal untouched.
   Requested Build assess existing Windows compile-only vcmitest route with PRE_TEST and
   accepted GoogleTest override, without executing tests or claiming corpus/native evidence.
18. **DPS measurement peer integrated `8a0226cc3`:** AttackPossibility.cpp selects an opponent
   of the defender's current controller for implicit damage measurement, not an opposite
   original-side unit. New DamageReductionControlTest1 compares distinct-defense explicit
   peers and checks implicit selection before/during/after hypnosis. No global matching
   semantics changed. Build owns BattleAI registration and explicit Focus composition;
   native unrun. Next ownership audit must trace authoritative retaliation semantics
   before changing original-side branches in exchange simulation.
19. **Attack-resource projection integrated `1a869f92e`:** BattleExchangeVariant.cpp copies CAmmo
   consumption from computed affected states instead of inferring one shot or a boolean
   retaliation transition. CAmmo base assignment retains owner-bound caches. New
   AttackResourceProjectionTest2 exercises real two-shot AP and first-of-two retaliation
   AP, model-only consumption and round reset. Server afterAttack semantics traced;
   original-side branches now affect logging only, global matching unchanged. Build owns
   gated registration; native unrun. Direct per-strike exchange overload remains separate.
20. **Retaliation-sequence integrated `4bf5f9834`:** AP normal retaliation now requires first
   strike index; future per-strike exchange loop passes that eligibility explicitly.
   AttackResourceProjectionTest adds one case (suite3) comparing two-strike AP/direct
   projection and authoritative action with two available retaliation charges: only
   one is consumed. Native unrun; depends on resource-copy and current-owner DPS changes.
   Coverage qualification: the direct test supplies first-strike eligibility itself;
   the future production-loop argument is SOURCE-reviewed only. A caller-only mutant
   removing that argument is not caught by this case; future-loop execution remains a gate.
   Subsequent `e2c615912` adds reviewed actual evaluateExchange coverage (suite4):
   fixed two-actor current queue, moved defender with three charges, explicit
   one-round/two-round-horizon reference and a strictly different repeated-retaliation
   counterfactual score. Native positive/caller-only mutant still unrun; not execution
   evidence. Build has been asked to wake Runtime on an admitted native/compile-only
   route decision or a concrete compile defect. No unauthorized launcher retries.
   No claim of added First Strike or ranged-retaliation support; those require separate
   authoritative ordering analysis. Build preserves ordered composition/registrations.
21. **Unresolved full-scope decisions:** current scope/design still do not specify NH
   ability roster/slot-vs-candidate policy, rank/prerequisite/exclusivity/offer/respec rules
   or save/pending-offer migration; castellan offices/replacement/mobility/defense/progression;
   full faction category/recruitment/building/growth mapping. Requested user resolution
   through Content; no invented Tester defaults or completion from legacy/UI placeholders.

Primary scaling/Commands still require pending integrated regressions. Ability offers/
migration and castellan office rules require explicit design. Core/Elite/Champion
labels exist but remaining faction/recruitment rules need decisions; do not invent
those. These family-specific decisions do NOT block specified magic/AI work.
Standing full1.0 assignment supersedes earlier 'no next source work requested'/idle
language: select the next eligible source task at each handoff, without waiting for
another Dispatcher request or an unrelated compile watch.

## Latest user progression direction — specification pending

Future secondary-skill development uses three associated ABILITIES per skill,
Heroes V-style rank/ability progression without a wheel. This supersedes the older
mastery expansion direction; design-document wording may lag the user instruction.
Do not invent mandatory alternation, prerequisites, offer rules or migration.
Assigned bounded H5 research is complete:
`build/new-horizons-linux/research/heroes-v-ability-progression-comparison.md`.
Official manuals plus publisher-supported fan editions1.5/2.1a/3.0 establish
rank-based ability capacity1/2/3, separate rank/ability choices, up-to-four offers,
and version-specific prerequisites—not mandatory alternation or exactly3 candidates.
The note lists outstanding NH decisions; it does not adopt H5 rules or migrate saves.
Preserve existing functional mastery code, numeric identities and saves until an
explicit versioned migration is specified; stop expanding the old mastery design.
Siege may eventually be spendable, but costs/maxima/refill remain undecided. The
illustrative Siege panel/art commission is Frontend/external-art work, not Runtime
rules approval. No artwork import, UI edits or execution permission follows.
Current priority remains native command acceptance with frozen Runtime4/reg4;
this design change does not reopen optional source-only breadth or the blocked route.

## Current coordination topology

Use named targets only: `HoMM3:Runtime`, `HoMM3:Frontend`, `HoMM3:Build`,
`HoMM3:Content`, `HoMM3:Artist`; Dispatcher is `HoMM3:Dispatcher` (do not inject
messages into its user chat). The redundant NewHorizons session/aliases are retired;
historical addresses below are evidence only. Existing conversations/windows/goals
continue unchanged. Future execution-condition/result wakes use `HoMM3:Runtime`.
This address update grants no GUI/build permission and does not restart deferred work.

## Current redesign checkpoint — resumed 2026-09-06

Active ownership is **lib/server/AI/native tests**, per `NH_WORKER_PLAN.md` and
`NEW_HORIZONS_DESIGN.md`; historical W1 sections below are evidence, not current
file boundaries. Build alone compiles/integrates. No Runtime UI/CMake/packaging
edits or commits. Full redesign remains the goal after the first command increment;
architecture experiments are closed. Command native milestone is `54213f042`;
activation/schema repair is `66ddb01bd`. Command/six-school foundation `95a7001e3`
has Linux native and Windows client/install evidence, not full school-family or
Windows gameplay acceptance. Its immutable GUI candidate must remain unchanged.

Read and adopted `NH_DELIVERY_PIPELINE.md` and `NH_AGENT_START.md`, retaining the
existing full-scope goal. Fix declared candidate defects first; keep unrelated
primary/mastery breadth outside its release lane. Build remains sole integrator.

### Priority correction: native progress, not further scaffolding

Runtime4/registration4 are frozen and sufficient for execution planning. Stop optional
source/test breadth and repetitive audit/ACK work while64 cases remain unrun. The
separate target-list fixture is an unsealed deferred draft, not an integration offer.
Build was asked to use an already supported permitted route for an actual compile/
small native step, or report the exact external blocker and next required action.
Do not relax genuine safety guards or replace a blocked route with more scaffolding.
Linux route is now DEFERRED: Build's admitted loader attempt refused before child
creation at `Capability guard: CapInh` (exit1/.12s, grant consumed). Build subsequently
reported its same-launcher inherited mask0000000800000000 with P/E/A zero. No permitted
compile/native route is currently available. External action required: provide or
explicitly authorize an existing zero-capability build/test launcher. No new guard
prototype, automatic retry, compiler claim or optional source expansion. Await that
changed execution condition; all64 cases remain unrun.

### CURRENT complete Focus Fire source offer4 — not executable acceptance

`build/focus-fire-runtime-source4/identity.json`, SHA256
`4fcd75aad49ecd94db4e93f8cd953aebbb8b41a2b4a9ec06b8701ecaf1214b00`.
Content requested one full seal after allocation/remaining source review. Exact
source3 +save4 +controller1 +missing-battle1 +aging1 +allocation1 composition verified:
36 bodies,27 existing roots unchanged,9 new paths absent,51 pinned members.
64 new SOURCE cases =63 Focus-named +1 LegacyCommandAllocationTest; persistence11
means10 Focus +1 Legacy, NOT11+1. Required filter `*FocusFire*:LegacyCommandAllocationTest.*`.
Existing HeroCommandPersistenceTest.cpp/four regression cases also repaired; already
registered, not part of64. Six new CPPs/three headers (new descriptor helper included).
Frontend declaration headers and paired Lua/data2 identities unchanged; API.md bytes
intentionally differ. Initial assembly Lua logical-path inspector RED preserved and
corrected; not a native failure. No source body changed beyond reviewed batches.
Content FINAL binding/reconstruction PASS read at
`testing/focus-fire-full-independent4/summary.json`:51/36/27+9/64 (Legacy1/AI16),
four existing legacy regressions, exact five-batch composition/no extra product delta;
paired bytes and Frontend headers unchanged. This is source-only, not gtest/native.
Registration4 is now sealed and Runtime-reviewed at
`build/focus-fire-registration-runtime-review4`:8 registration pins/51 Runtime pins,
exact two-root preimages/reverse edits, only descriptor-header change vs registration3,
six CPPs/three headers once, AI guard and64-case/Legacy1 filter verified; four existing
legacy regressions remain registered once. No CMake/compiler/native execution.
Intent4 reviewed at `build/focus-fire-private-intent-runtime-review4`: independently
read32 exact Git preimages at168217 (Runtime27+CMake2+data2+Lua1), four identities
match, no export/configure. Requested actual absolute INSTALL_PREFIX (compiled data
paths), EXPORT_COMPILE_COMMANDS/equivalent and explicit paired overlay destinations
including new v2 schema absence (confirmed at base), not blind tree copying.
Headless/Ninja/Debug/PCH-OFF/AI/Lua/PRE_TEST selections remain source intent only.
Explicit retained GTest override reviewed at `build/focus-fire-googletest-runtime-review1`:
208 ordinary files/keyset/size/hash match00d1b000, declared1.17.0, root CMake override
supported; not Git gitlink equivalence or /usr/src recapture. All208 modes differ
from historical origin modes (read-only444 examples); assembly must record its modes.
Complete Google notices read in gtest.h/gmock.h; retain them, no root LICENSE in subset.
No concrete source override blocker or assembly/configure/compiler permission.
Next: Build coherent fresh private configure/build/native proposals. Registration3/
source3 remain historical, not bindings for source4. No configure/compile/native/integration/UI/default permission follows.
All64 remain uncompiled/unrun; full redesign and integrated human/AI/save gates open.
Runtime API/guard agreement for Frontend's PRIVATE exact-ID modal list is recorded at
`research/focus-fire-modal-runtime-agreement1.md` under build/new-horizons-linux.
Weak lifetime/context, synchronous unit reacquisition, fresh current input guards and
CONFIRM, read-only cancel/hover, no fallback target/extra action. No new Runtime API
gap identified; this does not authorize root wiring, compiler or GUI execution.

### Latest executable checkpoint

- **Full-design breadth checkpoint (not restricted to Logistics/host closure):**
  `build/new-horizons-linux/research/runtime-full-scope-checkpoint-aaed.md` separates
  missing mechanics, implemented-but-unverified integrated gates and unresolved
  design choices with exact current source/contract paths. Only three Orders/two
  Doctrines, one new spell definition and two mastery families are implemented;
  six-school registration and14 creature labels are not the full spell/tier redesign.
  Later targeting/trigger/sharing/movement commands, Command development, new spell
  effects/AI, other Expert-skill choices and tier recruitment/mechanics remain work.
  Broad acceptance priorities include current command/default69 spell/cancellation
  journeys, managed Missile acquisition/cast/save, combined growth/mastery/AI and
  real disk-save/old-save/normal-Library continuity beyond Phase A. No build/run or
  new hold is requested by this source checkpoint; historical scoped passes remain.
  Next independent feature contract is
  `build/new-horizons-linux/research/runtime-focus-fire-contract1.md`: targeted
  exact-unit Order, frozen shooter cohort/premium, shared damage/AI path, expiry
  and new versioned battle state. Paired Lua/data ownership is confirmed with Build;
  no UI edits or execution permission are implied.
  Actual isolated rules component now exists at `build/focus-fire-rules-source1`
  (identity `c0f0f97d61a9c13b7094f42948ed5b02464771d128085e369bfb01c80ae50a56`):
  three C++/test bodies, eight unregistered/uncompiled native source cases;
  strict v2 vocabulary and preserved v1 tolerance. NOT integratable alone:
  the full feature is not yet integrated or verified. The complete currently authored
  Runtime/state/AI/save source set was SEALED for cross-owner review. PREDECESSOR
  `build/focus-fire-runtime-source3`, identity
  `cebfab755b597790595ae5cf6d3d47294b14469edf815c59d4dd8ea1e8244306`.
  Relative to source2/9e8be38a, only CBattleInfoCallback.cpp/FocusFireAITest.cpp change:
  hypothetical hostile-only splash attempted current-owner parity. NEW SOURCE RED
  `build/new-horizons-linux/research/focus-fire-source3-controller-red.md` confirms
  battleMatchOwner compares current attacker to INITIAL defender, so source3 does
  not achieve that parity and its premium predicate can reward a friendly target.
  Pending narrow immutable `build/focus-fire-controller-source1` fixes exactly two
  local seams with current/current comparisons; Essentials/ordinary legality unchanged.
  AI assertions now cover direct premium0/30, both unit-control flips and friendly-fire
  breath positions; real lifecycle0/30 controls retained. Content narrow review at
  `testing/focus-fire-controller-independent1` matched two bodies/Essentials and read
  oracles;16 predicate MODEL combinations show8 asymmetric/current-owner differences.
  No concrete narrow defect, no native proof or full caller-graph approval. Batch with save4, not full
  source4/registration rebind. Original HOSTILE-SPLASH.diff/RED are preserved;
  55 cases/13 AI, still no native result. Source2 and source1 remain immutable.
  API declarations are unchanged; API.md version/count BYTES differ. Frontend's
  source2 raw-equality RED/qualified receipt is preserved, not a declaration defect.
  Source1/0ec08813 remains immutable. Source inspection found later-blow casualty
  scoring still used original victim health despite copied damage states. Source2
  changes ONLY AttackPossibility.cpp and FocusFireAITest.cpp: score current copied
  health, skip dead collateral, add sequential two-shot scoring/health/ammo/actual
  authority SOURCE control. The other32 bodies/API/paired components are unchanged;
  CHANGES.md/FOLLOWUP.diff bind the delta. Not an observed native failure or PASS.
  CONTRACT.md/API.md define scope and stable interfaces; NATIVE-SOURCES.txt lists
  six Build-owned registration paths. Data2/schema wrapper and additive Lua pins
  are bound; Runtime verified data2's eight offer pins/two roots and exact added
  wrapper reference/unchanged first-five definitions, not native schema loading.
  Build/Frontend/Content received the requested non-goal full-offer wake. Build's
  private CMake registration source1 was reviewed at
  `build/focus-fire-registration-runtime-review1`: seven offer pins/two roots,
  exact reverse edits, six CPPs/two headers and AI guard match. No source wiring
  defect found for source1; its53 cases required ENABLE_BATTLE_AI (OFF omitted11),
  not a native result. Source2 has54/12 AI cases. Build supplied registration2;
  Runtime review at `build/focus-fire-registration-runtime-review2` verified seven
  pins, predecessor/current Runtime identities, unchanged CMake bodies/root bases
  and the exact source2/count-only control delta. No binding defect; no configure,
  compile, full-graph or native approval. Source1 evidence remains historical. Build notified; no configure or compile was run. This is combined
  review/compile planning, NOT integration, profile activation or execution
  approval. Mutable work remains in `build/focus-fire-runtime-work1`:
  26 existing private source copies plus eight new source paths; 55 native SOURCE
  cases, NONE compiled/run. BEGIN/CONFIRM/readback, targeted factory, authoritative
  snapshot, expiry, last-ammo-safe shared damage, save gates and real/model AI now
  have authored server/lifecycle/AI/independent-graph/old-format controls. Internal
  BattleStart validates before army attachment; spell-like area preview separates
  primary/collateral context. AI recomputes current v2 damage, filters acted-only
  candidates and preserves real unit/cart order when replacing model states.
  Source1 was pinned by SOURCE-PROGRESS6; current source3 SOURCE-CHECKPOINT.json
  pins all34 bodies with exact two-body predecessor delta and26 unchanged roots.
  Build/Content/Frontend notified. Registration3 is now reviewed at
  `build/focus-fire-registration-runtime-review3`: pins/predecessor/Runtime/root
  bases match, CMake bodies unchanged, controls only rebind source3/55;13 AI cases.
  No configure/native approval or reinterpretation of older registration results.
  Additional concrete save-identity finding/proposal is queued for the combined
  review batch, CURRENT `build/focus-fire-save-identity-review4`: null units can reach
  postDeserialize before validation; exact target IDs were existence-only checked.
  Content corroborated pre-binding order/ID premises, requiring valid callback context
  and a LOAD-branch control. WIP now has59 Focus SOURCE cases: adds that real binary-field
  reader/null-injection branch control (not malformed disk proof) plus same-world
  detached snapshot teardown. Further source finding: BattleInfo dtor clears borrowed
  army battle pointers; proposed owner==this guard preserves another canonical battle.
  Content corroborated owner guard; added requested actual-owner localInit/reset
  positive (separate world) so a no-op destructor cannot satisfy the tests.
  Further SOURCE fixture finding: CStack::serialize asserts independence and omits
  CUnitState; source3/legacy persistence tests serialize attached live stacks.
  New shared test-only descriptor writer projects fresh detached stacks/own bonuses
  while preserving actual BattleInfo metadata/reader and original graph. No assertion
  weakened, no ordinary midbattle-save support implied. Existing legacy persistence
  test also repaired privately. Content narrow SOURCE review at
  `testing/focus-fire-save-batch4-independent1` verified five bodies/preimages/header
  absence and descriptor fidelity/exported-only bonuses, lifetime and cleanup oracles;
  no concrete narrow defect found. This proves no Debug-native run or live-state/disk
  save. Five-body/36-source WIP delta still awaits full combined review with controller
  fix; prior save reviews1–3 preserved. Frontend also verified the five proposals,
  four preimages/header absence and descriptor semantics; no extra acceptance scope.
  Further combined SOURCE finding `MISSING-BATTLE-SOURCE-FINDING.md`: targeted
  StartAction dereferenced unknown battle IDs. Narrow immutable
  `build/focus-fire-missing-battle-source1` adds a targeted-only pre-prepare null
  guard/error, extends the existing internal oracle to absent IDs and both army/mana
  guards, then verifies an already active mark/used budget survives rejection.
  No legacy routing, replay-log rollback or actual retirement claim. Batch with
  save4/controller. Content narrow missing-context review passed source pins/oracles;
  no native or replay rollback proof. Further pre-existing command-aging gap confirmed:
  `build/focus-fire-command-aging-source1` privately ages only timed HERO_COMMAND model
  bonuses, including nested original-bearer value snapshots and retained dead units,
  and reacquires current baseline-queue units. Three new SOURCE controls include
  real/candidate/nested expiry, revive/Doctrine/spell boundaries and actual one/two-round
  BattleExchange comparison. Content matched aging1 bindings/three new oracles and
  found no new concrete correction; no native result. ALLOCATION follow-up now has
  narrow `build/focus-fire-allocation-source1` on save4: v2-only dense ID set admission,
  next-ID-only ADD and int32 allocation cap; no legacy numeric-policy change.
  Added sparse-reader rejection, extended descriptor-load/ADD/ghost REMOVE/ADD and
  explicit v1 collision-policy characterization (not safe allocation endorsement).
  WIP64/16AI/11persistence unrun. Allocation/remaining combined review requested;
  Subsequent Content allocation review found no new concrete defect and requested
  full sealing; source4 is now the current complete offer described above. These
  narrow reviews/seal do not grant native, integration or full-goal acceptance. No compilation, execution
  or integrated acceptance yet; findings require an immutable successor.
  Narrow CShots/CRetaliations copy-binding proposal is sealed separately at
  `build/focus-fire-copy-binding-source1` (identity6eafc82e): Content's
  `testing/focus-fire-copy-binding-independent1` found no concrete source defect,
  confirmed localInit-before-copy paths and retained retaliation round maximum.
  Native both-constructor/cart/different-bonus/warm-cache/self-copy/reset controls
  are authored, not run; caller lifetime and full feature remain unproven.
  Three more authoritative source controls now cover shooting-machine exclusion,
  preservation of UntilGetsTurn bonuses and forged internal StartAction snapshots.
  Narrow arithmetic proposal `build/focus-fire-arithmetic-source1` (517bf3e9) adds
  exact dyadic cpp_int fallback for overflowing v1 affine sums without narrowing
  v1 admission or altering ordinary finite-double results. Content's narrow review
  (`testing/focus-fire-arithmetic-independent1`) found no concrete source defect;
  4010 Fraction/dyadic MODEL cases+18 invalid variants are NOT C++/Boost execution.
  Requested zero-factor-invalid/nextafter/mixed-significand native controls added;
  the v1 fixture now explicitly authors v1 under either installed profile version.
  Additional commander-slot/tower exclusion (sentinel, not commander activation),
  spell-like physical preview, malformed saved-context and expired-mark downgrade
  cases are authored. No compilation/native acceptance; the full source offer is
  now available, distinct from the earlier narrow source/model reviews.
  See STATUS.md and SOURCE-RISKS.md for remaining exclusions/preview/malformed
  context checks, ordinary disk/installed/human gates and arithmetic review. No v1 bounds/default rules, previews, artwork or experimental
  castellan/caravan model were activated by this source work.
  HypotheticBattle actually lives in
  `AI/BattleAI/StackWithBonuses.{h,cpp}`, correcting the earlier proposal path.
  Build confirmed paired Lua/data ownership; its isolated additive shooting-only
  Lua diff was read, not executed. BEGIN/CONFIRM and current-controller/static-shot
  oracle clarifications are frozen in that component's SEMANTICS.md. No balance wait.
  Data1 vocabulary/pins and nine recorded offline method bodies were reviewed in
  `build/focus-fire-data-source1/runtime-source-review1.json`; data2 wrapper and
  latest bootstrap/seed/invocation source reviews remain queued, with no admission.
  Restoration adopted no old GUI/PID/native lease or Windows interactive proof.
  Content independently reviewed five dormant Area2/Guild0/CategoryEntrypoint2
  source cases with no concrete oracle defect; they remain unregistered/uncompiled
  and require a separate fresh-closure offer, not reuse of old native authority.

- **Concrete execution path, not more source deliverable prerequisites:** read
  `build/focus-fire-execution-path1.md`. Build identifies no additional Runtime-owned
  source blocker to a compile proposal. Content combined review remains pending.
  Build owns the source6 direct-leaf metadata executor/admission (proposed240s once),
  current tool/header/link/loader reconciliation and then a fresh private
  ENABLE_PCH=OFF/BattleAI ON overlay/configure/build in an approved quiet interval.
  Separate native55/regression/Lua/schema/profile/installed/disk/GUI gates follow;
  Windows test-enabled CI would require a distinct reviewed proposal, not repeating
  current player FULL. Runtime reviewed direct metadata source1 at
  `build/logistics-direct-inventory-runtime-review1`: full runner/leaf/launch/controls
  and invoked helper bodies read, offer pins/11 retained repository inputs and exact
  plan/recipe/cache/output240 bindings match. Three system tool bodies were NOT
  reobserved; no tests/main/collector/notification execution. No concrete defect found
  inside declared trusted-startup/responsive/nonforking metadata scope. This is not
  hard containment, per-role mapping, permission or compiler/ABI/GUI acceptance.
  Subsequent ONCE metadata attempt receipts now exist: tool-return reports exit0,
  boottime14122.54→14176.34 (53.80s), collector summary55714 entries, baselinefalse,
  stable_collection_only. Runtime read these two receipts, NOT the full captured
  row graph or independent actual gate. See `build/logistics-direct-inventory-attempt1`
  and `build/logistics-current-input-inventory1`; permission consumed. Content's
  `testing/direct-inventory-actual-readback1/summary.json` now reports independent
  retained-metadata reconciliation PASS:55714 rows,884 historical records/7306 deps,
  10064 role rows,53.76798s runner, cache/pins/receipts matched. Runtime read the summary;
  44 resolved targets remain UNRECORDED, not asserted absent/dead. This is not a fresh
  recollection or role approval. Build current-input/private PCH-OFF proposal remains.
  Needed-role proposal1 reviewed at `build/focus-fire-current-role-runtime-review1`:
  15 roles/Boost row match retained snapshot. Add already-recorded /bin/sh→dash for
  Ninja; only selected ar/ranlib/pkgconf target bodies are current explicit gaps,
  not all44. Concrete compile guard: root gtest_discover_tests defaults POST_BUILD;
  use reviewed PRE_TEST selection/generated-rule check to avoid premature project
  execution. Select ENABLE_TEST/Lua/headless options, private asset-copy destinations,
  actual plugin/search/flags and assertion mode. Proposal2 CONFIGURE-INTENT read and
  root conditions confirmed: ENABLE_MINIMAL_LIB=OFF selects real Lua; server/ is gated
  by CLIENT OR SERVER, not TEST. Headless CLIENTOFF/SERVERON with ONLY vcmitest target
  avoids a root patch; serverapp registration is not permission to build/run it.
  Proposed Debug/PRE_TEST/private asset destinations still require actual generated
  command/dependency inspection and separate admission. No Runtime source churn required.
  Seed role lists are not promoted; no compiler/native/ABI/GUI authority granted.
  Save-identity findings are queued for a reviewed batch, not speculative rebinding
  or a substitute for Build's closure work.

- **Explicit main Hero UI/separate Orders direction:** read
  `docs/NH_HERO_ORDERS_UI_REDESIGN.md`. Frontend owns main-screen integration and
  separate Spellbook/Orders controls/art. Runtime supplies only demonstrated missing
  read models/validation: one shared hero-action budget, bookless Orders, independent
  spell guards and legacy/tactics/controller/autocombat semantics remain unchanged.
  Sketch numbers/free points/Replace Skill and experimental castellans/caravans are
  not rules activation. Immediate Extras/convenience repair remains separate from
  both the larger UI redesign and owned Focus Fire integration.

- **Retained seed-candidate review, not bootstrap admission:** newer Build seed
  metadata observations are distinct from the retired Linux fences. Runtime read
  the retained-only candidate converter/controls and independently compared its
  actual1445 rows/1330 body records/8 links/111 directories/12 mapping pathnames and
  three unrecorded alias targets to exact retained seed d2602d58. Review at
  `build/logistics-seed-bootstrap-runtime-review1` found no narrow transformation
  defect; no host path named in records was reopened and no derive/collector was
  executed. Seven execution-role lists remain EMPTY, approved=false, manifest NULL.
  Build notified. Per-role imports/search policy, bootstrap/lifetime and fresh ABI
  remain separate requirements; this does not grant compiler/PCH/GUI authority.

- **CURRENT LINUX INPUT HOLD — host drift before Phase A admission:**
  `build/logistics-map-transport-overlay-source2/SYSTEM-DRIFT-RED.json` reports
  libc.so.6/libm.so.6/libmvec.so.1/ld-linux body changes. Runtime independently
  confirmed all four old/current hashes and canonical paths against the unchanged
 645-link ledger in `build/logistics-system-drift-runtime-review1.json`.
  No compiler/link/main was admitted or run by Runtime. Old native/loader fences
  are historical checkpoints, NOT current authority for new Linux jobs or GUI
  first execution. Do not silently refresh them. Build is investigating the host
  change; a separately reviewed current system/tool/header/startup/loader closure
  is required. Four confirmed bodies are not a complete host-change inventory.
  Historical tests and Windows artifact evidence remain unchanged. Build's
  `build/logistics-host-drift1` investigation records the Sep8 18:15 full-upgrade;
  inspected dpkg lines show libc2.43-2ubuntu2.3 -> .4 plus Python3.14/curl updates.
  Its old-key comparison reports22900 header/predicted keys unchanged and106 of
  7853 library keys changed/missing/retargeted, compiler8 bodies/resolutions stable.
  This is historical-key classification, not coverage of additions or an approved
  current baseline. Python/wrapper and GUI-driver changes need their own current
  dependency review; no rollback or new job is authorized by these findings.
  Current-inventory source5 adds unbuffered descriptor reads to the source4 byte
  budget/strict-Ninja repairs; Runtime verified its nine identity-bound files and
  recorded23 offline AST/helper/policy controls, not a filesystem collector run.
  External first-exec/bootstrap implementation and current stable inventory remain
  pending. `COMPILER-DSO-REUSE-DECISION.md` prefers a fresh private ABI after full
  closure review: unchanged compiler8/header bytes alone do not authorize old
  PCH/object reuse. Keep aaed/graph9 separate from later docs and Frontend dirt.

- **Final Runtime Logistics SOURCE integration offer:**
  `build/logistics-runtime-integration-source1/identity.json` c1926dca seals exact20
  files (source9's19 + supplemental wire), each byte-identical to graph9. All15
  existing root-base hashes matched and five new paths were absent at sealing.
  Contract/lineage/evidence hashes and review-only ROOT-DELTA.patch are included.
  At offer creation no root application or activation was performed. Build later
  recorded a separate explicit integration decision and applied the20 files plus
  only three baseline CPP registrations in test/CMakeLists.txt. Runtime's read-only
  `build/logistics-root-integration-runtime-review1.json` independently verifies
  all21 root bodies equal graph9, all1801 actually consumed source bodies equal the
  current root, and scoped git diff --check passes. No Runtime root application,
  stage/commit or default activation; data/guards remain outside this increment.
  Build subsequently committed exact21 as
  `aaed0677960d980f0180ac69926077ca61997215`, parent f7492bdc. Runtime's
  `build/logistics-commit-runtime-review1.json` independently verifies the local
  parent, exact changed path set and all21 committed blob hashes against graph9.
  Build reports push; Runtime did not independently query remote state. Windows
  incremental FULL34272556634 subsequently completed successfully at aaed:
  `build/logistics-windows-terminal-runtime-review1.json` checks watch.exit0,
  exact run/head, the completed successful build job and all26 step conclusions
  (three expected preflight-only/repack skips). Configure/compile/stage/package
  and workflow preview upload succeeded. This is terminal evidence, not Runtime
  downloaded-payload audit, Windows gameplay/GUI or d90 replacement/public release.
  Build subsequently read back the independent package gate as
  SCOPED_PACKAGE_AUDIT_PASS_WITH_QUALIFICATIONS in
  `build/logistics-windows-independent-gate-readback1.json` (five evidence pins).
  Preserve its CRT-origin/licensing and source CRLF/mode qualifications; no PE
  execution, legal warranty, native Windows gameplay/save or publication claim.
  This is not whole-goal completion. Guarded installed2 and Phase A tests remain
  outside baseline20/254/284.

- **Installed-v2 TEST native2 actual PASS:**
  `build/logistics-installed2-runtime-review.json`: exact source-derived2 completed,
  no skips, native/outer0,11.522s;35718 pre/post AND current input identities and6
  private write bodies/sizes independently checked. Actual installed engine-v2
  before map startup, world/hero capture and authoritative Logistics reply/bonus
  passed. TEST+18 resources only; not normal-Library/old-save/disk-game/GUI/Windows.
- **OFF254 fresh closure progressing:** graph9 differs from graph8 only by the
  verified source9 hidden/reveal CPP. Configure0/1.888s;884 commands exactly match
  normalized ON887 minus3 managed CPPs, no installed guards; private paths,
  PRE_TEST/noop test post-build and main link libraries checked. One fresh compile
  admitted by `build/logistics-default-compile-runtime-admission1.json`, exact
  plan4/script4, explicit Scrt1/configured-wrapper pins and post-job census.
  Actual outer/compiler0/617.024s: Runtime rehashed35137 fence entries/tool8/root3,
  graph4,11 PCHs and3 ELF64 artifacts;884 VALID dependency records/881 compiled
  outputs/eight link targets checked. Canonical partition6545 known+636 generated
  +123 ELF32/i386 client-only link-search candidates. Actual test/client Scrt1 is
  prefenced; test DT_NEEDED matches df14. See default-compile-runtime-review1 and
  runtime-link-tail1 JSONs. OFF254 subsequently passed:243 completed+11 exact
  historical skips, native/outer0, XML5.271s/runner16.468s; Runtime independently
  checked35713 pre/post/current identities and147 private writes in
  `build/logistics-default254-runtime-review1.json`. Content independently accepted
  its own terminal/admission audit. The actual resource profile matches
  historical OFF234's PRIVATE0.6 categories/69magic1, NOT public default0.5.1;
  managed-OFF build flags and installed profile scope must remain distinct.
- **Source-only compatibility correction and phase A:**
  Preserve `build/logistics-compatibility-source-plan1/CONTRACT.md` section A as an
  assumption RED: generic direct MASTERIES merge does not establish VMAP transport.
  Reviewed mapping/campaign scope has explicit MAGIC transport only. Do not call
  existing authored-v1 maps broken without transport evidence. Distinct unregistered
  six-case offer `build/logistics-map-transport-source1` (CPP c64f6176) characterizes
  writer/reader/startup loss separately from the direct-API exact-coverage rejection;
  custom valid ForcedMarch301 versus installed300 discriminates false round-trip
  comfort. Absent/empty/direct-null controls included. The separate overlay source
  proposal's11 first-hit quote bindings, fresh OFF test PCH/wrappers, compile flags
  and645-base-link identity were reviewed in map-transport-runtime-source-review1;
  actual executor/link argv and compile/native admission are still separate.
  Content then found unconditional teardown would erase failed VMAP evidence.
  Distinct `build/logistics-map-transport-source2` (CPP d52fdf12) retains the owned
  directory on HasFailure and reports its path to XML/stderr; successful cleanup
  and all six cases are unchanged. Source1/overlay remain preserved; future jobs
  must bind source2. Uncompiled/source-only; final20 integration payload unchanged.
  No product/format changes,
  no held-input edits, no compile/native proof. Phase B remains private disk saves,
  separately traced mod admission and fresh-Library/restart evidence, not memory
  or temporary-VMAP substitutes. Saved world/hero authority and generic map settings
  must be inspected separately.

- **Installed sentinel source2 compiled/linked; separate PCH witness closed:**
  build2 compile/link0/22.873s yields ea89122b. Runtime verified exact one-added-CPP
  link delta,348 actual headers and649 link inputs, preserving df14. A genuine gap
  was then found: the native-input fence omitted a precompile GCH hash. Witness1
  reproduced object2154 with explicit GCH pins but used foreground timeout, whose
  compiler-child timeout limitation was reported after its successful completion.
  Both qualifications remain historical. Distinct reviewed witness2 uses coreutils'
  owned group: actual outer/compiler0/17.210s,35725 equal pre/post entries,349 equal
  dependencies, object2154 byte-identical and bound by the existing ea891 link.
  `build/logistics-installed-pch-witness2-runtime-review.json` verifies this NEW
  prospective source/PCH/object/link checkpoint; no forced-timeout test, native2,
  installed-default gameplay or GUI claim. Tester owns the separate two-case gate.

- **Installed-v2 sentinel compile RED/repair:** source1 used unsupported
  BonusList::at(0) at line89. Distinct `build/logistics-installed-v2-source2`
  CPP66043b87 uses the declared const front() only after unchanged size==1 ASSERT.
  No oracle/profile/header/product changes; original737/source1/failed output and
  held source9/df14/284 remain intact. Source2 is uncompiled/unexecuted; Build owns
  its distinct overlay admission. Frontend's source-only spotcheck confirms generic
  family/text/icon consumer paths, but Logistics32/64 artwork is absent and mounted
  text/font-fit plus ordinary two-family choice/save/reload/dormancy remain untested.

- **Private full managed284 PASS:** actual outer/native0,273 completed +11 unchanged
  historical skips, XML6.305s/runner17.601s. Runtime independently matched the exact
  historical264 union repairedLogistics20, every skip name,35716 equal pre/post
  entries and df14fa9e executable in `build/logistics-managed284-runtime-review.json`.
  No installed-v2/default/bootstrap/GUI inference. Frontend notified of native
  readiness and still-open Logistics presentation/ordinary journey dependency.
- **Installed data seam reviewed, not executed:**
  `build/logistics-installed-data-source3-runtime-review.json` verifies five hashes,
  the original three data1 bodies, unchanged Artillery/default69 magic/all other
  settings, exactly six matching added texts and only a v1-or-v2 masteries schema
  seam. Local Draft4 three positive/seven negative controls pass. No generic merge
  change, default activation or artwork. Build owns the distinct TEST+18-resource
  profile and two installed-default sentinel cases; old-save/authored-v1-over-v2
  compatibility and integrated human/AI gates remain independent.

- **Repaired private Logistics20 PASS:** attempt2 native/outer0,20PASS/zero skips,
  runner11.727s (XML0.535s). Runtime compared exact source-derived case names,
  all completed statuses,35716 equal pre/post entries and actual df14fa9e body in
  `build/logistics-native20-attempt2-runtime-review.json`. Normal sight, zero-radius
  cap, genuinely hidden water and restored-visible AI controls all reached/passed;
  all three actual Nullkiller2 contexts passed. Original19P1F remains preserved.
  Full-world save test is in-memory, not disk GUI/restart. Broad284, installed-v2,
  full-family usability and whole redesign remain open.
- **Separate installed-v2 source gate prepared:**
  `build/logistics-installed-v2-source1`, new unregistered CPP737704ef/two cases.
  Explicit TEST bootstrap +18 resources/active vcmi-test; not normal-player LIB.
  Requires NH_REQUIRE_INSTALLED_LOGISTICS_PROFILE=1, reads actual engine v2 BEFORE
  loading, no mapLoaded/settings authorship, checks world/hero capture and actual
  Expert Logistics offer/authoritative Forced March/bonus/query drain. Fifteen
  quoted headers resolved to graph8; no held source9/284 input mutation. Build owns
  separate profile using data-source1 three files and separate compilation.
  This does not extend atomic merging or prove authored-v1/installed-v2 compatibility.

- **First actual Logistics20:19PASS/1FAIL/zero skips**, including all three real
  Nullkiller2 cases. `build/logistics-native20-attempt1/result.xml` fails the hidden
  tile precondition before its final AI assertion: HIDDEN correctly preserves
  owned-observer sight at the adjacent coast. No production visibility defect.
  Distinct `build/logistics-runtime-source9` (test CPP f8f979fb) retains normal
  sight as a control, applies a zero-radius SIGHT_RADIUS cap by GiveBonus, checks
  actual radius0 and hidden player tile versus authoritative WATER before the AI
  oracle, then re-reveals the same coast and requires Quartermaster again.
  Product/headers/wire/other tests unchanged; all19 predecessor/root hashes checked.
  Source9 is uncompiled/unexecuted. Build may review a single-test-CPP overlay
  using only verified private build3 header/PCH/object identities and exact include
  resolution; no copied root ABI or in-place source8/8b64/RED mutation.

- **Private Logistics source8 compile/link PASS, not execution:** frontload0/34.502s
  built three test CPPs + fresh test PCH; fullcompile3 then0/608.024s,889 remaining
  edges. Runtime independently rehashed test8b64e85f/client e6e2ddfe/facade65debdbd,
  all11 PCHs, four retained current-graph outputs, four generated inputs, root3
  binaries and4151 source files. `build/logistics-compile3-runtime-review.json`
  and `...-runtime-source-link-tail.json` verify884 compile outputs logged/present
  and eight exact link targets' object/archive inputs. Three unselected navigation/
  gtest_main/gmock_main objects are not requested consumers. Runtime's first link
  inspector overmatched gmock_main by rule prefix; its RED is preserved separately.
  Actual header-consumption/loader closure, native20/284 discovery/execution,
  installed-v2 and integrated UI gates remain pending. Build owns native-profile
  admission after the remaining dependency audit; no native invocation by Runtime.

- **Private Logistics compile2 RED:** actual exit1/570.695s, test CPP lines330/331
  used nonexistent `ETerrainId::DESERT`. Distinct `build/logistics-runtime-source8`
  changes only those two identifiers to canonical SAND (test CPP SHAa7a81a41).
  Core sand cost150 versus base100 and Expert Pathfinding75 + mastery50 preserves
  the stacked-discount clamp intent; base-cost and ROCK rejection assertions are
  unchanged. Source7 blocked() repair retained; all19 predecessor/root hashes
  checked unchanged, wire1 untouched. No native tests executed. Build owns the
  next distinct graph/rebuild; source8 remains uncompiled.

- **Private Logistics compile1 RED:** actual exit1/64.644s at
  `NewHorizonsMasteryEffects.cpp:53`, invalid use of `TerrainTile::blocked` as a
  field. Seven fresh PCHs but no final artifacts; no tests executed. Build reports
  35113 fences/root three binaries unchanged. Distinct `build/logistics-runtime-source7`
  repairs only that CPP expression to `tile->blocked()` (SHA36a537cd); all nineteen
  source6 hashes and root bases independently checked unchanged. Headers, test
  oracles, supplemental wire1 and prior graph preserved. Source7 is uncompiled;
  Build owns distinct graph/rebuild admission, then actual20/284 verification.

- **Private Logistics configure only:** Build's `build/logistics-configure1/summary.json`
  records configure0/2.014s with sanitized environment, absolute local GTest and
  PRE_TEST discovery. Runtime independently inspected the generated graph in
  `build/logistics-configure-runtime-review2.json`:887 compile commands in private
  directories,11 PCH entries, all three Logistics CPPs once and managed sources
  present. The test embeds private core/AI/Lua objects without a second facade;
  client links private facade/servercommon. Test POST_BUILD is a no-op; legitimate
  facade hooks recreate private resource links. No test/client executable or
  discovery result exists at inspection. Actual compilation, dependency consumption,
  transitive loader/output fencing and20/284 discovery/execution remain unproven.
  Build continues its loader/output review before bounded compile admission.

- **NON_GUI_PRIMITIVE1 writer2 coordination aborted; no primitive executed.**
  Runtime read actual `testing/default069-legacy-book1/native-primitive-writer2-deadline-abort.json`:
  metadata writer exit0, but approval1788882668.1012273 exceeded the final
  rendezvous deadline1788882664.9499702 by3.151s. Approval is unusable, no retry,
  primitive_invoked/attempt_present=false, all five holds explicitly released.
  Runtime authored only its own idle records and preserved the prior record on
  refresh. No native experiment, GUI, or gameplay acceptance follows from writer0.
  Logistics verification remains independently pending, not blocked by a claimed
  success or failure of a primitive that did not run.

- **DEFAULT051_D90_READBACK2 lifecycle/input gate completed normally.** Runtime
  read actual `testing/default051-d90-readback2/teardown.json`: exit0,
  client97.570s/session97.722s, complete exact readonly route true,192 clean
  samples,5418 unchanged controls, no save progression, no post-confirmation
  input/capture, and owned process/socket/runtime teardown true. Normal200/250
  flags are true. One actual session; prior expired GO attempts were prelaunch
  refusals. Subsequently read Tester's actual `offline-readback.json`: all eight
  screenshots reviewed, four click/key body pairs pixel-exact; saved21/28/7/14,
  mana10/14, movement1087/2028, leadership100/900, Expert siege and active Precision
  readback accepted. Runtime inspected the report, not a new GUI run. This remains
  outside SpellWindow/QuickPanel/private070/native-Windows/publication acceptance.
  Preserve READBACK1 exit130 and all coordination/refusal REDs.

- **DEFAULT051_D90_READBACK1 terminated without normal-exit acceptance.**
  Runtime read `testing/default051-d90-readback1/teardown.json`: exit130,
  client167.682s/session167.736s,330 clean samples,5418 unchanged controls,
  no save progression and owned process/socket/runtime teardown true. Exact
  route completion and normal250 are false; 200/300 are clock observations only.
  Tester reports normal bootstrap/5374/eight tabs before the close-hero ROI
  refusal; screenshot semantics/hover-ROI cause remain separate offline review.
  No bypass, no checked normal-exit or spellbook/private070 claim. Holds released
  only after actual teardown; publication remains held pending fresh READY/GO.

- **Latest private Logistics offer is `build/logistics-runtime-source6`:**
  19 files/18 proposed cases, all UNEXECUTED. Source6 only corrects a test's
  selector composition to `CSelector::And`; source5/prepared graph5 remain intact.
  Preserve source1..5 and their REDs:
  nonconst old-format version lookup mutated empty/float rules; crossover needed
  the same const inspection and legacy empty-envelope preservation; cached-path
  tests needed priming after level-up; hero choice application still checked
  Artillery rank and skill changes failed to refresh Logistics masteries. Source5
  fixes these last two seams; existing Logistics-only choice/dormancy oracles
  remain. No tracked gameplay/header/ABI change or native execution follows.
  Supplemental `build/logistics-level-wire-source1` offers two UNREGISTERED,
  UNEXECUTED tests for independent HeroLevelUp pre-gain flags, old-format flag
  clearing and rejected lossy downgrade; NOT part of the sealed19/18 graph.

- **Next default69 book fixture source binding:** original NHCommandsBooklessAI
  a9e0b31f authored2/2/3/10 retains custom HERO_BASE_SKILL values through init;
  default051 growth captures divisor10 and initializes manaLimit=>10, not the
  historical exporter assertion100. Actual modulev1/69 gives Haste/MagicArrow
  Sorcery1 with rank0 cost4; Bloodlust Chaos inherits loaded base cost/level.
  Pathfinding-only/book+Ballista and Gold starting bonus introduce no school or
  mana modifiers. Bind live battle cost/availability; assignment spends nothing,
  one legal Haste/Arrow cast should leave6 mana and consume shared hero action.
  No MAGIC override, new Missile or ordinary-book/cast acceptance inferred.

- **Next Logistics family is PRIVATE source-only, not executable evidence.**
  Explicit lease produced readonly `build/logistics-runtime-source1` (19 files,
  base hashes/diff/contract), paired with Build's `build/logistics-data-source1`.
  Stable effects3/4/5 add land300MP, the full existing ship-boarding capability,
  and flat50MP terrain discount. Boarding still pays the step cost, scales across
  land/sea caps, and retains the airship exception. Two-family pre-gain latches,
  version-gated saves/crossover, sequential queries, skill-owned bonuses/dormancy,
  and visibility-filtered AI are implemented in private copies only. Four state
  plus ten gameplay/AI cases are authored, **UNEXECUTED**. Root/d90/default051
  code and version remain unchanged. Next: Build source review/fresh private
  header-dependent graph and native regressions, not old-root object reuse.
  Tests author v2 under baseline installed v1; this is not installed-v2 bootstrap
  acceptance. Generic MASTERIES override merging remains unchanged; separate
  profile/isolation review is needed before old v1 fixtures run atop installed v2.

- **Portable ordinary seed under normal LIB preset GREEN.** Runtime read
  `magic-ordinary-export1-normal-bootstrap/summary.json`: two fresh CPPs/link/native0,
  1 PASS/0 SKIP,14.518s. Map45edc8d2b1f7ed621a36ccf0683acce65141aaa530813b78da728b1d1eb82ab7;
  exebf6b9668ae908f099d657184b9ce188999ca54f5e950b0429ca2536cbbb450c4.
  Prior b6bb map referenced four vcmi-test heroes and remains limited to that native
  registry. New exporter removes test heroes BEFORE writing, scans every written
  JSON key/string and asserts actual active mods/defined hero+creature registries
  contain no vcmi-test, retaining70/emptybook/SP24/guild/army/path assertions.
  Preserve the intervening pre-test RED: useTestPreset=true mounts/forces vcmi-test
  despite preset contents. Approved PRIVATE CVcmiTestConfig copy uses normal
  initializeFilesystem(false,false), replaces the original explicit object, and
  runs only this SOD exporter. No product bootstrap/ABI/assertion weakening.
  This normal LIB bootstrap is NOT actual client GUI execution. Initial paths only;
  no sequential movement/learning/cast/save acceptance. Build's new private949
  player plus portable map is offered separately; no GUI GO inferred here.

- **Widget registry-negative remains disabled.** Source review found the existing
  shared interface mutex around SDL dispatched callbacks and network dispatch,
  but unlocked/detached AI paths and raw BattleInfo lifetime preclude blanket
  approval. `research/quick-spell-roster/runtime-callback-synchronization-review.md`
  (under build evidence) states conditional protocol/evidence requirements. No
  registry mutation or guessed lock/thread disabling was performed.
  Separate positive-widget stop review found a real source defect: old overlay3585
  released book/callback/BattleInterface before acquiring the cleanup mutex while
  NET was live. Current source36dd9fed/headera99caa9c/checker255a9118 implements
  the reviewed split: revoke/bounded reader join without GUI release at cleanup
  entry; release under the EXISTING interface lock AFTER endNetwork returns
  (network joined and lock reacquired), before endGameplay/window/GAME/ENGINE
  teardown. Missing protected release is fatal rather than unsafe destruction.
  Runtime reviewed these exact sources, not C++ execution. Early-quit token
  revocation before confirmation and actual queued cancellation remain required;
  no GUI/negative/icon acceptance follows from source review.

- **Ordinary Missile exporter seed/path gate GREEN, not acquisition.** Runtime
  read `magic-ordinary-export1-authoring-callback` summary/XML: compile/link/native0,
  1 PASS/0 SKIP,12.459s. Map b6bb981cd2fd9f87b85f853c5483cf58995826b5e84206964a70a36fce45b044;
  exe74a6b13edfab39041b566dbb02299b5ed22c1907d4b965ca7e2007c744c029d5.
  Fresh empty spellbook/SP24/divisor10/actual70/default-no-override/built mandatory
  guild and exact armies passed. Recorded hero anchor(10,10), visitable(9,10),
  movement1560; guild anchor(8,10), visitable(6,10), initial route remaining1178;
  neutral anchor/visitable(14,10), initial route remaining1060. Both routes turn0,
  respectively VISIT/BATTLE, but NOT a sequential post-guild route.
  Preserve initial private/shadow API compile RED and writer artifact-lookup SIGSEGV.
  Test-only repairs use public APIs/qualified actual army slot, then the existing
  EditorCallback authoring lifecycle (callback outlives map/setMap before writer).
  They do not remove the spellbook or weaken seed assertions. Real fresh-game
  initialization still uses production autodetection and game-state callback.
  Build is assembling a separate private player candidate; no ordinary learning,
  cast, postbattle save/restart, GUI/default/public release acceptance yet.

- **Coherent47 committed by Build as d90c2ea7ae80456eae06f17f7286cf8debd8e705.**
  Runtime read actual commit parentdb2f6d947fe0a8b07ecb12715bc29df34a9dc496 and
  tree459472032415e4df2298bdb5e4c979bddf56f04c. EOF-only repair had its own new
  ON264 retest20.330s/test362b31a6ac3b5fe46ae37f7ce1b792f466782c1d15c11df05e5b7c22f31f22de;
  separate OFF234 restored a510. Old compiled identities were not relabeled.
  Tester verified actual47 index/commit. Build reported push and one Windows FULL
  run34193282905 with terminal watch; outcome remains pending here. Windows85
  prior source checks are not clean-d90 or native Windows runtime acceptance.
  Default0.5.1/public413/old950 remain unchanged. Ordinary exporter-paths source
  is independently reviewed but UNREGISTERED/UNEXECUTED; Runtime requested the
  next separate bounded compile/export lease, not an inferred export/GUI GO.

- **Integration5 actual registered ON/OFF gates GREEN.** Runtime read both
  summaries: ON264=253 PASS/11 SKIP,27.751s, actual root test40a4e6090a34a149220f93594923f387439bb041f01dae9b3df2f625a855c9be;
  OFF234=223 PASS/11 SKIP,10.016s, root test restoreda5105a3e042c299d62e2e5476f61ab332408a8796cbb842ae8536f2b1f3b76ff.
  Both configure/build/native0. Tester independently verified actual option/cache,
  generated-source overlays and extra-test presence/absence, not a native rerun.
  No default-content/player/GUI/Windows or checkout fixture reproduction claim.
  Source47 integration review is Build-owned; Runtime makes no commits/ABI edits.
  Approved independent ordinary exporter is now sealed as
  `managed-missile-ordinary-exporter-source-paths`, UNREGISTERED/UNEXECUTED.
  It requires separate export flag/path, actual70 default/no magic override,
  observes fresh empty book/SP24 (2.4 legacy units), mandatory friendly guild,
  computer-only Blue header, exact armies/coordinates/neutral flags and two initial
  path checks with actual visitable positions/movement records. These paths are NOT
  sequential post-guild movement. Future GUI scope is ordinary learning/casting and
  POST-BATTLE save/restart, not active-battle full save. No export/GO has occurred.

- **Narrow assertion-enabled GameSettings probe GREEN.** Runtime read actual
  `magic-null-assert1-local-static/summary.json`: fresh two-CPP macro/compile and
  object/executable/dynamic-symbol checks0; positive0, invalid-other SIGABRT(-6),
  core limits0/0,7.576s; exe e6eed8d8084b1fa74c5e27930e6d314c849430b4c634c300a1333d59fde49ea8.
  The prior probe double-free RED is retained: duplicate executable/facade static
  data interposition required probe-only static-data localization, not a production
  logic repair. This exercises the nullable-MAGIC getValue branch and retains the
  other-setting assertion. Not full Debug, GUI/default or Windows acceptance.
  Holds released, but transport/header edits still require a new lease. Build next
  owns default-OFF/opt-in-ON test registration gates and coherent source integration.

- **Private264 GREEN, Runtime read actual summary/XML.**
  `magic-managed264-native1`: three fresh extra compilations/link/native0,
  39.931s,264=253 PASS/11 baseline SKIP/0 FAIL; all30 extras executed.
  Exe b1db7060dcf4f98cb119ac1c993bd96eb2e5a5a5d53df41a34c2e5bbc7f1c7ae,
  data seal d5c0e05af1886243688769fdc7033187c2ad02c1eb9371ac3801740e0f6b5f71.
  Actual authored11 now passes full-v1→exact69 under unchanged installed70,
  absent70, null legacy, v2/copy, version gates, field schema, JSON/binary presence,
  both-reader malformed/partial rejection, schema-valid missing-formula header
  acceptance then runtime rejection, and unchanged other-setting behavior.
  Every prior source/native RED remains preserved. This Release-profile gate does
  NOT execute the assertion-enabled getValue branch or establish player acquisition,
  GUI/default/full Debug/Windows acceptance. Transport headers remain held for the
  separately offered narrow assertion-enabled GameSettings probe; source33 index
  is still old/paused. No ABI edits before that gate.

- **Integration4 full ABI graph/default234 green; private264 and assert probe pending.**
  Runtime read `magic-map-transport-integration4-reader-validated/summary.json`:
  configure/build/native0,234=223 PASS/11 SKIP,538.260s, protected/input flags true.
  Root facade d809c0ba3039fb988164c2f7a523b4218f481ddb8fb2300f2b8a3e8c08f8cd52,
  test a5105a3e042c299d62e2e5476f61ab332408a8796cbb842ae8536f2b1f3b76ff;
  client remains4a4f6cbb7bb265b3ca46b29a76c542637d84348040fb4caf1f1256f7b5d15d19.
  This is default69 regression, NOT executed authored null/vmap coverage.
  Final immutable transport6-reader-validated includes named field-shape validation
  in shared readHeader after version checks and before either reader continuation.
  Prior unexecuted6/9/45 offers and source-review race RED remain preserved.
  New authored11 tests add actual malformed/partial header+full-reader rejection and
  schema-valid missing Missile formula: header accepted, strict runtime capture rejects.
  Private264 must recompile all three extras against new ABI/data; no old private
  objects. `magic-null-assert-driver-source` separately requires assertion-enabled
  current GameSettings.cpp without Release PCH, explicit-null exit0 and separate
  invalid-other SIGABRT/core dumps disabled. It is not a full Debug build claim.
  Full hold released; header/transport remain held pending these subsequent gates.
  Source33 old index is paused, with no default/player/GUI/commit acceptance.

- **Integration3 default234 green; actual private256 exposes vmap transport RED.**
  Runtime read private256 summary/XML:243 PASS/11 SKIP/2 FAIL, compile3/link0,
  native1,37.018s, exe280ff57f9c6e27adf82d274c5c7bac8b48ba55ebe28b5f7ebf170a5bdf05fbd7.
  Underlying253 is242 PASS/11 SKIP, including all managed19; mastery flag restored.
  Only authored-v1 equality/exclusion and partial-rejection fail; absent70 passes.
  Initial authored3 source used the H3M-only mock incorrectly; preserved source RED
  and replaced only vmap reads with actual CMapService autodetection. That real
  entrypoint exposed missing writer/reader transport, not solved by atomic override.
  No postrun raw-header claim: its temporary archive had been removed.
  Postterminal authorized `magic-map-override-transport-source6` now implements
  MAGIC-only explicit-presence/null handling, copied optional getters in GameSettings
  and CMap, null-aware JSON/binary overrides, and nullable getValue assertion only
  for MAGIC. MapFormatJson emits ONLY authored override: present→major4 including
  null, absent→major3/no installed snapshot. Reader supports<=4 and rejects new
  field under older format. Old readers are NOT claimed compatible with major4.
  New `magic-authored-map-transport-source9tests` preserves original3 and adds actual
  written-header inspection, null/v2, version checks, named field schema probes,
  binary absent/null/object and other-setting controls. These new sources are
  UNEXECUTED/UNREGISTERED; header ABI requires FULL fresh graph rebuild, not prior
  private-object reuse. Build owns field schema and compilation. Source33 commit
  remains paused; no player/default/release/GUI inference.

- **Private managed19 hex-fixed GREEN, broad253 RED retained.** Runtime read
  actual hex-fixed summary/XML19 PASS/0 SKIP, compile2/link/native0,25.628s,
  exe5a7014acc7e812e1b1bc4002ff0104dd8458987ea60392063c411cf4ba080a6c.
  Actual evaluator selected canonical Missile and submitted hex; resolving its
  occupant established enemy identity, then ORIGINAL const action reached server:
  19820 damage/exact5mana/shared budget PASS. Prior18/1 RED was the test's invalid
  unit-pointer-only oracle, not bad-target proof. Managed17 (including actual70,
  full-world load/resave and manual68/5mana) passed. Tester independently inspected
  producer artifacts and624 reused link bodies; not an independent native rerun,
  ordinary acquisition, active-battle full save, player GUI/default or Windows.
  Subsequent actual broad253 XML:224 PASS/12 SKIP/17 FAIL. Fifteen failures expose
  generic deep-merge of v1 map fixture overrides over installed70; AI's installed
  version1 assertion and wrapper's default-only assumption are separate failures.
  Extra mastery-text skip is runner flag omission, not accepted new coverage.
  `managed253-profile-fixtures-source6` is UNEXECUTED test-only isolation/profile
  repair: explicit canonical69 baseline RAII in three fixtures; installed AI and
  wrapper keep strict default assertions with explicit private sentinel branch.
  This MUST NOT substitute for fresh authoredv1map-under70 compatibility. Separate
  product lease proposed for MAGIC_NEW_HORIZONS atomic override in GameSettings,
  with real authored-vmap→CGameState.init test. No product edit yet. Explicit-null
  authored-map persistence omission is a separate visible issue. Old33 source seals
  and every prior RED remain intact; integration/commit coherence is pending.

- **Consumer integration2 translator-fixed: actual234 =223 PASS/11 SKIP/0 FAIL.**
  Runtime read summary and XML at `magic-consumer-integration2-translator-fixed`.
  Configure/build/native0; baseline reward/guild4 and both command AI tests pass.
  Original independent f562 command26 RED was BEFORE AI choice: raw99 yielded842
  versus required>2500. Approved test-only repair retains100vs100 Angels and all
  strength/nonlethal/actual-AI/server/budget assertions. XML now records raw99,
  actual divisor10/effectlevel0/damage842, then accepted rating990 for99 effective
  units. Production balance/AI unchanged; this does not replace legacy-context or
  player acceptance. The first integration2 compile RED (missing MetaString translator)
  is retained; baseline4 and future17 received explicit staticTexts argument only.
  New root client4a4f6cbb7bb265b3ca46b29a76c542637d84348040fb4caf1f1256f7b5d15d19,
  facade3070c532b60740a926ab73d69e7a02fb5b845c7e01dec46ebbeda03486c86223,
  test5fec2b09a260166e7db18ac05036ea435c6c2455034eda94a518ac2986c1a829.
  Tester independently reviewed producer artifacts/22-source overlay, not a rerun.
  Compile hold released. Guard admission review now precedes Build private70 composer;
  NO import/default activation/GUI/Windows claim follows234.
  Held future17-translator-fixed and actual BattleEvaluator AI2 offers remain
  UNREGISTERED/UNEXECUTED. AI2 requires actual Missile and sentinel; positive chosen
  identity/target→server19820/5mana and old69 forced-book exclusion→command, not
  manual-cast substitution. Existing managed17 damage68/5mana controls preserved.
  New unregistered admitted-level0 guild test distinguishes roster admission from
  bounds checking; baseline NONE test alone did not establish that branch.

- **Full registered integration204 green; follow-up reward/guild guards ready.**
  Runtime read callback-fixed summary and actual XML204=195 PASS/9 SKIP/0 FAIL,
  configure/build/native0. This newly linked actual client/facade/test targets, not
  merely the earlier replacement executable. First consumer-test callback constness
  compile RED preserved; narrow mutable-callback repair uses no const_cast/API change.
  Old950 remains separate. New root client d0f71a77e464d3ab3dbbd6d43da0df4751a058e90d541909a344565391704168,
  facade5ccca3ab81074b4a667c28178829e38f7ae0633d83e1f9f38f6771da787eafb8,
  testf5627b19158bd5c51368cddd5d0eeecdc9ff979aee2c78a0d1ab627119785734.
  No managed spell import/default activation follows.
  Subsequent approved `magic-reward-guild-guards-source4` is UNEXECUTED: named
  JsonRandom candidates recheck roster without losing original map-ban overrides;
  scalar NONE remains absence, arrays reject unavailable members rather than weaken
  reward/limiter requirements. Info spell variables reject before publication and
  invalid text IDs fail before name dereference. Mandatory/possible guild entries
  check admission and level bounds before indexing. All scalar source callers traced:
  arrays, guarded spellCast.NONE, and variable publication/text. Reward scroll path
  stores supplied spell ID directly; no random fallback found in that traced path.
  NEW managed17 future suite requires explicit sentinel and actual registered70,
  remains UNREGISTERED/UNEXECUTED; includes valid69/null/v2/load/resave/conflict,
  exact mana and AI effect/server action, reward/limiter/variable/guild controls.
  Actual AI candidate selection and broader integration remain outstanding.
  New category full-load-entrypoint2 is separately UNREGISTERED/UNEXECUTED, not
  part of204. Old source offers and immutable37 snapshot preserved.

- **BATTLE4_LAYOUT forced teardown RED retained.**
  Runtime read teardown:284.308/session284.730,561 clean samples, protected checks
  true/no saves/PIDs/display. Normal exit checks are FALSE; no200/250 PASS. Numeric
  elapsed time is below300 separately, not successful normal teardown. Card dispatch
  is not yet pixel acceptance. Build explicitly safety-released; authorized Runtime
  source work resumed. Do not convert cleanup into card/GUI acceptance.

- **Saved-roster query3 and consumer9 source-ready; execution pending Build.**
  `magic-roster-query-source3-explicit-id` preserves initial query3 and fixes the
  mixed enum/SpellID initializer before execution. Four query cases UNEXECUTED.
  Exact public copied-bool APIs in NewHorizonsSpellAvailability.h:
  spellAllowedByWorldRoster(const IGameInfoCallback &, SpellID) and
  spellAllowedByBattleRoster(const CBattleInfoCallback &, SpellID). Frontend read
  declarations and authored separate source-only cache/prelookup/showAll guards.
  `magic-roster-consumers-source9` adds eight UNEXECUTED consumer cases and guards:
  non-NH common coverage retained, absent new NH content exempted, every present
  NH common row requires v2, scoped Magic Missile requires saved directDamage;
  no book/SPELL/school/level grant or allowBanned bypass, empty excluded schools,
  safe invalid IDs, map enumeration/common-cast/NK2 guards. No Hero header API
  addition remains. All12 paths outside37; green ISPELL damage seam exact.
  Adversarial removed-core query contexts are explicitly invalid full saves;
  bonus fixtures are not ordinary artifact acquisition. New managed-identity
  profile/import, actual NK2/AI selection, reward/guild and old-save breadth still
  require their own integrated gates. Build owns full registration/new independent
  fence/build, preserving old950/37. No activation or whole-roster claim.

- **BATTLE4 actual battle/quit route, cards unexecuted.**
  Actual teardown independently read:170.800/171.213,337 clean samples/all structural
  fences true/savesempty. Build verified release; authorized source work resumed.
  Ordinary pursuit reached battle; prepared gear layout mismatch prevented cards.
  Keep that preparation RED, not card/product PASS. Actual Options/desktop/mouse
  quit route reported separately. World help/minimum viewport remain outstanding.

- **Private common-mechanics12 green; spell import still prohibited pending roster gates.**
  Actual magic-mechanics-private12-lifecycle-fixed summary/log/XML inspected:
  compile/link/native0,12 PASS/0 skip, source/input/protected controls unchanged.
  Immutable test SHA a58e20811f247537fe2b98730acf6f90bc0b72fa245fc6ed34c4e466260eedc3;
  private executable c0ce9ffedf55f0b655d18e8d4386906877951d1e1844c4c990c69932a7a060fe.
  BaseMechanics uses explicit event override incl0, once-read nonzero legacy caster,
  saved BATTLE formula incl0, then original raw fallback/clamp. Real hero divisor10/
  power24 yields68 through actual AI effect prediction and authoritative action;
  prediction leaves real HP/mana unchanged, second action rejects. Mana assertion
  proves decrease only, not exact charge. Passive proxy controls cover overrides,
  negative clamp, divisor1, absent formula and incoming battle/world conflict.
  Preserved REDs: profile permission setup; proxy-in-HERO SIGSEGV (actual cost path
  requires CGHeroInstance); private12 and diagnostic12 each10 PASS/2 FAIL for incoming
  HP0/maxHP1/invalid target despite raw250/68. Test-only production localInit lifecycle
  repair gives HP10000/maxHP10/alive while raw250/68 stays unchanged; restores original
  army.battle pointers after incoming destruction without reinitializing original DAG.
  Environment/target consistency cleanup is NOT separately proved causal (hypothetic
  environment returns its owner). No production formula fault inferred from these REDs.
  Diagnostic terminal predates later test edits by25s; immutable offers preserved.
  No shared-target/player rebuild, new Missile identity import, AI spell selection,
  full CGameState load, GUI or full-design acceptance follows. Next: saved-roster
  policy/consumer gates before any new spell import, with exact ownership intersections.

- **Future magic primitive and named schema gates; v2 runtime source offered.**
  Strict DATA_INTEGER primitive amendment preserves the initial source offer and
  adds integral-FLOAT20.0/null/true-integer bounds controls. Runtime independently
  parsed include-fixed primitive XML8/0FAIL and exit0; initial missing-Iinclude
  standalone setup RED retained. Build reports named schema5 PASS via standalone
  warning-policy harness (missing-Ilib/header-warning setup REDs retained), plus
  named30 probe/offline5 after fixing native formula-null acceptance. These are
  not casting/AI or full-save gates. Authorized NewHorizonsMagic.h/.cpp and NEW
  NewHorizonsMagicV2RulesTest.cpp now sealed under magic-v2-runtime-rules-source3:
  seven tests initially UNEXECUTED. Subsequent standalone combined20 and regression27
  XML independently inspected clean; regression build/run exits0. Regression27 covers
  new rules7 + primitive8 + named schema5 + old magic3 + old schema4, no skipped tests
  reported. Build's first unused-parameter/Werror harness RED remains preserved.
  No shared-target, roster import, casting, AI or full-save acceptance follows.
  Optional copied formula/value access uses supplied saved
  scoped spell identity, not installed formula defaults. Existing installed-common
  coverage remains unchanged: old-snapshot/new-installed-spell policy and all
  availability consumers must be addressed before importing/activating Missile.
  Explicit event OptionalValue64 zero must short-circuit formula evaluation;
  legacy numeric caster zero still means absence. No mechanics/CMake/default edit.

- **NAV5374 first guard RED and distinct strictINTERIOR bounded teardown.**
  First pass refused tab2/key1 before dispatch; no four-tab/Precision acceptance.
  StrictINTERIOR retry reported all eight guarded dispatches; actual screenshot
  content acceptance remains pending. Runtime independently read teardown207.617/
  207.743,409 clean samples/all structural fences true/only unchanged5374 input.
  Target200 MISSED, mandatory250/hard300 met. Build verified/released pause; no
  progression/battle/new-save/overflow/full-goal claim. Frozen37/950 unchanged.

- **FASTSETUP WORLD4 partial GUI gate; next spell primitive source started.**
  Tester/Build viewed actual20Pixie Core/20AirElemental Elite/2Phoenix Champion/
  100Pikeman no-row cards and Core description+source/version help. Runtime read
  actual teardown: exit227.826/session228.019,449 clean samples, all controls exact,
  savesempty. Target200 MISSED, mandatory250/hard300 met. No Elite/Champion help,
  battle, navigation, legacy-mapped fallback, restart or minimum-viewport claim.
  Build explicitly released GUI pause while keeping37/950 frozen.
  Accepted separate future primitive lane now adds ONLY three new unregistered
  files: lib/spells/NewHorizonsDirectDamage.h/.cpp and
  test/spells/NewHorizonsDirectDamageTest.cpp; immutable source offer under
  magic-direct-damage-primitive-source. Eight tests UNEXECUTED. Optional v2 formula
  parsing (strict v1 rejection), copied bounded base/coefficient, widened evaluation
  and invalid input rejection implemented. Existing37/CMake/config/default/casting/
  AI untouched. New helper is not yet the live spell API; saved-roster integration,
  actual effect/override precedence, new spell registration and AI remain pending.

- **Current category foundation0afc38 and private0.6 gate, with GUI still open.**
  Independently confirmed HEAD0afc38f09f5e391dcfdb4f6af1f3fa0eea77e987 after exact37
  staged-path/hash review. Private950 remains its actual base83+declared source
  identity, not relabelled as a rebuilt commit. Exporter compile1 (private commander
  access/default PathfinderOptions constructor) repaired only through public
  getCommander()/PathfinderOptions(*gameState()), preserving the original37/RED.
  Actual private0.6 exposed the partial3-row fixture merging installed14: scoped
  StateTest RAII isolation cafbf4 retains valid Sprite absence, adds exact3-row/JSON
  assertions; no production merge change. Isolated37 build0/current-copy hashes
  verified. Actual category060-isolated-all-new-horizons.xml160=152PASS/8skip exit0
  independently parsed; forced mastery text and actual ordinary export belong to
  that qualified run, not the earlier RED. Ordinary map/source/English assertions
  have native coverage; no ordinary card acceptance yet.
  First WORLD4 GUI setup guard rejected Begin before dispatch; no game/cards/save.
  Independently read testing/category060-world-gui/teardown.json: exit179.407,
  session179.874,354 clean samples/all950/37/assets/map controls intact, savesempty.
  Build released GUI pause but retains frozen inputs. Separate faster setup/freshGO
  required; no Runtime product defect inferred. Next Magic Missile/saved-roster
  family remains a private proposal. Build schema alignment acknowledged: envelope1,
  ruleset2, v2-only directDamage integerbase/coefficient0..1000000; widen arithmetic,
  positive divisor and override precedence. No current activation/source37 change.

- **Category/native25 + both controlled wrapper negatives verified.**
  Initial future36 build1 fixture RED: nonexistent PIKEMAN enum and incomplete
  CObstacleInstance/CampaignState. Original36/log retained. Authorized test2 repair
  uses canonical decoded/validated pikeman IDs and full serializer types; fixed
  build0 linked actual client/test, all36 hashes exact. category-native25.xml25PASS,
  no failures/skips, exit0; registered NAV CTest1/1 exit0. No GUI implied.
  Independently inspected category-world-negative-* and category-battle-negative-*
  phase exits/XML. Each negative build0/native1 gives exactly its named wrapper
  failure with the other case passing; each exact restoration/fullbuild0/native0
  gives clean2. Current36 and all three restored binary hashes independently match.
  World header927392c2 restored; battle930e6b3a restored; final vcmitestec65b78c,
  facadea98e5d01, clientdb04749a. Same facade across negative/clean is not unexplained
  production proof: vcmitest embeds internal sources; malformed consumer is direct
  wire.iser & target in test TU. loadFromMemory only primes valid prior state here.
  These are discriminating wrapper tests, not malformed full-save entrypoint proof.
  No production bug, GUI, release change or full redesign completion inferred.
  Next: Build broad regressions/private0.6 integration and separately authorized
  ordinary exporter/GUI gates; later actual malformed loadFromMemory coverage.
  Authorized light-only next-family/fixture proposals are in research under build:
  runtime-next-family-plan.md (Magic Missile + saved roster/formula) and narrower
  category-ordinary-fixture-draft.md (four slots, no category overrides/queries).
  Drafts do not authorize product edits, exporter or GUI; legacy mapped-Pixie gate
  needs a NEW normal immutable413 save -> fresh0.6 load, never a5374 rewrite.

- **Packaged413 fresh5374 readback PASS at actual package scope.**
  Independently read testing/linux-413930-readback/summary.json: engine413930,
  packaging83cf5443e8ce11b87288297722bb32a3b3023633,1161-file manifeste79a1b74.
  Fresh5374 -> OrrinL3XP2000/eight Experts/100Pikes+Ballista/Precision ACTIVE;
  base=total21/28/7/14,last3/4/1/2,mana10/14,MP1087/2028. Actual Quit102.331..102.508,
  confirm102.891..103.069, normalexit103.097 before200/250/300;203 clean samples,
  exact teardown/package/maps/save/future-source controls unchanged. No new save,
  battle effects, AI, shortcuts, future UI or Windows runtime acceptance inferred.

- **Future creature category context lane authored; SOURCE ONLY, not413.**
  Explicit post-seal lease covers19 Runtime paths in immutable
  build/new-horizons-linux/category-context-source-review19/{identity.json,files,
  paths.txt,contract.json}. Nine primitive/binary plus nine context tests are
  UNREGISTERED/UNCOMPILED/UNEXECUTED. Build owns schema, opt-in data and registration.
  World getCreatureCategory(CreatureID) and battleGetCreatureCategory(CreatureID)
  return optional copied category/text/source/version views. Typed world/battle
  snapshots use NEW_HORIZONS_CREATURE_CATEGORIES after MASTERIES; old absence clears
  existing/constructor capture, with no installed/world fallback. BattleProxy
  forwards the real battle for AI. Entire entity table validates before publication;
  loaded category candidates validate before replacement. Invalid positive/negative
  IDs and unmapped canonical entities return null before unsafe dereference.
  Tests include literal different world-callback/battle category+source identity
  through actual HypotheticBattle (adversarial callback, not a GUI journey), RAII
  installed-settings replacement, primed old-world/old-battle clearing/resave,
  failed-world all-or-nothing capture, implicit-scope alias rejection and immutable
  tier/attack/upgrades/army/leadership assertions. No scoring or recruitment change.
  contract.json is REVIEW METADATA, not drop-in config: six proposed category text
  IDs and fourteen explicitly inspected Conflux keys; Firebird Champion provisional,
  no complete-roster approval. Three fixture rows stay test-only. Frontend/Tester
  received API/source offer; no category UI wiring authorized. Earlier unregistered
  draft notes are historical, not the current integration state.
  Separately inspected sealed413 Linux release build exit0 and698/698 client link;
  no install/package/new-binary GUI or Windows result inferred. Next: Build-owned
  release gates first, then future schema/registration/native source review fixes.
  Separate requested addon: test/creatures/NewHorizonsCreatureCategorySchemaTest.cpp,
  SHA0a5708e17714b6fc7f56f275cb67e35a4e7bfedc488f55f5eb6b1acecf150602,
  five additional UNEXECUTED native tests against the actual named config/schema
  and real gameSettings wrapper. Positive/empty and malformed nested negatives;
  unknown entity-key shape deliberately remains schema-valid and separately fails
  Runtime capture. The19-path review copy is unchanged; Build registration pending.
  Tester identified missing current-wire entity-rejection discrimination. Separate
  NewHorizonsCreatureCategoryWireTest.cpp addon (SHAfbbedc77c303199559deb24706da086976e3a3447fa6606a1c7d792df1d83640)
  now authors two UNEXECUTED actual world/battle serializer/loader tests: replace
  exactly one category payload with structurally valid unknown-entity input, check
  exact entity error and prior category JSON/view preservation. Not whole-world
  rollback. Requested Build-only separate world/battle load-guard mutations and
  exact restoration; none executed. Requested later test-only diagnostic tightening
  of InvalidWorldTableCannotPublish; original19 source remains unchanged meanwhile.
  Independently reviewed Build category-build-source-review9: nine current/copy
  hashes and defaultb770 match; actual schema/data/texts/composer/registration diffs
  align with the source contract. Source-scope ACK only; reported offline30 is not
  native proof. Schema/real-wrapper tests now have actual files to load when built.

- **Fresh5374 saved Precision readback PASS; activation integrated.**
  Independently read testing/mastery-precision-l3-readback/summary.json: same947
  fresh L3 XP2000/Expert Artillery+7 Experts/100Pikes/Ballista, Precision ACTIVE with
  distance+wall exclusion and remaining-restrictions description. Base=total21/28/
  7/14, last3/4/1/2, mana10/14, MP1087/2028. No progress/choice/new save/effects/AI.
  Quit168.695..168.872, confirm169.253..169.431, exit0 at169.511;334 clean samples,
  exact teardown and all source8/candidate/map/save controls unchanged. Earlier
  deadline RED retained. Actual HEAD413930bc32d0f8a7e56342a55084d816ae09e0d3,
  eight committed activation paths and defaultb770 hash independently verified;
  Build reports push/staged identity. Next Build freeze is413930 Windows FULL/cloud
  and Linux release build/audit;947 is not rebuilt/relabelled. Remaining ordinary
  AI/effects, platform and full-family requirements are not claimed complete.

- **Default0.5.1 activation build/native identity independently verified.**
  activation051-build exit0 links client/test; all eight current/review-copy hashes
  match activation051-review8, and default module is BYTEEXACT947 b770f6b4.
  Actual activation051-all-feature141=139PASS/2skip; future61x2 each58PASS/3skip;
  prior128=126PASS/2skip and39=38PASS/1skip, every exit0/no failures. No Runtime CPP
  or category integration accompanies this activation. Build's earlier two Python
  fixture REDs/25-repair scope remain distinct from these actual native gates.
  Fresh saved5374 Precision readback/ordinary AI/effects and Windows coherent FULL
  gates remain separate; no whole-redesign acceptance or947 relabeling inferred.

- **Corrected minimal ordinary L3 choice/save gate PASS, scoped and timed.**
  Independently read testing/mastery-l3-minimal-protocol/summary.json: fresh aaea
  HUD -> ordinary second Seer/L3 -> explicit middle Precision Select/Confirm at
  141.8..142.2 -> HUD21/28/7/14 -> successful normal NEWEXPERT-L2-ne3 save.
  Actual677850 bytes SHA5374a51331153f7105b93fa36799b7e85e1e28f4dfb3ed5851d5b3beb4dcffd1,
  readonly precision-l3-control retained. Entry150/choice-save230/quit300/hard450
  limits met; soft250 quit target MISSED. Per-action Quit259.460..259.636 and
  confirmation260.017..260.194; normalexit0 at260.346,513 clean samples/exact
  teardown. Initial wrong filename assertion and post-exit identity assertion
  blocking trailing wait preserved; not save or gameplay failures. Prior mandatory
  deadline RED remains untouched.947/all earlier controls unchanged. No optional
  post-choice readback, fresh L3 reload, effects, AI or battle acceptance. Next
  required separate gates: fresh saved Precision readback and ordinary AI/effects
  scope; full redesign/category/spell/mastery breadth remains unfinished.

- **Fresh L2/L3 GUI is partial evidence with mandatory timing RED.**
  Independently read testing/mastery-newly-expert-help947-reload/summary.json:
  fresh aaea L2 XP1000/eight Experts/no chosen mastery/future eligibility and
  18/24/6/12 readback verified; second ordinary1000XP -> L3 gains3/4/1/2 -> three
  mandatory, unselected mastery cards observed.300 guard blocked planned choice
  at315.5. Cleanup batch372.873 resolved Precision solely to clear modal and quit;
  actual Quit/confirmation individually UNTImed, necessarily within372.873..374.585
  and AFTER mandatory350. Exit0 at374.585; stale400/450 helper banner was not an
  extension. Late cleanup choice is NOT a clean Precision gate. No L3 save or
  post-choice readback, battle/endturn/help/ACK-race acceptance.739 clean samples,
  exact five-process/socket teardown; only unchanged676018-byte aaea input remains;
  947/old947/925/dee/e5/ecb/maps controls preserved. No Runtime defect established.
  A new authorized, narrower L3-choice/save journey is required; do not resume or
  relabel this expired attempt, or repeat already-proven readback at its expense.

- **Ordinary newly-Expert StageA verified at bounded GUI scope.**
  Independently read testing/mastery-newly-expert-help947-first/summary.json:
  L1 Advanced Artillery+7 Experts -> ordinary Seer1000XP -> L2 gains3/4/1/2 ->
  sole Expert Artillery. Actual development shows no mastery chosen/future-level
  eligibility/no awaiting text (not direct serialized-pending inspection).
  Base=total18/24/6/12, mana10/12, MP1628/2028, capacity100/825, Ballista x4.
  Normal NEWGAME-ne2 saved676018 bytes,
  SHAaaea7743b9c8b826111549616301fc50c67ec33027d5baa65c6de581cf7195bc,
  readonly newly-expert-l2-control retained. Level2 XP field not separately captured.
  StageB omitted at210 cutoff; own300 quit target MISSED, actual quit batch387.597,
  normalexit0 at388.789 before400.767 clean samples/exact teardown/socket removal;
  947/old947/925/dee/e5/ecb/maps/public891 controls unchanged. No L3, fresh reload,
  battle, AI or further acceptance. Next required separate proposal: fresh L2 load
  then second ordinary Seer/L3 and explicit mastery; no Runtime defect established.

- **Help-fixed947 ordinary QS/QL and four-card GUI gate independently read.**
  testing/convenience947-help-fixed-gui/summary.json records English QS/enabled QL
  hover/right-click help; actual QS -> safe WEST step -> actual QL/normal confirm ->
  restored position/OrrinL1 XP0/army100Pikes+20Vampires+20Lords+20Nagas. MP1560/1560
  observed AFTER restore only; gold20700 unchanged, no pre/moved-MP or income claim.
  Both Vampire cards show Flying/NoRetaliation/Undead; Lord alone real LifeDrain100%
  text; Naga NoRetaliation without Undead; Pike JoustingImmunity without false traits.
  LifeDrain/Jousting icon cells remain blank outside selected ten mappings: broader
  presentation gap, not all-ability coverage. No F8/F9/battle/endturn/new XP/mastery/
  AI/fresh-process proof. New protected QS671307 bytes,
  SHAecb86e25fad4311784fd1675724902f8b8892022fc9cd11cac17d7f49033d3b3.
  Quit349.240/confirm~358.4/normalexit0 at358.577;707 clean samples, exact five-process
  and socket/lock teardown. Input-helper ValueError and shutdownXIO retained apart
  from gameplay. New947/old947/925/dee/e5/maps/public891 anchors unchanged.
  Lease released; no Runtime defect established. Remaining mastery journeys and
  full Runtime families still require completion beyond this convenience pass.

- **947 first convenience GUI stopped on presentation RED; Runtime semantics not
  implicated.** Independently read testing/convenience947-gui-first/summary.json:
  ordinary map/gold20000/hero15-20-5-10, visible QS and initially disabled QL;
  actual mouse QS created671560-byte Quicksave,
  SHAdee34173c79fee9e00d5d8bdca13a9530506e36dce2c8e34a4f20a2a291b678a,
  preserved as quick-button-day1-control. Hover exposed raw
  vcmi.adventureMap.quickSave.help.hover; Frontend/Build own the scoped data-prefix
  repair/new freeze, not a patch to947. No movement/QL/cards/F8-F9/battle/endturn
  acceptance. Actual Quit-to-Desktop242.182s, normalexit0 at265.551; shutdown input
  XIO retained separately.523 clean samples, all owned processes/socket/lock absent;
  947/925/e5/three maps/public891 controls preserved. Lease released; no Runtime
  gameplay fix inferred. Fresh repaired-candidate GUI gate remains required.

- **Combined native41/41 and all three export identities independently verified.**
  convenience-fixture-assets-activated XML41PASS/0skip and exit0. Preserve TWO
  auxiliary setup REDs separately: missing vcmi-test, then missing original
  DATA/LCDESC. Third runner uses authorized external read-only Data symlink; no
  purchaser/candidate writes. NHConvenienceArmy.h3m793 compressed/10784 raw,
  SHA40405710905aedf86ac54e6d1e0142e9e5db2013a90b1ae9c177b3550f7a51b5;
  both original mastery maps retain2f7d02ea/e5b02f04 hashes. All gzip lengths/hashes
  independently matched convenience-fixture-exported-maps.json under testing/
  combined-dd6-fixture-assets/cache/vcmi/testMaps. Tester received exact native
  trait truth and requested independent full947 audit/ordinary GUI proposal.
  Read combined-dd6-convenience-private-first identity: dd6+usability46/0.5.1,
  clienta7669de5, facade31a70506, moduleb770f6b4; developer ELF paths/private only.
  Immutable identity's earlier pending-native wording is historical; do not rewrite
  sealed947. No button/card/mastery journey GUI acceptance is inferred from41.

- **Foundation integrated at dd6f6e07af7e445cec863082efebb34cce5dab77.**
  Independently confirmed HEAD, exact86 commit paths/default module excluded and
  Runtime51 unchanged. Build reports push/identity/privacy gates; no activation or
  full acceptance. Combined follow-up is explicitly dd6+approved usability46, NOT
  an86-only binary. Combined client/test build exit0 and all133 pre-export source
  hashes independently matched. Build's new private947 is separate from protected925.
- Requested convenience exporter delivered before category work:
  test/server/battles/NewHorizonsConvenienceFixtureExportTest.cpp e9ee193e...,
  ordinary NHConvenienceArmy SOD/100Pikes+20Vampires+20VampireLords+20Nagas and
  Expert Artillery/Ballista. Native assertions distinguish both undead/no-retaliation
  Vampires from Lord-only actual lifeDrain script trigger, Naga and Pike controls.
  No rule/primary/bonus/save injection; deterministic gzip/reparse assertions.
  Build registered it deliberately; convenience-fixture build0/baseline0(one opt-in
  skip). Activated1 is AUXILIARY setup RED "Failed to find mod vcmi-test" before
  executing41 cases, not a product/assertion failure. Separate fixture-root rerun
  requested; no actual convenience map bytes/GUI claim yet.
- Authorized category work remains exactly THREE NEW UNREGISTERED paths, listed
  in category-primitives-source-only.json: lib/entities/creature/
  NewHorizonsCreatureCategoryRules.{h,cpp} and test/creatures/
  NewHorizonsCreatureCategoryRulesTest.cpp (seven unexecuted tests). Pure captured
  structural lookup/DTO only; no CreatureID resolution, canonical mapping, world/
  battle callbacks, serializer/CMake/config writes or live API. Explicit three-row
  Conflux test fixture is NOT a canonical roster. No current held134 source changes.

- **Broad AI/mastery gates and exact foundation boundary independently approved.**
  mastery-ai-mastery-activated40/40; all-feature140=138PASS/2skip; future61x2 each
  58PASS/3skip; prior128=126PASS/2skip and39=38PASS/1skip, every actual exit0.
  Rehashed all86 current files AND immutable mastery-integration-review-ai86 copies,
  matching identity8216b354971ba27980ee6853f4e89a1ddc81cfa0064ee591c0adbefb56aae330;
  all Runtime51 match mastery-runtime-51-held.json (8705e380...). Original80 unchanged,
  only old testCMake/Volley fixture differ; AP.h/AP.cpp/BE.cpp/newAI test are four adds.
  Evidence mastery-runtime-ai86-review.json. Explicit Runtime51/86 FOUNDATION
  boundary approval sent; source re-HOLD. Default0.4/usability/Sorcery excluded;
  no activation, GUI AI/newly-Expert, publication or full-redesign approval.
  Source-only next-category API proposal sent to Frontend (NOT implemented): optional
  readonly world/battle CreatureID lookup, explicit saved category/text/source mapping,
  old absence AND unmapped CreatureID null; battle absence MUST NOT fall back to
  world/current defaults. No out-of-game encyclopedia view without saved context,
  tier/leadership inference or implicit Conflux recruitment rewrite. Frontend ACKed
  these semantics; exact header/enum/field/method names will be supplied only with
  coordinated implementation. Explicit mapping/upgrade entries need Build review.
  Full mapping and implementation remain future coordinated work.

- **Required exchange-only mutation and recovery independently verified.**
  mastery-ai-count-negative-native.xml:6=4PASS/2FAIL, ONLY TwoTurnExchange fails;
  scores0.18983318 vs0.26633307 (legacy),0.56666607 vs1.7566636 (Volley).
  Initial AP predictions and real server/control counts remain PASS. This isolates
  the later-loop grant omission; numbers are AI scores, not physical shot counts.
  Negative build0/native1; exact BE byte restoration to4a159e21 checked against
  before-image; supervisor0/restore0; clean build0/native0/XML6PASS. Summary records
  trace absence after clean rebuild. All REDs retained; no source mutation survives.
  Build requested broader private40/full140/61x2/128/39 gates on restored normal
  source before foundation review. Expected refreshed Runtime51/total86 boundary
  must be verified against actual file list. Frozen925/e5efe human/readback evidence
  remains separate; further ordinary newly-Expert/AI/combat journeys still open.

- **AI repair narrow6 GREEN; required mutation proof/broader gates still pending.**
  Production first run build0/trace-absence0/XML6=4PASS/2 new exchange-oracle FLOAT
  failures (0.26633307 vs0.27199969;1.7566636 vs1.8246634) remains intact.
  Source review identified different initial scoring paths: AP uses original
  defender per hit; single tracker uses progressive damage. Authorized test-only
  e16725e0 reference now replays initial AP (independently HP-tested) then literal
  2/3 single later hits; strict FLOAT_EQ unchanged, three production hashes fixed.
  mastery-ai-count-oracle build0/native0/trace-absence0/XML6PASS independently read.
  Initial AP scores0.118999898/0.373999596 and literal later2/3 recorded in XML.
  Required BE-only old-count negative variant/restore bytes and exact plan prepared
  in mastery-ai-count-negative-plan.json: normal4a159e21, negative2062b3bc, expected
  4PASS/2TwoTurnFAIL then exact restore/clean6GREEN. Live source NOT mutated yet.
  Build schedules that bounded gate after authorized Artist180s proof slot; no
  competing work or candidate925 changes. Full mastery40/all-feature140 and prior
  regressions must follow; foundation approval is still held.

- **Clean fixture checkpoint isolates the AI defect.**
  mastery-ai-count-fixture-clean build0/trace-absence0/native1/XML4: original two
  controls PASS; only predicted-health1vs2 and3vs9 assertions fail. Actual server
  2/3, free/resolved target and survival now pass. Initial nested-manifest harness
  parser/missing-script prelaunch RED retained separately; no C++ ran in that attempt.
- Authorized AI-only repair is SOURCE_READY, not executed yet:
  mastery-ai-count-production-repair.json/.diff pins four paths with before/after
  hashes. AttackPossibility.{h,cpp} adds shared getAttackCount (innate plus fighting
  hero's creature-specific grant on unit battle side); both immediate evaluator
  and BattleExchangeVariant consume it. Server/unit API remain unchanged.
  New test file additionally exercises actual two-turn BattleExchangeEvaluator,
  including non-initial attack loop, against independent single-attack tracker
  oracle2*(2/3), checking no real HP/ammo mutation. Earlier assertions remain.
  Expected narrow6 cases; registered mastery40/all-feature140 afterward. No claim
  that this new exchange fixture or production repair passes before Build execution.

- **Server-count RED localized to overlapping fixture targets, not a rule defect.**
  mastery-ai-count-server-trace build0/native1/restore0; exact server restoration
  SHA83ef6a921a5cb34580426e37b06f52d6175affd9ca220890c13b8885f8aa07d6 verified.
  Requested synthetic unit3/4 resolved by hex to original unit2/10HP at15,5.
  Volley server correctly computes base1+hero2=3; in the new maximum-damage fixture,
  that original target dies after shot2, so iteration2 correctly skips. Original
  execution control survived to shot3 by seed; its3-event proof was real but not
  against the intended10000-creature target. Trace artifact/log remains diagnostic
  only; clean rebuild required, never candidate925/commit/publication.
  Authorized exact two-test repair is held in mastery-ai-count-fixture-repair.json/
  .diff: newAI test742c9541 and original Volley test6e6b55d5 use asserted-free14,5,
  resolved-target identity checks and durable-target survival. Existing2/3 counts,
  prediction equality and non-Ballista1 control remain. Old82 snapshot retained.
  Build clean four-case checkpoint requested before AI production repair; expected
  prediction-only RED remains unverified until that actual run.

- **Actual combat-AI RED includes a separate unexplained server-count RED.**
  mastery-ai-count-red build0/native1: two cases fail predicted health loss1vs2
  (legacy) and3vs9 (Volley); additional Volley server attack-events2vs3 fails.
  These first numbers are health, not shot counts. Preserve all three assertions.
  Diagnostic-only new-test revision7a18b505935ddef1963cad3564994e2350e3fffc6573acdf15dbc849a1cf469e
  adds phase properties; mastery-ai-count-diagnostic build0/native1/XML4:
  two ORIGINAL server controls PASS, same two new cases/all three assertions FAIL.
  Volley heroGranted2/selected1/innate1/ammo24/sameFightingHero=true remain before/
  after prediction, after beginCombat, before shot; afterward HGA2/selected1/innate1
  remain but ammo22. Legacy HGA1, ammo24->22. Thus no evidenced selection/HGA/ammo
  loss caused by prediction/start; rank property is blank from uint8 character
  formatting, not a proven rank loss. Requested bounded existing-binary debugger
  localization of server mid-action totalRangedAttacks/side/hero/loop before any
  repair. No production code changed, no unqualified server3/AI-only-cause claim.

- **Fresh saved-Volley readback PASS independently read:**
  testing/mastery-reload-first/summary.json records exact e5efe637 save on925,
  OrrinL2/XP1000/100Pikes/Expert Artillery/Basic Pathfinding+Sorcery Magic;
  base=total18/24/6/12, last3/4/1/2, mana10/12, movement1160/1560;
  capacity100/825 and saved Volley(active)+1. Quit initiated181.6s, exit0 at183.120,
  361 clean samples, exact teardown and925/maps/protected saves unchanged. No new
  turn/combat/save; previous setup/Gold/late-quit qualifications remain.
- **Foundation approval now HOLD for concrete combat-AI characterization.**
  Read-only audit: AttackPossibility.cpp349 and BattleExchangeVariant.cpp831 use
  unit.getTotalAttacks (ADDITIONAL_ATTACK), whereas server melee/shooting adds
  hero HERO_GRANTS_ATTACKS. Existing actual server2/3-shot and adventure-choice
  proofs do not prove combat valuation. New outside82 test
  test/battleAI/NewHorizonsMasteryAttackCountTest.cpp,
  SHA35751c9fa7cf38c5bea09397cf75e7c548767162e211e4fb1c88f43132a35d81,
  checks real AttackPossibility cached-shot damage against expected2/3 then counts
  actual server shots, with real level/query Volley selection. No production fix.
  Independently hashed82 review inputs unchanged before Build's deliberate test-only
  registration. Sole Build targetvcmitest900s/two jobs plus120s two-case filter now
  running; no GUI or competing heavy work. Await actual RED, not inferred failure.
  Unit API/server must remain unchanged to avoid double counting on any AI repair.

- **First ordinary mastery GUI is partial acceptance, with deadline RED retained.**
  Independently read testing/mastery-gui-first/summary.json: ordinary ExpertChoices
  Seer1000XP -> level2 -> Basic Sorcery secondary -> mandatory three-card mastery;
  Return/Escape without selection did not choose; explicit1/confirm accepted Volley.
  Normal named NEWGAME-m1 save675676 bytes,
  SHAe5efe637bca25bd4bb765dc0c363e15b3bcb87d82e2837f84cb0cad25b51c2dd,
  with readonly mastery-day1-control. Gold was NOT verified (resources suggest a
  resource starting bonus). Saved development pane/fresh reload, popup routing,
  combat and newly-Expert journey were NOT performed. Initial private1x1 black
  window setup RED was corrected within lease using video-only1280x800/windowed.
  Gameplay stopped445.5s, actual quit initiation490.3 exceeded450 target; normalexit0
  at491.020<600, cleanup-only after actual quit, no hang/extension claim. Tester
  confirms925/control hashes unchanged and client/Xvfb/socket/launchers gone.
  Lease released; no Runtime gameplay defect yet. Next required gate is a separately
  authorized fresh load/readback of this actual save before wider mastery gameplay.

- Independently parsed subsequent gates: mastery-regression future baseline61 and
  curated61 each58PASS/3skip; prior baseline128=126PASS/2skip and curated39=38PASS/
  1skip; mastery-all-feature-native136=134PASS/2skip, all exits0, no failures.
  Private `mastery-preview-private-first/BUILD-IDENTITY.json` declares69 held source
  paths, compiled base296068af0, module0.5.0, client33ebf7d13643e52670c69d02777b38e5d851758ad121f884bb3370abd9d45a33,
  facadeb9122598d6cea93846781ea4b7c5dbce817f00a3c233ef5cfe9847f836977354,
  and the two independently verified ordinary map hashes. Build reports925 frozen
  files; Tester owns exhaustive candidate audit and normal-input acceptance. This
  is private/uncommitted with developer ELF paths, not a distributable or GUI pass.
  Source remains held pending Tester acceptance/any concrete defect; full mastery
  breadth, remaining commands/spells/categories and full redesign remain incomplete.

- **Activated mastery native/export gate independently verified:**
  `mastery-first-activated-fixture-root.{xml,exit}` is36PASS/0skip, exit0 in actual
  private0.5 with required six translated texts and both ordinary exports. Preserve
  earlier missing-vcmi-test runner setup RED separately; Build supplied only its
  native fixture root, not gameplay rule injection. Baseline exporter checkpoint
  `future-mastery-export-*` all exits0,36=33PASS/3 intended opt-in skips.
  Exported gzip/raw identities independently checked:
  NHMasteryExpertChoices.h3m807/10991 bytes,
  SHA2f7d02eaff768fed8562fddceaa4082f2930e6aee42cd35eb8bca5503f2679a9;
  NHMasteryNewlyExpert.h3m819/11032 bytes,
  SHAe5b02f04ea2a9c45204632ec4ef0ab99d569c9fbdd95e40ababac8835143c656.
  Both under testing/mastery-native-first/cache/vcmi/testMaps, ordinary authored
  SOD initialization without primary/rule/save overrides. Tester received exact
  trigger/reply/effect/native scope and these identities; AI encounter routes remain
  unscripted and unproven in GUI. Build's61x2/128/39 regressions are running under
  source hold; exact GUI candidate/leases and integrated mastery acceptance still
  required. Native test-only fixture resources must not be mistaken for GUI payload.

- **First mastery native GREEN independently parsed:**
  `mastery-schema-repair-native.xml`:34=33PASS/0FAIL/1 expected translation-activation
  skip. Build's actual diagnostic found schema `pattern` is NotImplemented; its
  supported exact three-stem enum repairs canonical schema validation without
  framework/assertion changes. Runtime46 unchanged. Build deliberately registered
  the separate two-case ordinary exporter only after this34 gate: next baseline36
  expects33PASS/3 opt-in skips; actual private0.5 must require text resolution and
  both exports separately. New69-path hold/sole bounded compile active. No activated
  text, exported-byte, ordinary GUI or full-scope acceptance yet. Read new
  NH_USER_FEEDBACK.md at296068af0: F8/F9 and Undead-art reports are not proven runtime
  omissions/mod causes; Frontend traces first, Runtime handles any evidenced rule/
  save defect. Frozen891 release identity remains separate from this dirty family.

- **First actual mastery native result independently parsed:** fixture retry build0,
  native1; `future-mastery-fixture-native.xml/log`:34 tests,30PASS/3FAIL/1 explicit
  private-preview text skip. Actual Nullkiller2 callback/packet/ACK in all three
  escort contexts PASS; six active/legacy distance/wall/shot/regen paths PASS;
  server order/rejection, delayed-Expert latch, chained XP, dormancy, full-world
  save/reload/pending re-exposure, old absence and sequence controls PASS. Three
  failures are schema-related: canonical named positive, actual settings-wrapper
  positive, and schema-valid semantic-negative controls. Forwarded Build-owned
  schema investigation; preserve assertions and original logs. No private0.5 text
  execution, ordinary exported maps, GUI acceptance or full-redesign completion
  inferred from these30 passes. Runtime remains held awaiting bounded schema repair.

- WindowHandler retry reached140/187 then failed in Runtime's mastery test fixture:
  CCallback is final and direct world serialization lacked complete dependent types.
  `future-mastery-windowhandler-build.log` retained; still no native test execution.
  Bounded two-path repair: test/server/battles/NewHorizonsMasteryTest.cpp now composes
  a REAL final CCallback with an IClient loopback transport (rather than deriving
  from/replacing its mastery callback); actual Nullkiller2 callback constructs the
  request, transport preserves payload, invokes ApplyGhNetPackVisitor and returns
  matching request/ACK status. Added full-world serialization definition includes;
  no save assertions or serializer guards removed. Effects.h forward declaration
  now correctly says struct Bonus. Exact two-file diff and full46-path manifest:
  `future-mastery-fixture-repair.{diff,paths,json}`; original before-images hash-match
  prior hold, remaining44 Runtime paths unchanged, still34 test cases. Re-HOLD ready
  for Build's sole retry; compiled clientcommon is not gameplay/native acceptance.

- Sequence-repair compilation passed the original unsigned64 guard, then stopped
  at396/582 on Frontend's incomplete WindowHandler type in HeroMasteryWindow.cpp112.
  `future-mastery-sequence-build.log`/exit1 are retained; no native cases executed.
  Frontend supplied an include-only repair and refreshed12-path manifest
  `research/mastery-ui/source-ready-windowhandler-fixed.json` (other11 unchanged).
  Runtime46 stay held at `future-mastery-sequence-repair.json`; Build alone resumes
  the bounded compiler/native checkpoint. Full redesign and mastery acceptance remain
  unproven; ordinary exporter remains excluded from this34-case checkpoint.

- First actual mastery C++ RED preserved in `future-mastery-test-enabled-build.log`
  (69/621): BinaryDeserializer correctly refuses raw uint64 serialization. Earlier
  `future-mastery-first-*` is the distinct ENABLE_TEST/unknown-vcmitest harness RED.
  Bounded Runtime repair touches exactly five previously held paths: Rules.h,
  State.h, PacksForClient.h, PacksForServer.h and RulesTest.cpp. All five sequence
  serialization sites now share checked signed high/low32 halves; no framework
  guard changes, signed narrowing, lost high bits or weakened domain validation.
  Wire representation retains all uint64 values; existing saved-state crossover
  limit at INT64_MAX remains explicit and unchanged. Three unexecuted regressions
  cover offer/selection/client/server replies at full-width boundaries, malformed
  halves rejecting before assignment, and saved-counter limit/exhaustion. Filter
  now expands34 cases (not original31). Exact bounded diff reconstructed and verified
  against original held hashes: `future-mastery-sequence-repair.diff`; new complete
  46-path digest map `future-mastery-sequence-repair.json`. Remaining41 paths unchanged.
  No native test has executed yet; requesting Build resume against this repair.
  Separate unregistered `NewHorizonsMasteryFixtureExportTest.cpp` authors two ordinary
  opt-in maps, Expert and newly-Expert boundary, with human Seer XP and an unscripted
  computer encounter; no exported bytes/GUI claim or inclusion in this first gate.

- **Runtime SOURCE_READY for first mastery compile/native checkpoint; 46 paths held**
  in `build/new-horizons-linux/future-mastery-runtime-source-ready.{paths,json}`.
  Still UNCOMPILED, no acceptance/GUI claim. New library CPPs: hero/
  NewHorizonsMasteryRules.cpp, NewHorizonsMasteryState.cpp,
  NewHorizonsMasteryEffects.cpp; new tests: hero/NewHorizonsMasteryRulesTest.cpp,
  hero/NewHorizonsMasteryStateTest.cpp, server/battles/NewHorizonsMasteryTest.cpp.
  Filter `*NewHorizonsMastery*` expands to31 tests (one explicit text-activation skip
  outside private0.5; use NH_REQUIRE_MASTERY_TEXTS=1 under actual mastery preview).
  Added real server query rejection/ordering, pending world reload/exposure, old
  binary/crossover absence, dormant/reactivated effects, chained levels and actual
  wall/distance/shot-count/activation regeneration active+legacy/non-Ballista paths.
  Real Nullkiller2 callback tests run three escort compositions, submit the dedicated
  packet through ApplyGhNetPackVisitor and process request/ACK status; policy also
  checks reordered options. Scores are provisional, not balanced or GUI-proven.
  Important timing repair: HeroLevelUp now carries saved artilleryExpertBeforeGain
  captured BEFORE primary gains, so delayed readiness cannot misclassify Expert
  obtained while the normal dialog waits; native regression authored. Automatic
  map XP still captures before secondary changes. Frontend's earlier9-file readiness
  is held RED for covered-dialog ACK/resolution routing; combined compilation waits
  for its repaired readiness and Build's registration/grant. Ordinary mastery export
  and integrated Tester acceptance remain future work after native diagnosis.

- **Mastery API_SOURCE_READY for Frontend binding only, not combined SOURCE_READY:**
  crossover JSON now preserves the complete saved registry and pending/chosen
  identity, with strict integer/shape/duplicate checks and two more unexecuted
  tests (13 total rules/state tests). Placement can rebind pending hero/owner only
  with identical saved options and a fresh sequence. Added actual authoritative
  HeroMasteryOffer/Dialog/Chosen and dedicated HeroMasteryReply packets, visitor
  applications and registered IDs270–273. CHeroMasteryDialogQuery accepts only the
  dedicated reply; top query, owner, hero, sequence, level, Expert rank and index
  are validated before mutation. State/effects apply before QueryResolved/ACK;
  invalid replies preserve the query. Normal secondary choice now precedes mastery,
  with XP continuation after accepted mastery; startup/load/idle query scheduling
  exposes saved pending/deferred map-XP eligibility. Actual APIs sent Frontend:
  CGameInterface::heroGotMastery(offer,queryID), CCallback::chooseHeroMastery
  (hero,queryID,sequence,index)->requestID/-1; CGHeroInstance::getMasteryView() optional
  copies choices with active status, pending, eligibleNextLevel and awaitingChoice.
  Frontend owns the client visitor/window/ACK binding. AI callback/valuation and
  real native server/effect tests are next; no compile/execution readiness yet.
  Tester separately reported exact frozen891 packaged start/combat and prebattle
  reload/Day2 passes; these are not mastery evidence and no891 bytes were changed.

- Mastery source checkpoint (still **uncompiled, unactivated, NOT SOURCE_READY**):
  `NewHorizonsMasteryState.{h,cpp}` now models saved pre-level eligibility,
  immutable pending offers, monotonically sequenced selections and rejection without
  consumption. Four new unexecuted state tests distinguish newly Expert from already
  Expert, exercise rejected/duplicate replies, binary pending/chosen roundtrips and
  no-rules absence. Added independent setting/world snapshot and
  NEW_HORIZONS_MASTERIES serialization feature plus hero snapshot/absence latch.
  Real HeroLevelUp packet application captures BEFORE level advancement; automatic
  map-XP progression captures BEFORE secondary changes (offers remain deferred).
  Hero methods now validate/apply offers/choices and rebuild owned mastery bonuses;
  Artillery rank changes deactivate/reactivate selected effects without rank4.
  Missing before any readiness claim: crossover JSON, saved readview, actual server
  query/packets/ACK/secondary-then-mastery flow and load/startup exposure, AI choice,
  real wall/distance/regen/shot-count positive/non-Ballista/legacy tests, resolved
  localized-text controls and integrated GUI. No compiler permission; Tester891
  exact-package GUI lease is active, source-only work continues, frozen891 untouched.

- Mastery source progressed: strict independent JSON parser now validates version1
  Artillery registry, exact three distinct scoped IDs/effects and effect-specific
  magnitudes. Seven unexecuted rules tests cover named schema/actual settings
  wrapper, duplicates/effects/scope beyond structural schema, saved options,
  reply bounds and saved-magnitude description substitution. New
  `NewHorizonsMasteryEffects.{h,cpp}` constructs real Volley/Precision/Repair bonuses
  with appended HERO_MASTERY source; Volley uses hero Ballista subtype, precision/
  repair use a Ballista creature limiter. These builders are not yet installed by
  a gameplay choice; no mechanic/AI execution or SOURCE_READY claim. Build authored
  canonical schema/data/texts/private0.5 generator, default0.4 remains unchanged.
  World/hero persistence, eligibility capture, query/packet/ACK lifecycle and AI
  choice/effect tests remain the immediate required implementation before compilation.
  Compiler lane is now free but Runtime has no grant and will not compile.

- **Post891 mastery source family started, unactivated/uncompiled:** HEAD89165787e
  confirmed. New `NewHorizonsMasteryRules.{h,cpp}` currently defines typed MasteryID,
  three-option offer DTO, structural validation and stateless reply validation;
  `test/hero/NewHorizonsMasteryRulesTest.cpp` has three unexecuted controls.
  Offer.level uses uint32_t like the hero, avoiding the prior Windows narrowing
  failure. This is NOT yet a wired progression, saved hero field or active effect.
  Build/Frontend/Tester received the concrete v1 contract: independent
  `heroes.newHorizonsMasteries`, schemaVersion/rulesetVersion1, skills keyed
  `core:artillery`, options containing id/effect/magnitude/nameTextId/
  descriptionTextId/iconKey. IDs `new-horizons:artilleryVolley`,
  `new-horizons:artilleryPrecision`, `new-horizons:artilleryRepair`; effects
  volley1 (extra Ballista attack), precision1 (distance/wall penalty removal),
  repair50 (pre-turn Ballista HP regeneration). Existing real mechanics will be
  reused with Ballista-only restrictions and positive/non-Ballista/legacy tests.
  Trigger is supported skill already Expert BEFORE level gain; additional mandatory
  choice AFTER normal secondary choice, newly Expert waits for next level. No rank4,
  cancel/skip or fixed-first AI. Reply must carry queryID, heroID, saved sequence and
  index0..2; current top query/owner/level/Expert/unchosen checks precede mutation.
  PendingDialog/ack lifecycle and apply-before-client ordering are required; exact
  new packet/callback/view names are not yet implemented or ready for UI binding.
  Build owns data/schema/CMake/metadata, Frontend owns new window/glue/art; no
  defaults or891 release changes. Next executable source task: strict JSON registry,
  saved eligibility/pending/chosen state and authoritative query/effect integration.

- **Ordinary combat-AI siege GUI PASS independently read summary:**
  `testing/capability-ai-gui-59/summary.json` records normal Options Ballista
  permission/autocombat after ordinary pursuit and manual Pikeman defend, then
  actual BattleAI selection/server actions (not scripted AI calls or manual shots).
  Eight Ballista damage events13,12,10,12,13,9,11,12 total92; Pikemen finished the
  remaining28. Victory120XP,5 losses/995 survivors; normal quit0 at359.185s before
  450,708 samples, no child/owned INET, exact processes/socket/lock absent and
  all protected inputs unchanged. Raw log SHAefe34686f23f... retained. This closes
  the exercised AI Ballista journey, not every siege formula/skill, save/transfer
  in this lease, or mastery/category/full-redesign breadth. Foundation review
  approval remains bounded; await Build's integrated identity/activation gates.

- **Bounded capability foundation Runtime review APPROVED:** independently checked
  `capability-integration-review/identity.json` (37 paths): every working-file hash
  and every frozen `files/` copy matches; no changed/untracked Runtime-owned path
  lies outside the manifest. `git diff --check` passes. Re-read production diffs
  for saved/crossover identity, optional views, shared movement scaling, projected
  army AI and siege payload ownership. No blocking finding in this bounded scope:
  old absence is latched, arithmetic bounded, troop counts/current movement never
  changed by read/projection APIs, range multiplier shared by estimates/authority,
  legacy range fallback preserved. Native61/100/separate1 and documented GUI
  journeys support this foundation, not full secondary-AI/mastery/category breadth.
  Approval is for Build's unactivated foundation commit only; default0.3 remains,
  AI GUI/activation gates are separate. No product writes until scope integration;
  no diaries, pycache or published/frozen assets belong in this commit. Next-family
  changes must follow the foundation/activation checkpoint without moving its
  release identity. Runtime does not stage, commit or compile.

- **Remaining saved presence controls GUI PASS independently reviewed:**
  `testing/capability-presence-gui-59/summary.json` explicitly identifies loaded
  PRIMARY45 SHA45aae669... and NEITHER SHAf7d8aa403... (not the retained f9 copy).
  Ordinary menus restored primary-only level2 base18/24/6/12, total20/24/6/12,
  last3/4/1/2, mana10/12, movement877/1500 with NO capability pane. Same-process
  menu load of f7 restored2/2/3/10, XP0, mana95/100,15 Pikemen/9 Archers with NO
  development entry and original four schools/costs5/6/5. Normal quit0 at396.893s
  before450 cutoff,706 samples, no child/owned INET, exact process/socket/lock
  absence and protected originals/copies unchanged. No new save/turn/battle.
  All four reachable presence combinations now have distinct GUI evidence across
  the documented ordinary/nondefault routes; this is not eight fixtures, f9
  acceptance, AI siege/formula-breadth or mastery/category completion.

- **Main capability reload and ordinary next-day refresh independently reviewed:**
  `testing/capability-main-reload-59/summary.json` confirms8dc0 reload restored
  both primary15/20/5/10 and capacity750/75%, hero1000/town0, current688/max1170.
  Ordinary Blue AI turn reached Day2 with1170/1170,1000 troops intact and gold
  20500->21000. Normal manually named `Autosave-111-day2.vsgm1`,576549 bytes,
  SHA16406d0915a32cfb5fe84caa0293f10304b8be5c7f459139681f99e517672b3c,
  preserved read-only; filename is NOT evidence of an automatic save.
  Exit0 at351.998s missed requested quit-before330 target; Tester reports only
  cleanup after last progression258.7s, within unchanged420 supervisor. Retain
  this timing qualification.645 samples, no child/owned INET, exact processes/
  socket/lock absent and protected inputs unchanged. No Day2 restart, other
  presence-state or AI siege/formula-breadth claim follows from this ordinary turn.

- **Ordinary transfer/no-refund/main-save GUI PASS independently read:**
  `testing/capability-transfer-gui-59/summary.json` records hero1000->500->1000,
  town0->500->0, total1000 preserved; actual current movement688 throughout.
  Reopened development limits1170->1560->1170 and factors75->100->75 match saved
  capacity750. Distinct normal `NEWGAME-mainday1.vsgm1`,574828 bytes, SHA
  `8dc0ed18869abc39ba06c33f1a3f179603e5a53eaa611b1eed4c022d80902b77`,
  has a read-only control copy. Normal quit0 at468.420s before480 cutoff,924
  samples, no child/owned INET, exact processes/socket/lock absent; protected
  candidate/map/historical inputs unchanged. Initial save-filter focus mistake
  was corrected before the actual save and retained as evidence. No next-day,
  reload, combat or other-presence claim for this lease; fresh main-save load and
  ordinary next-day refresh remain pending separately authorized GUI gates.

- **Focused ordinary capability battle GUI PASS, independently read summary:**
  `testing/capability-battle-gui-59/summary.json` records normal quit0 at298.346s,
  588 samples, no child/owned INET and exact process/socket/lock absence. Gold setup,
  ordinary pursuit of12 Archers, six Pikeman defends and manual Expert Ballista
  targeting produced damage12,12,13,10,13,11,10,11,13,13,2 (120 total). First two
  shots left10 Archers with top HP6; victory120XP,4 Pikemen lost,996 surviving.
  All916/map/protected/historical inputs unchanged. Raw log SHA9e92358b6654...;
  Tester preserved its initial UTF8-parser failure and audited unchanged bytes with
  ASCII regex. Prior hard-bound124 remains RED. No army transfer, normal new save,
  main-scenario reload or other-presence claim follows from this battle pass.

- **Main cap59 GUI hard-bound RED, retained:** Runtime read
  `testing/capability-main-gui-59/summary.json` and final screenshot. Exit124 at
  604.207s is NOT a normal quit. Both-view15/20/5/10, XP0,1000 Pikemen/Expert
  Ballista, mana10/10, movement1170 and capacity1000/750/75% were observed. Final
  frame still says "Press any key to start battle immediately" with1000 Pikemen,
  12 Archers and Ballista; no defend/shot/damage, normal distinct save or transfer
  occurred. Last recorded input was pursueYES at366s. Summary confirms1058 samples,
  no child/owned INET, exact processes/socket/lock absent and all protected hashes
  unchanged. Source log reaches BattleSetActiveStack application; this does not
  establish combat interaction or diagnose a Runtime defect. No code repair or
  implicit rerun/extension is justified by the current evidence. A separately
  granted narrow combat/transfer/save journey remains necessary.

- **Saved capability-only absence now proved graphically across presets:** Runtime
  read `testing/capability-only-reload-cap59/summary.json`. A fresh unchanged cap59
  process with both installed rule families enabled loaded the normal38f8 save:
  authored2/2/3/10, XP0,1000 Pikemen, Expert Artillery/Ballista, mana100/100 and
  movement1170/1170 persisted, as did no-growth snapshot and capacity1000/750/75%.
  Scrolled control/base-range qualifiers retained; no default profile adoption.
  Exit0 at331.686s (Tester reports progression stopped before330s, cleanup only
  afterward),530 samples, no child/owned INET, exact processes/socket/lock absent.
  Both916 inventories and original/control/profile-copy save identities unchanged.
  No turn/new save/battle or other presence-state proof in this lease. Main cap59
  both-view/army-transfer/combat journey still needs its own grant and evidence.

- **Capability-only GUI/save checkpoint independently read:**
  `testing/capability-only-gui-61-authored/summary.json` records ordinary nondefault
  new game2/2/3/10, XP0,1000 Pikemen, Expert Artillery/Ballista, mana100/100 and
  movement1170/1170. Tester reports truthful no-growth presentation, capacity
  1000/750/factor75%, scrollable100/0/0 control chances and base-range/eligibility
  qualifiers. Normal Day1 save435144 bytes SHA
  `38f8b3975973e11c6c8be7b8be4664fdc0152aa320a2e33a423660eb387f1f93`
  preserved read-only. Exit0 at463.621s,838 samples, no child/owned INET,
  client/Xvfb/socket/lock absent, all916 candidate hashes and historical inputs
  unchanged. No turn, battle or reload occurred. Next necessary gate is ordinary
  load of this saved identity under unchanged all-cap59, with a new explicit lease;
  saved primary absence under enabled defaults is still unproven graphically.

- **Queued daily refresh and capability-only export now natively GREEN:** Runtime
  independently parsed all six `future-capability-61-*.xml` files and exits:
  regular61 each58 PASS/3 skips, regressions128/39 with2/1 skips, activated100
  with98 PASS/2 expected skips, separate capability-only export1 PASS, all exits0.
  Thus the real server NewDay control and actual caps-on/growth-off ordinary export
  are verified natively. Build reports frozen `capability-only-private-61` using the
  same cap59 ELFs, separately identified metadata and map SHA
  `4524bece8b97b38fc1f1b9272e1e08d3428f772ff9b4188550292644001e7eaf`.
  Tester diagnostic audit is next: no GUI grant/journey or saved-identity reload
  acceptance yet. Main cap59 and working0.3 remain unchanged. This supplies a real
  nondefault control route, not four default-preset fixtures or full redesign proof.

- **Fourth view-state provenance gap explicitly retained:** no existing ordinary
  map/save proves capability-only presentation. Native cap-only uses a test override
  and cannot supply GUI provenance. Proposed a separately audited, nondefault
  Build-owned caps-on/growth-off preset; normal new game/save there, then load that
  save in unchanged cap59. No frontend state or save editing. Build metadata and
  Tester authorization/audit are pending, not an available GUI route yet.
  Authored `ExportOrdinaryCapabilityOnlyIdentityControl` in the existing exporter:
  separate `NH_EXPORT_CAPABILITY_ONLY_FIXTURES=1`, fails if growth is enabled;
  `NHCapabilitiesOnlyControl.h3m` has explicitly authored2/2/3/10, mana100,1000Pikes,
  Expert Artillery, capacity750/used1000/factor75%, initial1170 movement. Actual
  preset initialization and exact gzip/readback required; no rule override. This
  new export is uncompiled/unexecuted and must NOT be enabled with all-features
  export flags. Along with queued daily-refresh test, regular suite becomes61;
  run this diagnostic export alone under its own preset. Frozen cap59 unchanged.

- **Private0.4 actual activation/export independently verified:** Runtime read
  `future-capability-activated.xml`/exit:98 tests,97 PASS,1 expected skip,exit0;
  all three ordinary exports actually PASS, including capability map. Compared
  current source with `capabilities-preview-private-59/BUILD-IDENTITY.json` before
  further edits: every recorded source hash matched. Candidate stays immutable,
  working module remains0.3, and no GUI/publication acceptance is implied.
- After copy/hold release, added one unexecuted, test-only daily-refresh diagnostic
  `AuthoritativeNewDayRefreshUsesCapacityAndSkillWithoutLosingTroops` in the existing
  capability state suite. It calls the actual server new-day hook, checks day/
  refreshed movement and intact4000-creature army; explicit synthetic profile/ranks
  expect780 then1014 after Leadership training, with no instant movement award.
  This is outside the frozen candidate/native98 claim. Queue at Build's next grant
  (future suite60 / activated99 if otherwise unchanged), not a reason to delay the
  candidate's independent GUI audit. No product/default/map edits were made.

- **Capability native WAIT retry GREEN independently read:**
  `future-capability-wait-build.exit`0 and both58 XMLs show57 PASS/1 export skip;
  128/39 regression XMLs/exits also0. Real AI WAIT -> ordinary queue -> fresh
  SHOOT -> validated server health bounds now pass. No activation/GUI inference.
- **Bounded ordinary export source READY:** added
  `NewHorizonsHeroFixtureExportTest.ExportOrdinaryOvercapacityArmyAndTrainedBallista`
  in the existing exporter CPP, gated by `NH_EXPORT_CAPABILITY_FIXTURES=1`.
  Explicit opt-in without actual capability activation fails rather than skips.
  New map `NHCapabilitiesArmySiege.h3m`: Orrin11,10,1000 Pikemen, Pathfinding Basic,
  Artillery Expert, no Leadership/book, equipped Ballista; empty Red town8,10,
  Blue AI town30,30;12 hostile Archers15,10. Pursue if offered flight; defend
  Pikemen to permit Ballista actions. No rule/primary override or existing-map edit.
  Expected actual profile750 capacity/1000 used/75% limit factor, speed4 land base
  1560 ->1170 initial movement. Reversible500-troop town transfer, daily refresh,
  normal combat and save/restart are proposed GUI steps, NOT tested journeys.
  Native checks canonical world identity, starting profile/army/equipment/control,
  parser header and exact gzip/readback. Export unexecuted pending Build's private
  0.4 activation. Regular future suite now59 with two opt-in skips expected; actual
  export must separately run1 PASS. Runtime HOLD after this source checkpoint.

- **First linked capability test RED investigated:** Build/client/test link0;
  both58 contexts report56 PASS,1 skip,1 failure in the real-AI shot fixture;
  128/39 regressions green. Runtime read the baseline failure log and enum:
  action0x06 is WAIT. `BattleExchangeEvaluator::findBestTarget` explicitly evaluates
  waited attacks and can retain waiting for safe ranged attacks with a shooting
  penalty; immediate SHOOT was not established. Bounded fixture repair now requires
  the observed AI WAIT, submits it through validated server action, follows ordinary
  turn traversal, verifies waited activation, then requires a fresh evaluator's
  SHOOT. Existing doubled-shot/server-health bounds remain unchanged. No AI-policy
  edit, forced activation, guard bypass or final-choice relaxation. This retry is
  not yet executed; READY/HOLD for Build with original RED evidence retained.

- First capability build exited1 before tests; Runtime independently inspected
  `future-capability-build.log`. Four fixture references used nonexistent
  `CreatureID::PIKEMAN` and five reads accessed private hero movement. Bounded
  test-only repair uses existing `creatureByName("core:pikeman")` and public
  `movementPointsRemaining()` throughout both affected cases. All original
  quantities and movement assertions retained; no encapsulation/product changes.
  READY/HOLD for Build incremental retry; no native pass or client-link claim.

- **Combined Runtime SOURCE_READY / HOLD for first capability build:** Runtime
  source writing stops at this checkpoint until Build returns actual results or
  explicitly releases it. `git diff --check` passes; nothing compiled by Runtime.
  Register four new lib files (`NewHorizonsLeadership` and
  `NewHorizonsCapabilityRules`, headers/CPPs) and two new test CPPs. Native additions
  are22 cases: `NewHorizonsLeadership.*`4, `NewHorizonsCapabilityRules.*`7,
  `NewHorizonsCapabilityStateTest.*`11 (last suite in existing growth test CPP).
  Include these explicit suite filters: existing future36 +22 means58, not an
  assumption that old filters discover new names. New state tests now include an
  actual BattleEvaluator-selected ballista shot through validated server action
  after ordinary turn traversal, with doubled-shot/range/health bounds.
  Source bridge, optional views, projected-army AI and saved/crossover identity are
  included; actual native and GUI outcomes remain unproven.
  Runtime read Build's canonical data/schema. Canonical provisional inputs are now
  Might750+75/level, Magic500+50/level, Leadership0/25/50/100 and minimum50%; older
  synthetic2000/200/30% native cases are intentionally not canonical oracles.
  Added named `vcmi:newHorizonsCapabilities` and real `vcmi:gameSettings` wrapper
  full/empty positives, six shape negatives, complete18-class checks, missing and
  unknown-class runtime controls, and independent resolved-snapshot checks.
  Working module/c550 frozen release remains unactivated for this family.

- **Siege bridge source reviewed:** Build added the positive `siegeSkillMultiplier`
  branch to `scripts/damage/siegeWeapon.lua`; Runtime read it and verified legacy
  A+1 and SIEGE/turret gates remain. Build reports isolated Lua fixture0 (not native
  bridge/AI execution). Native payload now uses the battle's actual owner hero,
  only for siege weapons. `CGHeroInstance::getSiegeCapabilities()` is an optional
  source API with Artillery/Ballistics/First Aid ranks, ballista base-range multiplier
  and actual MANUAL_CONTROL probabilities for ballista/catapult/tent. No total
  damage or guaranteed player-action claim follows from the range multiplier.
  Old/c550 absent capability snapshots return nullopt. The source is not compiled;
  state suite now ten cases plus eight primitive/parser cases. Native/AI/GUI gates
  remain mandatory before acceptance or activation.

- **Further capability source (unbuilt):** `getTurnInfo(days, projectedArmy)` and
  read-only `getLeadershipCapacity(army)` now let Nullkiller2 `ChainActor` use the
  evaluated exchanged army's capacity rather than its carrier's old usage. This
  changes capacity scaling only; it is not a claim to repair all pre-existing
  hypothetical-army speed calculations. Native projection test asserts no transfers
  or movement grants. Capability-only (no primary growth) presentation gate also
  has an explicit test; Frontend was told to show either optional independently.
  Runtime added `DamageAttackInfo.siegeSkillMultiplier` (script-serialized int):
  zero keeps legacy range math, positive comes from saved capability/Artillery.
  Battle callback fills it for damage calculations/AI estimates. Build was sent
  the exact `siegeWeapon.lua` branch request; Lua source is NOT changed by Runtime
  and the effect cannot be claimed until its branch and native cast/damage gates
  run. Two actual damage tests now contrast future rank multiplier versus legacy
  Attack behavior. Current new state suite is nine cases plus eight primitive/
  parser cases, all unexecuted; no compiler or GUI during the sole release lane.

- **Capabilities live-source integration authored, not built:** added independent
  `NEW_HORIZONS_CAPABILITIES` serialization feature after growth, world setting
  `heroes.newHorizonsCapabilities`, callback snapshot, and per-hero resolved rules
  with capture latch. Binary/crossover absence (including c550 growth heroes) stays
  absent on reinitialization. No canonical config or default activation changed.
  `CGHeroInstance::getLeadershipCapacity()` returns optional capacity/used/percentage
  from saved class profile, actual level/Leadership rank and real roster counts.
  `TurnInfo` applies it to shared land/sea/air limits for daily refresh, pathfinding
  and embarkation; does not change current movement or remove/reject army units.
  Five `NewHorizonsCapabilityStateTest` cases in the existing growth test source
  cover initialization, all-layer/count/split/skill behavior, world roundtrip,
  c550-version absence and old/current crossover. All unexecuted. Pure parser and
  arithmetic suites add eight cases, also unregistered/unexecuted. Future compiler
  registration must include both new lib CPPs and the two new test CPPs.
  Remaining immediate source work: hypothetical exchanged-army AI movement,
  skill-only real siege damage bridge (Lua owned by Build), native authority/AI
  tests and named-schema/default-data controls. No siege UI read view or gameplay
  acceptance claim yet; fixed c550 release clone/candidate remains untouched.

- **Growth checkpoint fixed:** HEAD independently confirmed as
  `c5503cc3515a455084e387f260378f700b51ea3d`. Build reports final default36/128/39,
  data11/Lua2 green and committed default0.3; this is not growth publication.
  New work must remain separate from this fixed release identity.
- **Next family source started, unregistered/unexecuted:** new
  `lib/entities/hero/NewHorizonsLeadership.{h,cpp}` and
  `test/hero/NewHorizonsLeadershipTest.cpp` provide four arithmetic tests.
  Class base + per-level growth, then skill percentage; no primary rating or
  creature-tier inference. Proposed non-destructive soft-cap movement percentage
  is capacity/usage bounded by an explicit minimum. Tests use provisional example
  class values, not a canonical installed table. No hero API, saved rules, army
  accounting, movement enforcement, AI or activation is wired yet. Never present
  this arithmetic object as an active hero capability. Build owns registration and
  compilation. Next executable task: versioned secondary rules/identity and exact
  authoritative movement application, plus skill-only siege integration coordinated
  with Build-owned Lua; preserve legacy behavior and all armies.
  Source trace: `CGHeroInstance::movementPointsLimit()` delegates to `TurnInfo`;
  its land/water/air limits also drive pathfinding and embarkation. Integration
  must scale those common limits rather than only the UI or day-start packet.
  Added wide, neutral-preserving `leadershipMovement()` arithmetic/control. Army
  changes must not award movement; existing daily refresh/remaining-point semantics
  stay explicit. Proposed initial usage is one point per adventure army creature
  (including undead; commanders/artifact machines and battle-only summons are not
  roster entries), not a hidden legacy-tier weight. Siege Lua currently computes
  ballista range from inherited base/artifact Attack; next-family skill-only branch
  must replace that for saved capability heroes without changing legacy casters.
  Build's frozen-clone c550 Linux release build owns the sole compiler lane; these
  four tests remain unregistered/unexecuted and no GUI is launched by Runtime.
- Added separate `NewHorizonsCapabilityRules.{h,cpp}` and four
  `NewHorizonsCapabilityRulesTest.cpp` cases (also unregistered/unexecuted).
  Proposed `heroes.newHorizonsCapabilities` world snapshot has schemaVersion1,
  rulesetVersion1, `classProfiles:{scopedClass:{base,perLevel}}`,
  `leadership:{skillBonusPercent:[0,basic,advanced,expert],minimumMovementPercent}`
  and `siege:{ballistaDamageMultiplier:[1,basic,advanced,expert]}`. Resolved snapshots
  replace classProfiles with profile. Strict parser rejects unknown fields, bad
  versions/ranks, fractional/nonfinite/out-of-range values and duplicate resolved
  classes; new-game full class coverage is separate from saved-world validation.
  Absent snapshots validate as legacy but cannot enter capability arithmetic.
  Siege multiplier accepts no hero level/primary inputs. Contract sent to Build;
  no config/schema/activation edits made. Next source task is world/hero capture,
  serialization/crossover latch and optional actual hero view, followed by common
  movement/army accounting and coordinated Lua mechanics, not UI inference.

- **Additional default-activation fixture RED:** independently read
  `growth-default-regression-curated.xml`: fullbook export expected mana200 but
  actual20 under canonical growth. This export was skipped in activated75 and
  enabled by the39-test runner. Bounded test-only repair now explicitly expects
  human20 with saved growth /200 legacy, with authored Knowledge20 and matching
  limit assertions; Blue Knowledge10 similarly checks10/100. Spellbook contents,
  four-rank conversion, six-school nonempty membership, armies and exact H3M/gzip
  checks remain unchanged. Map bytes/name are preserved (its historical mana200
  description is not a new-growth scenario promise). No production formula or
  candidate metadata changes. This additional fixture delta awaits Build rerun
  and must be included in final review rather than claiming chain-only changes.

- **Final Runtime growth review:** independently read `future-hero-chain-build.exit`0
  and all five chain XMLs/exits: future36 =35 PASS +1 export skip in both contexts;
  activated75 =73 PASS +2 skips; regressions128/39 with2/1 skips, all exits0.
  The chained authoritative cap/zero-gain control is now verified natively, not
  as a GUI diagnostic journey.
  Compared current source against the GUI candidate's87-entry `BUILD-IDENTITY.json`
  source hash map. All changed/untracked Runtime-owned paths are accounted for;
  **no Runtime product source differs**. Only Runtime test difference is the chain
  case and its two includes: removing precisely those reproduces the recorded
  candidate SHA exactly. Other manifest mismatch is Build-owned module-generator
  tooling. Working `Mods/new-horizons/mod.json` now hashes byte-identically to the
  GUI-tested candidate metadata (`c3e47cf73bf9...`). `git diff --check` passes.
  Runtime approves this bounded growth scope for Build's coherent reviewed commit,
  excluding unrelated CRT/privacy work. No Runtime staging/commit or claim of full
  new-spell/mastery/tier completion; next-family product edits remain deferred until
  Build supplies the checkpoint identity/release.

- **Restart and legacy GUI controls now independently reviewed:** Runtime read
  `testing/hero-gui-reload-context/summary.json`: Level2 reload restored base,
  total, last gains, Axe/book, XP1000, Pathfinding/Luck and mana10/12. Ordinary
  end-turn reached Day2 with mana11/12, movement1500 and unchanged gains; normal
  Day2 save succeeded, exit0, all914 candidate files unchanged. Tester also reports
  Blue Nullkiller2 build/recruit/exchange/exploration, not a new-scale battle-AI GUI
  effects proof.
  `hero-gui-legacy034-context/summary.json` confirms original f7d8aa403a2f save
  loaded in the future client with2/2/3/10, mana95/100, XP0, 15/9 army and no growth
  entry. Four original schools, Haste6/MagicArrow5 correctly retain this input's
  identity. New control save2dc284883c1f succeeded, normal exit0, original input and
  all914 frozen files unchanged. No legacy+1/Doctrine-NONE/chained/cap-zero GUI
  claim. Both summaries confirm client/Xvfb absence and no child/owned INET findings.
  GUI lease is released; wait for Build's native36/activated75 compiler grant,
  then coherent growth review. No new capability edits in these product files.

- **First ordinary growth GUI proof:** Runtime read
  `testing/hero-gui-gold-context/summary.json` and screenshots
  `11-actual-four-gain-levelup.png` / `12-level2-growth-luck-mana.png`.
  Normal Axe pickup/backpack/re-equip gave Total Attack17/15/17 with Base15;
  ordinary Seer1000XP produced four actual gains3/4/1/2 and Basic Luck selection.
  Visible level2 base18/24/6/12, total20/24/6/12, mana10/12 and luck1 match rules.
  Named Start/Level2 saves have SHA prefixes62b620208f1e/45aae6697370; restart was
  explicitly NOT yet verified in this summary. Exit0, 959 monitoring samples,
  no child/owned INET findings, all914 frozen files unchanged. Build has arranged
  the separate reload/old034 gates; preserve its quiet scheduling. Native36 remains
  queued, not part of the candidate/native35 evidence.

- **Latest context rerun independently verified:** all five
  `future-hero-context-*` XMLs/exits are GREEN: activated74 =72 PASS +2 skips;
  original-context future suites35 =34 PASS +1 skip each; baseline regression128
  =126 PASS +2 skips, curated39 =38 PASS +1 skip. All exits0; Build reports
  incremental build0. The bounded fixture corrections retain their original
  behavioral assertions and now pass under actual canonical activation too.
  Build briefly holds product inputs to copy a NEW green private candidate;
  prior914-file RED candidate remains untouched. Manifest/launcher preflight and
  actual Tester GUI acceptance remain required; shipping module is not activated.

- **Private canonical activation checkpoint:** actual XP export XML
  `future-hero-actual-export.xml`1 PASS independently read; ordinary no-override
  map exists at `testing/hero-native-35/cache/vcmi/testMaps/NHHeroGrowthXP.h3m`,
  767 bytes. This is initialization/export proof, not a GUI quest journey.
  Expanded actual-preset suite `future-hero-activated-regression.xml`74 has
  68 PASS /2 skips /4 failures, independently inspected. Private candidate and
  original RED logs remain preserved; working/shipping module unchanged.
- Bounded fixture classification/repair (not yet rerun): Clone fixture intended
  three-turn duration but supplied raw Power3 under divisor10; now supplies
  `3*savedDivisor` and asserts duration3, retaining live-clone/switch assertions.
  Magic AI fixture intended effective Power99 but supplied raw99; now supplies
  `99*savedDivisor`, adds exact7725 damage control and retains real selection and
  execution assertions. Two legacy-magic fixtures disabled commands/magic while
  inheriting newly activated growth, correctly rejected by production validation.
  The shared command fixture now also selects legacy ratings when commands are
  disabled; explicit nullopt/empty-growth controls were added. No product formula,
  validation or candidate-copy changes. Ready for Build's bounded activated and
  original-context reruns before any GUI offer.

- **Latest independently inspected result:** `future-hero-packet-*` XMLs/exits
  are GREEN: both future contexts35 =34 PASS +1 expected export skip, baseline
  regressions128 =126 PASS +2 skips, curated39 =38 PASS +1 skip, all exits0.
  Real Fire Wall creation/trigger and independent `BattleStart` obstacle retention
  now pass. Adventure snapshots still exclude active battles; no GUI mid-battle
  save support is claimed. Build reports successful incremental compilation.
  Build has placed a short global product-source hold to copy a private future
  candidate and prepare candidate-only preset/export. Runtime changes no registered
  inputs; working/shipping module remains0.2 and immutable034 is untouched.
  Actual XP export and integrated future gameplay remain pending.

- **Bridge follow-up actual RED:** Runtime read `future-hero-bridge-*` XMLs;
  both35-test contexts fail only at `restored.currentBattles.size()==1` (actual0).
  Creation divisor10 and actual trigger damage now pass; 128/39 regressions stay
  green. `CGameState::serialize` intentionally excludes active battles. The test
  assumed unsupported mid-battle world-save semantics, not a lost obstacle field.
  Bounded test repair retains world serialization, explicitly checks no active
  battles in that snapshot, then serializes/applies a real `BattleStart` against
  its independent army graph. Wall count, raw power43, divisor10 and spent action
  availability are checked after that packet roundtrip. Renamed the case to
  `RealFireWallCreationTriggerAndBattlePacketKeepLatchedScale`; no production
  persistence changes or claim of mid-battle save support. Repair unexecuted.

- **Current actual RED, after the 30-green checkpoint below:** Runtime inspected
  `future-hero-mechanics-*` XMLs: both future contexts **35 =33 PASS /1 FAIL
  /1 expected export skip**; regressions128/39 remain no failures (2/1 skips).
  Build reports client/test build0. Canonical data, real named settings wrapper,
  actual Summon and Sacrifice now pass. Fire Wall fails at creation: stored divisor1
  instead of10, before trigger/save assertions execute.
  Bounded source trace found the intermediate Build-owned Lua
  `SpellObstacleDescriptor.{h,cpp}` lacks the field, script serializer entry and
  `toObstacle()` copy. Lua emits it and Runtime JSON/fromInfo already handles it;
  the descriptor drops it between those layers. Requested Build's narrow fix with
  legacy default1; existing native Fire Wall assertions remain unchanged. Do not
  claim trigger/full-save or private canonical activation acceptance yet.

- **Latest verified future checkpoint:** Runtime independently read
  `future-hero-ready-build.exit`0 and all four `future-hero-ready-*` XMLs/exits:
  future baseline/curated **30/30 PASS each**, regression baseline **128 =126 PASS
  +2 skips**, curated **39 =38 PASS +1 skip**, all exits0. The real readiness
  transition and scaled-hero BattleAI test now pass. Old 29-test RED evidence is
  retained. Client/test build success is not graphical acceptance. No canonical
  activation, future commit or change to immutable034 is implied.

#### Next unactivated canonical hero data — explicit provisional v1 proposal

Build owns `config/newHorizonsHeroes.json` (unwrapped snapshot), the named schema
and any eventual `heroes.newHorizons` settings reference. Prepare data separately;
**do not enable it in the shipping preset yet**. Use schemaVersion/rulesetVersion1,
`powerDivisor:10`, `maxPrimary:10000` (Build's accepted provisional proposal).
The cap is an overflow/safety boundary,
not an intended progression target. Keep the existing per-hero mana bonus base
1000%; Runtime normalizes its existing multipliers to Knowledge-as-base-mana.
Intelligence/artifact modifiers remain modifiers, not a second rolled attribute.

For the first canonical table, choose the earlier universal priority proposal:
20/15/10/5 starting and 4/3/2/1 growth assigned in the following priority order.
These are **provisional authoring decisions**, not a claim the external document
settled every class. The later 4/4/1/1 and 5/3/1/1 examples remain supported by the
parser/tests, but are not silently substituted into this v1 table. In particular,
canonical Knight should reproduce 72/96/24/48 at level20 without extras; the
integration fixture's universal 4/4/1/1 is deliberately synthetic, not canonical.

| Classes (resolve actual core registry keys) | Priority, high to low |
| --- | --- |
| Knight, Beastmaster | Defense, Attack, Knowledge, Power |
| Ranger, Barbarian | Attack, Defense, Knowledge, Power |
| Demoniac, Death Knight, Overlord, Planeswalker | Attack, Defense, Power, Knowledge |
| Alchemist | Defense, Knowledge, Attack, Power |
| Cleric, Druid | Knowledge, Power, Defense, Attack |
| Wizard | Knowledge, Power, Attack, Defense |
| Witch | Knowledge, Defense, Power, Attack |
| Necromancer, Elementalist | Power, Knowledge, Defense, Attack |
| Heretic, Warlock | Power, Knowledge, Attack, Defense |
| Battle Mage | Power, Attack, Knowledge, Defense |

The table above now reflects the actual Build-authored unactivated file, reviewed
by Runtime; several priorities differ from Runtime's initial proposal. They are
accepted provisional choices, not undocumented claims of a settled class table.

Initial `extraGrowth` follows Build's accepted four-entry proposal: `core:offence`
-> Attack, `core:armorer` -> Defense, `core:sorcery` -> Power, `core:intelligence`
-> Knowledge, each `[0,10,20,30]`. These provisional specialization rolls are
independent of one another and additive to the ten guaranteed points. This is
not a claim that every school/secondary skill already grants growth. Additional
skill opportunities can be explicitly authored in later versioned data; use actual
scoped NH school skills rather than retired elemental IDs if adding schools.
Order the array deterministically; its saved order determines RNG opportunities.
No Leadership/Siege/Command-rank/mastery entries are invented by this data.

Authored map primary values remain authored values; the profile start is not a
retroactive reconstruction of their current base. Existing binary/crossover
heroes retain their captured identity. Empty/missing old rules stay legacy even
when a later preset contains new defaults. Hero-applicable A/D ratings strengthen
command coefficients, not raw creature attack/defense; creature-specific
specialties survive. Spell damage scales only its power term, preserving fixed
mastery terms; integer duration uses effective whole power (minimum one for hero
enchantments). Summon/Sacrifice Lua expressions and obstacle descriptors have the
reviewed matching divisor handling, but see remaining proof boundaries below.

#### Next coherent native/fixture checkpoint (source-only until Build runs)

Added a real canonical-file/named-schema/full-ID-coverage test with all18 priority
permutations, Knight level20, cap/divisor and four actual skill opportunities.
Added actual Summon and Sacrifice casts, and Fire Wall creation/trigger-handler/
full-save checks to `NewHorizonsHeroGrowthTest`. These new tests are unexecuted;
the last verified checkpoint remains30 green, not these proposed additional gates.

New `NewHorizonsHeroFixtureExportTest.cpp` opts in with `NH_EXPORT_HERO_FIXTURES=1`
and requires an actually activated separate future preset. It has **no mapLoaded
or saved-rule override**. Planned ordinary `NHHeroGrowthXP.h3m`: Red Orrin at17,10,
XP0, Pathfinding only, no authored primary values, book/Haste/Magic Arrow; Red town
at8,10, Blue AI town30,30; nearby Seer Hut21,10 has an Orrin-only normal quest
rewarding1000XP without taking troops. Expected initial base15/20/5/10, mana10;
first actual level gains3/4/1/2 (no starting extra-growth skill), base18/24/6/12.
Current mana does not automatically refill on level-up; Intelligence chosen in
that dialogue can further modify the new limit. Export checks real initialization,
header, exact gzip/readback; it does not claim the Seer GUI journey occurred.
Tester should inspect growth window, complete the normal quest/level-up choice,
check actual four gains, equipment modifiers and save/reload;
source fixture now also places the original Centaur's Axe at18,12 (+2 Attack).
Pick up/inspect auto-equip, move to backpack, re-equip: level1 Base15 unchanged,
Total17 equipped/15 unequipped; after the first level Base18, Total20/18.
This is an ordinary placed pickup, not a given-artifact or primary override.
Actual export/GUI evidence is still pending. Separately labelled chained-XP and
cap-zero diagnostics remain future controls, not changes to the main canonical map;
 load an original034
save in the same future client to verify no growth entry/legacy+1 behavior.

Frontend's level-up fix snapshots actual lastGains and level by value in
heroGotLevel before queuing the window. Runtime reviewed the ordering: state
visitor applies levelUp(primaryGains) before that client callback. Re-reading the
hero later could display a subsequent level; the snapshot avoids that risk.

#### Growth checkpoint review/commit boundary

Do not add leadership/siege/mastery/category changes to the same product files
until Build reviews and commits this growth checkpoint. Runtime's coherent scope:

- Primary profile/growth/scaling helpers and saved hero-rules parser/view; world
  settings/callback snapshot plus hero binary/crossover identity and serialization
  version. Old/default caster divisor1 and old/null hero view remain mandatory.
- Authoritative four-delta level-up packets, readiness ordering, seeded independent
  rolls and map-XP initialization; mana normalization, A/D bonus inheritance
  boundary and matching adventure-AI estimates.
- Native spell power-only scaling, proxy/obstacle snapshot behavior; Build-owned
  Lua descriptor/binding/formula changes are necessary cross-owner dependencies.
- Native canonical/schema/context/AI/cast/packet tests and ordinary no-override XP
  export; explicit fixture context fixes retain behavior assertions. Supporting
  SpellAvailability remains unwired and must not be described as new spell-roster
  implementation if included in review.
- Frontend owns actual snapshot-based growth and four-gain level-up views/assets;
  Build owns canonical data/schema/CMake/private-candidate tooling. Exclude
  unrelated release/CRT/privacy changes from the growth review scope.

Before the checkpoint commit: finish independent restart/reload and old034 controls,
run the queued native36 cap/chain diagnostic with Build's compiler grant, and review
source identity/dirty-file scope. Do not infer tested diagnostic GUI/cap saves or
Windows growth gameplay from these results. Working/shipping activation remains a
separate Build decision; no Runtime staging, commits or compiler invocations.

After this checkpoint, propose saved leadership/siege rules and actual read-only
views first. Leadership is class/archetype base plus per-level capacity with skill
modifiers, not another primary roll; declare a non-destructive capacity policy
before enforcement. Siege derives from trained mechanics, not hero level. Then
implement validated Expert mastery eligibility/three choices, followed by explicit
saved creature categories. Send exact versioned schema/view/choice contracts before
Frontend binds them; no placeholder values or legacy-tier inference. These remain
full-goal obligations, not part of this growth acceptance claim.

#### Post-freeze independent source work

Added one **unexecuted native diagnostic** to `NewHorizonsHeroGrowthTest`:
`ChainedLevelQueriesReportActualCapClippedGainsIncludingAllZeros`. It uses the
existing synthetic fixture cap (not canonical data), fills eight non-extra skills
at Expert, and submits real query replies across three level-ups. Expected actual
packets/views are `[4,0,0,0]`, `[1,0,0,0]`, then all zeros at cap; an earlier copied
view must retain its own gains/base. No ordinary XP map, frozen candidate, product
rule or GUI state was modified. Queue this single test with Build after its next
compiler grant; do not claim it ran or exported a diagnostic save.

Following growth GUI feedback, the next proposed family is real saved leadership/
siege capabilities, then mastery eligibility/three choices and validated selection,
then explicit saved creature categories. No new public views exist yet. Leadership
must be class/archetype base plus level growth with skill modifiers, not an A/D
formula or additional random primary stat. Capacity policy must preserve armies;
siege must reflect trained mechanics. Frontend was told not to infer these values
or categories from existing tier labels/icons.

#### Outstanding growth activation/acceptance boundaries

- Validate the actual canonical file and named gameSettings wrapper; exercise its
  real new-game activation rather than only per-map native test overrides.
- Native end-to-end scaled Summon counts, Sacrifice healing, and spell-created
  obstacle creation/trigger/save/BattleStart still need dedicated controls. Current
  obstacle proof covers proxy/default scale, not that entire journey. Interpreter
  doubles and compilation are not a substitute for those tests.
- Test ordinary hero progression, read-only window/tooltips, equipment changes,
  save/reload and AI in an integrated future candidate with Tester. No new-scale
  GUI or Windows gameplay acceptance exists yet. Preserve original-mode controls.
- Leadership capacity and siege capability remain unimplemented; neither consumes
  the four-primary growth budget. Any future capacity rule must preserve existing
  armies, never silently delete creatures. Masteries, Command/Wisdom advanced
  specialization, remaining Orders/Doctrines/spell effects and creature tiers remain
  full-goal work, not satisfied by this growth increment.


- New committed foundation is `034238454`; Runtime independently read exit 0 for
  `repair034-build`, `magic-034-committed-build`, and repeated 128/39 profile runs.
  Build froze a separate immutable034 candidate. Tester reports phase1 normal
  exit0, schema Parsing OK, repeated All/paging interaction and Expert Implosion
  cost13/damage750. Phase2 preserved old four tabs/costs5/6/5 and reloaded/rehired
  the same Orrin with mana95, but timed out before transfer/NONE; no product crash
  claim. Subsequent cleanup/release was independently verified by Build, followed
  by ready-army reload15/9, mana95 and new-battle entry. NONE chooser still not
  captured. No Runtime GUI/process control. Teacher/full-family gates remain.
- **Future lane now authorized beyond primitives; immutable034 remains excluded.**
  Build registered the twelve PrimaryProfile/Growth/Scale/SpellAvailability files
  in mutable CMake only. Runtime independently read `future-primitives-build.exit`
  and both profile exits0, plus XML **13/13 PASS in each profile**. These are not
  tests of live growth integration. SpellAvailability remains unwired.
- New mutable integration is source-ready, **not yet compiled or activated**:
  `NewHorizonsHeroRules.{h,cpp}`, per-world and resolved per-hero saved snapshots,
  new `NEW_HORIZONS_HERO_GROWTH` serialization feature after MAGIC; old binary and
  crossover absence stays legacy, including a capture latch against re-init.
  Game setting is `HEROES_NEW_HORIZONS` / `heroes.newHorizons`. Build owns the
  unactivated named `newHorizonsHeroes` schema and future canonical data.
  Exact v1 shape sent to Build: `{schemaVersion:1,rulesetVersion:1,powerDivisor,
  maxPrimary,classProfiles:{scopedClass:{starting:[A,D,P,K],growth:[A,D,P,K]}},
  extraGrowth:[{skill:scopedSkill,primary:0..3,chances:[0,basic,advanced,expert]}]}`.
  Divisor1..1000, cap100..1000000, four positive gains sum10; chance0..100,
  unique skills, scoped IDs, starting<=cap; full class coverage for new games,
  not retroactive completeness for loaded snapshots.
- Source integration uses the saved per-hero RNG for independent extras, sends
  all four authoritative SetPrimarySkill deltas and actual `HeroLevelUp.primaryGains`,
  and shares the same growth path with map-XP initialization. Hero-applicable A/D
  bonuses stop at the hero inheritance boundary, while creature-specific bonuses
  survive. Hero rating getters use saved caps rather than the legacy99 cache;
  Knowledge is base mana with existing capability multipliers normalized intact.
  Spell raw formulas scale only the power term; fixed mastery terms remain.
  Caster/Proxy default divisor1 is retained. Build explicitly transferred only
  `include/vcmi/spells/Caster.h` to Runtime for this API change.
- Actual source read-only API now exists: `CGHeroInstance::getPrimaryGrowthView()`
  returns optional `PrimaryGrowthView`. Base=current intrinsic ratings, modified=
  effective ratings, profile.starting=saved class start (authored map values remain
  distinct), profile.growth=guaranteed next proposal before cap, extraGrowth=
  independent learned-skill chances, lastGains=most recent actual level deltas.
  Old heroes return nullopt. Frontend owns presentation; no leadership/siege/
  mastery/category fields are invented. Native/activation acceptance still pending.
- Runtime reviewed Build's exact five-file Lua/binding patch: summon divides only
  its power product, Sacrifice only P, obstacle/moat latch `casterPowerDivisor`.
  Native obstacle state/proxy now save that divisor independently of later caster
  availability; legacy/creature default1 remains. Two interpreter tests PASS was
  independently read, not confused with native binding/state verification.
- New source tests: `NewHorizonsHeroRulesTest`3 named-schema/semantic/snapshot cases
  and `NewHorizonsHeroGrowthTest`13 initialization, map-XP growth, seeded extras,
  nontrivial 50% saved-RNG continuation,
  authoritative deltas, full-state/034/crossover persistence, real damage/Order
  isolation, actual scaled cast/mana/budget and obstacle proxy controls. Next:
  First integration build actually exited1: `future-hero-integration-build.log`
  first error705, incomplete `GameSettings` in the new full-state serialization
  test. Runtime inspected the error and added the direct `GameSettings.h` include;
  serializer behavior/assertions are unchanged. Build released a short repair
  window: added the null-callback guard to `getFightingStrength()` and a detached
  campaign control preserving saved rating150 while reporting neutral strength1;
  the connected hero must still report command strength above1. These repairs
  compiled in the repair build. Runtime independently inspected all four actual
  XMLs/exits: `future-hero-future-{baseline,curated}` each29 with28 PASS/1 FAIL;
  `future-hero-regression-{baseline,curated}`128/39 with no failures, exits0.
  The only failing case was authority level-up: primary deltas applied, but level
  and lastGains remained pending. `CHeroLevelUpDialogQuery::onAdded/onExposure`
  requires adventure-interface readiness; the fixture omitted that event.
  Test-only repair now asserts the deferred level/zero lastGains, invokes the
  normal `onAdvInterfaceReady` handler, then retains all original level2 and
  four actual-gain assertions. No production query/validation changes. Ready for
  Build's next authorized incremental rerun; green remains unproven. No activation/RC edits.
- While the local compiler lane is reserved for release dependency repairs,
  independently added unregistered `test/battleAI/NewHorizonsHeroGrowthAITest.cpp`.
  It uses actual saved hero-rule initialization, Power990/divisor10, Knowledge1000,
  real BattleEvaluator selection against legal Charge, and authoritative spell
  execution/damage/mana/budget assertions. This is one source-only future test,
  not an executed AI acceptance claim or a change to the pending 29-test repair.
  Queue registration/execution with Build after the current lease.

- Actual 14-proof RED captured and XML independently read:
  `magic-reward-red-commands-native-resume.xml` **13 PASS / Hat FAIL, EXIT1**;
  `magic-reward-red-magic-native.xml` **4 schema PASS / 10 mechanics FAIL, EXIT1**.
  Earlier proof API errors were corrected without changing assertions.
- Bounded production fixes compiled successfully. Actual
  `magic-reward-green-baseline.xml`: **128 total, 126 PASS / 2 skips, EXIT0**;
  curated XML: **39 total, 37 PASS / 1 skip / 1 filter-context FAIL, EXIT1**.
  Runtime independently read both. Nine formerly failing behaviors and all four
  schemas pass. Remaining exception was a proof-origin error: core cannot depend
  on NH school IDs. Test-only fix now uses each school's actual owning scope,
  asserts exact identifier resolution and core→NH denial, retaining every expected
  membership set. No production dependency bypass. Final rerun now GREEN:
  `magic-filters-final-baseline.*` **128 = 126 PASS / 2 skips, EXIT0**;
  `magic-filters-final-curated.*` **39 = 38 PASS / 1 skip, EXIT0**. Runtime
  independently inspected XML and exit files. Build now holds registered sources
  for reviewed commit, incremental Windows/Linux identity builds and new freeze.
- Production repairs canonicalize authored secondary
  IDs/variables in JsonKeyExtractor; use saved spell levels and new/original school
  union; resolve server skill changes and reward IDs BEFORE rank arithmetic;
  resolve limiter checks, reward/limiter components and quest text, including
  no-selected-hero quest components using its existing game callback. The LEVEL
  factor now counts known spells. Eight owned files, no global entity mutation,
  getter aliases, frontend API changes or player-validation bypass.
- GUI95 exposed unsupported `patternProperties` (78 unknown scoped keys). Build
  repaired mutable schema with supported typed `additionalProperties`; all four
  named-schema tests now PASS in both native profiles, exercising full/empty/real
  settings and malformed nested spell/faction/version data.
  No generic validation suppression and no mutation of immutable95.
- `NewHorizonsMagicFixtureExportTest` actually PASSES: ordinary full book
  **69 original / 59 combat spells**, map-authored rank3/2/1/1 converted through
  actual curated initialization, no rule overrides, parser/gzip exact readback.
  `testing/magic-native/cache/vcmi/testMaps/NHMagicFullBookRanks.h3m` is 666 bytes.
  School membership counts are 12/11/16/18/7/10 (overlap intentional). Content was
  notified for independent header/hash and later GUI audit. Independent fixture
  audit now reported PASS; no broad school GUI pass yet.

- First six-school build actually passed **691/691, EXIT0**. Baseline
  `magic-first-baseline.*`: 103 tests, 101 passes, one expected skip, one RED.
  Curated `magic-first-curated.*`: 8 tests, 7 passes, one RED. Runtime inspected
  both failure logs. Real six-school rank/cost/server cast, starting conversion,
  legacy-world exclusion, full game and BattleStart saved rules all passed.
- Both fixes and added controls are now actually GREEN: build EXIT0,
  `magic-fixes-baseline.*` **109 total / 108 passes / one expected skip, EXIT0**;
  `magic-fixes-curated.*` **20 total / 19 passes / one context skip, EXIT0**.
  Runtime independently inspected both XML files. Real installed Havoc AI choice,
  exact server cost, turn controls and legacy-header/world/new-game continuation
  all pass. Registered production is briefly held for Build's coherent milestone
  review, commit-identity rebuild and immutable copy. No Runtime builds or commits.
- The latter requires a separate private native `config/vcmi/testModSettings.json`
  preset including `core`, `vcmi`, `vcmi-test`, `new-horizons`. Keep baseline profile
  unchanged; school tests explicitly skip when its required registry is absent.
- Both formerly predicted REDs are now actual: successful Charge expired a
  preexisting STACK_GETS_TURN bonus (speed 10→5); actual ActiveModsInSaveList threw
  ModIncompatibility for the legacy header. Assertions remain intact.
- Fix 1 appends HERO_COMMAND to BattleUnitTurnReason, uses it only for successful
  command reactivation, and exempts it alongside existing UNIT_SPELLCAST from
  turn-bound bonus expiry. Legacy HERO_SPELLCAST/normal-turn behavior is unchanged.
- Fix 2 permits only an EXCESSIVE exact curated NH module in the save loader,
  documenting its non-replacing/save-scoped content invariant. The global mod
  verifier is untouched; required missing/disabled NH and other excess/missing
  dependencies still reject. Added safety controls pass. Required NH rejection
  was exercised in ONE baseline installed-state configuration: the latest native
  XML now records and asserts **DISABLED** against installed inventory. NH-absent
  NOT_INSTALLED is not a separately executed configuration; do not claim both.
  VERSION_MISMATCH alone is not an ordinary-save blocker in ActiveModsInSaveList
  (its caller ignores that status).
- Tester reports repaired activation works after real save/quit/restart/load, all
  three Orders, shared Bloodlust budget, Doctrine switch/persistence, seven rounds
  of bookless Blue AI choosing Aggressive. New-battle NONE and spell-AI journey are
  still pending. The first failed 542 profile genuinely omitted NH from its active
  preset; its save is legacy, not something to reinterpret. Build's launcher fix
  explicitly activates the curated module. Preserve those independent artifacts.

### Six-school foundation WIP (no compile or gameplay acceptance yet)

`lib/spells/NewHorizonsMagic.{h,cpp}` validates saved `magic.newHorizons` settings:
versions 1/1, ordered six scoped schools, all common hero-spell memberships,
optional per-spell level/cost[4], faction major/minor and optional positive weights
(default 3/1), six schoolSkills and legacy skillReplacements. Canonical
`config/newHorizonsMagic.json` is the **unwrapped** object; Build wraps it in generated
module settings. Invalid/unregistered data fails closed, not an inert spell list.

Public game APIs: `getMagicRules`, `getActiveSpellSchools`, `getSpellSchools(SpellID)`,
`getSpellLevel(SpellID)`. Battle counterparts: `battleGetActiveSpellSchools`,
`battleGetSpellSchools`, `battleGetSpellLevel`. Hero adds `getMagicRules`,
`getSpellSchools(const spells::Spell *)`, `getSpellLevel(const spells::Spell *)`;
existing best-school/rank and cost getters now use that snapshot. Frontend wired
those actual APIs, not hardcoded fictional IDs.

CGameState and BattleInfo carry separately serialized magic snapshots; proxies
and CGameInfoCallback delegate to the owning snapshot (not generic MapInfoCallback:
EditorCallback deliberately has no gameState and keeps its safe legacy default). NEW_HORIZONS_MAGIC is appended
before enum aliases with monotonic assertions. SpellSchool gains feature-gated
scoped-string serialization with legacy numeric reads; missing scoped identities
throw rather than falling back to an unrelated module.

Casting/learning coverage in source: hero mastery/damage-school bonuses, exact
adventure and battle mana costs, spell-level mechanics and filters, Mage Guild
school-weighted pools and saved-level partitions, Scholar/Eagle Eye limits, AI
spell/scroll/school reward and boat-cost queries. Old elemental tomes and damage
artifacts retain affinity behavior; globals CSpell.schools/level/cost are untouched.
AI's AtLeastOneMagicRule also uses saved schoolSkills and actual known-spell
membership instead of permanently preferring old school IDs.
`test/battleAI/NewHorizonsMagicAITest.cpp` now actually PASSES evaluator/authority
choice, Havoc Expert rank, saved cost and shared budget in the curated 20-test run;
crucially it relies on actual module activation, not a fixture override.

Build's pre-commit source review found a Tome AI affinity regression: the school
factor matches only new schools, not original affinity. Runtime additionally found
that the existing `knownWeight` counts UNKNOWN spells while its caller uses
`1-factor`: the new mismatch therefore MAX-values every original Tome, not zero.
`test/battleAI/NewHorizonsTomeAITest.cpp` now has actual RED→GREEN in both profiles.
Runtime independently inspected XML: four-school RED scores unknown=0/known=20000;
six-school RED scores 20000/20000 for all four tomes. The narrow affinity-union and
SCHOOL-known-counter repair passes all 4+4 proofs. Actual grantability is checked,
not just a score formula. Runtime independently verified final 113 baseline / 24
curated XML results, each with one expected/context skip and no failures.

Foundation source identity is now `95a7001e3`. The first Windows feature client
and install completed: `sdl-main-feature-build.exit` is 0 and
`build/new-horizons-windows-cross/install/VCMI_client.exe` exists (Runtime verified
both). This is build/install evidence, NOT Windows gameplay acceptance. The
Windows-only `VCMIDirs.cpp` repair uses the Boost path's native wide `c_str()`
instead of the unsupported wstring stream constructor; Linux was untouched.
Build completed the committed-identity Linux rerun and immutable GUI copy, then
released mutable production. The reward gaps are not closed by that foundation.

The now-registered reward/feedback/filter/application and LEVEL tests prove the
failures reported above: authored IDs bypassed conversion, quests could reject
migrated ranks, feedback displayed retired schools, and raw reward rank arithmetic
could downgrade a trained school if only the final server callback were remapped.
Spellbinder's Hat also had the analogous LEVEL-known-counter inversion.
Production repairs followed actual RED; their next GREEN run remains pending.

New-game starting old magic skills convert by saved data (duplicate ranks use max,
not addition); offering filters respect map bans and keep NH skills out of legacy
worlds. Six real ranked secondary skills/art/data are Build/Frontend-owned.

Still required: Tome AI proof/repair, broader guild/adventure/reward integration
coverage, dedicated new spell-effect families/AI, and integrated six-school UI
journeys. Positive scoped cast/persistence and legacy-header fixes now have the
actual native evidence above. Growth/scaled primary and derived
attributes, masteries and creature tiers remain later full owned requirements.

Before registering additional common hero spells, preserve the shipped 69-spell
snapshot boundary: current `validateRules` requires coverage of every installed
common spell, and `spellSchools` rejects missing entries. New roster work must
separate new-game completeness from old-snapshot validation and enforce per-world
spell availability (including artifact/AI enumeration), rather than breaking old
six-school saves or leaking new spells into legacy worlds. This is a prerequisite
for that future expansion, not an additional blocker for the current 69-spell
candidate.

During the next registered-source freeze, authored only an independent future
primitive: `lib/entities/hero/NewHorizonsPrimaryProfile.{h,cpp}` and
`test/hero/NewHorizonsPrimaryProfileTest.cpp`. These unregistered files parse
`{starting:[A,D,P,K],growth:[A,D,P,K]}`, require four positive growth increments
summing to ten, and compute deterministic int64 base ratings. Three source-only
proofs cover the level-20 Knight example, class-specific distributions, malformed
data and overflow prevention. This is **not** saved hero-growth activation or a
frontend view/choice API; primary caps, creature-stat isolation, mana, independent
skill rolls and derived attributes remain unimplemented.

### Implemented source, not yet integrated acceptance

- `HeroCommand` IDs NONE=0, CHARGE=1, HOLD_THE_LINE=2, ADVANCE=3,
  AGGRESSIVE=4, DEFENSIVE=5; `BattleAction::makeHeroCommand(side, command)` uses
  existing validated MakeAction transport. Queries: `battleUsesHeroCommands`,
  `battleCanUseHeroCommand`, `battleGetActiveOrder`, `battleGetActiveDoctrine`.
- Full coefficient JSON is captured at new-game init, serialized per game and
  copied into battle state. Missing old-save rules default to legacy, independent
  of currently installed module defaults. Build owns canonical config, strict
  schema and generated inline module settings/equality checks.
- Commands use StartAction/SetStackEffect/EndAction, existing damage/speed bonus
  mechanics and a dedicated non-spell bonus source. Shared once-per-round budget
  excludes spells in both directions; commands cost no mana/book/creature turn.
- Declared first-slice semantics: recipients are currently living ordinary own
  stacks (not turrets/SIEGE_WEAPON). Orders expire next round. Doctrines persist
  across rounds **within the battle**, switch without stacking; same selection
  and NONE/removal reject without spending. No cross-battle hero preference,
  stationary-history requirement for Hold, or Wait restriction for Aggressive
  is implemented. These limitations are explicit, not claims of full philosophy.
- BattleAI evaluates legal command effects in its existing hypothetical exchange
  scoring alongside legal spell/target pairs, with no fixed default Order. Actual
  situational AI tests pass in the committed command milestone; six-school AI
  behavior remains to be verified under its separate real registry/profile.

### Actual failures, fixes and evidence

`commands-build-fix2.log` failed instantiating complete game-state serialization.
Focused concrete-type includes were added only to `HeroCommandTest.cpp`, preserving
all assertions; Build's resumed client/test build exited 0.

`commands-native-resume.log/xml`: **17/19 pass**, including all nine spell/Order/
Doctrine budget combinations and real damage/movement/expiry/replacement controls.
NamedSettings failed because the synthetic array lacked its required resource mod
scope; fixed with `ModScope::scopeBuiltin()` (no lookup fallback). Full-state
roundtrip failed resolving an identifier. `commands-baseline-resume.log/xml`:
**63 pass, one expected skip, three town binary-compatibility failures**.

Root cause: Runtime incorrectly inserted HERO_COMMANDS after the MINIMAL enum alias,
which made CURRENT=894 and disabled later serializer feature gates. Fixed by moving
HERO_COMMANDS immediately after TOWN_CUSTOM_INITIAL_GARRISON, before aliases, with
an explicit monotonic static_assert. Do not treat pre-fix feature save bytes as a
valid redesigned-rules candidate. Assertions were not weakened.

Actual corrected-version run `commands-version-fixed.log/xml`: 86 passes, one
expected skip, one failed AI fixture. All 19 command tests and all 66 baseline
regressions passed. The AI fixture's Magic Arrow at capped power 99 was not a
sound dominance oracle against 100 Angels. Changed only that fixture to Implosion,
asserting effective power, legal cast, substantial damage relative to melee and
nonlethality; retained actual evaluator choice and authoritative server execution.

Build subsequently reports actual build EXIT0 and `commands-integration-resume.log/
xml/exit`: **91 passes plus one expected export skip, EXIT0**, including both real
AI choices, all four persistence/recipient tests and all prior baselines. Build log:
`commands-resume-20260906T191510Z.log/.exit`. Native green is not GUI acceptance.

### New native proofs and next executable task

- `test/battleAI/HeroCommandAITest.cpp`: actual evaluator chooses a beneficial
  command without a spellbook, or a strong offensive spell despite available
  Orders; each chosen action then goes through the real server validator. Checks
  mana and exhausted shared budget. Both now pass.
- `test/server/battles/HeroCommandPersistenceTest.cpp`: separately authored full
  BattleStart packet roundtrip into independent pre-battle game/army state, then
  actual packet application, round expiry and validated Doctrine switch. Build
  registered/compiled/ran it: original state is checked intact. All four tests
  pass, including war-machine/enemy exclusion, no ordinary recipient availability,
  and the explicit late-arrival limitation: new units gain no retroactive Doctrine
  bonus; switching Doctrine applies to then-living eligible stacks. Clone's existing
  Lua implementation creates a fresh unit, not a copy of command bonuses.
  This is not ordinary mid-battle GUI save support: CGameState excludes active
  battles from normal serialization.

`HeroCommandFixtureExportTest.cpp` is now source-ready, not yet executed:
`NH_EXPORT_COMMAND_FIXTURES=1`, filter `BooklessAndSpell/HeroCommandFixtureExportTest.*`.
Exports `NHCommandsBooklessAI.h3m` and `NHCommandsSpellAI.h3m` under the existing
private native cache's `testMaps` only after parser and real-init assertions, then
checks gzip EOF/CRC and byte equality. Red hero 0: A2/D2/P3/K10, book with Haste,
Bloodlust, Magic Arrow. Blue hero 2: A2/D2/P3 or 99/K10, explicitly bookless or book
with Magic Arrow/Implosion. Both: 600 Dendroid Guards, 80 Grand Elves, Ballista,
100 mana, Basic Pathfinding only. Anchors (17,10)/(20,10), towns (8,10)/(30,30).
Select Red human, leave Blue computer, and choose Gold starting bonuses in normal
setup; the H3M permits both player types, while native init explicitly checks Blue
AI. No GUI state injection or existing-save activation.

Exporter subsequently passed: Build reports 94 tests, 93 passes and one expected
skip, with both named assets copied/audited. No GUI acceptance yet.

New independently reproduced rejection defect: `commands-rejection-red.log/xml/exit`
shows a rejected second command reactivated the unit (3 activations instead of 2)
and expired its temporary speed bonus (5 instead of 10). Existing green tests had
not asserted that state invariant. `HeroCommandRejectionTest.cpp` retains both
failing assertions. Runtime fixed `BattleProcessor.cpp` to return before flow
processing for rejected HERO_COMMAND only. Do not indiscriminately gate all failed
actions: existing unit clients deactivate/block on submission and their
`requestRealized` has no failed-MakeAction recovery. Command chooser only closes and
sends, so it needs no synthetic activation. This preserves existing unit/spell
recovery; no frontend mutation or protocol shortcut. Actual
`commands-rejection-green.xml/log/exit` now verifies **95 total, 94 passes, one
expected skip, EXIT0**; Runtime independently inspected the XML and rejection
suite. Build integrated the scoped native milestone as
`54213f0425500208fe259a6255914f05ad71d663`; identity rebuild/candidate copy remains
Build-owned. This is not GUI or full-scope acceptance.

Independent, unregistered next-batch proof files (not in that milestone):
- `HeroCommandEligibilityTest.cpp`: tactics, missing commander and invalid-side
  guards; also preexisting STACK_GETS_TURN bonus BEFORE a successful Charge.
  That positive characterization is expected to fail from source review because
  command reactivation still uses legacy HERO_SPELLCAST expiry. It is not yet an
  executed defect or an additional Tester GUI hold. Preserve legacy spell behavior
  when addressing it; a distinct command reactivation reason is the narrow option.
- `HeroCommandCloneTest.cpp`: actual server HERO_SPELL Clone under an active
  Doctrine, no copied command bonus, then a subsequent Doctrine switch applying
  to both original and clone. Source-only, not yet compiled/executed.

Recovered the original read-only Word document under a PDF name at
an external read-only copy of the original design document; re-extracted all 990 paragraphs
under `/tmp` and read completely. Do not redistribute source document or art.
Future-school compatibility findings: preserve builtin four IDs/global legacy
spell classification; expose saved active school/membership mappings. SpellSchool
currently serializes as StaticIdentifier (numeric), so six-school work must address
stable IDs or feature-gated scoped-name serialization, retaining old numeric reads.
Prose/list Blind school disagreement joins the declared provisional data choices.

Next: Build reruns the rejection proof and full combined suite, then Tester performs
the frozen normal-input human/AI journey with the authored maps. Fix any concrete
failures before first-increment acceptance, preserving old saves. Independent human/AI UI/save journey
is still required before first-increment acceptance. Six schools, growth/scaled
attributes, masteries and tiers remain later owned implementation families, not
completed or blocked by remote API authentication.

## W1 — simulation / runner ownership

Owns `client/ServerRunner.cpp`, `client/ServerRunner.h`, and `server/` only (plus this coordination note). Initial tree was clean. Read AGENTS, MVP, upstream Coding Guidelines, Networking and Code Structure; Networking's universal-TCP statement is historical and contradicted by current implementation.

### Proven startup trace / W2 interface

`CMainMenu::openLobby` -> `CServerHandler::startLocalServerAndConnect(false)` -> runner `start(loadMode == MULTI, connectToLobby, si)` -> runner `connect`. `ServerThreadRunner` runs `CVCMIServer::prepare` and `run` on `runServer`; non-lobby `connect` uses `createInternalConnection`. `NetworkServer` construction creates no socket; only `start` creates TCP acceptor. Internal connections retain serialized packets, `CVCMIServerPackVisitor`, and `CGameHandler::handleReceivedPack` validation/AI ordering.

**W2 requested change:** ordinary single-player must select `ServerThreadRunner` regardless of saved `server.useProcess`; preserve `start(false, false, si)` and current connection/shutdown flow. No runner API change needed. W1 will not edit `CServerHandler` or menu files.

### W1 proved defect and implemented minimal fix

`CVCMIServer` constructor starts UDP discovery while initial state is LOBBY, before `prepare(false, false)` knows transport intent. Moved discovery startup into the `listenForConnections` branch after successful TCP startup in `server/CVCMIServer.cpp`. No discovery creation for internal-only sessions. Global-lobby login still explicitly calls `startAcceptingIncomingConnections(true)` and retains discovery then. No change to simulation, commands, AI, save/load or threading architecture. No other owner files/notes present at initial inspection.

### W5 focused verification request

Check constructor has no discovery startup; `prepare(false,false)` creates only the socket-free NetworkServer holder; explicit listening alone starts TCP + discovery; internal start/load/restart/shutdown never creates discovery. Independently test stale `useProcess=true` selection after W2 fix. Source checks do not establish playable acceptance.

### Build / authorization

No assigned build root communicated to W1 yet; no new root, package installs, GUI/game launches, commits or pushes performed. W6's concurrent CMakePresets change was inspected and preserved; it proposes `build/new-horizons-linux`. W6/integrator should provide build readiness and focused test target. Runtime/graphical acceptance remains pending separate authorization.

### W1 verification / W2 response

Read `docs/NH_FRONTEND_HANDOFF.md` once it appeared. Agree exact file boundaries and unchanged runner interface; W2's thread-selection and debug escape fixes complement this patch. No W1 edits to runner/header were needed for the discovery fix.

Five inline Python unittest source checks passed: constructor discovery regression (also confirmed HEAD contains the defect), discovery guarded by explicit listening and sequenced after TCP start, socket-free internal holder and discovery-null state transitions, unchanged internal runner connection/simulation loop, and unchanged authoritative packet dispatch. `git diff --check` passed. These are source checks, not compiled or runtime tests; W5 should supply durable independent negative coverage.

Initial failure review found that preparation exceptions terminated the process. The following implementation supersedes that deferred proposal; full game runtime verification remains outstanding.

### W1 readiness/lifetime implementation — Frontend catch contract

`IServerRunner` API is unchanged. `ServerThreadRunner::start` now owns its readiness promise inside the worker. Exceptions from thread naming or `prepare` are captured, the failed thread is joined, the partial server destroyed, and the original exception rethrown synchronously from `start`. Constructor/thread-creation failures also propagate synchronously, without a live worker. Successful return still means preparation is complete, not that the client connection callback has run. No fallback to process/TCP is introduced.

**Frontend action:** catch `std::exception` around local runner startup, reset the runner and report through existing failure UI; do not call `connectToServer` after failure. The runner can safely be reset, shut down or waited after a failed start. Unknown exceptions are also preserved (not converted into arbitrary messages). Do not retry a failed preparation automatically or wait for a connection callback which was never scheduled.

`wait` is safe before startup and on repeated calls. Destruction stops and joins any remaining worker. Starting an already joinable runner is rejected with `std::logic_error`, without replacing its server. Lifecycle calls must remain serialized on the owning client thread; these changes do not promise concurrent start/reset safety. Normal successful-session packet-based disconnect remains unchanged.

`shutdown` now calls new `CVCMIServer::stop`, which delegates to the existing thread-safe Asio event-loop stop, rather than racing the simulation by writing `state`/destroying discovery from the GUI thread. Cancellation before the loop enters `run` is retained by Asio's stopped state. After the loop exits, `CVCMIServer::run` finalizes SHUTDOWN on the simulation thread, preserving final state and discovery cleanup without a GUI-side state race. `wait` still waits for a currently executing callback to finish; frontend must retain its existing interface-mutex release around joins. A queued connection-established callback after cancellation is a frontend-owned state check, not a reason to change internal transport here. Exceptions during gameplay `run` are outside the preparation promise and remain existing behavior.

### W6 compile coordination

The active build owns compilation; W1 will not start a competing CMake/Ninja build. Please ensure changed `client/ServerRunner.cpp` and `server/CVCMIServer.cpp` are recompiled (and header dependents rebuilt) before integration. Added `server/tests/test_server_runner.py`. Four default source checks passed via `python3 server/tests/test_server_runner.py`; `git diff --check` passed. The build owner should run `python3 server/tests/test_server_runner.py --build-dir build/new-horizons-linux` after/between native compile work. This compiles the actual runner implementation/header against fake collaborators with GCC C++20, warnings-as-errors, then runs with a timeout: construction/prepare exception preservation, cleanup after failure, reuse, duplicate-start rejection, repeated shutdown/wait, 100 early cancellations, internal connection selection, and destructor joining. It writes only one test executable in the existing assigned build root. Build owner subsequently ran the harness: `build/new-horizons-linux/integration-runner-test.log` records all four source checks and production-runner/fake-server lifecycle tests passing. W1 independently read that result; no harness-revealed runtime defect requires a patch. It is not a substitute for real-server/Asio or graphical acceptance.

### To NewHorizons:Frontend — independent cancellation review

Reviewed the current two-file frontend diff against the runner implementation. No overlapping edits made.

**F1 (high): cancel then immediate restart can accept a stale connection or race a join.** `CSimpleJoinScreen::leaveScreen` sets CONNECTION_CANCELLED then immediately `close()` exposes the menu. Before the queued old `onConnectionEstablished` takes the interface mutex, a new menu action can call `resetStateForLobby` and create a new runner, setting CONNECTING again. The old callback now passes the CONNECTING assertion and installs the old connection as the new session. Alternatively, the old callback observes CANCELLED and enters `waitForServerShutdown`, which releases the interface mutex around `serverRunner->wait()`. A new menu action can replace/destroy that same runner while its join is in progress, causing concurrent join/lifetime misuse; the callback may subsequently reset the NEW runner. Idempotent sequential `wait()` is not concurrent-join protection. Keep setup/restart unavailable until cancellation cleanup completes, and/or give callback cleanup stable session identity and runner ownership. Do not rely solely on the global client state check after a new session can start.

**F2 (medium): cancellation after connection-established but before lobby entry need not run cleanup.** Once `onConnectionEstablished` has run, no further connection-established callback is pending. `leaveScreen` stops the simulation loop and closes the window, but internal `stop()` and server destruction do not generate client `onDisconnected`; `InternalConnection` has no disconnecting destructor. Internal success also schedules no retry timer. Therefore neither newly added CANCELLED callback branch is guaranteed to join/reset the cancelled runner or clear the old connection before the menu is usable. Ensure the cancel action itself arranges deterministic cleanup, including the already-established case, rather than relying exclusively on a future connection/disconnection event. This reinforces F1's gate requirement. Existing stop semantics are cancellation, not a transport disconnect notification.

**Other reviewed cases:** preparation occurs synchronously during progress-window construction, so normal GUI Cancel cannot run before `start` reports readiness. A thrown preparation failure has already joined/reset on the runner side; frontend catch/reset/NONE/rethrow followed by `openLocalGameSetup`'s std::exception dialog is compatible. Constructor/thread-creation failures also have no live worker. Sequential shutdown/wait/reset/destructor repetition is safe. No process/TCP fallback was introduced. Unknown non-std exceptions intentionally remain rethrown rather than user-message-converted.
