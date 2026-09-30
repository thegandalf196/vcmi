# New Horizons implementation sprints

## Purpose and authority

This is the durable execution register for completing New Horizons. It answers:

- what is being implemented now;
- what will be implemented next;
- what remains across the whole design;
- which dependency or verification gate prevents an item from being called done;
- which commit, test, build, or playable snapshot proves each completed step.

It does not replace `design-sources/New Horizons.md`, which remains the sole
canonical design specification. It does not replace `NH_USER_PRIORITY_QUEUE.md`,
whose open user-assigned items take precedence. `NH_COMPLETION_AUDIT.md` remains
the broad requirement inventory; this file turns that inventory into an ordered
working sequence.

## Maintenance contract

Update this register whenever work is selected, materially changes state, is
blocked, is committed, or obtains new target-platform/playable evidence. Never
move an item to Done merely because source exists or a narrow static check passes.

Every implementation item moves through these evidence states:

1. **Planned** — canonical rule and dependencies identified.
2. **In source** — authoritative behavior, AI, persistence, UI/log feedback,
   content and provisional art are present where applicable.
3. **Reviewed** — independent review findings are repaired.
4. **Native verified** — focused native compilation/tests pass on the exact
   commit and platform claimed.
5. **Playable delivered** — a validated immutable snapshot/package containing
   that exact commit is selected or published.
6. **Accepted** — required in-game visual/gameplay review has passed.

For each failed build, update `NH_RELEASE_FAILURES.md` with its run/head, exact
failure, cause, repair, guard, and first succeeding target run. Never discard a
failed run merely because a later run succeeds.

## Current implementation priority — complete Skills perks and spells

### 2026-09-30 Phase 1 source/native checkpoint — Hydra's Vitality

Source committed and pushed as `75c8aea71b8c4be48d561d727a897ee88d62c9fb`;
remote branch identity was verified and the worktree was clean. Full Windows
preview [run 36665665686](https://github.com/thegandalf196/vcmi/actions/runs/36665665686)
is queued on that exact source (`preflight_only=false`). Poll this same run;
dispatch is not a Windows compile/package result. Do not cancel/restart it
merely because an observation times out. No Linux launcher snapshot promotion.

2026-09-30 final source/native gate: both Linux targets build successfully;
the isolated refreshed Hydra filter passes 8/8 and existing health guards
16/16, zero skips. Runtime and actual AI submission/activation parity are
verified, with all legal Orders retained in the controlled AI fixture. Temporary
diagnostics are removed. Content/inventory/perk checks pass 73/73; UI source,
module mirror and diff guards pass. Independent review has no blocking finding.
Coverage is now 57/67 combat identities, Nature 9/11, active perks 114/310.
Full combat save/load/status interactions, reach-aware Order valuation,
two-packet expiry presentation and rendered/playable acceptance remain Phase 2.
No launcher promotion. Next unblocked exploration is Elemental Convergence;
Nature's Wrath awaits its two recorded chain-rule clarifications.

UP-041 follows pushed Verdant Prison checkpoint `758da1d99` and its delivery
record `740df792e`. A bare STACK_HEALTH enchantment would grant free body HP
to every non-front survivor. Implement a compact current-health cohort ledger
only when needed, retain normal health behavior otherwise, and keep activation,
expiry/Dispel and detached AI on the same principal paths. Runtime owns health/
lifecycle plumbing; AI and UI use separate files. Root owns registration,
canonical rounding clarification, original Provisional art, focused validation
and reviewed delivery. Do not increment coverage before those gates pass.

Registration checkpoint: the Level-4, 16-Mana single-target spell/effect and
both native test sources are wired. Purpose-made HoMM3-art 44/32/30 icons are
bound, with retained master/prompt/provenance and inspected reductions; art is
Provisional. Health/runtime and AI workers are active. Two new UI-worker spawns
were rejected by the agent service thread limit; an existing completed worker
slot was reused for the UI-only contract. The Windows run above was re-polled
and is live in package-audit/preflight, not yet a compile result. Coverage stays
at the prior verified checkpoint until the Hydra principal path builds/passes.

Shared-preview checkpoint: canonical targeting, noncompounding capacity and
fractional per-survivor regeneration details are explicit in the Markdown.
The shared saved-v3 effect value computes the capped capacity percentage from
raw SP rather than the legacy divisor; Lua/UI consume that same value.
Content, UI inventory and canonical perk-data checks pass 73/73 after repairing
the stale activation inventory documented in the failure ledger. The UI source
guard passes, but is explicitly not compile/render/runtime evidence. Runtime
cohort implementation and native fixtures remain in progress; do not build
against missing worker files or call the spell delivered. The same Windows
Verdant run was verified live in **Compile Windows x64 client**.

Health-review checkpoint: compact cohorts now exist in shared unit state.
The isolated damage/heal/expiry review found no principal count error there,
but identified a concrete temporary-resurrection cleanup defect: removing
`resurrected * maximumHP` can delete more creatures than the resurrection
count when survivors have different current HP. Root classified this as a
blocking count-integrity repair, not deferred reward polish. Remove exactly
the recorded creature count and add a focused guard before delivery. Require
normalization after bonus addition so the pre-effect health UPDATE cannot
expose free HP, and disable capacity regeneration after its source expires.
Percentage preview now uses millionths of one percent, retaining School
fractions until the final creature-HP floor. UI and AI drafts are frozen;
native execution waits for the runtime/script/test checkpoint.

Independent maintenance delivery: `dff0fe557` is committed and pushed, repairing
only the expected active-perk inventory for nine perks already active in the
previously delivered configuration. Independent read-only review confirmed
that it does not depend on Hydra's unfinished runtime or activate new content.
The 73 focused data checks pass. Hydra remains uncommitted and uncounted while
the runtime owner finishes raw-hex target resolution, controller-aware friendly
eligibility, pre-cost capacity limits and native health-integrity fixtures.

Narrow lifecycle re-review found no blocking source issue in bonus-change
normalization, authoritative round-expiry updates or genuine-activation healing.
Keep the two-packet expiry presentation boundary as deferred rendered Phase 2
work: `BattleNextRound` precedes its normalization UPDATE. This is not a native
compile or gameplay certification. No coverage increase is justified yet.

Build checkpoint: both native fixture sources are present; the serialized Linux
client/test build is running with eight jobs. All source/data guards still pass
(73 Python checks, UI wiring, module mirror and diff checks). Two principal
detached-state omissions are repaired: bonus normalization now reads projected
units, and hypothetical genuine activations consume capacity regeneration.
The C++ pre-cost path now rejects unrepresentable capacities independently of
Lua applicability. Fixture review corrected normal-action recast timing, base
capacity expectations and genuine authoritative activation triggering. Because
two source fixes landed during the first compile pass, require an incremental
rebuild afterward before the tester refreshes the isolated runner. No native
test result, source delivery or coverage gain is claimed by this checkpoint.

The first pass stopped on a status-icon pointer-type mismatch, repaired in
the failure ledger. The second pass recompiled the latest target-validation
source, linked `libvcmi.so` and `libvcmiclientcommon.a`, and progressed into
test compilation. Independent final source review reports no remaining blocking
finding, conditional on the build and focused native results. The build remains
live; do not restart it merely because an observation times out. The separate
Windows Verdant job `36659663956` is still compiling its frozen older source.

Native checkpoint: both Linux targets and the no-stale-object follow-up build
pass. The isolated refreshed Hydra filter runs eight cases with no skips;
five pass, while raw-tail-hex selection, v2 fixture configuration and actual
AI spell selection need repair. The separate health/Regeneration/Cure filter
passes 16/16, no skips. Preserve the failed assertions and retained evidence;
runtime and AI owners are repairing separate files. Coverage remains 56/67,
and this feature remains uncommitted until the focused failures are resolved.

Next-slice preparation is read-only: Nature's Wrath can reuse the existing
nearest-unvisited chain transform and detached cast evaluation with a mixed
damage/survivor-healing effect. Worldroot extends its 17-stack cap to 19 and
strengthens only the SP-derived term by 10%. The canonical document supplies
no numerical jump range, and resistance/path behavior needs clarification.
Two non-blocking user questions are pending: unlimited nearest-stack jumps
versus a finite range, and retaining versus skipping resisted enemy links.
Do not silently implement the unresolved choices; finish Hydra's current
repair/build/native/commit gate first. Tie handling should remain deterministic.

2026-09-30 retry2 checkpoint: client/test targets rebuild successfully; all
six server cases and invalid-target AI pass (7/8 overall, zero skips). The
actual friendly spell-selection case still chooses an Order even after the
distant enemy count is reduced, so actual forecast/candidate-score tracing is
required rather than another speculative fixture adjustment. Existing health
guards again pass 16/16. Coverage remains unchanged; no Hydra commit yet.
The same Windows Verdant run has now completed compile/package/upload
successfully; its frozen source is distinct from these Hydra changes.

### 2026-09-29 Phase 1 source/native checkpoint — Verdant Prison

Committed and pushed as `758da1d99abc74fbe7aeefbb00249269b44c5ec3`.
The full Windows build was dispatched on that exact source as
[run 36659663956](https://github.com/thegandalf196/vcmi/actions/runs/36659663956).
The same run completed successfully on 2026-09-30: Windows x64 compilation,
runtime staging, recursive PE/license/source packaging and downloadable preview
upload all passed. This proves packaging of frozen source `758da1d99`, not
Hydra's later dirty changes or in-game visual acceptance. No Linux launcher
snapshot was promoted.

UP-040 follows pushed Summon Trolls commit `dd73972b7`. Reuse its exact-HP
summon and prospective health paths for the canonical Dendroid ring, dividing
one shared pool across legal placements rather than giving the full pool to
every stack. Runtime and UI have separate file ownership; AI follows the
shared geometry. Root integrates registration, canonical rounding detail,
validation, original Provisional art and delivery. Both Linux targets link;
the isolated active-profile filter passes 11/11 and Summon Trolls guard passes
10/10, zero skips. Content/inventory passes 55/55; targeting source guard,
module mirror and diff checks pass. Independent review has no remaining
production blocker. Runtime includes resistance/immunity and reflected-anchor
handling; actual AI submission matches detached per-hex HP/placement forecasts.
Coverage is 56/67 combat identities, Nature 8/11, and 114/310 active perks.
Original spell art remains Provisional; Warden art is Not done. Full combat
save/load, broad reward/status interactions, AI tactical quality and rendered/
playable acceptance remain Phase 2. No launcher snapshot is promoted.

Next-slice exploration: Hydra's Vitality cannot be implemented faithfully by
adding only a timed `STACK_HEALTH` bonus. `CHealth::creatureHealthAvailable`
derives every full survivor's current HP from its live maximum, so that would
instantly heal a multi-creature stack on cast. Ordinary `HEAL` only fills the
front creature's wounds. The next slice needs explicit unfilled enhanced
capacity, per-survivor activation regeneration without resurrection, and
expiry normalization, shared by authoritative and hypothetical state. Reuse
the genuine activation hook and existing serialized health state; do not
substitute instant healing or a Guardian Spirit shield for this mechanic.
Per-creature/fractional rounding must be recorded alongside implementation.

### 2026-09-29 Phase 1 source/native checkpoint — Summon Trolls

UP-039 was implemented in separate runtime, targeting UI and BattleAI lanes.
Root owns registration, canonical rounding clarification, original Provisional
art, focused validation and integration. The spell uses chosen
empty-hex placement and exact aggregate HP, not the generic summon effect's
automatic placement or whole-creature floor rounding. Beastcaller scales the
whole pool; School rank scales only its Spell Power term. Both Linux targets
link, all ten focused runtime/AI cases pass with zero skips, and two existing
Phantom Army/Transfigure Matter AI guards pass. Content/inventory passes 54/54;
the module mirror and targeting source guard pass. Exact HP/count and spawn/
update JSON roundtrips are verified; independent review has no blocker.
New hypothetical units now inherit ordinary army bonuses through an owned,
source-only stack bearer, matching authoritative Elixir health and count.
Coverage is 55/67 combat identities, Nature 7/11, and 113/310 active perks.
Original art remains Provisional and Beastcaller art remains Not done.
Full mid-combat binary save/reload, broader reward/effect interactions, AI
placement quality and rendered/playable acceptance remain Phase 2 work.
No launcher snapshot is promoted. Next: Verdant Prison and Verdant Warden.

Cross-platform batch checkpoint: GitHub notice/dependency preflight
[run 36656624940](https://github.com/thegandalf196/vcmi/actions/runs/36656624940)
was dispatched on pushed source `dd73972b7` with `preflight_only=true`.
The same run completed successfully. This proves notice/dependency preflight,
not Windows compilation or packaging. Verdant Prison source work continues
independently; dispatch the full Windows build after its reviewed/native
checkpoint is pushed, so the batch includes the new slice.

### 2026-09-29 Phase 1 source/native checkpoint — Vengeful Vines

UP-038 implements the six-hex S-bend using one shared geometry function for
authoritative targeting, full-footprint preview and BattleAI enumeration.
Runtime, frontend and AI have separate file ownership; root owns registration,
art integration, build and delivery. Content validation passes 51/51. The
saved formula uses integer coefficient 11 with the common divisor 10, preserving
the canonical `20 + 1.1 × SP` damage. Fixed Speed −2 and two-round duration
are independent of School rank; rank strengthens the Spell Power term only.
The purpose-made HoMM3-art icon has native/enlarged exports, exact prompt and
provenance, and remains Provisional. Both Linux client/test targets link and
the isolated active-profile filter passes 13/13, zero skips, including actual
AI submission and projected/resolved damage parity. Independent review has no
remaining blocker; preview mismatch and native failure repairs are retained
in the release-failure ledger. Coverage is 54/67 combat identities, Nature
6/11, and 112/310 active perks (unchanged). Full combat save/load, Dispel,
combined movement statuses, hypnosis ownership, wider AI horizons and rendered
keyboard/visual acceptance remain Phase 2 work. No playable snapshot is
promoted. Next missing Nature identity: Summon Trolls.

### 2026-09-29 Phase 1 source checkpoint — Entangle and Rootcaller

UP-037 adds the canonical Nature Level-1 movement-only root, Rootcaller
duration extension, BattleAI targeting/valuation and existing-slot status.
Registration increases to 53/67 combat identities and 112/310 active perks;
Nature is 5/11 by identity. Both Linux targets link and all 17 focused native
cases pass with zero skips, including actual AI casting and the required
root/action/lifecycle paths. Content passes 50/50, perk inventory 2/2, status
wiring 4/4; module mirror and diff checks pass. Independent review's blockers
were repaired; fixture failures and repairs are in the release-failure ledger.
Original Provisional spell art is retained with prompt/provenance and bound
to the live spell. No playable snapshot is promoted by this source checkpoint.

Independent review found two blockers before building: unconditional scoped
spell decoding could throw in classic battles without the module, and a v2
roster retaining Entangle could admit an ineffective cast. Repair both with
safe lookup and authoritative pre-cost version rejection; keep regressions
focused. Combined classic Bind lifecycle, save/load, Dispel, wider AI threat
horizons and rendered/playable acceptance remain Phase 2 work. Next coverage
item after this gate: Nature Vengeful Vines.

### 2026-09-29 Phase 1 native checkpoint — Crusade! and Crusader

UP-036 completes the remaining Light combat-spell identity: a 24-Mana,
three-round friendly-army empowerment with capped Attack/Defense and flat
Initiative, fractional independent magical reduction, and negative-Morale
protection. Crusader adds one round. Runtime, BattleAI and status writers have
separate file ownership; root owns content, module, build and integration.
Focused authoritative and actual AI choice/projection tests are required.
Use the appropriate original Prayer assets by reference for the working spell;
bespoke icon approval and rendered/playable acceptance stay separate. Do not
promote the normal launcher's snapshot merely because development builds pass.

The authoritative effect, saved fractional reduction, status, combat log,
Crusader and BattleAI paths are in source. Echoed Duration applies once to
the fixed base: three rounds ordinarily, four with either duration perk,
five with both. Both Linux targets link; the isolated active-profile filter
passes 19/19 with zero skips, including actual AI submission and casting.
Content passes 49/49, perk inventory 2/2, UI wiring 2/2, module mirror and
diff checks pass. Independent review has no blocking finding. Coverage is
52/67 registered combat identities and 111/310 active perks; Light is 11/11
by identity. Generic duration artifacts, full battle save/reload, Dispel,
hypnosis and wider AI horizons are recorded for Phase 2. Rendering, bespoke
perk art and playable delivery remain open. Next missing spell: Nature
Entangle; do not return to exhaustive Crusade interaction testing before
increasing missing implementation coverage.

### 2026-09-29 Phase 1 native checkpoint — Sorcery Slow

Saved-v3 Slow now applies an Initiative-only reduction of
`min(50%, 20% + floor(scaled Spell Power / 5))`. Sorcery rank, Spellcraft,
and eligible cast modifiers strengthen only the Spell Power term; the fixed
20% base does not scale. Temporal Field still applies 60% to the final
ordinary Slow penalty after target-specific specialties. Ordinary v3 hero
Slow lasts two rounds before Temporalist and existing duration extensions.
Saved v1/v2 casts retain configured magnitude and Spell-Power-based duration.
Hero-context help reports the current pre-specialty estimate and fixed base
duration; the same Lua effect serves hypothetical AI previews and actual
casts. This closes one more authored non-damage School-rank effect under
UP-027 without changing the 37/67 registered combat-spell identity count.

The Linux `vcmitest` and `vcmiclient` targets link. A focused active-profile
filter passes 19/19 with zero skips, including all four rank coefficients,
the 50% cap, Mass magnitude, Temporalist, v1/v2 fallback, preview/cast
parity, and hero-help assertions. Independent review found no Phase 1
blocker. Deferred Phase 2 checks include combined Spellcraft/Warcasting/
Empower rounding, added `SPELL_DURATION` bonuses, and Echoed Duration
specifically for Slow. A broader name filter exposed four unrelated
pre-existing fixture failures: two old Ice Bolt saved-rule builders still
contain `selectedPlacement`, and two AI Temporal Field fixtures violate
the earlier-perk-tier rule. No playable snapshot or rendered tooltip
acceptance is claimed. The next Phase 1 slice should increase missing
spell/perk coverage rather than repeat this Slow integration matrix.

### 2026-09-29 Phase 1 native checkpoint — Shadow Life Drain

Life Drain is now a registered Level-1 Shadow combat spell for saved-v3
New Horizons. Its human target picker selects a living enemy and then a living
friendly stack; the server validates that exact ordered pair before any action
or Mana is spent. It deals `25 + 1.8 × Spell Power` damage, then heals the
friendly stack for 60% of damage actually inflicted, limited to surviving
creatures. The Blood Drinker hook raises the fraction to 75% when its perk is
active. AI enumerates legal complete pairs. The cast logs both damage and the
amount of health actually restored. A purpose-made provisional spell icon has
44×44, 32×32, and 30×30 exports and a retained master/prompt.

The Linux `vcmitest` and `vcmiclient` targets link. A fresh isolated active
New Horizons test profile passes **12/12** focused formula, script,
authoritative server, and AI target-enumeration tests with zero skips. The
client source guard, content-module mirror check, JSON/JSONC parsing, Lua
syntax check, and `git diff --check` pass. Independent review found no Phase 1
blocker. These are source/native results, not graphical/playable acceptance.
Phase 2 should cover Magic Mirror/reflection of paired spells, friendly
resistance and Blood Drinker execution, AI healing valuation, and broader
spell interactions. The next missing Shadow identity is Hex of Pain; the
priority queue remains authoritative before starting it.

### 2026-09-29 Phase 1 native checkpoint — Hex of Pain

Hex of Pain adds one active Level-2 Shadow combat-spell identity (38/67):
three rounds of reactive Shadow damage after each attack or retaliation,
with actual-inflicted-damage clipping and no recursive attack event. BattleAI
projects that injury into attack choices and values the curse as future
prevented enemy attack value. An original purpose-made icon family is bound at
44, 32, and 30 pixels and remains Provisional pending native rendering and
user approval. The Linux client and test targets link; 6/6 focused active-
profile authoritative/AI tests and 36/36 content tests pass. Painweaver's
specified +20% Spell-Power-component interaction, broad save/dispelling and
playable/graphical verification remain open. The next missing Shadow identity
is Frailty, subject to the user-priority queue.

### 2026-09-29 Phase 1 native checkpoint — Shadow Malediction

Basic Shadow Magic's Malediction is active and extends canonical saved-v3 Curse
and Sorrow from three to four rounds. Curse's inherited Spell-Power-based
duration is replaced with its authored fixed three-round rule in v3; v1/v2
saved profiles retain the legacy effects. Recasts replace and refresh their
timed bonuses, spellbook help and battle logs report the actual duration, and
BattleAI values projected Curse/Sorrow duration from hypothetical effects.
Normal Basic-perk selection now opens Advanced Shadow progression. A distinct
provisional thorn-bound hourglass icon was produced with the HoMM3 art workflow,
with master, prompt, 44×44/32×32 comparison, four runtime states and named
client binding.

Linux `vcmitest` and `vcmiclient` link. Under an isolated active New Horizons
profile the focused authoritative filter passes 8/8 and the projected-AI
filter passes 5/5, zero skips. The 17-case perk-data test, module-mirror check,
targeted icon-state/hash check and `git diff --check` pass. Independent review
found no Phase 1 blocker. The full active-perk art guard remains red on 21
pre-existing neutral-icon gaps; rendered/playable Malediction and full AI
action-choice acceptance are not claimed. Phase 2 should examine AI overlap
between current exchange and duration forecasts and equal-strength recast
valuation. Next high-value gap: another missing Shadow spell such as Life Drain,
or another Basic perk that unlocks a progression-deadlocked Skill.

### 2026-09-29 Phase 1 native checkpoint — Shadow Sorrow

The inherited Sorrow roster assignment is corrected from Chaos to canonical
Shadow. Saved-v3 Sorrow is Level 1, costs 4 Mana, targets one hostile stack,
and lowers Morale for three rounds by `min(3, 1 + floor(scaled raw SP / 70))`.
School rank, Spellcraft, Warcasting, and Empower scale only that raw-SP term;
the legacy primary-growth divisor is intentionally not applied. A stronger
recast replaces the earlier penalty and refreshes duration without stacking.
The tooltip, battle log, authoritative cast, and AI's hypothetical scoring
consume this rule; saved v1/v2 retain their old Chaos/Mass behavior.

The Linux `vcmitest` and `vcmiclient` targets link. Under an isolated active New Horizons
profile, all 7/7 authoritative Sorrow cases pass in 1.612 seconds and all 3/3
AI projected-score cases pass in 1.00 second; the content-module mirror and
`git diff --check` pass. Independent review found no blocking issue. This is
source/native evidence, not rendered or playable acceptance; Sorrow was
already counted among the 36/67 identities, so the identity count does not
change. AI's full action choice, unchanged-potency refresh valuation,
malformed explicit-null saved-row hardening, and save/load roundtrip remain
Phase 2 checks. The canonical sentence "cannot reduce Morale below 10"
conflicts with the global −10..+10 range; user clarification is pending, so
the existing global clamp applies. Malediction remains planned. The next
missing-identity candidate is Shadow Life Drain, subject to the priority queue.

### 2026-09-29 Phase 1 native checkpoint — Quicksand exact placement

The saved-v3 Quicksand row now explicitly opts into exact caster-selected
placement. The shared count/legality contract drives ordered client hex
selection, remaining-count/undo/confirm feedback, server validation before
action announcement and effect application, the Lua obstacle effect, and
BattleAI's delayed ground-movement pressure choice. The new obstacles are
concealed even when the spell effect uses minimal content settings; the
`StartAction` presentation omits their coordinates while the authoritative
action retains them. The appended action-serialization feature rejects a
multi-hex Quicksand vector on older protocols. Old v1/v2 and markerless-v3
saved battles retain random placement.

Linux `vcmitest` and `vcmiclient` link. The curated focused filter passes
9/9 native Quicksand rules/Lua/server/AI cases; 12 magic-data tests, both
repeated-placement UI source guards, the generated-module check, and
`git diff --check` pass. Independent review found and the integrator repaired
missing Lua API and client-method wiring before this build. The source guards
are not rendered UI acceptance; no GUI was launched or playable snapshot
promoted. Phase 2 retains concealed enemy-obstacle placement collisions,
full network confidentiality of broadcast obstacle packets, trap lifecycle,
and native-resolution panel readability. Mire Shaper's extra-patch cap still
requires a canonical decision before activation.

### 2026-09-29 Phase 1 native checkpoint — Holy Armor and magical reduction

Holy Armor is registered as a Level-2 Light combat spell (8 Mana, one friendly
stack, two rounds) with a purpose-made provisional icon family. Its reduction
is `min(60%, 30% + 0.20% × scaled Spell Power)`; only the Spell Power term
receives the saved School-rank, Spellcraft, Warcasting, and Empower effects.
The authoritative spell applies one independent `SPELL_DAMAGE_REDUCTION`
source. Current-roster magical damage combines independent reduction sources
multiplicatively, caps the aggregate at 95%, and applies relative penetration;
older saved rosters without Holy Armor keep their prior reduction path. The
same path serves forecast and actual hero/creature spell casts. Non-damaging
spell effects remain unaffected. BattleAI values the projected Armor strength
against visible creature-caster magical damage without reading hidden enemy
hero spells. An independent Astra review found no blocking defect.

Both Linux `vcmitest` and `vcmiclient` link, the curated active-profile focused
Holy Armor/MDR/AI filter passes 25/25, 39 focused Python content tests pass,
and the module mirror check passes. This is source/native evidence, not a
playable visual acceptance or promoted launcher snapshot. Deferred Phase 2
checks: two-round expiry, repeat cast, save/load, Fire Shield's separate Lua
immunity/reflection path (which lacks the saved-roster opt-in), and mixed
reduction/penetration interactions in broad battles. AI currently does not
estimate hero-only magical threats; its creature-pressure and health fallback
are intentionally approximate and require later calibration.

### 2026-09-29 Phase 1 native checkpoint — Quicksand v3 count

UP-027's next concrete gap is Nature Quicksand. Its saved-v3 patch count now
uses the authored formula instead of inherited 4/6/8 mastery data:
`min(5, 2 + floor(scaled Spell Power / 60))` rule. The fixed two-patch base is
unscaled; School rank, Spellcraft, Empower, and battle-only Warcasting compose
on the Spell Power term before one floor. Old v1/v2 profiles must retain their
configured 4/6/8 behavior. This is a **partial Quicksand slice**: the current
NO_TARGET spell still chooses random legal tiles rather than accepting exact
caster-selected, ordered hexes. Required placement UI, authoritative exact
count/hex validation, and deliberate AI placement remain open. Mire Shaper's
additional patch is also still planned; its interaction with the five-patch
cap needs a canonical decision before that perk is activated. The single
saved-profile-aware helper feeds the Lua obstacle application and dynamic
spellbook description. An independent source review found no blocking count,
save, or Lua defect; it identified and the worker repaired a non-discriminating
Empower/Warcasting test. Linux `vcmitest` and `vcmiclient` link, and the
active-profile adjacent `ObstacleTest.*`, `ObstacleApplyTest.*`, and
`NewHorizonsMagicV2RulesTest.*` filter passes 31/31, including the real Lua
placement count at SP 59 and v1/v2 configured-count preservation. The first
test invocation without the custom-school XDG profile failed to resolve the
Nature ID; the active-profile run required by the test contract passed. No
playable Quicksand claim follows from this source/native checkpoint.

An adjacent current-head Spell Lock/Archery filter ran 32 tests: 16 passed,
16 failed. Read-only classification found 15 failures attributable to stale
test fixtures or assertions (cast allowance metadata, strict perk-tier
prerequisites, an unset mock SpellID, invalid creature ability fixture,
obsolete help wording, and an allied-shooter-blocker expectation). The
remaining Skirmisher counterfire forecast assertion depends on enemy-hero
information hidden from the player-scoped AI view; record that visibility
contract question for Phase 2. This is not a green Spell Lock/Archery gate,
but no crash, corruption, or demonstrated authoritative regression blocks
the current Phase 1 implementation slice. Repair the fixtures at a suitable
integration checkpoint, without weakening the production guards.

### 2026-09-29 Phase 1 checkpoint — Empower Spell and Expert Spellcraft

Empower Spell is now a functional Advanced Spellcraft perk: after Wisdom, a
spell costing at least 12 Mana gains +25% to its Spell Power-derived numerical
term. The multiplier reaches direct damage, authored and generic non-damage
effects, and generic durations without scaling fixed bases or flat bonuses.
The selected perk unlocks normal Expert Spellcraft progression, activating
the existing 130% Expert rank coefficient. Original four-state crystal art is
Provisional. Linux `vcmitest` and `vcmiclient` link. The final focused and
adjacent spell filter passes 69/69 native cases; 17 perk-data cases, two
UI-inventory cases, and the module-generation check pass. Independent review
caught and verified repairs for Regeneration overflow, saved-v3 duration
preservation, tooltip punctuation, and Spell Lock saturation arithmetic. The
broad active-perk art guard still reports 21
older unmapped active perks; Empower's own art checks pass. A wider adjacent
filter found five Warcasting tests whose fixtures violate the already-existing
Basic-before-Advanced perk rule; their source was not changed in this slice.
Record them for Phase 2. Mass Slow and broader Lua interaction tests also
remain deferred. No playable promotion or visual acceptance is claimed.

Next Phase 1 coverage target: the highest-priority missing UP-023 spell/Skill
slice after this Spellcraft progression bridge, not more Spellcraft test
hardening merely because additional interaction tests could be written.

### 2026-09-29 Phase 1 checkpoint — Spell Penetration and Advanced Spellcraft

Basic Spell Penetration now has a saved selected-perk gate and ignores 20% of
hostile targets' Magical Damage Reduction on hero spell damage, sharing the
authoritative/prediction path while leaving Mana, resistance and immunity
unchanged. Selecting it permits normal advancement to Advanced Spellcraft;
the pre-existing 120% coefficient is now registered active. New purpose-made
four-state art is Provisional. Linux `vcmitest` and `vcmiclient` link; 4/4
focused native cases, 17/17 registry/data tests and the module mirror check
pass. Independent review found no Phase 1 blocker. The active-perk art guard
still reports 21 older unmapped perks; this new icon passes its own checks.
Cross-perk penetration composition and rendered/playable review are deferred.
Next: one working Advanced Spellcraft perk to unlock Expert progression.

### 2026-09-28/29 Phase 1 checkpoint — Basic Spellcraft efficiency

UP-023 advances Skill-rank coverage from 81/93 to 82/93. Basic Spellcraft is
registered active: its saved-v3 110% efficiency multiplies the applicable
School-rank factor without rounding the intermediate percentage. The shared
basis-point path reaches direct-damage cast/forecast, Cure, Bless, Poison,
Regeneration, Focus Magic, Spell Lock, Time Stop, Transfigure Matter, Phantom
Army, Summon, Sacrifice, and the other authored Lua numeric paths touched in
this slice. Fixed spell bases stay fixed. Old v3 snapshots without the new
field use 100% Spellcraft; v1/v2 reject it. Contextual spell help reports the
live coefficient. AI Poison, Regeneration and Spell Lock projections use the
same coefficient. Formula tests cover manually assigned Advanced/Expert ranks,
but those ranks remain planned because normal advancement needs working Basic
and Advanced Spellcraft perks.

The Linux `vcmitest` and `vcmiclient` targets link; the active-mod focused
filter passes 15/15, the adjacent Focus Magic/saved-rules filter passes 32/32,
and 64 offline magic/content/perk checks pass. The module mirror check passes.
Independent Astra review found a Focus Magic authoritative/tooltip mismatch;
it was repaired and given a real-cast assertion before the passing runs.
Deferred Phase 2: old-v3 Summon/Sacrifice casts may now gain School scaling
that those script paths previously lacked, and non-100% Lua execution needs a
representative runtime test. No rendered/playable acceptance is claimed.

### 2026-09-28 Phase 1 checkpoint — Nature Poison

UP-023 now has a distinct Level-2 Nature hero spell (`new-horizons:poison`),
not a reclassification of the old `core:poison` creature ability. The saved-v3
roster supplies its 7-Mana guild identity, and the authoritative cast applies
the existing serialized physical-Poison state for three escalating activation
ticks; Cure removes it and ordinary Dispel leaves it. A shared formula scales
only the Spell Power term by Nature rank, while BattleAI values the marginal
remaining ticks on detached states. Purpose-made Provisional icon art is bound
through the HoMM3 art workflow, and the existing physical-Poison status panel
provides battle feedback.

The Linux `vcmitest` and `vcmiclient` targets link, a fresh isolated TEST preset with New
Horizons active passes eight focused cast/tick/AI cases with zero skips, and
the old-v2 roster exclusion plus adjacent Magic Arrow AI regression each pass
1/1. The offline content suite passes 47/47 and the module mirror check passes.
Two stale presets skipped every case; their runs are not execution evidence.
Independent Astra review found a detached-state test setup error, repaired
before the passing run. Hero-source kill attribution, broader save/dispel
interactions, rendered icon approval and playable promotion remain open.
Combat-spell identity coverage is now 35/67; it is not effect-completeness
coverage. The next high-value shared gap identified is Spellcraft's missing
rank efficiency and progression perks, with 0/3 rank effects currently active.

### 2026-09-28 active Phase 1 checkpoint — universal Blacksmith and Nature Regeneration

UP-024's saved capability ruleset v4 now defines universal Ballista/Ammo Cart/First Aid Tent stock and nine faction-favored prices. The authoritative town offer is deduplicated at the lowest price, is used by server charging and the new human shop, and is queried by recurring Nullkiller purchase hooks. Stronghold's Ballista Yard grants a nonstacking weekly +20 Siege on town visit, including when built with a hero present. The client source/geometry guard, AI source guard, 53 Python data cases and the focused linked runtime filter pass. Both Linux `vcmitest` and `vcmiclient` link; rendered shop and playable acceptance are not claimed. Independent Astra review's stale-bonus test assertion, build-while-visiting path, and UI ruleset-gate findings were repaired. Broader AI purchase behavior and week-boundary save interaction remain Phase 2 evidence.

UP-023's Nature Level-1 Regeneration and Basic Herbalist are in source with an original provisional icon family, saved fixed-point wound marks, activation-start healing, battle status feedback, and BattleAI forecast. Independent Astra review found and prompted fixes for marks transferring across a casualty, repeated AI forecast healing, and a test expectation error. The final combined active-profile runtime filter passes 17/17 cases across spell formula, authoritative battle, AI, saved shop rules, and Yard purchase/refresh; both Linux targets link. This advances one spell identity and one perk, but rendered status presentation and playable delivery remain pending and UP-023 remains open.

The shared `BonusType` change forced a large native rebuild. Source guards and 53 focused Python data tests pass. A first linked build stopped on an AI `unique_ptr` extraction compile error; the `.get()` repair is in source, the resumed `vcmitest`/`vcmiclient` build linked, and the failure/repair are retained in `NH_RELEASE_FAILURES.md`. An initial focused runtime attempt also exposed three test setup defects (same-round recast, week-boundary expectation, and spellbook mutation/missing artifact) plus the real AI hypothetical-rate gap; those were repaired without relaxing authoritative action legality. The final active-profile 17/17 filter has no skips.

### 2026-09-28 active Phase 1 slice — Storm of Daggers

Implement the remaining Sorcery combat-spell identity as a target-selected
damage-pool spell: one to five distinct enemy stacks, saved-v3 School-rank
scaling of its Spell Power term, equal per-target split, atomic rejection of
invalid selections, human numbered selection/forecast, and BattleAI subset
choice. Engine, UI, AI, and purpose-made original spell/impact art have separate
file ownership. A single cast should repeat a dagger impact on each selected
stack; the borrowed Magic Arrow projectile and Chain Lightning ray are not
acceptable stand-ins. Focused authoritative, AI, client, data and asset gates
are the Phase 1 completion target; rendered/playable art acceptance remains
separate.

Independent Astra source review found two blocking acceptance issues before
this slice can count toward coverage: Storm's fractional Spell Power term must
survive until final half-up rounding, and BattleAI must filter illegal singleton
targets before ranking candidate subsets. Both corrections are in the pushed
Phase 1 checkpoint: the authoritative Storm filter passes 4/4 and the bounded
AI subset/valuation filter passes 2/2 under the curated New Horizons profile;
`vcmitest` and `vcmiclient` link. The client owner replaced the flat selector backdrop
with a continuous leather surface and nested battle-style frame; native
rendering remains unverified. Additional invalid-target case coverage is a
deferred integration finding, not a Phase 1 blocker.

Deferred Phase 2 interaction to verify: current Magic Mirror resolution may
reflect a multi-target spell according to its first selected target rather than
resolve reflection independently per selected stack. The canonical Storm text
does not settle this; do not present an unverified interpretation as complete.

### 2026-09-28 active Phase 1 slice — Adventure Spell unlocks

Implement the shared town-owned Guild I–V purchase path for Summon Boat,
Water Walk, Town Portal, Fly, and Dimension Door. Server/state owns validation,
resource payment, persisted unlock tiers, and teaching the current and later
visiting heroes. Client owns an exercisable Mage Guild purchase view; Nullkiller2
uses the same validated command. Keep file ownership disjoint. A scoped build
and focused purchase/AI checks are the Phase 1 gate; rendered polish and wider
save/interaction coverage remain separately tracked for later phases.

Source/native checkpoint: all five tier-mapped Adventure Spells have an
authoritative town-owned purchase command, versioned unlock state, visiting-
hero teaching, Mage Guild purchase controls, and Nullkiller purchasing. The
Linux `vcmitest` and `vcmiclient` targets link. In an isolated New Horizons
profile, six focused server/AI cases and one polymorphic packet round-trip
pass with zero skips; the client source guard passes. Independent Astra review
found no remaining blocking authority/serialization defect. This is not a
rendered gameplay check or a promoted playable snapshot. Broad interactions
and shop presentation remain Phase 2 / visual verification work.

The prior Holy Wrath slice has a built authoritative implementation, 10/10
focused server cases, 1/1 actual BattleEvaluator choice case, a purpose-made
provisional icon family, and independent cap-order review. It is sufficient to
advance Phase 1 coverage, not a claim of playable release acceptance.

### 2026-09-28 selected slice — Holy Wrath

Implement the missing Level-3 Light spell as a complete vertical slice under
UP-023: 11 Mana, one enemy target, `40 + 2 × Spell Power` damage, with one
final 1.5× multiplier against Undead or Inferno-origin creatures. Saved-v3
Light rank scales only the Spell Power term. Reuse the authoritative damage
path for detached AI forecasts, retain the v1/v2 roster boundary, and provide
purpose-made provisional icon art through the HoMM3 art workflow. Record
target build, focused cast/AI/acquisition tests, source review and the eventual
playable delivery separately. This work does not close Bulwark's Deep Bulwark
gap or the remaining missing spells and perks.

### 2026-09-28 resumption checkpoint

UP-025's latest split-dialog revision builds and passes its source guards, but
the user's cohesive leather reference remains a visual acceptance target, not
proof of the rendered result. A single designated Tester captured the actual
`Split Imps` window on an owned private display from frozen unpromoted candidate
`344129b2c0a7aa3ce8591fce4d0c2a0d91cc2b34bea28f3dd2dd59bb78150fae`.
The pasted full-width gold seams are absent and the controls are visible on a
continuous leather field. Texture-join/button-well aesthetics and variant
owner combinations still need user review. At that capture checkpoint the
launcher still selected the earlier promoted snapshot.

Subsequently, the identical two UI source files were applied to the detached
committed source line, excluding unrelated dirty mechanics. The UI-only Linux
client built; three split/garrison guards passed; frozen snapshot
`107947d37280117049ec8573081cf226fb9dee4e958729c9fb02ec7f4ab696b3`
advanced 49 AI turn starts in a 35-second private headless smoke with no server
problem or crash. It is now the selected `play-new-horizons-linux.sh` snapshot.
This delivers a playable visual candidate, not user aesthetic acceptance.
The separate combined-source smoke found a signal-11 crash in one run and an
AI Leadership rejection in another; that build remains unpromoted and needs
diagnosis before a broad Skills-and-spells delivery.

For UP-027, the current Linux client, library, and native test targets link;
seven focused Bless/rank/AI tests pass in an isolated New Horizons TEST profile.
The global spell-overlay effect on v1/v2 saves is under compatibility review,
and the remaining non-damage rank effects remain open. For UP-023, the shared
Bulwark automatic-activation prerequisite passes eight focused native cases,
including lethal Poison death-state serialization; seven advanced perks are
still planned. These are source/native checkpoints, not a complete playable
Skills-and-spells release.

Mire Grip AI forecast/expiry parity now passes three focused native cases and
an independent Astra source review, including collateral triggering and
retention until actual activation. This does not activate Mire Grip or clear
the remaining advanced Bulwark gaps.

The first overlay repair is now in source, independently reviewed, and native
focused-verified: the 23 Expert no-Mass ranges are selected from saved v3 battle
rules instead of patched into shared spell data. Four isolated native cases
cover v1/v2/v3 lookup, v2/v3 Bless targeting and Expert effect rank, and an
explicit Temporal Field Mass path. Berserk, Dispel, Chain Lightning, Bless/Curse
and Ice Bolt global effects remain a separate compatibility backlog; no new
launcher promotion follows from this one slice.

Berserk is the second saved-profile overlay repair: v1/v2 retain the original
area cast, while saved v3 selects single-creature targeting through battle
mechanics. The native `vcmitest` target links and six focused tests pass,
including authoritative area/single-target behavior and a v3 friendly-target
rejection without spent mana; 33 focused content tests pass. This is not a
playable promotion or closure of the other global spell-overlay leaks.

Chain Lightning is the third saved-profile overlay repair: its fixed-five
count is resolved from saved v3 rules during shared Lua spell targeting, not
globally patched into `CSpell` data. The current `vcmitest` target links and
three focused native cases pass, covering v1/v2 rank-dependent previews and
four-target base casts versus v3 five-target previews/casts. The content guard
passes 33/33. Other overlay effects and broad playable validation remain open.

Dispel is the fourth saved-profile repair: v3 resolves its friend-or-foe
single-stack targeting and full status-removal effect in battle mechanics,
without inherited Expert obstacle removal; v1/v2 retain core behavior. The
native target links and seven focused cases pass, including the Selective
Dispel no-default-Mass guard; the content guard passes 33/33. Bless/Curse and
Ice Bolt remain global-effect leaks, and no gameplay snapshot is promoted.

Bless and Curse now resolve their v3 natural damage endpoints through saved
battle rules rather than global spell patches. Old v1/v2 Expert endpoint
modifiers remain +1/-1. The Linux native test target linked; 11 focused Bless
profile cases, one Bless AI forecast/cast parity case, and the content guard
passed with the curated test mod active. Ice Bolt remains a separate saved-
profile leak; this source/native checkpoint is not a playable promotion.

Ice Bolt's legacy -2 movement-range effect is now saved-profile-gated in the
shared spell-effect path: v1/v2 retain it, while v3 is damage-only. The native
test target links; three focused v1/v2/v3 authoritative-cast and AI-preview
cases pass, as does the content guard. Independent review found no blocker.
Application edge-case and save/load tests, broader spell coverage, and a
playable snapshot remain outstanding.

The same active-profile native run initially exposed three Conductor/
Annihilator test fixtures that selected Advanced/Expert perks without earlier
tier perks. Production progression was unchanged; corrected fixtures now
select their prerequisites. Root reran the full direct-damage mechanics suite:
36/36 passed in about 8.4 seconds.

The Toxic Spines AI forecast now values positive residual physical Poison in
AI units rather than adding raw damage to a value estimate. One focused native
test passes, and the full native test target links. Bulwark remains planned,
with other perk/runtime and visual gaps still open.

The Bulwark Defend tooltip now mirrors Shared Cover's adjacent-Defender bonus
and Vengeful Mire's melee-only reflection increase while preserving private
hero visibility. `vcmiclient` compiled/linked (97/97) and nine focused UI
source checks pass. No graphical/playable verification or advanced-perk
activation follows from this display slice.

For the AI Leadership smoke, two focused accepted wandering-creature offer
tests now pass: no-free-slot and one-free-slot partial admissions conserve all
Halflings and open the expected garrison dialog without a Leadership error.
They do not reproduce the separate AI complaint. A one-creature remainder
manual swap discrepancy has its own follow-up; the combined-source signal-11
run remains unexplained. No broad gameplay snapshot was promoted.

The user reprioritized functional completion on 2026-09-27: implement every
missing canonical Skill rank, perk and spell before returning to broad faction
completion or nonessential art polish. Purpose-made provisional art remains part
of an active mechanic's minimum usable surface, but final-art iteration follows
functional breadth. UP-023 owns the exhaustive matrix and evidence. UP-024 owns
the newly remembered universal Blacksmith inventory rule and Stronghold Ballista
Yard's existing canonical +20 weekly Siege visit effect.

The interrupted Fortress base-growth slice remains preserved uncommitted in the
worktree. Do not discard or misrepresent it as integrated; resume it under UP-022
after the functional Skill/perk/spell lane unless it becomes a direct dependency.

### Active functional slices — Spell Lock and Archery

**Spell Lock:** source implementation has passed final independent Astra review
after three repair passes. Compound effects such as Teleport drop the whole
paired effect instead of invoking a script with an empty target; real-mechanics
tests compare execution with `castEval` for damage, status, dispel, Teleport and
mixed locked/unlocked area targets; and explicitly nonmagical creature abilities
such as Death Cloud and Fireball Ability bypass the seal in both real and
forecast paths. Protection, cleansing, frozen duration handling and AI valuation
now consistently apply only to magical effects. Focused Python content checks
and `git diff --check` pass. Native compile/tests, exact target build and playable
acceptance remain separate gates; catalogue status alone is not completion.

**Archery Basic perks:** Target Caller, Skirmisher, Point-Blank Shot and
Counterfire have passed independent Astra source review after repair. The slice
now includes server-validated player-selected Skirmisher firing hexes, one
cached reachability calculation rather than render-loop pathfinding, projected
AI evaluation of every legal firing position, ordinary ranged multi-shot/ammo
semantics at 75% per strike, Point-Blank's physical adjacent-shot exception,
and Counterfire incapacitation, recursion, retaliation-resource and saved-round
handling. Perfect Moment applies to the first Skirmisher strike only. Focused
data checks and `git diff --check` pass; native compilation/tests, target build
and playable UI verification remain separate gates. The six Advanced/Expert
perks are now in uncommitted source with targeted syntax checks, data tests,
server/AI regression cases and an independent review in progress. Native test
execution is currently blocked by unrelated curated-module drift at CMake
reconfiguration; do not run the broad content generator over preserved changes.
After the full ten-perk Archery slice is closed,
Bulwark of the Mire is the next full Skill slice; do not insert another Skill or
art-polish lane first.

**Spell Lock Windows follow-up:** runs `36343003125` and `36347971057` failed
in BattleAI compilation for distinct incomplete-type and duration-return-type
errors. The repairs are pushed through `ddcd57391`; exact-head Windows run
`36353181774` succeeded and published artifact `10943952550`. This establishes
target compilation, not playable Spell Lock acceptance.

**Bulwark of the Mire:** first three Basic perks are active in source and data:
Mireborn, Thick Hide, Bog Ambush. Authoritative physical-damage and reaction
paths, BattleAI forecasts/Defend choice, hoverable Defend status feedback, and
focused regressions have undergone independent source review. Seven perks remain
planned. The Basic source was committed as `40628d29d` and exact-head Windows
run `36360403677` succeeded, publishing artifact `10945274902`. Native Bulwark
test execution and rendered/playable verification remain open; no full-Skill
completion or playable acceptance is claimed. Advanced/Expert runtime and AI
source are in progress, including a distinct physical Poison status for Toxic
Spines; keep those uncommitted until reviewed and validated.

2026-09-28 update: six further Bulwark perks are now active in uncommitted
production data. Deep Bulwark alone remains planned because no nonmagical
displacement mechanic exists yet. Focused native runtime 11/11 and BattleAI
8/8 cases pass with the production perk registry; independent source review
found no activation blocker. The broader active-profile Bulwark regression
passes 53/53 after seven fixture corrections. Toxic Spines needs a persistent client Poison
status display, and rendered/playable plus target-package acceptance remain
open. This checkpoint supersedes the seven-planned count above, not its
historical Basic build evidence.

**Canonical Markdown migration:** the user selected the repaired Markdown as
the sole design authority. DOCX-to-Markdown fidelity repair restored all 31
perk pools and the non-perk tables identified by independent review. A final
Astra cell-text sweep found one stray Shield of Chaos scope word; it was
corrected. Six School Skill descriptions were also reconciled with the
already-approved inscribed-spell casting rule. All 16 source-derived tests pass;
the scoped source migration was committed and pushed as `8c4ad7e5f`.
Target-package delivery remains a separate gate.

**Magic School rank potency:** the user added a Heroes V-like first-pass rule:
School rank improves the Spell Power coefficient on damage spells (initial
100/115/130/145% ladder), while non-damage effects get considered improvements.
Expert never automatically grants Mass. The shared rule is now integrated in
canonical Markdown and Pending Changes records the integration; UP-027 tracks
remaining implementation. Runtime/schema and NH-only spell-data lanes are
active. Focused data assertions pass, but native, save-compatibility, AI,
rendered UI, target-build, and playable evidence is not yet established.

**Delivery checkpoint:** full Windows workflow run `36341858040` succeeded at
committed head `70117e251a5fcf5f2163adbfb8be94626a57b56a` with
`preflight_only=false`. It compiled, packaged and uploaded artifact
`New-Horizons-Windows-x64-70117e251a5fcf5f2163adbfb8be94626a57b56a`
(`10940446726`, 621,090,196 bytes), proving the target build/package gate for
the Leadership empty-slot follow-up. Rendered label inspection and playable
behavior remain separate acceptance gates. The earlier run `36339991468` was
source preflight only and is not a playable build.

## Current sprint — Leadership-safe army exchange

### Shift split/combine crash and legal partial transfer

**State:** The dump-confirmed split-window crash is fixed and playable-confirmed
by the user in Windows artifact `10938170495`. The subsequent empty-hero-slot
Leadership defect and split-dialog ownership-label request are repaired,
independently source-reviewed, and exact-head Windows build/package verified by
run `36341858040` and artifact `10940446726`. Rendered inspection, localization
and playable acceptance remain pending under UP-021.

Confirmed failure: `CSplitWindow::apply()` runs its transfer callback before it
closes. An over-capacity Leadership check pushes an explanatory info dialog;
the split window then calls `WindowBase::close()` while it is no longer the top
window, producing the unhandled `std::runtime_error` in exact artifact
`6948b1aa56df3358febe86cd48017552ca1fe735`. Independently harden the numeric
split path against non-positive deltas; do not misattribute that adjacent bug as
the observed dump failure.

Required result:

- reproduce and identify the failing Shift split/combine request and whether an
  over-capacity Leadership transition is its trigger;
- keep the server authoritative and validate stale/invalid requests without
  mutating either army;
- when combining equal creatures into a hero's army, transfer exactly the
  largest count that fits the destination slot's current Leadership capacity;
- leave any excess in the source slot, and leave both stacks unchanged with a
  precise explanation when zero creatures fit;
- keep the split dialog and all shared combine routes consistent with exact-fit,
  partial-fit, zero-fit, empty-slot, same-army and cross-army cases;
- add focused authoritative/client/AI regression evidence, independent review,
  commit/push and exact target-build evidence before playable promotion.

Implemented source checkpoint (2026-09-27):

- split dialogs close before callbacks can open an error window;
- ordinary same-creature combines are authoritative partial-merge intents;
- the server clamps only those merge intents to the current per-slot Leadership
  capacity and preserves excess plus any required last source creature;
- exact numeric splits are never silently clamped, legitimate reverse slider
  moves are normalized client-side, and malformed negative/stale requests are
  rejected without mutation;
- empty-slot exchange and legacy/no-cap behavior are preserved;
- focused server regressions and two client source guards are present;
- an independent Astra review found three routing regressions and two test
  compile blockers, all repaired; final re-review reported no blocking finding.

Static evidence: both client guards, Python compilation and `git diff --check`
pass. Exact-head dependency/source preflight run 36332113616 passed for commit
`be8cb13a5`; full compile/package run 36333365693 succeeded and uploaded
`New-Horizons-Windows-x64-be8cb13a58a5dfe17d76aeab431608b918c821df`
(artifact `10938170495`, 617,643,648 bytes). Native tests, GUI reproduction and
playable acceptance remain outstanding and are not inferred from either build
route.

Empty-slot follow-up source checkpoint (2026-09-27): an ordinary whole-stack
drag from a garrison into an empty hero slot is now an authoritative partial
move intent. The server moves the current Leadership-legal maximum and preserves
the remainder; stale two-empty requests reject safely. The server regressions
establish a valid visiting-hero exchange and mirror the UI's destination-first
request orientation. The split window retains explicit `Hero: <name>` and
`Garrison: <name>` labels. An Astra review found and caused repairs for a missing
source-stack guard, an invalid exchange fixture, the real UI orientation, and a
misdeclared label member. Focused source guards pass. Native compilation/tests,
exact-head packaging, localization, rendered layout and user play remain open.

Latest user follow-up (2026-09-27): a complete move of a hero's final stack
into a garrison emitted `No creatures to split` for a one-creature source. The
new source route shows the localized last-army explanation at zero movable
creatures; positive whole-stack intents reach the server, which retains one
creature and clamps any Leadership-limited destination transfer. An Astra review
found and caused the remaining garrison-click exact-split route to use that
whole-stack intent. Focused server tests and client guards are present and source
checks pass; native/target-build/playable evidence is pending.

The user's transfer-dialog mock is `https://i.imgur.com/j1G5Qzi.png`. A source
layout checkpoint replaces clipped owner wording with built-in hero portraits
and garrison crests below the creature art, extends the original dialog at
runtime to 298×440 using installed assets, and keeps bounded full-name help for
ambiguous markers. Independent Astra review is clear and source guards pass;
rendered appearance and input remain unverified. UP-025 tracks acceptance.

### Next dedicated sprint — Fortress completion

**State:** Deferred under UP-022 until the higher-priority UP-023
Skill/perk/spell completion lane is closed, unless a Fortress mechanic becomes
a direct dependency of that lane.

Build a granular canonical requirement matrix first, then close Fortress heroes,
classes, biographies, specialties, creatures, buildings, faction Skill and every
perk, progression/acquisition, global-system interactions, AI, UI/log feedback,
provisional artwork, tests and delivery evidence. A partially active faction or
passing content parse is not completion.

## Preserved parallel checkpoint — Armorer foundation and delivery closure

### A. Iron Discipline — active implementation

**State:** Source committed and pushed; independent review clear; static
validation passing; exact-head Windows/native verification and playable delivery
pending.

Canonical result: Hold the Line also reduces magical damage by half of its
current physical reduction.

Current source scope:

- save the exact half-percent reduction in basis points when Hold is issued;
- apply it to anchored, unbroken, currently allied recipients through the shared
  spell-damage path, including spell penetration and Fire Shield reflection;
- suspend both physical and magical Hold protection when control changes;
- keep authoritative casts, forecasts, and Battle AI projections consistent and
  non-mutating;
- make Battle AI value bounded public magical threat without reading a concealed
  enemy spellbook;
- show the exact value in Order UI/status and activation logs, including armed
  Warcasting;
- activate purpose-made four-state provisional HoMM3 artwork and retain source,
  prompt, provenance, reductions, and hashes;
- serialize the public Order snapshot with safe old-save defaults and down-save
  rejection when data would be lost.

Evidence already obtained:

- provisional art commit `4828cccdb` and runtime/AI/UI/test commit `9806a27ef`
  are pushed on `definitive-mvp`;
- canonical module regeneration check passes;
- all 140 `test_new_horizons*.py` tests pass;
- active-perk artwork/source/runtime guard passes with 74 unique icons;
- Orders client source guard, JSON/CSV parsing, privacy scan and whitespace check
  pass;
- independent review identified Fire Shield, Hypnotize, and Warcasting-preview
  gaps; all three are repaired, and final source re-review found no blocker.
- exact Windows run `36326436603` completed successfully at full head
  `9806a27eff4ee4b427c92b270cc7ac5ea45b06bb`; it compiled, packaged and uploaded
  `New-Horizons-Windows-x64-9806a27eff4ee4b427c92b270cc7ac5ea45b06bb`
  (artifact `10935745939`, 617,638,770 bytes). This establishes target-build and
  package evidence for the source revision, not focused gameplay execution or
  playable acceptance.

Remaining acceptance:

- run the focused `IronDisciplineTest`, `HeroOrderStatePersistenceTest`, and
  Armorer AI cases on the matching native build where the route permits;
- record any failure and its prevention before retrying;
- produce and promote a validated playable snapshot, then obtain in-game visual
  and gameplay acceptance.

### B. Shield Master — target-build closure

**State:** Exact Windows run `36322531152` completed successfully at
`6948b1aa56df3358febe86cd48017552ca1fe735`. It compiled, packaged and uploaded
`New-Horizons-Windows-x64-6948b1aa56df3358febe86cd48017552ca1fe735`
(artifact `10933193980`, 614,831,501 bytes). This proves the Windows build/package
route for that source; it does not by itself prove focused gameplay behavior.

Remaining acceptance:

- execute the focused Shield Master native tests if/when the package route exposes
  a test-enabled binary;
- playable promotion and in-game Protect/interception visual review remain
  separate gates.

### C. Priority-queue verification closures

**State:** UP-003 Metamagic is source-complete but still needs target-native and
playable verification. UP-013 supplied Mage Guild artwork is implemented and
playably delivered; only authorized rendered review/user acceptance remains.
UP-001 Tower construction layout and the other open priority entries retain their
own evidence and blockers in `NH_USER_PRIORITY_QUEUE.md`.

The current sprint may close source work without falsely closing these separate
visual/playable gates.

## Next sprint — finish Basic Armorer

### Pavise

**State:** Implemented, independently reviewed, committed, and exact-head
Windows-build verified. Focused native tests and playable visual/runtime
acceptance remain pending.

Canonical result: when a friendly stack Defends, ranged physical creature damage
against it is reduced by an additional 25%.

Required scope before activation:

- authoritative Defend lifecycle and ranged physical-only damage calculation;
- independent-reduction/cap interaction and controls for melee, magical, siege,
  collateral, dispel/control and round transitions as applicable;
- Battle AI Defend valuation and hypothetical parity without live mutation;
- save/network compatibility if new persistent state is required;
- resolved combat-log attribution and visible stack/perk feedback;
- purpose-made provisional artwork through the HoMM3 Art workflow;
- focused native tests, independent review, commit/push and exact-head build.

Resolved implementation direction:

- Pavise is an independent 25% multiplicative physical-damage reduction source,
  composed inside the existing 80% combined reduction cap. Thus an existing 20%
  reduction plus Pavise leaves `0.80 x 0.75 = 0.60` damage, or 40% total
  reduction; it is not an additive 45%;
- eligibility is derived for each hit from physical ranged damage by an ordinary
  creature attacker, the target's live Defend state, and the target's current
  controlling hero owning Pavise. Turrets, siege weapons, commander placeholders,
  melee and magical damage are excluded;
- existing Defend state and cloned hypothetical battle state provide lifecycle
  and AI parity, so Pavise adds no separately serialized battle field.

Completing Pavise gives Armorer three implemented Basic choices plus the already
implemented Basic-perk set needed by the strict Skill/perk progression model.

Implementation checkpoint (2026-09-27): the authoritative damage path, previews,
Defend log, Battle AI valuation, active catalog/module bindings, focused server
and AI tests, and purpose-made provisional HoMM3 artwork are integrated. Pavise
is a separate 25% multiplicative ranged-physical reduction inside the existing
80% aggregate cap. It derives ownership from the target's current controller and
uses ordinary Defend lifetime, so it adds no serialized state. Independent Astra
review caught and caused repairs for spell-like shooters' physical melee,
wait-then-move AI behavior, Defend's ordinary Defense bonus in the test baseline,
the cap assertion, and a detached test-state mutation. Final re-review found no
blocking source issue. The active-art guard and 45 focused Python data tests pass;
native/runtime acceptance is not yet claimed. Exact workflow run `36333519971`
succeeded at commit `7862ca7eeccec4a266209ce1450e11eded418713` and uploaded
`New-Horizons-Windows-x64-7862ca7eeccec4a266209ce1450e11eded418713`
(artifact `10938463974`, 621,082,490 bytes). This proves the Windows compile and
package route for that exact source revision, not focused gameplay execution.

## Following sprint — Advanced Armorer sequence

Implement and verify, in canonical order unless a dependency requires a smaller
foundation first:

1. Formation Fighting
2. Unyielding
3. Veteran
4. Defiant

Each item requires authoritative behavior, Battle AI, persistence when stateful,
UI/log feedback, provisional artwork, focused tests, independent review and exact
delivery evidence. Do not activate inert catalogue entries to satisfy progression.

## Subsequent sprint — Expert Armorer sequence

1. Last Stand
2. Bastion

These are intentionally scheduled after the shared physical-reduction and
per-stack lifecycle foundations exercised by the Basic and Advanced perks.

## Remaining product work after Armorer

The complete objective remains much broader than the current skill sprint. The
following workstreams stay open until a requirement-by-requirement audit proves
otherwise:

- all remaining planned Skill ranks and perks across Archery, Battlecraft, War
  Machines, Discipline, Recruitment, Command, all six magic schools, Spellcraft,
  Wisdom, Warcasting, Logistics, Diplomacy, Estates, Learning, Luck and every
  faction-specific Skill;
- every spell definition, removal/replacement of legacy acquisition routes,
  specialties, teachers, Mage Guild generation/access, targeting, overcharge,
  duration, AI use, icons, effects and logs;
- strict Basic Skill → Basic perk → Advanced Skill → Advanced perk → Expert
  Skill → Expert perk progression across level-up and every teaching source;
- faction heroes, biographies, class growth, specialties, creatures, buildings,
  dwelling/prerequisite swaps, recruitment, Leadership and AI behavior;
- adventure movement, Logistics, travel spells, safe end-of-day landing and AI
  path execution;
- Hero/Spell/Order action architecture, generic class-resource presentation,
  combat status UI and comprehensive resolved-outcome logging;
- spell-point capacity, Buffer Mana, Intelligence, artifacts, Arcane Reservoir,
  Magic Spring, restoration and save/load edge cases;
- UI/art inventory closure: every Not done/Provisional asset must become either
  accepted Final art or retain an explicit remaining gate;
- complete save compatibility, deterministic replays, AI nonmutation, Linux and
  Windows builds, installed-resource validation, playable snapshots and actual
  in-game acceptance journeys.

## Sprint completion record

Append closed sprint checkpoints here with exact commit(s), review disposition,
test commands/results, CI run(s), artifact/snapshot identity, known limitations
and next sprint selected. Keep failures in the failure ledger rather than erasing
them from history.
