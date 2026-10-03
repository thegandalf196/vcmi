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

2026-10-03 UP-183 verified: Corpse Preservation is active. Actual ordinary
magical casualties require the perk; Disintegrate remains excluded. Ordered
usable health cohorts implement newest-first restoration, temporary expiry and
re-death cause replacement without fabricating Overheal corpses. Core1826,
client18663 and test50692 pass; frozen77992 passes after the legacy-null repair.
Initial principal4/9 and getter failure34931 remain preserved as fixture lessons;
repaired48299 passes. Principal retry9/9 and adjacent15/15 pass, zero skips,
1.751s/1.740s. Active both-target build passes; active9/9 passes1.794s, proving
production registry active and test override false in all five battle cases.
Data/inventory19/19 and module drift pass; the first inventory check caught
swapped Implementation/Art columns, now repaired. Independent review finds no
remaining blocker. Binary SHA-256:
001072515cdc1f22f068c038ffc242c304cfb4b84fe780c3128b37bd4650a77a.
Coverage197/310 active perks,113 planned; Necromancy4/10, faction56/90, ranks84/93
and spells60/67 unchanged. Midbattle persistence, broad restoration/form
interactions and rendered acceptance remain Phase2; purpose-made art Not done.
No local playable snapshot promotion. Previous Windows37123447269 succeeds on
1c2b7cf2c, without this new source. Next bounded coverage map: Soul Harvester's
Elite-casualty conversion and multiple-output authority/AI seams.

2026-10-03 UP-183 implementation checkpoint: Corpse Preservation's approved
magical-casualty gate and newest-usable-first restoration policy are canonical.
Production source is frozen: cause-aware health cohorts, temporary resurrection
identity, surplus-safe Overheal, original-form ownership, explicit Lua spell
ingress and authoritative eligibility filtering. Embedded health JSON preserves
matching provenance; binary battle descriptors that omit health reject it rather
than claim full midbattle persistence. Independent bounded review finds no
blocker. Serialized core build1826 is running; actual-cast, filtered Necromancy,
health-ledger and wire-guard fixtures still require native acceptance. The perk
remains planned, with verified coverage196/310 unchanged. Data/inventory19/19
passes. Preserve Windows37123447269 on the previous committed source; no local
playable promotion or current-source Windows artifact is claimed.

2026-10-02 UP-154 verified: Tactics is active. Core37002 and repaired both-target
10000/39337 pass. Principal retry24146 passes8/8 in23.514s; adjacent11237
passes10/10 in17.054s, zero skips. Data/inventory19/19 and module drift pass.
Coverage184/310 active perks,126 planned; Battlecraft4/10, ranks84/93 and
faction49/90 unchanged. Original interrupted build and7/8 fixture failure remain
preserved. Constructor-order defect is repaired. Rendered/actualAI deployment
handoff and wider siege/phase interactions are Phase2; no playable promotion.
Next missing Basic Battlecraft Overwatch map is complete, awaiting Teleport/Blink
scope clarification; no implementation is claimed from that map.
Tactics source`a85f2e44e303effe166badb5765422f4eeb6585a` is pushed.
Notice37086103464 is queued; full Windows37082097577 is still live on older
7aaa48c1. Preserve it and stage the newer full run after its terminal result and
the newer notice success; no Windows package or local launcher promotion yet.

2026-10-02 UP-154 source integration is in progress. Shared independent
deployment state/packets and authoritative side/footprint guards are source-frozen;
core target build37002 passes. Human/AI handoff and native fixture still require
freeze, combined compilation and principal execution. Tactics registration is
staged active for production acquisition tests, not yet accepted coverage:
verified count remains183/310, Battlecraft3/10. Data/inventory19/19 and module
drift pass. Interim review found no blocker; post-opening malformed deployment
hardening belongs to Phase2. UP-155 Overwatch receives a read-only hook map while
this source remains frozen; it must not consume the Tactics delivery checkpoint.

2026-10-02 UP-153 verified: Passing Lines is active. Both-target build9087 and
fixture retry38200 pass. Principal retry13004 passes6/6 in4.330s; adjacent87077
passes10/10 in2.280s, zero skips. Data/inventory19/19, module drift and independent
review pass. Coverage183/310 active perks,127 planned; Battlecraft3/10,
ranks84/93 and faction49/90 unchanged. Original4pass/2fail artifacts remain
preserved with lazy-view/activation-token fixture lessons. Phase2 retains wider
hazard/gate/control combinations and tactical AI selection; no playable promotion.
Windows37077420212 succeeds on older37dd359b8, including Battle Plan but not
Passing Lines. Next coverage preparation is Basic Battlecraft Tactics.
Passing Lines source7aaa48c1be92db6056973dfd4a3e6ad9164302c5 is pushed;
notice37081984549 succeeds. Full Windows37082097577 is queued on that exact
source, not yet compile/package evidence. Preserve this run while mapping Tactics.
UP154 maps are complete. Tactics needs independent saved deployment progression
for both armies, strict authoritative side/zone checks, and client/AI phase-switch
notification. Root selects attacker-then-defender scheduling and existing
scenario/siege accessibility restrictions; opening effects and round1 wait for
all eligible phases. No implementation or new activation from the map.

2026-10-02 UP-153 Passing Lines begins with bounded runtime, consumer and fixture
maps. Shared transit eligibility must allow friendly occupancy only, with empty
legal destinations and ordinary movement triggers. It is not Ghost Walk, flight
or teleportation. Root owns architecture and all builds/Git. No source activation
or coverage increase from mapping; current perks182/310. UP149/150/151 await
their recorded decisions, and UP130 remains composition-scope blocked.

2026-10-02 UP-148 verified checkpoint: Battle Plan is active. Both Linux targets
build; principal5/5 passes in13.180s and activated production-registry30/30 in
45.567s, zero skips. Free opening Orders precede any Creature Activation for
both eligible sides, retain HERO and do not trigger Double Command. Actual AI
submission/server acceptance, no-anchor exhaustion and once-use have evidence.
Data/client34/34, module drift and final source review pass. Coverage182/310,
128 planned; Command7/10, ranks84/93 and faction49/90 unchanged. Rendered UI,
broader opening interactions and exhausted grant-ID preflight handling are
Phase2. No full midbattle resume or playable promotion is claimed. Next Iron
Will is read-only mapped and awaits its same-command carryover lifetime answer.
Source52c4f89a636923260ea0ac8d4e1a2c79aab76bda is pushed. Notice37076319236
is running; preserve the existing full Windows37071436091 until terminal.
Notice37076319236 subsequently succeeds; full37071436091 succeeds on older
51340a3d4. New full Windows37077420212 is confirmed in_progress on37dd359b8,
which includes Battle Plan. Poll this exact job; do not dispatch a replacement
on observation timeout. UP150 Crisis and UP151 Seize Initiative are bounded
maps; Crisis awaits the action-resolution timing answer, alongside UP149's
same-command Iron Will carryover question. Coverage remains182/310.

2026-10-02 UP-148 implementation begins: Battle Plan's free opening Order.
One resolved pre-combat state per side and a dedicated BATTLE_PLAN receipt
preserve the normal Hero Action and never trigger Double Command. Deterministic
attacker/defender choices run after deployment and round initialization, before
Morale, regeneration, movement resets or any genuine Creature Activation.
The existing Orders chooser supplies automatic choice and target cancellation;
15 focused client source guards pass. Runtime, AI and focused fixtures are
separate lanes; root owns integration and activation. Coverage remains 181/310
pending both-target build and actual native evidence. No playable promotion.

2026-10-02 UP-147 verified checkpoint: Double Command is active. Principal retry
30525 passes 6/6 in 99.078s; activated focused 99320 passes 47/47 in 134.777s,
zero skips. Both Linux targets build; data/client 30/30, module drift and source
review pass. Coverage is 181/310 perks, 129 planned; Command 6/10, ranks 84/93
and faction perks 49/90 unchanged. Immediate distinct Order choice, deferred
Second Wind, actual AI use, descriptor metadata and fail-before-spend grant
exhaustion have focused evidence. Original failure logs remain retained, repaired
without weakening production validation. Rendered chooser QA, wider interactions
and generic hypothetical packet replay are Phase 2; no full midbattle save/resume
or playable promotion is claimed. Next: UP-148 Battle Plan before round 1's first
Creature Activation, preserving the normal Hero Action.
Source is committed/pushed as 51340a3d48607a096acd1dcf2975bafdcfc03ef7.
Notice preflight 37071300435 is running. Full Windows build and immutable
playable delivery remain separate; no local launcher snapshot was promoted.
That notice completed successfully; accidental run 37071223589 is terminal
cancelled. Full Windows 37071436091 runs on 51340a3d4. Continue coverage work
while polling this same run; no replacement job or Windows-success claim yet.

2026-10-02 UP-147 implementation begins after the completed coexistence foundation.
The accepted architecture uses one saved per-side contextual continuation with
NONE / ORDER_REQUIRED / SECOND_WIND_READY phases and a combat-used bit. The
accepted primary receipt must spend HERO on ORDER; an ORDER-only receipt cannot
trigger it. A source-labelled dedicated grant pays only the immediate different
Order, and ordinary actions cannot defer that sequence. The existing Orders pane
opens automatically and target cancellation returns to it, with no perk
Activate/Decline prompt. First-Order Second Wind activation waits for resolution;
an empty legal-choice set closes authoritatively and resumes the deferred flow.
Runtime/core, AI and native-fixture ownership are separate Luna lanes; root owns
UI, version, integration, builds and registration. Source-only client guards
pass11/11 including seven existing Perfect Moment guards. No C++ build or native
acceptance is claimed yet, Double Command remains planned, and coverage stays
180/310 perks,84/93 ranks,49/90 faction perks. No local playable promotion.
Subsequent both-target retry 68259 passes. Principal 86481 passes 3/6, zero skips;
the actual AI and exhaustion paths pass. Target-ID fixture corrections and a
two-stage descriptor/live validation repair precede the next rebuild. Descriptor
roundtrip checks do not certify ongoing-battle save/resume. Double Command stays
planned until actual focused native acceptance; counts remain unchanged.

2026-10-02 UP-146 verified foundational slice: simultaneous different Orders.
The canonical coexistence rule now has one authoritative collection per side,
typed runtime/AI consumers, independent damage factors and state consumption,
append-only saves and preservation-aware validated packets. Existing UI hooks
show all Orders without granting actions. Both Linux targets build; principal
retry75974 passes20/20 in31.867s, zero skips. Adjacent87780 passes38/46: all37
Order/Iron Discipline/persistence cases pass; eight unchanged Vengeance fixtures
fail before Order execution at the earlier-perk setup gate and are Phase2 work.
Source guard7/7 and independent review pass. Original compile/native fixture
failure artifacts remain preserved, corrected without weakening production.
Counts remain180/310 perks,84/93 ranks,49/90 faction perks; Double Command's
actual trigger is the next dependent coverage item. Source is pushed; no GUI,
rendered acceptance or immutable playable promotion. Uncapped compound numeric
matrices and wider control/save interactions remain explicitly deferred.
Source is now committed/pushed asf57f58a84c8d82d49c9b5f555b12eb08f62e4585;
push exits0. Notice preflight37060224004 is live on that source. Poll it through
terminal, then dispatch the full Windows build; do not restart it for an
observation timeout. Earlier fullWindows37049519240 is success onb99c49c32.
Local immutable playable delivery remains pending.
Notice37060224004 completed successfully. Full Windows37060422101 is live
on7a90085cb0d96a9b379bf4afc83a2fe66354bf41 (doc-only checkpoint following
f57f58a84 gameplay source). Poll the same run through terminal; no replacement
full job or Windows-success claim while it remains in progress.
That exact full run subsequently completed successfully at 2026-10-02T21:29:11Z:
compile and package passed on 7a90085cb0d96a9b379bf4afc83a2fe66354bf41.
This verifies the earlier coexistence source, not the uncommitted Double Command
candidate. No Windows graphical acceptance or local snapshot promotion follows.

2026-10-02 UP-145 verified checkpoint: Blood Scent now active with capped,
attack-local live/AI output and privacy-safe saved rank increments. Client50746,
test baseline25076, fixture40698/rebuild84207 and activated both-target build
pass. Principal retry91133 passes5/5 in1.713s, activated62923 passes36/36 in8.312s,
zero skips. Data36/36/module drift pass. Coverage180/310,130 planned; faction49/90,
Bloodrage6/10; ranks84/93 unchanged. First3/5 fixture-math failure is preserved
and repaired without changing production math. No graphical/playable promotion.
Next missing Bloodrage entries: First Blood/Slayer await overlap decision,
Avatar awaits attack-local cap interaction decision; Rage Through Pain requires
personal-state persistence and lethal/control design review. Full Windows
37049519240 completed successfully on prior b99c49c32, not this new source,
at2026-10-02T19:45:55Z; compile and packaging passed. This does not verify
Blood Scent or the in-progress multiple-Order source.
Blood Scent source is committed/pushed0a0914e1ce8ab1f22f5aa977e8284ceb6b6ff1c3.
The previous full run is terminal; newer source still needs its notice preflight
and full build after source delivery. No local launcher promotion is inferred.

2026-10-02 next coverage slice: Blood Scent's target-sensitive attack-local
Bloodrage increment. Root owns architecture, serialization, builds and activation;
independent runtime and AI/save maps are delegated. Preserve the saved cap and
enemy-hero privacy. Counts remain179/310 pending focused acceptance. Existing
Windows build37049519240 remains confirmed in_progress on b99c49c32; monitor that
same run rather than dispatch a replacement.
Next read-only Rage Through Pain map identifies damageInternal as the shared
crossing event (not polling), per-unit JSON/copy state for live/AI replication,
and the existing CStack binary omission as a required persistence seam. A future
implementation must preserve its one-shot personal increment without advancing
global Bloodrage or weakening lossy-save guards. Lethal/revival and control-change
semantics require root design review before that slice; no activation from map.

UP-139 verified checkpoint: retry4772 builds both targets; principal35313
passes10/10 in2.669s and adjacent27391 passes6/6 in1.369s, zero skips.
Python36/36/module drift and final reviewer gates pass. Commit this coherent
structural foundation; retain the Phase1 design choices (absolute landmarks,
perk stacking) and Phase2 AI utility/localization findings. No perk activation,
new spell identity count or playable promotion is inferred. Cataclysm's next
map confirms existing UP-111 scope ambiguity; do not repeat or silently bypass it.

UP-139 current slice: implement the missing Havoc scenery/fortification producer
before Demolitionist/Meteorologist. Three separate workers own runtime, AI and
focused native fixtures; root owns data/schema and serialized builds. Numeric
fortification output remains an explicit tunable prototype, not Phase3 balance.
Empty/immune unit areas must still resolve legitimate structural effects; old
profiles retain old behavior. Two design questions remain open (fixed landmarks,
perk stacking). Scope is not reported complete while those are unanswered.
Client20497 exits0 after a12-job rebuild. Frozen runtime/AI fixtures and a
native parser opt-in test are registered; vcmitest48092 is live with12 jobs.
Focused36 Python checks and generated-module drift pass. Supplemental content
inventory56/59 exposes a pre-existing five-Mass-identity omission, tracked in
NH_RELEASE_FAILURES.md for Phase2. Principal native acceptance remains pending;
do not run a stale binary or promote an immutable playable snapshot from this.

2026-10-02 checkpoint: Mine Layer principal10/10 passes and registration is
enabled. Activated retry70019 passes10/10; client build,35 data/schema/inventory
tests, generated-module drift and independent registration review pass.
Bastion's final fixture build92361/native45892 pass8/8 in2.618s; it is now
active following independent review. Combined activated gates remain next.
Combined activated both-target28218/native67346 now pass18/18 in5.197s,
zero skips, with35 data/schema/inventory tests and module drift green.
Source commits779289300 (Mine Layer) and6f848c9a8 (Bastion) are pushed.
Windows notice preflight37018538339 is queued on6f848c9a8. Re-poll that exact
run before dispatching the full Windows build; queued is not passed. No Linux
playable snapshot was promoted. Phase1 continues with Havoc structural effects.
Notice37018538339 completed successfully. Full Windows37018692299 is queued
on df94df8ec (same feature source plus tracking docs). Re-poll this live build,
do not infer a compile/package pass or restart from an observation timeout.
Earlier fixture failures and lessons are preserved in the failure register.
Mine Layer is committed/pushed779289300. Next is the missing Havoc structural
spell foundation, needed by Demolitionist/Meteorologist, rather than more tests
around already functioning perks. Windows
full37008135705 completed successfully on8c5f5ec87; newer source is not included.
Do not conflate native/source completion with playable delivery. Phase1 continues.

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

2026-10-02 UP-143 activation checkpoint: principal retry64160 passes7/7 in2.554s,
zero skips. Both-target snapshot46666 and activated builds succeed; final focused
70764 passes31/31 in6.987s with zero skips. Data36/36, module drift and UI source
guard pass. Coverage179/310 active,131 planned; faction48/90, Bloodrage5/10;
ranks84/93 unchanged. The original5/6 failure was fixed with resolved per-side
bonus snapshots, not a spectator-only fixture. Next Bloodrage gaps: First Blood,
Blood Scent, Rage Through Pain, Slayer and Avatar of Rage; UP-141 still awaits
casualty rounding. Art/graphical/playable acceptance and broad matrices remain
separate. Source commit/push is next.
Source is now delivered as b99c49c32aff8beb8f0b615edc845d55435784c9;
Windows notice preflight37049324047 is confirmed in_progress on this source.
Next full Windows dispatch depends on its successful terminal result. First Blood
and Slayer's overlapping increment count awaits a narrow user answer; next
unblocked Bloodrage work is Blood Scent, Rage Through Pain and Avatar of Rage.
Notice preflight37049324047 is terminal success; full Windows37049519240 is
confirmed queued on b99c49c32aff8beb8f0b615edc845d55435784c9. Preserve/poll this
run rather than restarting after an observation timeout. No Windows acceptance
or new immutable local launcher snapshot is inferred from dispatch.

2026-10-02 UP-143 threshold slice: implementing Unrelenting and Berserker
through shared dynamic unit-environment hooks. Existing live creature-stat,
movement/AI and retaliation paths will consume these queries; no new panel,
counter or runtime scan. Current-controller eligibility follows half the saved
cap, including Endless Bloodshed. Ordinary retaliation caching and spent usage
remain intact; the conditional allowance is not cached. Runtime and focused
fixture work are separate Luna lanes; AI and Astra reviews are bounded.
Activation and increased counts require exact-source builds and native evidence.

2026-10-02 UP-143/144 activation checkpoint: principal66256 passes4/4, zero
skips in1.559s; serialized client91439/test68195 and activated both-target18196
builds pass. Shared live/detached Fury floor and saved80 cap are active. Data36/36,
module drift and existing resource-panel source guard pass. Coverage177/310,
133 planned; Bloodrage3/10, faction46/90; ranks84/93 unchanged. Activated adjacent
gate69374 initially passed40/41; the isolated legacy fixture-profile repair builds
in6389, and activated retry20229 passes41/41 in29.684s with zero skips.
Evidence: `UP144-activated-retry.log`/`.xml`. No immutable playable promotion or broad save claim.
Next highest-priority Bloodrage items are Unrelenting/Berserker's shared
Speed/retaliation threshold hooks; UP-141 still awaits casualty clarification.

2026-10-02 current slice UP-143/144: separate Luna runtime, detached-AI and
focused fixture owners implement Fury Unbound and Endless Bloodshed. Root
owns the append-only cap serialization feature, existing resource-panel getter
binding, activation, builds and Git; Astra reviews material correctness. The
other seven planned Bloodrage perks remain missing. Preserve ordinary legal
Basic->Advanced->Expert acquisition, rank-sized increments and death exclusions.
No per-update scan or new action; counts remain175/310 until acceptance.

2026-10-02 UP-142 activation checkpoint: Commanding Presence's shared
live/detached Morale floor is implemented against each recipient's effective
Order benefit. Principal retry18653 passes9/9, zero skips in21.568s; both Linux
targets build, data36/36 and generated-module drift pass. Coverage174->175/310,
planned136->135, Command4->5/10; ranks84/93 unchanged. Activated adjacent gate39487
passes23/23 in25.382s, zero skips; final review has no blocker. No immutable
playable promotion. Next unblocked work is Bloodrage's
threshold/cap foundation (UP-143/144), preserving legal Advanced progression.
Miracle Worker still awaits its casualty-output clarification.
UP-142 source is committed/pushed401f80384451e0522ff8df8f035901863c03025a.
Native/source acceptance does not promote the launcher or certify a new Windows
package; those delivery states remain separate.

2026-10-02 next slice: UP-142 Commanding Presence's recipient-lifetime decision
is integrated into canonical Markdown and full registry help. A shared read-only
effective-Order predicate and final Morale floor are under implementation, with
a separate focused fixture owner. Steadfast is already committed/pushed.
UP-144 maps Endless Bloodshed's shared cap path independently; no duplicate
counter or UI-only maximum is acceptable. Counts remain174/310 and84/93 until
Commanding Presence's principal execution/build gates pass.

2026-10-02 current slice: UP-140 Steadfast production/runtime/AI source and
serialization prerequisite compile in both Linux targets; principal14/14 passes.
The first failures led to fixture-cap/prerequisite repairs and a real added-stack
aura initialization-order correction. Adjacent9/10 passes; the remaining existing
whole-battle Veteran-history serialization rejection stays explicit for Phase2.
Steadfast is active; activated23/23 passes with zero skips and final review has
no blocker. Data36/36 and generated-module drift pass; be569afa4 is committed
and pushed. Next: UP-142 canonical integration and effective Order membership.
UP-141 Miracle Worker awaits casualty-rounding clarification. UP-142 Commanding
Presence map is complete; the user resolved its floor ends with the recipient's
spent/broken Order benefit. Canonical integration/implementation follow Steadfast.
UP-143 maps three missing Bloodrage threshold perks without altering the frozen
Steadfast candidate. Current activation is174/310,136 planned,84/93 ranks.
Older checkpoints below are historical, not the next-work selection.

UP-135 selected: Expert Armorer Bastion. Separate runtime, AI and fixture
owners implement a per-stack round marker and shared Defend/Hold the Line
recipient gate. Its70% final physical-damage factor is distinct from additive
physical reduction and from Immovable's allowance. Accepted attack events spend
the marker; comparing the round renews it without polling. Preserve current
control, ordinary creature attack provenance and detached branch isolation.
Registration stays planned until the principal build/native gates pass.
Runtime/AI/fixture independent review has no blocker. Both-target79589 exits0
after correcting the recorded Counterfire state-interface compile failure92791.
Principal64640 passes4/8 with zero skips; the fixture's repeated action lifecycle
and hidden defender-perk projection are under repair. Keep Bastion planned.
UP-136 Defiant's distributed retaliation-denial map is complete and blocked on
the asked source scope/linked Morale choices. UP-137 Mine Layer has a clear
shared mechanics count seam plus a necessary server validator alignment; no
new saved state/polling or general framework is needed. Implement after the
Bastion candidate gate; do not repeat either completed map.

UP-133 verified subset committed/pushed7e02b092f; registry remains planned
until the area scope question is answered. UP-134 Extend Spell mapping is
complete: shared adjustEffectDuration plus accepted round allowance and detached
copy/advance are required. Temporary terrain/summon scope and Counterspelled
consumption remain design questions; no invented Time Stop round lifetime or
permanent polling. Do not repeat this map.

UP-133 bounded three-damage-area helper builds client48085/test18427;
shared Controlled Blast regression89309 passes6/6 in2.658s, zero skips.
New fixture90773 builds and principal96284 passes7/7 in2.238s, zero skips.
Independent runtime Astra review has no blocker. Time Stop/Earthquake scope awaits
the user; registration remains
planned and coverage remains171/310. Do not equate shared regression with the
new perk's principal acceptance.
Unbreakable preflight37006272158 now succeeds. Full Windows37008135705 is
queued on8c5f5ec87, containing Broad Muster and Unbreakable, but not the dirty
Precise Casting candidate. Compile/package success is still pending.

UP-133 selected: implement Precise Casting's friendly central-stack exclusion
for conventional area effects, with runtime, detached-AI and focused fixture
mapping separated. Reuse Controlled Blast's existing center-identity path where
appropriate, but do not mistake its three damage spells for proof of the broader
perk's complete scope. Registration and coverage remain unchanged until actual
production, compile and principal verification gates pass.
Windows full37000555568 on7331e1056 now succeeds through compile, recursive
package audit and preview upload. Its nonexpired751939717-byte artifact predates
Broad Muster and Unbreakable. Their newer preflight37006272158 is confirmed
in progress; Broad Muster preflight37002243267 is terminal cancelled, not passed.
No Windows graphical acceptance or latest-feature playable claim is inferred.

UP-131 verified: Unbreakable is active; both Linux targets build. Principal
retry10314 passes10/10 in3.330s and activated69637 passes10/10 in3.303s, zero
skips. Data/schema/inventory35/35, module drift and independent frozen review
pass. Coverage171/310 active,139 planned; Discipline6/10. Failed positive-Morale
fixture30730 and its ordinary-movement repair remain in the failure ledger.
No GUI or promotion. Multi-round AI valuation and broader stochastic ordering
are Phase2. UP-132 Cross-School Formula mapping is complete; actual multi-school
memberships and Counterspelled source casts require user answers before source
work. Do not repeat the map or invent accepted-cast history from StartAction.
Unbreakable source is committed/pushed asff18ed6b9. New-source Windows
preflight37006272158 is queued behind the preserved older full37000555568
and Broad Muster preflight37002243267. No Windows package or playable promotion
is claimed. The native gates describe frozen pre-commit source bytes.

UP-131 selected, 2026-10-02: implement Expert Discipline Unbreakable using the
existing shared negative-Morale suppression path. Runtime, detached AI and
focused native fixture have separate ownership. A round-local allowance is
distinct from Rally's combat-long use; consume the renewable allowance first
without spending both or changing Twist's first draw. Append explicit saved
state compatibility and reset at the existing round event, not by polling.
Registration remains planned until build and principal gates pass. Coverage
remains170/310; no GUI or playable promotion. UP-130 Esprit de Corps reconfirms
the earlier unanswered mixed-faction/Undead scope question and is blocked;
root interpretation is not authority to resolve that question.

UP-128 verified checkpoint: Broad Muster is active. Both targets build40839;
principal54272 passes18/18 in3.701s and activated82143 passes18/18 in3.704s,
zero skips. Legal ranks, exact allocation, rejection/overflow atomicity, shared
allowance, saved stock/markers, old solo wire and AI helpers are covered.
Data/schema/inventory35/35, module/UI drift checks and independent reviews pass.
Coverage170/310 active,140 planned; Recruitment6/10. No new gameplay counter or
polling; appended wire feature preserves solo compatibility. Long-label fit,
actual UI/AI query execution and broader stock/Gold/free-slot valuation remain
Phase2. No GUI/promotion. Diplomacy map UP-129 is consolidated into existing
UP-048's unanswered authored-free-join policy; do not repeat the same audit or
change neutral-surplus lifecycle without a deliberate decision.
Broad Muster source committed/pushed as0f2d8cac8. New-source Windows
preflight37002243267 is queued behind full37000555568; concurrency does not
cancel that running older build. Native evidence above is the frozen pre-commit
candidate, not a promoted package. Full Broad Muster Windows compilation still
requires a successful preflight followed by its target build.

UP-128 in-source checkpoint: one optional two-row Core request validates the
shared total and both overflow bounds before one marker+stock transaction.
Native scrollable choices show both destinations/counts; AI chooses a split
only when Leadership-admitted value improves over every solo option. Root owns
focused actual/negative/save/wire fixtures after the fourth worker activation
was service-rejected. Static UI/module checks and data/schema/inventory35/35
pass. Source is frozen and build40839 is live; Broad Muster stays planned until
native acceptance. No coverage increase, GUI or playable delivery is claimed.
Diplomacy's missing deterministic foundation (UP-129) is mapping read-only while
this candidate builds. External Recruiter Windows preflight36998928632 passed;
full37000555568 was dispatched on7331e1056, excluding dirty Broad Muster.

UP-124 verified checkpoint: External Recruiter is active. Final fixture rebuild
8494 and activated client/test build exit0; principal15376 passes11/11 in2.877s,
activated81048 passes11/11 in2.899s, zero skips. Data/schema/inventory35/35,
module drift and Muster UI wiring pass; independent source/fixture reviews have
no blocker. Coverage169/310 active,141 planned; Recruitment5/10. Shared weekly
allowance/target locks, fixed+2 outside towns, free tier-one recruitment and
Leadership remain authoritative. No saved-state addition or polling. Phase2
retains natural visit/window/AI execution, full-army merging, mixed rows and
restored queries. Source/native only; no playable promotion or GUI claim.
Contacts (UP-126) and Drill Sergeant (UP-127) await distinct pool/cohort answers;
continue another unblocked missing perk while those decisions remain open.
External Recruiter source is committed/pushed as6cb08a8cb. Windows
preflight36998928632 is confirmed live on that source, including453828742's
MSVC repair. Broad Muster (UP-128) is mapped without a specification blocker:
implement one atomic optional two-row request, explicit exact allocation UI,
minimum AI split selection and focused malformed/duplicate/overflow guards.
Its implementation remains next; do not claim coverage from the map.

UP-124 implementation checkpoint, 2026-10-02: External Recruiter uses existing
weekly hero allowance and dwelling target markers. Runtime and UI are assigned
separate ownership; required AI/native verification follows when the service
allows another worker. Preserve free tier-1 recruits using one shared cost rule,
exact active-visit validation, fixed+2 Core stock and normal Leadership checks.
No activation or coverage increase is claimed yet. Windows preflight36992596028
passed on9d8c5f4d4; it did not compile or package the game.
Four-worker concurrency was confirmed through the actual agent API by reusing
completed allocated threads; policy is pushed as42ed09b7e. All four candidate
workers are now terminal. External Recruiter runtime/UI/AI/fixture source is
frozen, localization and module generation are integrated, static UI and drift
guards pass. The next gate is the serialized client/test build plus focused
Muster native tests; activation and source commit remain pending. Both targets
built successfully (44293). Principal37505 passed9/11; two fixture failures
require legal earlier perk tiers. Independent Astra production review has no
blocker. A Luna tester owns the fixture repair; root serializes the retry.
Windows full build36994237037 failed on6ca967db6 in an ambiguous MSVC source-ID
declaration. Brace initialization is pushed as453828742; succeeding CI remains
pending. UP-126 Recruiter's Contacts mapping is complete but multirow empty-pool
semantics await clarification; do not activate it based on a guessed policy.

UP-123 map checkpoint, 2026-10-02: missing Chaos Pandemonium needs a generic
effect-level DEBUFF classification, not a negative-spell list or a raw Bonus
count. Physical-affliction grouping/state-backed Poison is reusable, but mixed
Shield of Chaos and non-spell No Quarter require explicit metadata. Rational
SP scaling and per-stack global preview are mapped. Repeated-debuff cardinality
and Pandemonium Master's interpretation await two precise user answers. No
registration, implementation or coverage increase is inferred from this map.
UP-120's verified Spellward source slice is pushed as9d8c5f4d4; no playable
snapshot was promoted. Continue another unblocked UP-023 item while these
design decisions remain open.

UP-120 verified checkpoint, 2026-10-02: Spellward supplies independent10%
magical protection under the current controller. Paid casts, combined/capped
reduction, rank/inactive guards and detached castEval agree. The proxy repair
returns computed defense without exposing hidden heroes and preserves projected
control changes. Build80192 and activated12348 exit0; principal24023 passes
21/21 in5.858s and activated60120 passes22/22 in6.000s, zero skips.
Data/schema/inventory35/35 and generated module check pass. Independent Astra
review has no blocking findings. Coverage168/310 active,142 planned;
Warcasting5/5 active/planned. No state duplication or polling, GUI/promotion.
Bespoke art is Not done and generic presentation Provisional. Wider save and
magical-ability interactions remain Phase2. Mire Shaper, Combat Casting and
Enchanted Command are mapped but await item-level design answers.

UP-119 mapping checkpoint, 2026-10-02: Mire Shaper's implementation surface
is mapped by two Luna agents. Shared quicksandPatchCount already feeds spell
help, Mechanics, server validation, Lua creation, placement UI and AI; no new
state or polling is needed. Legal rank/perk acquisition and native test seams
are identified. The previous Quicksand checkpoint explicitly left its extra
patch's cap ordering unresolved. Asked whether six is allowed or five remains
absolute; both agents finished without source edits. Perk remains planned;
coverage stays167/310. Do not promote a recommended interpretation to authority.
No build, GUI or playable promotion was needed for this read-only map.

UP-118 consumer checkpoint, 2026-10-02: Earthquake field damage/Fractured Ground
and selected-section siege structural damage are implemented; Geomancer is
active. Both targets compile; final80978 exits0. Native91000 passes63/63
in8.411s, zero skips; data/schema/inventory35/35 and module check pass. Actual
paid AI cast, immunity exclusion, detached/live forecasts, weighted movement
and strict legacy-profile guards are included. Independent Astra review has
no blocking findings. Coverage166->167/310 active,144->143 planned; Nature7/3.
Structural100 HP (Geomancer125) is a labelled tunable, not a new canonical rule.
Borrowed field art remains Not done, generic UI Provisional; no GUI/promotion.
Wider save/movement interactions, special Metamagic-event forecasts and optional
scenery destruction remain Phase2. Next unblocked missing perk: Advanced Nature
Mire Shaper; map the additional Quicksand patch against existing count/placement
rules before implementation. Nature's Wrath/Worldroot remains design-blocked.

UP-118 prerequisite checkpoint, 2026-10-02: generic spell-created terrain now
stores a bounded movement surcharge with packet/JSON and feature-gated binary
state. Shared walking reachability charges newly entered footprint cells, uses
the maximum overlapping cost and ignores expired fields; flight is unchanged.
Client54585, test92767 and focused82811 exit0; native72881 passes12/12 in3.287s,
zero skips. Root direct review repaired pre-run double charging; a separate
reviewer spawn was service-rejected. Earthquake and Geomancer remain incomplete
and coverage is unchanged166/310. Next: separate weighted budget from traveled
hexes, implement authoritative field terrain/damage and selected-area siege
structural damage, then activate Geomancer only after both paths have evidence.
No GUI or playable promotion; wider integration stays recorded for Phase2.

Verified UP-115/116 continuation, 2026-10-02: Basic Sanctuary Keeper and
Venomancer are active. Exact linked Morale lifetime and20% whole-Base Poison
snapshot, including physical-source exclusion, legal offers, inactive/legacy
guards and materialized detached/live parity pass. Both real AI-selected casts
are accepted with normal paid Mana. Client90317 and final both-target10531
exit0; principal20512 passes25/25 in6.559s, activated76413 passes30/30 in7.833s,
zero skips. Data/schema/inventory34/34 and module check pass; independent review
has no remaining blocker. Coverage164->166/310, planned146->144; Light9/1,
Nature6/4. Failure lessons are persisted. Phase2 retains negative-Morale-only
AI selection and wider Morale/specialty/save/modifier interactions. No GUI or
playable promotion; generic UI Provisional, authored perk art Not done.
UP-117 maps Nature's Wrath; missing range/conduction/resistance decisions await
answers. Next unblocked missing-content audit: Earthquake/Fractured Ground
and Geomancer, without substituting a balance-only or polish task.

Latest verified UP-114 continuation, 2026-10-02: all five distinct Mass entries
are active. Mass Slow completes the set with Temporal Field's physical-book
virtual grant,60% post-cap/specialty Initiative effect, normal duration and
three-times listed cost before Wisdom. Ordinary and Mass Slow refresh one
family status; old saved profiles retain their toggle/budget, while new ones
reject that transport. No new saved counters or polling. Client33547 and final
both-target53442 exit0; principal7002 passes22/22 in5.821s, activated47843 passes
36/36 in9.512s, zero skips. Real AI selection/server acceptance, historical AI,
Communion and Heavenly Gale pass after saved-family valuation and no-location
projection repairs. Data/schema/inventory34/34 and module drift check pass;
independent review has no blocker. Distinct variants5/5, active perks164/310,
planned146, canonical identities60/67. Broader save/modifier/rendered checks
remain Phase2. Source/native verification is not playable delivery; no promotion.
Next unblocked missing feature: Light Basic Sanctuary Keeper's Sanctuary-linked
+2 Morale, including effect expiry/refresh/removal and detached AI projection.

Latest verified UP-114 continuation, 2026-10-02: Mass Regeneration and Advanced
Verdant Communion are active. Living-recipient eligibility, virtual grant and
revocation, triple cost, ranked wound snapshots, survivor-only healing, shared
family refresh and materialized detached parity have native evidence. The real
AI emits the no-location destination and the server accepts its selected cast.
Final both-target55569 exits0; principal79005 passes26/26 in7.453s, activated
81701 passes30/30 in8.697s, zero skips. Data/schema/inventory33/33 and module
check pass; independent review has no remaining blocker. Coverage164/310 active,
146 planned; Nature5/5 and distinct Mass variants4/5. Source/native verification
is not playable delivery. Phase2 retains broad save/modifier interactions and
the synthetic exclusion-roster round-advance diagnostic. Next: distinct Mass
Slow/Temporal Field, including its60% magnitude consumer and permanent grant.

Latest verified UP-114 continuation: Mass Bless/Litany is active. Distinct
saved-v3 virtual grant, ally targeting, triple cost before Wisdom, capped School
scaling and Benediction use the shared foundation. Principal fixtures found a
real materialized Bless refresh defect; shared timed Lua explicitly replaces
the family marker, and detached/live prior-status refresh and Curse removal now
pass. Client23367 and both-target20799/28088 exit0; repaired31806 passes55/55
in10.977s and activated5126 passes55/55 in11.867s, zero skips. Data/schema/
inventory32/32 and module drift check pass. Coverage163/310 active,147 planned;
Light8/2 and distinct variants3/5. Independent review has no material blocker;
all required workers finished. The stale Bless tooltip assertion is repaired
and included. No GUI or playable promotion. Next: Mass Regeneration/Verdant
Communion, then distinct Mass Slow. Phase2 retains broad save/load, AI selection
and modifier interactions. UP-113 remains item-gated on its normal chain limit.

Latest verified UP-114 slice: distinct Mass Curse/Sorrow and Grand Malediction
are active. Saved-v3 rows define the base family and perk grant; virtual entries
require the selected active perk and physical Spellbook, never durable learning.
Base-family status IDs preserve normal/Mass refresh while actual variant IDs
retain selection, action and Mana identity. Metadata is restricted to100% until
the Mass Slow consumer exists. Both-target37060 exits0; principal99435 passes
48/48 in7.091s and activated21991 passes48/48 in7.326s, zero skips. Data/schema/
inventory32/32 and module check pass. Coverage162/310 active,148 planned;
Shadow9/1 and distinct variants2/5. Independent review has no remaining blocker.
All required workers finished. No GUI or playable promotion. Phase2 retains
wider save/map-ban/counter/dispel interactions and the one explicitly excluded
stale Bless tooltip-text assertion. Next missing slice: Mass Bless and Litany,
including family-aware Bless duration and Benediction; then Mass Regeneration
and distinct Mass Slow. UP-113 remains gated on its propagation-limit definition.

Latest verified slice: UP-112 Blood Drinker and Painweaver. Three Luna workers
owned separate Life Drain, Hex and detached AI fixture files; root integrated
and independently reviewed the candidate. Blood Drinker uses its existing
actual-damage healing hook; Painweaver scales only Hex's cast-time Spell Power
component. Existing bonus snapshots carry the result without new state/polling.
Final both-target68123 exits0; principal6616 passes23/23 in6.246s and
activated33834 passes29/29 in7.838s, zero skips. Data/inventory19/19 and
module drift check pass. Coverage161/310 active,149 planned; Shadow8/2.
Build/fixture failures and repairs are persisted. Phase2 retains observed
strategic AI nonselection, reflected Life Drain paired-target semantics,
recipient-healing preview and wider modifier/save interactions. Generic UI
provisional; authored art Not done; no GUI/playable promotion. UP-113's
undefined normal propagation limit awaits the recorded scope/number question.
Next UP-114 read-only map is complete: distinct perk-granted Mass entries need
generic grant/family support, ordinary-learning exclusion and deliberate old
Temporal Field saved-profile compatibility. No coverage from mapping.

Previous verified slice: UP-109 Controlled Blast and UP-110 Pyromancer/Cryomancer.
Read-only maps are complete; three bounded Luna workers own disjoint runtime,
damage and native-fixture files. Root owns shared integration, acquisition/AI
fixtures, registration and focused build/native verification. Controlled Blast
filters only the friendly original center occupant for Fireball, Inferno and
Meteor Shower; the shared Lua effect transform also serves detached forecasts.
Damage perks modify only the Spell Power damage coefficient, including Fire
Wall's existing snapshot, never durations or the flat base. The hover preview's
empty-target fallback must remain Cure-only so it cannot reintroduce a protected
damage target. Mapping alone did not count as completed coverage or delivery.
The candidate is now native verified and activated: client38230, repaired
both-target48589 and v3-fixture10278 exit0; principal5598 passes20/20 in5.977s,
activated19887 passes28/28 in8.153s, zero skips. Data/inventory19/19 and module
check pass. Coverage159/310 active,151 planned; Havoc6/4. Source/fixture review
has no remaining blocker. The failed compile and invalid v2 setup run are
persisted in the release-failures register, with repairs and succeeding evidence.
Phase2 keeps wider defense/coefficient, proxy/reflection and hybrid v2 fixture
interactions; authored art is Not done and generic UI provisional. No GUI or
playable promotion. UP-111 Cataclysm map is complete: baseline Armageddon's
physical-obstacle cleanup is also missing. Ordinary magical-obstacle scope is
an item-level clarification gate, not permission to block independent coverage.

Previous verified slice: UP-107 Estates Land Surveyor.
Native verified and activated: principal87442 passes3/3, activated61224 passes
18/18 in7.206s, zero skips; client11819/baseline13332/both-target30265 exit0.
Data/inventory19/19 and module drift check pass. Coverage156/310 active,154
planned; Estates4/6. Source/fixture reviews have no blocker; Phase2 retains
independent holders, guarded/abandoned execution, old-format gates and broader
fan-out/AI strategy. Localization and authored art remain deferred; no GUI or
playable promotion. No build/native is live. Next UP-108 Divine Mandate maps
are complete, held at the expiry/use-accounting choices; this is an item-level
design gate, not permission to block all remaining missing coverage.
Production is frozen and independently reviewed with no blocker. A versioned
hero weekly marker uses existing property replication and the shared successful
mine capture hook; ordinary income supplies the output calculation. Root guards
bounded adjacent capture routing against prior mine garrison visits. The minimal
mine builder enables future mine-specific fixtures without modifying production
map formats.

Previous verified slice: UP-106 Estates Financier. Its exact weekly1% treasury
interest uses one pre-turn snapshot with a1000 Gold cap per active holder.
Both-target21766 exits0; principal39424 passes3/3, activated95915 passes15/15
in61.975s, zero skips. Data/inventory19/19 and module drift check pass. Coverage
155/310 active,155 planned; Estates3/7. Independent review reports no blocker.
Phase2 retains selected-holder rank loss/planned status suppression, broader
calendar/save/client fan-out and strategic weekly AI forecasts. No GUI/promotion.
UP-105 was a duplicate Perfect Fortune selection: UP-081 already records its
map and unresolved immunity choice, so no further duplicate exploration occurs.
UP-103 Rapid Embarkation is held at the Navigation
stacking choice (fixed10% or halved5%). Its full-charge/shared-path source map
is complete; no implementation is counted. UP-104 Pursuit March is the
independent mapped candidate, held at its recovery-cap/expenditure question.
Continue from pushed736ffe39e and the verified Land Surveyor slice; do not
let one item-level ambiguity block all missing specification implementation.

Latest verified slice: UP-102 Logistics Roadmaster and Wayfarer. Shared rational
costs and cached active-perk flags feed authority, player forecasts and AI routes.
Both-target20420 exits0; activated28363 passes25/25, zero skips in4.827s,
including legal offers, accepted movement and AI cache refresh. Data/inventory
19/19 and module drift check pass. Coverage154/310 active,156 planned;
Logistics5/5. Independent production review reports no blocker. Art and playable
delivery remain pending; Phase2 retains full client visitor fan-out, broader
multi-day/mode interactions and old-save loading. Next choose an unblocked
missing specification item; do not turn these focused gates into a broad matrix.

Latest verified slice: UP-101 Quartermaster. Genuine once-per-combat extra
activation applies50% output to Ballista, Tent and Catapult, with side-owned
versioned/replicated state, shared forecasts, AI Tent/Catapult consumers and
authoritative log feedback. Final both-target21374 exits0; principal47670 passes
6/6 and activated88418 passes22/22 in8.107s, zero skips; data/inventory19/19.
Coverage152/310 active,158 planned; War Machines5/5. Art and playable delivery
remain pending. Phase2 retains future-lookahead state consumption, low-output
Catapult fallback and broader activation/Order interactions. Next select an
unblocked missing item from the priority queue; Field Workshop's destroyed-target
question and Breachmaker adjacency remain independent design gates.

Latest UP-101 gate: repaired build completes both executable links, and a fresh
both-target check exits0. Principal73624 passes five of six cases, zero skips;
the Catapult fixture fails activation setup before checking structural output.
A bounded Luna fixture owner is diagnosing the cause. Keep registration planned
and counts unchanged until the corrected six-case gate passes. Failed build and
native evidence remain in NH_RELEASE_FAILURES.md.

UP-101 source is frozen and reviewed without a remaining blocker. Both-target
build88648 runs with12 jobs (`UP101-build.log`). Principal native filter is
NewHorizonsQuartermasterTest.* (six cases), including legal offer, actual
Ballista/Tent/Catapult output, Tent AI hook, no-perk/cart guards, versioned state
and detached forecasts. Keep registration planned until the focused gate passes.
Review repaired terminal battle UAF, lightweight Catapult proxy safety and Fire
Wall lifecycle admission; lessons are retained in NH_RELEASE_FAILURES.md.

UP-101 implementation is now delegated to separate Luna runtime and consumer
owners. Root appends NEW_HORIZONS_REDUCED_EXTRA_ACTIVATION and wire type289;
the requested isolated tester spawn was service-rejected, so assign it when an
execution slot frees. No concurrent source owners share files. Quartermaster
remains planned until focused compile/native evidence, and no GUI or playable
snapshot promotion is authorized by this implementation checkpoint.

2026-10-01 continuation: the preceding reply only confirmed an already-recorded
Twist of Fate decision and made no new implementation progress. Clean worktree
revalidated. UP-101 Quartermaster is selected while UP-100's destroyed-target
question remains open. Separate actual Luna explorations map runtime lifecycle
and UI/AI/fixture seams before root chooses the shared 50%-effectiveness contract.
No new activation, build, coverage or playable-delivery evidence yet.
Both Quartermaster maps are now complete and their exact seams/root correction
are retained under UP-101. Next execution is the bounded runtime, consumer and
fixture implementation with exclusive file ownership, not another exploration
of these same paths. The current lifecycle does not automatically refresh all
action flags for a new turn reason; add explicit true-extra-activation handling.
Half output applies before healing/structural caps and composes with Master
Gunner's second-shot multiplier. Coverage151/310 remains unchanged.

2026-10-01 continuation: adfabbc46 is pushed and the worktree was clean. The
previous cycle was verified progress, not a wait. UP-100 Field Workshop is the
next complete unblocked candidate: implement both allied-machine and friendly-
fortification Tent repairs at normal Siege output, with shared validation and
forecasts plus minimum UI/AI hooks. Two independent read-only Luna maps prepare
authority/state and consumer/fixture seams. Counts remain151/310 until verified;
Breachmaker adjacency and other pending design questions remain item-level gates,
not a reason to stop Phase1.
Field Workshop maps are complete. Exact seams and the automatic-control empty-
troop-list trap are retained under UP-100. Destroyed-target scope is a genuine
design gate: repairing existing damaged targets is straightforward; rebuilding
towers needs shooter reconstruction and occupied breaches need legality rules.
Do not implement a silent exclusion and call the whole perk active. Coverage is
still151/310. Other unblocked missing items can proceed after this map checkpoint;
Quartermaster is the next War Machines candidate to map if the answer is absent.

Latest completed slice: UP-099 Master Gunner. The second Ballista shot is a
separately selected60% attack inside the same activation; shared state/forecast,
authority, UI decline/Wait controls and fresh AI target selection are implemented.
Both-target76128 exits0. Principal71745 passes4/4 and activated74243 passes16/16,
zero skips in1.450s/5.022s; data/inventory19/19 pass. Coverage151/310 active perks,
159 planned; War Machines4/6. Build/fixture failures and repairs are retained in
`NH_RELEASE_FAILURES.md`. No GUI/art acceptance or playable delivery is implied.
Phase2 retains Second Wind handoff between shots, extra-attack stacking,
controller-transfer compatibility, first-shot lookahead, log localization and
full binary battle snapshot verification. Next highest-priority prepared work is
Breachmaker structural overflow, pending the asked fortification adjacency choice;
other unblocked missing specification items remain available if that choice is
not answered. Do not idle the full Phase1 goal on one content ambiguity.

2026-10-01 continuation after pushed407788932: coverage150/310; clean worktree
on resumption. Independent read-only maps prepare Breachmaker and Master Gunner.
Breachmaker has raw pre-cap structural damage in ServerCallbackProxy and current
per-part HP in SiegeInfo; shared CatapultAttack state application also drives AI
projections. No fortification adjacency table exists. The keep/outer-wall topology
choice is asked before implementation; enum or AI target order is not geometry.
Retain NewHorizonsWarMachinesTest real-town and HypotheticWallTest parity leads.
Master Gunner requires a selectable second shot within the same activation,
not another generic activation or an automatic repeat at the first target.
UP-099 is selected for implementation. Exclusive Luna owners cover shared/server
state and damage, separate AI/client interaction paths, and an isolated fixture.
Root appends NEW_HORIZONS_RANGED_FOLLOW_UP once and adds a bounded BattleInfo
binary sidecar because CStack omits CUnitState in binary snapshots. UnitChanges
JSON remains the replicated live state; old-format downgrade must fail rather
than lose a pending shot. A dedicated continuation preserves activation lifecycle
through the first shot. No build or new active count before source freeze and
the accepted independently targeted second-shot/60% principal gate.

Completed working slice: UP-095 War Machines Surgeon. Its Tent-triggered single
physical-affliction cleanse needs Poison → Disease → Bleeding priority, then
application order for other eligible physical afflictions. A Luna read-only map
has completed the read-only map: the centralized Tent cast and Poison/Disease
removal seams exist, but generic physical eligibility/application order and
Bleeding representation do not. Root must establish that shared foundation
before complete registration. Do not count a Poison-only special case as complete Surgeon coverage.
The generic marker foundation is now in source: explicit physical-affliction
identity and application order use existing bonus parameters, with parser/schema/
docs and an upfront save downgrade guard. Disease has an explicit marker; outgoing
effect packets stamp order before authoritative application. Shared live/detached
lifecycle and isolated tests are still being implemented. Independent metadata/
packet review repaired an MSVC floating-point-to-int64 boundary before build;
data/inventory19/19 pass. Root runtime review identified duplicate-marker index
and unset-order handling defects; the runtime owner is repairing them before
freezing for compilation. No build/native or Surgeon completion is claimed.
Independent runtime review then found non-spell marker groups surviving child AI
removal because the old projection filter captures only spells/Orders. This is a
blocking generic-state issue and is being repaired with a parent/child regression
before compilation. Surgeon Tent/AI consumers are being implemented in parallel
on separately owned files; no perk activation or coverage increase yet.
Current gate: live/detached and Tent/AI source are frozen and reviewed. The
marker-only removal/recapture/aging repair has its regression;13 foundation and4
real-healing cases are registered. Three compile failures (direct headers and
fixture declarations) were repaired without weakening assertions. Retry67115 is
running both targets with12 jobs; native acceptance and activation remain pending.
Final evidence supersedes the above in-progress chronology: both-target64786
exits0; principal29476 passes17/17 and activated59354 passes34/34, zero skips
in6.552s. Data/inventory19/19 pass; independent final review has no blocker.
Surgeon is active; coverage148/310 with162 planned, War Machines1/9. Shared
affliction marker lifecycle, four real priority heals, stored-Poison cleansing,
negative guards and AI selection are verified. No Bleeding producer, artwork
approval, GUI or playable promotion is claimed. Phase2 retains packet-wide
preprocessing rollback on later-unit errors, control-change interactions,
producer-duration consistency and combat-log localization.
UP-094 Discipline questions remain pending, not a reason to idle the backlog.

Completed working slice: UP-096 War Machines Piercing Bolts. Surgeon is pushed as
424ed5a02 and its checkpoint worktree was clean. One Luna owns shared callback/
damage payload/Lua; another owns an isolated real-shot fixture. Root owns review,
CMake, registration and gates. Do not activate before principal evidence.
Retained architecture map: Creature
Defense is the early getDefense/getDefenseIgnored Lua attack-vs-Defense layer,
not the later hero-Defense-based Bulwark mitigation. A current-controller,
physical Ballista-shot contribution in the shared DamageAttackInfo payload can
feed that same layer for actual damage, UI prediction and BattleAI, without
mislabeling it as Archery or Arcane Breach. The existing canonical Ballista-shot
fixture provides a small deterministic starting point. Implementation is underway;
no new active count is claimed. No new persistent state or artwork is required.
Production is frozen and independently reviewed without a blocker; client70423
builds successfully. The isolated native fixture is still being written and is
not registered yet. No activation/count change. A separate Luna read-only map
of Battlefield Medic's casualty-restoration and Tent/AI seams is assigned as the
next candidate, without touching source or displacing Piercing Bolts gates.
Phase2 fixture maintenance finding (source inspection, not a new failed run):
the older NewHorizonsWarMachinesTest in NewHorizonsHeroGrowthTest loads current
capability data then forces v3 without removing v4 warMachineShop, the same setup
pattern rejected in the earlier Surgeon gate. Its explicit v3 expectations need
a coherent historical fixture or current-schema migration. Do not use this old
fixture as acceptance evidence for the current Piercing Bolts slice; the new
fixture retains canonical current capability data.
Battlefield Medic read-only map complete: post-cast doHealAction can restore from
half the calculated Siege output via existing RESURRECT/provenance caps, separate
from actual survivor HP gain. Surgeon must remain gated on survivor healing before
any Medic restoration. Shared Tent prediction/AI needs restoration count feedback;
no new casualty ledger is indicated. Persistence after combat is unspecified, so
the user is asked permanent army restoration vs combat-only restoration. This
candidate remains mapped, not implemented, until that design choice is settled.
Final Piercing Bolts evidence supersedes the in-progress chronology: client70423
and combined42241 exit0; principal18354 passes4/4 with zero skips in1.560s.
Activated21661 passes all4 new cases,4 Surgeon and spell-like classification;
two existing Archery fixtures fail at omitted earlier-tier perk prerequisites.
Independent review classifies legal fixture setup repair as deferred Phase2,
not a new damage regression; retain the9-pass/2-fail batch, do not call it green.
Data/inventory19/19 pass. Piercing Bolts active, coverage149/310 with161 planned,
War Machines2/8. Actual controller-transfer coverage remains Phase2. No GUI,
art approval or playable promotion. Next candidate is Battlefield Medic, whose
restored-creature post-combat persistence awaits clarification.
Current next-item map: UP-097 Counter-Battery/Fortification Engineer. A separate
Luna traces deliberate enemy-machine targets, defensive-tower manual control,
shared final damage and125% Siege output. Root must settle full targeting scope
before selecting implementation; do not count a multiplier-only subset as the
whole Counter-Battery perk. The pushed Piercing Bolts checkpoint is50a85e3bf.
Current implementation selected: UP-098 Fortification Engineer. Its standalone
125% Siege/manual defending-tower rule is clear and can progress while other
design questions remain open. A Luna owns contextual callback/header/flow, and
another owns a real fortified-town native fixture. Root owns integration/gates.
Existing tower damage payload and validated manual-shot UI are reused; the bonus
scales Siege before evaluating the output, not the entire damage value. No new
stored state, source completion or active count is claimed before acceptance.
Counter-Battery map confirms existing legal machine shots and shared UI; tower
auto-selection deliberately prefers non-machines. Damage is+50% final against
enemy war machines. Its manual-vs-automatic tower-targeting overlap with
Fortification Engineer is asked, so Counter-Battery remains mapped, not active.
Retain the shared final multiplier and AI cache/target-choice seams for that
decision. Fortification Engineer's prototype rounding is floor(125% Siege) before
the existing integer output formula, never125% of the total base-inclusive output.
Final UP-098 checkpoint: client43691 and both-target19393 exit0. Principal2955
passes4/4 real-siege/eligibility cases; activated75235 passes12/12 Engineer,
Piercing Bolts and Surgeon cases, zero skips in3.960s. Data/inventory19/19 pass.
Engineer is active, coverage150/310 with160 planned; War Machines3/7. No new
persistent state, art approval, GUI or playable promotion. Ordinary automatic
tower activation and controller-transfer breadth remain Phase2. Precision
Bombardment's read-only map found existing Basic-rank target selection/control
overlap, not a basis for silently guaranteeing structural hits or nerfing rank
control. Counter-Battery/Medic still await their recorded design decisions.

UP-093 Fearless is active and Phase1 verified. Both-target36048 and repaired24535
exit0; principal13527 passes5/5 and activated30226 passes27/27, zero skips in9.008s.
Data/inventory19/19 pass; independent Astra production/fixture review has no
blocker. Coverage147/310 active,163 planned; Discipline5/5. Source-aware immunity,
current-controller turn-start feedback and nominal AI forecast are implemented.
The detached fixture was repaired to respect hero visibility, not bypass it.
Phase2 retains future shared-stack-key sources, RNG-state assertions and seeded
AI chance/history correlation. Art Not done; no playable promotion. Next-item
maps identify Heroic Spirit activation timing and Veteran Cohesion HP denominator
questions; clarification is pending without blocking other coverage work.

UP-092 Hold Fast is active and Phase1 verified. Both-target2758 exits0;
principal85726 passes7/7 and activated69879 passes28/28, zero skips in8.612s.
Data/inventory19/19 pass; independent Astra reviews have no remaining blocker.
Coverage146/310 active,164 planned; Discipline4/6. The generic activation-begin
duration, authoritative Defend/Hold Line grants, logs, AI forecasts and guarded
bonus persistence are implemented. Canonical Defend completion and current-owner
Second Wind activation/end defects were repaired, not bypassed by weaker fixtures.
No art approval or playable promotion. Phase2 retains future negative-duration
Purify consumers, within-activation controller changes and Morale forecast
correlations. Next: source-aware Fearless immunity, mapped without source edits.

UP-091 Standard Bearer is active and Phase1 verified. Both-target42607 exits0;
principal82873 passes4/4 and activated74455 passes39/39 with zero skips in10.603s.
Data/inventory19/19 pass; independent Astra reviews find no blocker. Coverage
145/310 active,165 planned; Discipline3/7. Dynamic current-friendly adjacency,
raw-before-cap Morale, actual positive/negative gates, branch isolation and the
existing panel's display/refresh hook are implemented. No new layout/art or
playable promotion. Phase2 retains explicit double-wide and death/resurrection
coverage. Next UP-092 Hold Fast: a generic genuine-activation expiry must not
inherit STACK_GETS_TURN's premature Hero-spell expiry or missed Second Wind start.

UP-091 Reserve is active and Phase1 verified. Both-target34777 exits0;
activated native69809 passes16/16 with zero skips in4.778s, and data/inventory19/19
pass. Actual delayed +2 movement, unchanged Initiative, immediate expiry,
current-controller ownership, branch isolation and serialized sidecar/UnitChanges
are verified. Coverage144/310 active,166 planned; Battlecraft2/8. Independent
Astra review was service-rejected; root reviewed the slice without inventing that
approval. Purpose-made art and playable promotion remain open. Phase2 retains
Wait-choice attack-catalogue regeneration and the pre-existing full binary
unit-state snapshot contract. Next: Standard Bearer, using the retained dynamic
adjacency map rather than cached sibling-dependent bonus limiters.

UP-090 Rally is active and Phase1 verified. Both-target build93251 exits0
(`UP090-build.log`); principal3559 passes4/4, activated native7731 passes47/47,
zero skips in13.611s, and data/inventory19/19 pass. Independent production review
has no blocker; its stochastic-precedence and one-event-AI fixture findings were
strengthened before the gate. Coverage143/310 active,167 planned; Discipline2/8.
Exact AI first-trigger ordering/correlation remains Phase2. No purpose-made art
approval, GUI launch or playable promotion. The next bounded
Esprit de Corps map identifies separate mixed-faction and undead-presence Morale
penalties, and hero context missing from Nullkiller's temporary-army projection.
User clarification is requested on which composition penalties its total-1
reduction covers; do not silently choose the narrower mixed-faction interpretation.

Previous completed item: UP-089 Twist of Fate is active and Phase1 verified.
Final both-target31690 and native95364 pass43/43, zero skips in12.421s; data19/19.
Independent Astra activation review finds no blocker. Coverage142/310 active,
168 planned; Luck6/4. No playable promotion or purpose-made art approval.
Next UP-090 Rally: independent battle-long cancellation state, first actual bad
Morale suppression before Twist, preserved cached first draw, ordinary activation,
replication/save state and candidate-local AI. Cross-stack probabilistic ordering
and future Unbreakable coexistence are explicit later integration/design work.

### 2026-10-01 current slice — Twist of Fate shared reroll infrastructure

Latest checkpoint: the scripted hostile boolean/count bridges and local AI
callback are implemented. First build18304 exposed C++ callback/Unit interface
mismatches, repaired without a rule change. Retry23124 builds both targets;
native26641 passes39/39, zero skips in10.901s, including four actual negative
Luck/Morale/suppression/hostile Death Blow cases. Data/inventory19/19 pass.
Principal Lua scripted tests remain unregistered/unbuilt; full-perk activation,
late-collateral evidence and independent scripted review are next. Coverage is
still141/310 active,169 planned. No GUI or playable promotion.

Scripted fixture checkpoint: both-target50122 exits0; combined native6674 passes
42/42, zero skips in12.110s. Real Lua tests verify Destruction's failed final
redraw, the exact final capped Death Stare kill count, and immune targets retaining
Twist. Independent Astra scripted review remains service-unavailable after
repeated retries; root reviewed the diff. Commit this verified bounded slice,
then add late Hand of Fate collateral evidence before activating/counting Twist.
Full attack-script dispatch and broader interaction/AI matrices belong to Phase2.

UP-089's approved scope includes negative Luck/Morale, failed hostile resistance
and successful hostile chance abilities; not damage variance, failed benefits
or random selection. Root selected independent side-owned enabled/used state,
not strike fortune snapshots, so attack packets cannot reset a spell/proc-spent
allowance. Shared worker implemented append-only state and packet287 with
monotonic validated application. Root added a generic authoritative resolver
that publishes expenditure before one final redraw, hero-named combat feedback,
ServerCallback/server-spell bridge and recorder forwarding, and detached copied
branch state. A separate worker supplies six bounded infrastructure fixtures.
Registration remains planned: no perk coverage increase until real callsites,
actual-target resistance/reflection handling and AI forecasts are wired and
verified. Coverage stays141/310 active,169 planned; Luck5/5.

The tester's first spawn and reviewer spawn/follow-up were service-rejected by
the thread limit; tester retry succeeded after the shared worker completed.
Independent review and both-target/focused execution gates remain pending.
No GUI, promotion or full-perk completion is claimed. Runtime mapping requires
fixed effective fractional proc chance and MR spending only on actual prepared
hostile recipients after reflection, never the current all-unit prepass.

All source is frozen, including six fixtures. Independent Astra review retry
succeeded after fixture completion. Both-target1364 is running with12 jobs,
log `UP089-infrastructure-build.log`; focused infrastructure/Luck native execution
awaits its terminal result. No native verification or source commit yet.

Independent infrastructure review completed: no blocker. Deferred direct
assertions for invalid-side resolver fallback and malformed current state loads
are recorded for Phase2; runtime interception and AI valuation remain required
Phase1 implementation work, not deferred integration substitutes.

Infrastructure gate passed: both-target1364 exits0; native73236 passes32/32,
zero skips in8.536s (`UP089-infrastructure.log`/`.xml`); data/inventory19/19 pass.
Binary SHA `adefcb23c6001b687c0f425d29dafbc69ff9fbe749edbb31063a5c86275b08b8`.
Freeze is released for actual runtime wiring. Registration/coverage unchanged;
this is a verified dependency checkpoint, not completed Twist of Fate.

Runtime continuation: attack/Morale and hostile-proc callsites are frozen. Root
review rejected post-target-collection MR resolution because Chain Lightning
routes during preparation and Hand of Fate chooses collateral during application.
The repaired spell slice uses a shared per-recipient lazy final decision, preserving
legacy first draws, with authoritative callback/RNG access scoped to the cast.
Prediction suppresses it; reflection rebuilds the cache. Root added branch-local
AI resolver application and first-event negative Luck/hostile MR forecasts.
Broader conditional multi-event valuation remains a Phase2 finding.

New concurrent worker spawns were service-rejected; an idle Luna follow-up now
owns only the new actual-runtime fixture. Both-target compile77876 is live with
12 jobs (`UP089-runtime-build.log`) while that test file remains unregistered.
Data/inventory19/19 pass. No runtime-native pass, global activation, coverage
increase, commit or playable promotion is claimed yet.

Production compile77876 exits0; regression native59072 passes32/32 with zero
skips in8.445s (`UP089-runtime-regressions.log`/`.xml`). Binary SHA-256
`e1196ff56aa5e28adc2240fc7598099266a0d654b5a781abac1cec2bd0b2d7c2`.
The new fixture is still being written and is not covered by this pass. Runtime
acceptance and independent review remain pending; no perk-count increase yet.

Runtime dependency checkpoint: both-target4456 exits0 and final native34416
passes35/35, zero skips in9.458s (`UP089-runtime-verified.log`/`.xml`). Binary SHA
`e6bd7c8ccd8ee258a953e1e4103005def3be6210b51ca3d7e56d5a7efba5b852`.
Three new cases cover actual lazy chain MR with a secondary-hop guard, first-event
Luck forecasting, and local hypothetical resolver expenditure. Independent source
and fixture-repair reviews have no blocker; failures are retained in the failure
register. No activation/count increase: scripted Destruction, Transmutation and
Death Stare still need harmed-recipient reroll support, followed by principal
attack/Morale/proc and late-collateral evidence. These are required Phase1 work.

### 2026-10-01 verified slice — Luck Chain of Fortune

UP-087 follows the approved different-stack recipient and carry-until-used
wording. Shared side state owns one pending origin and a once-per-round trigger
flag; different-stack consumption precedes possible rearming, same-stack
follow-ups do not consume, and No Luck retains immunity without preserving the
benefit. Old state defaults inert through append-only serialization. Runtime,
AI and fixture ownership are partitioned; root owns state/setup/config/CMake/
build/Git. Registration is staged; completed coverage stays140/310. Focused
native/save/packet/AI evidence is required before increasing it. No art or
playable promotion is claimed. Gambler's source/native cycle is pushed as
680d142c5; Opportunist's reaction question remains pending.

Frozen source: independent review finds no blocker. Six new focused cases now
include UNKNOWN candidate/selected replay and same-origin carry preservation.
Data/inventory19/19 and diff checks pass. Both-target74505 runs with12 jobs,
log `UP087-build.log`; native verification is pending. Broad perk/reaction
matrices and playable-log acceptance remain Phase2, not blockers to counting
the principal implementation once its focused execution gates pass.

Final both-target3912 exits0 (`UP087-repaired-build.log`); native73716 passes
26/26, zero skips in6.779s (`UP087-verified.log`/`.xml`). Initial24/26 failures
were fixture errors: live RNG settings versus forecast chance tables, and an
initiator's explicit retaliation-blocking bonus. Corrections preserve all
principal assertions; independent repair review has no blocker. Binary SHA-256
`9a0a233a0abb92f6eb1ca9ad570568301bc8e1d30fa784e4ecde484a599a180e`.
Coverage now141/310 active,169 planned; Luck5/5. Data/inventory19/19 pass.
Art and playable delivery remain pending. Next is Twist of Fate; the user
approved its explicit adverse-roll classification, now canonical.

Source commit0e403406d is pushed, with matching HEAD/origin. Launcher snapshot
remains unchanged. Twist's bounded map proposes one affected-side/adverse-result
resolver and a generic side-state packet for non-attack transitions; root must
freeze controller/reflection/proc-chance contracts before runtime/AI delegation.

### 2026-10-01 verified slice — Luck Gambler

UP-086 implements first-friendly-attack+3 Luck each round and failed-positive
trigger-2 Luck on the attacking unit until its next genuine activation. Shared
round expenditure is independent of whether a roll has a known outcome; the
per-unit timed bonus follows controller changes. Only the Gambler bonus expires
through battleBeginsActivation, including Second Wind, without broadening other
legacy lifetimes. Runtime, AI and fixture work are partitioned; shared state,
append-only version/setup/helpers/registration are root-owned. Staged activation
does not increase completed coverage. Exact stochastic multihit/penalty
correlation remains Phase2 breadth; principal paths and branch isolation must
work now. No art or playable promotion claim.

Final both-target76677 passes; native39678 passes20/20, zero skips in5.324s,
reports `UP086-verified.log`/`.xml`. Six new cases cover the principal
authoritative, packet/save and detached paths, with14 Luck regressions. Fixture
visibility and ordinary Advanced Luck+2 baseline failures were repaired without
production rule changes and retained in NH_RELEASE_FAILURES. Data/inventory
19/19 pass; independent source review has no blocker. Coverage140/310 active,
170 planned; Luck4/6. Art Not done and playable delivery pending. Chain of
Fortune's approved different-stack/carry-until-used semantics are canonical;
its implementation is next. Opportunist's movement-continuation map is ready,
with a pending own-activation/reaction question.

### 2026-10-01 current slice — Luck Second Chance

UP-084 implements the next unblocked Basic Luck perk. Independent battle-long active
and spent flags are added to the existing replicated army Luck state; Nature's
Providence keeps its independent round-long flag. Both first-trigger conditions
qualify on the same rolled negative when both apply, without inventing an extra
sequential shield. Append-only NEW_HORIZONS_SECOND_CHANCE protects binary/wire
compatibility and old states default inert. Runtime/shared eligibility and
detached AI branch consumption are source/native verified. Both-target23927
passes; native6011 passes14/14, zero skips in3.859s, reports
`UP084-verified.log`/`.xml`. Data/inventory19/19 pass; repaired independent review
has no blocker. Coverage139/310 active,171 planned; Luck3/7. Actual first-trigger
suppression, round persistence, side isolation, serialization, double shots,
retaliation, forced-positive exclusivity and excluded sources have evidence.
Probabilistic multihit distribution, explicit stochastic-result replay and
fully absorbed reaction/controller-change breadth remain Phase2. Art Not done;
no playable promotion. Serendipity's round1 question is pending; Gambler is the
next unblocked read-only map.

### 2026-10-01 current slice — Luck Lucky Aim

UP-082 implements the next unblocked Basic Luck perk while Perfect Fortune's
automatic-trigger immunity question awaits direction. Shared damage payload
adds25% target Creature Defense ignore only for ordinary physical creature
shots marked positive Luck; Elven Precision retains its25% and combines in the
same capped target-side calculation. No polling, state field or new save format.
Client73900 exits0; final both-target62197 passes. Native69961 passes8/8,
zero skips in2.487s, including three new cases, Fortune's Favor regression and
two older Elven Precision cases. Data/inventory19/19 pass; repaired independent
review finds no blocker. Registry138/310 active,172 planned; Luck2/8.
Failed fixture/API/geometry/formula runs remain recorded, with no production
damage rule altered to satisfy the tests. Spell-like and war-machine attacks
remain ineligible. Executed-shot/combined-perk matrices and fractional rounding
remain Phase2; no new art approval or playable promotion.

### 2026-10-01 next slice — Luck Fortune's Favor / Last Stand boundary

UP-078 is source/native verified. UP-079 Last Stand's map is complete, but
clone/Phantom eligibility and ending the saved stack's own activation await
user answers. UP-080 is the next unblocked Basic foundation: Fortune's Favor
adds +25 percentage points through existing LUCKY_STRIKE_DAMAGE_PERCENTAGE,
opening Luck's ordinary advancement. Refresh its derived hero bonus only on
existing perk/rank/reconstruction transitions; do not poll during damage or
create a second multiplier. Shared Lua/server/AI already consume this bonus.
Runtime and registration are now verified: the existing secondary-skill bonus
rebuild derives +25 only for the active perk, and accepted Luck selections
refresh it without requiring a rank change. Client build17957 exits0;
data/inventory19/19 pass; independent source review finds no blocker. Final
both-target56878 and native69200 pass,4/4 zero skips in1.398s, including legal
offer/lifecycle, deterministic damage and detached AI expectation. Registry
coverage137/310 active,173 planned; Luck1/9. Explicit save roundtrips, reaction
combinations and Sylvan coexistence remain Phase2. No launcher promotion or art
approval is implied. UP-081 Perfect Fortune is mapped but automatic-trigger
eligibility needs a bounded decision before implementation.

### 2026-10-01 verified slice — Armorer Veteran

UP-078 maps the next missing Advanced perk after Formation Fighting, committed
and pushed as f774b24c3. Veteran restores 15% of physical creature damage
suffered since the stack's previous activation at activation start, without
resurrecting casualties. Runtime and detached AI must share provenance, surviving
wound caps and actual activation semantics. Reuse existing damage/activation
and saved state abstractions before adding history. Runtime and AI maps are
bounded and read-only until the root assigns disjoint ownership. Coverage stays
135/310 active perks, ranks84/93 and combat identities60/67 until implementation
and focused native gates pass; no playable promotion or new art is implied.

Source checkpoint: shared history/recovery and live/detached activation paths
are implemented; content/inventory19/19 pass and client12894 compiles. Existing
PHYSICAL_CREATURE provenance includes already-classified physical Poison and
reflection; temporary/Guardian Spirit absorption never contributes to Veteran.
Independent Astra review identifies a blocking AI Guardian Spirit double-
absorption/pre-clamp defect, now assigned back to the AI worker with focused
preview/commit HP-buffer-history regression coverage. Keep counts unchanged
until the repaired source builds and native evidence passes. No broad suite,
GUI automation, artwork change or launcher promotion is being performed.

Final both-target8101 passes; native19447 passes14/14 without skips in4.124s.
Reports `UP078-focused-buffer.log`/`.xml`, binary SHA-256
`ef35142a822610a400a5f9dad60f358fb21645a2cb15736ce325a84f0428dca8`.
Data/inventory19/19 pass; independent Astra review blockers are repaired.
Coverage135→136/310 active perks, planned175→174; Armorer6/4 active/planned.
Ranks84/93 and combat identities60/67 unchanged. Phase2 retains full-absorption
multistrikes and Guardian reaction/Rain matrices; purpose-made art remains
Not done. Failed runs are retained; no playable promotion or rendered claim.

### 2026-10-01 verified slice — Formation Fighting

UP-077 implements current-controller friendly footprint protection, independent
10% capped physical reduction, Shroud immunity and Flank melee/history immunity,
while retaining Combined Arms ranged value. Final both-target74477 passes;
native61868 passes18/18 without skips in4.465s; data/inventory19/19 pass.
Coverage134→135/310 active perks, planned176→175; Armorer5/5 active/planned,
ranks84/93 and combat identities60/67 unchanged. Independent source/fixture
review blockers are repaired. Phase2 retains multi-blow other-ally projections,
hidden foe perk uncertainty and the existing Encirclement repeated-hit fixture
failure. No art or playable promotion. Next unblocked missing coverage:
Armorer Veteran's activation-time surviving-creature physical damage recovery.

### 2026-10-01 current slice — Formation Fighting / Diplomacy boundary

UP-076 reuses the prior UP-048 Diplomacy map. Authored free-join exceptions
remain awaiting user direction; ranks are not activated. The pricing audit
confirms full original-stack Gold cost despite the global joining percentage
is deliberate legacy configuration. Parsed per-object HotA percentage is a
separate existing gap, not permission to silently alter map admission.
UP-077 implements the unblocked Advanced Armorer Formation Fighting perk:
live friendly adjacency provides flanking immunity and additional10% physical
reduction through shared authoritative/detached damage evaluation. Geometry,
current allegiance, movement/death and global cap must remain coherent.
Bounded Luna mapping precedes source ownership. Coverage remains134/310
perks, ranks84/93 and combat identities60/67 until focused build/native evidence.

### 2026-10-01 verified slice — Estate Network / Quick Study

UP-075 now has production, registration, focused server/query and AI evidence.
Both-target20329 passes; native80431 passes29/29, zero skips, in10.865s;
final data/inventory19/19 pass. Perks132→134/310, Estates2/10, Learning2/10;
ranks84/93 and combat identities60/67 unchanged. Existing calendar/RNG/query
snapshots suffice: no new counter or per-frame invariant was added. Purpose-made
art remains Not done; no launcher promotion. Phase2 retains comparative economic
perk valuation, pending-query/crash-recovery and custom calendar/script cases.
The next missing foundation is deterministic Diplomacy (all three ranks and
ordinary neutral joining); map authoritative shared eligibility/cost, Leadership
transfer and minimum AI usage before implementing. Do not let additional tests
around these verified perks displace that missing system.

### 2026-10-01 current slice — Estate Network / Quick Study

UP-075 maps two independent missing Advanced perks while Academic Study's
first-visit timing awaits the user. Estate Network must use the authoritative
weekly event, including the initial week, without granting ordinary daily
income on setup day. Quick Study must redraw the whole initial level-up offer
at reached levels5/10/etc before its query is presented, with only one primary
growth award and no fresh draw on re-exposure. Existing saved calendar, RNG and
query snapshots should be reused. Root owns integration/registration/builds;
bounded Luna workers map separate weekly-income and hero-level-up paths.
No activation, coverage increase or playable delivery is claimed yet.

### 2026-10-01 verified slice — Learning Mentor / AI market selection

Mentor's field/town weekly teaching is source/native verified, including real
Nullkiller selection and authoritative meeting, saved replicated usage and
recipient Learning composition. AI resource trading selects the best eligible
owned-town exchange effectiveness. Merchant Prince remains planned; this is its
minimum AI prerequisite, not a second activated perk. Both-target81553 passes;
native52779 passes24/24, zero skips; final data/inventory19/19 pass following
the broader78/78 checkpoint. Perks131→132/310, Learning0/10→1/9; ranks84/93
and combat identities60/67 unchanged. Preserve failed fixtures/builds and the
existing Muster tier-prerequisite finding in NH_RELEASE_FAILURES.md. Phase2
retains nested town-building XP, mixed-owner meetings, mid-prompt reload and
comparative AI choices/proactive meeting paths. No art or launcher promotion.
Next unblocked missing feature: UP-074 Academic Study, mapped read-only while
Mentor verification completes. Historian/Marketplace/Convergence choices wait
at their recorded boundaries; do not guess those decisions.

Mentor/market slice committed and pushed as07fe8d95c. UP-074's map confirms
heroVisitCastle and reusable serialized visitedObjects, not a duplicate history
field. Earlier visits before perk acquisition are not currently recorded for
towns; the eligibility timing question has been sent to the user. Keep it
unactivated until that choice is resolved; shared Learning-adjusted XP and
marker-before-award are required regardless. Subsequent unblocked coverage may
proceed without inventing the answer.

### 2026-10-01 current slice — Historian and Marketplace policy

UP-073 Mentor is now the unblocked Learning runtime slice: replicate weekly
use before XP, handle both field/town meetings and maintain level-up query
ordering. Historian, Merchant Prince and Convergence remain blocked at their
recorded design boundaries. Merchant Prince's independent AI prerequisite
selects the best shared resource-exchange effectiveness rather than the first
town; source review has no blocker and its focused fixture is wired. No perk
activation or coverage increase is claimed from that selection helper alone.

Grand Formula/Tax Collector are committed and pushed in1fe1690c2. UP-071
maps Learning Historian's adventure reward provenance and Estates Merchant
Prince's existing shared rate API in parallel. Prefer missing Basic perk
progression over additional broad testing of the verified prior slice. No
generic all-XP modifier or duplicated trade formula is acceptable. Steward,
Concentration and Polymorph retain their unresolved design boundaries.
A third independent read-only map selects UP-072 Elemental Convergence, one
of the seven missing combat identities. Reuse native summoning and captured
terrain/HP rules; no guessed mapping or provisional description-only spell.

### 2026-10-01 verified slice — Grand Formula and Tax Collector

Both perks are implemented, registered and independently reviewed. Final
both-target build68608 passes; focused native45801 passes38/38 without skips,
including actual casts, shared history, non-damage scaling, payout and AI.
Data/inventory78/78 pass. Coverage129→131/310 active perks, planned181→179;
Spellcraft4/10, Estates1/10, ranks84/93 and combat identities60/67 unchanged.
Retain failed fixture builds/runs in NH_RELEASE_FAILURES.md. Phase2 keeps
handicap/reload/ownership combinations and battle-specific tooltip math.
No playable promotion or purpose-made art acceptance. Next mapped missing
coverage: Steward's daily town contribution, pending two-resident stacking
decision; Concentration, Polymorph and Basic Toxic Spines retain design blockers.

### 2026-10-01 current slice — Spellcraft Grand Formula / Concentration boundary

UP-069 selects another unblocked missing perk while UP-066 Phantom/expiry and
UP-065 Basic Toxic Spines await design answers. Implement Grand Formula using
the existing accepted-level history and a shared SP-only 150% factor before
other multipliers. Audit Concentration's single-stack targeting boundary in
parallel with independent focused-test mapping; resolve material ambiguity
before implementing that perk. No new counter or per-frame scan is intended.
Root retains registration, integration, builds/Git and evidence updates.

UP-070 audits Estates Tax Collector in parallel as an independent first Basic
perk/progression path. Existing daily income and AI forecasts must share the
owned-town +50/cap500 amount; no spells ownership overlap and no recurring
runtime scan outside income requests. Production client build passes and both
sources have non-blocking review; native execution remains pending. The live
town-count API reconstructs its vector from owned objects, not constant time.
A read-only next-slice map locates Steward's daily owned-town event and AI seam
while root finishes Grand Formula/Tax Collector verification. No Steward source
implementation or activation is claimed.

### 2026-10-01 current slice — random battle-form AI and Mana Conservation

UP-066's next unblocked dependency uses a shared typed effect candidate API:
the authoritative uniform draw and detached AI mean consume the same complete
same-category pool and nearest-legal landing positions. The AI must retain
unfavorable outcomes in that mean, price actual detached offensive profiles,
and bypass RNGStub's single-draw cast evaluation without bypassing accepted
Hero Action/Counterspell validation. Runtime and AI workers own disjoint files.
Polymorph remains inactive pending Phantom composition and exceptional expiry
decisions plus complete lifecycle wiring.

UP-068 is independent UP-023 missing-perk coverage. Mana Conservation requires
accepted-cost accounting rather than initial/final Mana subtraction: gross
positive spell payments and Counterspell ward payments count, separate refunds
do not erase expenditure, and hostile drains do not count as payments. Restore
20% (floor), capped at 20, to Normal Spell Points after ordinary result cleanup,
preserving Buffer and capacity. A separate worker owns replicated accounting
and the battle-result path; root owns the serialization version, registration,
builds, focused verification and Git. No coverage increase or promotion yet.

Independent frozen-production review found no blocking issue. Phase 2 retains
damage-obstacle movement costs (lazy forecast caches intentionally omit them),
effective-ownership interactions with Hypnotize/Berserk, and later movement/status
expiry rather than repeated current attack pressure in the two-round estimate.
Mana Conservation's retreat/surrender and configured draw rewards are currently
source-reviewed, not native-fixture certified. Applicability and candidate-pool
footprint checks presently duplicate logic; no mismatch was found, but their
boundary deserves a direct no-space API regression in the later integration pass.
Both-target build `66640` passes. Native `65013` executes 69 cases, zero skips:
all ten Mana Conservation cases pass, but one injected random-form AI valuation
case fails its independent mean and real evaluator selection assertions. That
bounded worker is repairing the discrepancy; retain the failure log and do not
certify the AI slice yet. Mana Conservation advances active perks 128→129/310,
planned 182→181 and Wisdom 7/3→8/2. Content/perk/inventory checks pass 78/78.
No playable snapshot has been promoted.

Final checkpoint: both-target repair build `52390` passes; native `31943` passes
69/69, zero skips, in 17.000s. The AI dependency now has expected-mean, harmful
outcome, midpoint, live-state/RNG and real accepted-casting evidence. Independent
review has no blocker; content/inventory 78/78 and generated module/diff gates
pass. Mana Conservation is committed/pushed as `266c2c175`. Polymorph activation
still awaits the recorded Phantom and exceptional expiry answers; no combat
identity increase. Next unblocked Phase 1 coverage should target another missing
generic perk rather than broadening this already-verified forecast matrix.

### 2026-09-30 current slice — battle-form clone and presentation support

Following cast/result commit `56715b367`, independent Luna workers own cloned
stack admission and one-hit cleanup, event-driven effective-creature sprite
refresh, and generic form status in the existing stack panel. Root integrates
the duration accessor, test wiring, focused builds/native validation and Git;
an Astra review is required before this checkpoint is called verified.
Time Stop must pause the form's timer. Existing creature portraits/animations
are referenced, not extracted or replaced with newly invented artwork.

This remains a partial Polymorph dependency slice. Phantom Army's separate
Integrity/body profile, full expiry/Dispel geometry, expected-random-outcome AI,
and accepted hero-action/Mana casting remain unfinished. The exceptional case
where no original footprint can fit on expiry awaits the user's answer. Preserve
the user's nearest-legal relocation decision and do not exclude a form because
its old anchor cannot fit it. No activation, count increase, GUI acceptance or
launcher promotion is claimed while these workers are running.

Checkpoint outcome: final both-target build `57163` passes and isolated native
retry `39543` passes 51/51, zero skips. Reports and binary hash are recorded in
UP-066 and NH_RELEASE_FAILURES.md. Independent review and module/diff checks
pass; clone destruction, paused duration with round-local Initiative reset,
status helper/overflow and prior health/result/native-bonus guards are verified.
The unchanged ordinary CloneApply tests exposed a missing no-form delegation
fast path; that production repair is included and its failed run retained.
Sprite refresh remains source/compile evidence, not graphical acceptance.
Coverage remains 60/67 combat identities and 128/310 active perks. Next unblocked
Polymorph dependency is expected-random-outcome AI; Phantom body/Integrity
composition and no-space expiry await explicit design answers. No promotion.

### 2026-09-30 current slice — Polymorph casting and result projection

The shared foundation was pushed in `786a19777`. This follow-up adds the native
same-category cast effect, strict nearest-legal reversion API and original-form
result projections. Separate Luna workers own the spell effect and battle-result
consumer; root owns placement, JSON schema/documentation and build/test wiring.
An Astra reviewer checks the bounded checkpoint. The helper explicitly reports
no legal reversion position without mutating the stack. Whether expiry should
retain the form and retry in that case is awaiting the user's answer.

This is not yet Polymorph activation. Clone/Phantom profile support, lifecycle
placement/Time Stop ordering, random-outcome AI valuation and required client
presentation remain Phase 1 dependencies. A detached RNG returning the middle
candidate does not establish expected-value AI support. No coverage-count or
playable-delivery increase is claimed from adding a generic effect alone.

Checkpoint outcome: build `70446` and focused-fixture rebuild `32737` pass;
native retry `13545` passes 28/28 with zero skips. Native effect packet
application, exact HP/identity/Initiative, strict relocation/reversion and
original-species early-result/Necromancy/gated-reserve accounting are verified.
Independent source/repair reviews and module/diff checks pass. First-run fixture
admission failures are retained in NH_RELEASE_FAILURES.md. Polymorph remains
inactive and combat identity coverage remains 60/67. Next highest-priority
dependency is temporary-profile/lifecycle support, followed by random-outcome
AI and client presentation; the exceptional no-space expiry rule awaits its
answer. No playable snapshot was promoted.

### 2026-09-30 current slice — Polymorph shared form/HP foundation

UP-066 is in progress, with two Luna workers owning disjoint shared-health and
native/detached creature-bonus views. Root owns footprint relocation, wiring,
serialization compatibility, integration and focused builds; an Astra reviewer
checks the shared boundary. The user's nearest-legal-position decision is
canonical. Placement must reject occupied hexes even if AI pathfinding predicts
that their occupants could be destroyed. Preserve exact creature HP separately
from temporary HP and original-species casualty/resurrection/remains provenance.
No spell activation, coverage increment, playable delivery or build success is
claimed at this implementation checkpoint. Full casting, expiry/result footprint
handling, AI spell selection and status presentation remain the following slice.

Foundation is now source/native verified: final both-target build `85599`
passes and native retry passes 21/21, zero skips. Exact health/provenance,
acquired-CStack JSON/native views, nested AI rank context and strict placement
are covered alongside existing Health/Shadow Gift guards. Source review has no
remaining blocker; module/diff checks pass. Retain all failed probe reports and
fixture repairs. Full spell activation/result/geometry/status/AI selection and
active capacity/Time Stop/clone integration remain unfinished. Combat identities
stay 60/67, ranks 84/93 and active perks 128/310; no playable promotion.

### 2026-09-30 current slice — Arcane Focus

UP-065's Basic Toxic Spines contradiction is diagnosed and awaits the user's
reflection/rank decision. The previous interruption produced actionable trigger
evidence, not a verified fix. Resume independent UP-067 while that decision is
pending: first accepted hero spell receives +20% to its Spell Power component,
with existing battle-long completion state shared by authoritative and detached
AI execution. Capture eligibility before completion publication; cover direct
Sorrow/Quicksand helpers as well as damage and temporary buffs. Two Luna workers
own separate runtime/native and AI/native fixtures. Root owns activation, wiring,
focused builds, review and Git. No coverage increment or playable promotion yet.

Final source checkpoint: both targets build (`55273`), 27 focused native cases
pass without skips (`49925`), content/perk checks pass 76/76, placement/module/
diff gates pass, and review has no blocker. Land Mine's numerical count bypass
is repaired across Lua/client/AI, with legacy raw thresholds preserved. The
first AI fixture legitimately selected an Order with only 10 Spell Power; the
corrected fixture uses 200 and proves real spell choice/accepted submission
without disabling Orders. Active perks advance to 128/310, 182 planned;
Spellcraft 3/10, ranks 84/93 and combat identities 60/67 unchanged. Wider perk
interactions and full battle save/load remain Phase 2; art, graphical previews
and playable delivery remain pending. Next: Polymorph shared form/HP foundation,
including the user's approved nearest-legal-position relocation. UP-065 remains
blocked on Basic reflection/rank choice.

### 2026-09-30 user-priority interruption — main-menu branding and version

UP-064 takes precedence at the user's explicit request. Available Complete and
Armageddon's Blade illustrations receive eight bounded generated subtitle
patches rather than redistributed full original backgrounds. The existing
0.14.0 module version becomes a single authoring value shared with a small
yellow bottom-left menu label; historical bumps and the ongoing checkpoint
policy are documented in NH_VERSIONING.md. Native-size private compositions
exist; client compilation and nine focused checks pass. Independent review has
no remaining blocking finding. Rendered runtime and playable delivery remain
pending; no launcher promotion was performed.
The unfinished UP-063 working-tree slice below is preserved, not discarded,
staged accidentally, or counted as completed by this menu work.

### 2026-09-30 current slice — Shield of Chaos and Paradox Shield

UP-063 is in source with independent review complete and no blocking finding.
Two Luna workers implemented disjoint runtime/native and AI/native files; root
integrates data, canonical clarification, registration and validation. Base
protection is source-grouped physical/magical basis points, not spell immunity;
Paradox obeys the user-retained physical cap. Signed detached AI weighs damage
protection against expected Morale/Luck output changes for either allegiance.
All 78 earlier offline gates pass; final both-target Linux build `41010` passes.
Native test fixtures now advance real rounds between Hero Actions and retain
the full two-round refresh/expiry checks. Counts are not advanced before native
verification. Native `61362` now passes all 13 cases without skips; the final
content/perk gate passes 76/76, generated module matches, and final review finds
no blocker. Coverage advances to 60/67 combat identities, 127/310 active perks,
with ranks unchanged at 84/93. The failed detached preview retained a pre-cast
unit pointer; the fixture now reacquires the mutation's clone and verifies its
bonus, without weakening AI choice or authoritative submission. Wider
future-threat/recast forecasts are Phase 2 findings; art and
playable delivery remain separate. Preserve the live frozen Windows build.

### 2026-09-30 current slice — Berserk forced-action foundation

UP-062 is implementing the mapped Chaos gap. Shared targeting owns a read-only
list of nearest movement-cost candidates; only the authoritative server draws
among equal-distance stacks. Fresh v3 shooters must enter melee and walk toward
the selected target when out of range, while legacy profiles retain their old
shooting and deterministic tie behavior. BattleAI must preserve exact forced
movement/no-action and evaluate friendly as well as hostile harm without live RNG.
Two Luna workers own separate callback/test and AI/test files; root owns server,
activation tests, integration and focused builds. No new perk is activated yet.
Negative-Morale consumption and all-blocked approach remain unresolved clauses;
the present edits do not establish next-activation expiry or Frenzied Curse.
The targeting foundation now builds both Linux targets (final `27932`) and
passes native `9314`: 21/21, zero skips, including obstacle-path nearest targets,
seeded authoritative melee ties, defender movement, legacy casts and actual
accepted/read-only AI. Binary
`83356a9a474e1300cbe78c66616e4dd004ef9fcab7305d44310b813f8e1bdee3`;
reports `UP062-berserk-foundation-final-focused.log`/`.xml`. All 77 offline
checks and module/diff checks pass; independent review has no remaining blocker.
Compile and fixture failures are retained with their repairs/debugger evidence.
Counts remain 59/67 combat identities, 84/93 ranks and 126/310 active perks.
Wider multi-activation tied-branch/forced-walk projection is deferred Phase 2.
Full expiry and Frenzied remain Phase 1, pending the user's Morale decision.
Next unblocked Chaos base-effect candidate: Shield of Chaos, before its Paradox
Shield modifier. No graphical run or playable promotion occurred.

Source checkpoint `8c462143286f910e91eea0849afe9d83d4eb4209` is pushed and
remote-matched. The existing full Windows run `36719626047` remains live on
`63431ceb3`; it contains Misfortune/Summon Boat, not this newer Berserk slice.
Preserve it and dispatch the next source checkpoint after its terminal result;
do not restart or cancel merely because newer commits exist.

### 2026-09-30 current slice — Misfortune probability foundation

UP-061 implements the missing canonical base effect before activating its
Weaver modifier: final positive-Luck cap (negative Luck preserved), capped
SP-derived duration and favorable random creature probabilities. Shared
basis-point bonuses retain ordinary timed expiry/Dispel and append-only
serialization with loss-rejecting downsave guards. Explicit consumers cover
Death Blow, attack-triggered spells, destruction/transmutation and binomial
Death Stare; deterministic abilities, hero-owned machine chances and harmful
Fear rolls remain unchanged. Weaver subtracts ten multiplier percentage points
before the same 25% floor. AI has shared Luck and Death Blow expectation hooks.
Luna runtime/AI workers froze disjoint files; Astra review finds no blocking
source defect. Both Linux targets link after retained fixture compile
corrections; final rebuild 84281 succeeds. Native 42389 passes 25/25, zero
skips: 18 new runtime/AI/helper cases plus seven direct guards. It proves
selected/unselected Weaver, coefficient/floor, actual Death Stare, positive
versus negative Luck, legal Dispel/round expiry, v2 isolation, current/downsave
marker representation, help and accepted/read-only AI. The initial permanent
marker defect is fixed and its failure retained; the later expiry crash is
attributed by gdb to a null test assertion after correct expiry, not runtime.
Reports `UP061-misfortune-expiry-retry2-focused.log`/`.xml`; binary SHA-256
`01f92c0564da87a2d21e2a471f692f2f95c6af4ce86df7370dbddcba9589629e`.
All builds remain serialized at `-j12`. Source delivery is the next gate.
Offline gates pass 77/77 after repairing the activation allowlist/inventory;
the initial drift failures remain in the release failure register. Registration
is 126/310 active perks, 184 planned, Chaos 2/8, with Weaver's principal path
native verified. Combat identities remain 59/67 and ranks 84/93; no blanket
Misfortune effect-complete count is claimed while resistance scope is pending.

Innate creature Magic Resistance classification awaits the user's decision;
do not reduce mixed hero/aura resistance silently. Phase 2 review gaps are
effect-aware AI expectations for other favorable proc families, direct seeded
fractional-roll and Sylvan/Perfect Moment execution tests, and custom
Misfortune specialty modifiers (none configured canonically). Dedicated Weaver
art remains Not done; no GUI/profile/snapshot promotion. The canonical formula's
missing subtraction symbol is repaired from its own examples and its hash is
refreshed; this is a transcription repair, not a new balance decision.
Next highest-priority mapped Chaos work is UP-062 Berserk/Frenzied Curse:
next-activation lifetime, shooter melee and movement-cost/random-tie selection,
exact forced movement in AI and +2 Speed perk. Bad-Morale consumption is awaiting
the user's clarification; implement unambiguous clauses without inventing it.

Source checkpoint `63431ceb3cc0e216f9aff9785445e522fab7cddf` is pushed;
remote identity matches with a clean checkpoint. Full Windows run
[36719626047](https://github.com/thegandalf196/vcmi/actions/runs/36719626047)
completed successfully on that frozen source. The unexpired package artifact
`11103922205` is `New-Horizons-Windows-x64-63431ceb3cc0e216f9aff9785445e522fab7cddf`
(750719556 bytes). It contains Summon Boat/Misfortune, not the later Berserk or
Shield source. This is compile/package evidence, not graphical acceptance.
A matching newer full build should follow the reviewed Shield source checkpoint.

### 2026-09-30 next slice — Summon Boat existing-only policy

The previous cycle changed authoritative state: Hand of Fate is implemented,
native verified and pushed. Fate Dealer's two-draw distribution is not specified
well enough to choose replacement silently; the user question and policy map
are recorded in UP-060. Its base defense-unfiltered pool remains authoritative.
Continue the unblocked UP-056 Summon Boat clause instead: never create a new
boat in captured New Horizons rules, and never let Nullkiller forecast creation
that the authoritative spell rejects. Preserve legacy/custom spell behavior.
The slice is now source/native verified: client build 54426 and test build
61522 succeed. Native 83331 passes 13/13, zero skips, including the five new
runtime/actual-AI cases plus eight direct guards. Binary SHA-256
`a674e4a67a73b5cf18357ddbf4b1fafedad87fa8cc43df01eff666b69b5bc79b`;
reports `UP056-summon-boat-existing-only-initial-focused.log`/`.xml`.
All 77 offline checks and module/diff gates pass; independent source/test review
has no blocker. No failed native/build retry for this slice. No GUI or launcher
promotion. Adjacent target selection/preview remains missing Phase 1 UI, not
polish; broad occupied/multiple-boat/tie and packet-observer coverage is Phase 2.
Counts remain combat identities 59/67, ranks 84/93 and active perks 125/310:
this repairs a missing clause of an already registered Adventure identity.
Windows run 36710097476 subsequently succeeds on its frozen Hand of Fate
head. Package artifact 11096561868 is unexpired (750709876 bytes); it does
not contain this later Summon Boat slice or Misfortune. Preserve the completed
run and dispatch a new full build only after the current checkpoint is pushed.
Read-only Luna next-slice map finds a foundational Chaos gap: Misfortune still
uses legacy -1/-2 Luck, not canonical positive-Luck suppression, and favorable
creature probabilities have no shared runtime/AI policy. Its coefficient and
Misfortune Weaver's ten-point decrement are unambiguous; eligible ability rolls
must be classified explicitly. This outranks activating a tooltip-only Weaver
perk. Record the missing base mechanic in the functional ledger and use this
as the next unblocked Chaos foundation while Fate Dealer sampling is pending.

### 2026-09-30 Hand of Fate source/native checkpoint

Source commit `8473b53e169067315fbd5f637182f76ccb6d28e1` is pushed; local
and remote HEAD match. Full Windows run
[36710097476](https://github.com/thegandalf196/vcmi/actions/runs/36710097476)
is successful on that frozen source head. Package artifact `11096561868`,
`New-Horizons-Windows-x64-8473b53e169067315fbd5f637182f76ccb6d28e1`,
is unexpired and 750709876 bytes. This is Windows compile/package evidence,
not graphical gameplay acceptance or a package containing later commits.

UP-057 adds the missing Level 3 Chaos damage spell to fresh saved rules and
the content module: primary `70 + 2.5 × SP`, ordinary coefficient scaling,
uniform secondary selection across other living battlefield stacks on either
side, and a raw spill of half the primary's actual HP loss. The selected
recipient's defenses apply without reroll or repeated caster damage bonuses.
That user-approved mitigation decision is integrated into the canonical section
and summary table, with its source hash refreshed. Lua secondary resolution
retains the cast's original resistance rolls through application. AI uses a
signed expected-damage value, including friendly harm, rather than a random
stub recipient; preview forecasts only the selected primary. Dedicated spill
log entries identify the recipient and damage before/after defenses.
Luna runtime and AI workers own separate files; root owns the shared bridge,
registration and final validation. Both Linux targets build; final native gate
54761 passes 17/17, zero skips, and all 77 offline checks pass. Astra review
found no principal-path blocker. Combat identity coverage becomes 59/67,
Chaos 5/11; ranks 84/93 and active perks 125/310 are unchanged.
Borrowed Magic Arrow icons/impact remain Not done art. Fate Dealer is still
planned and is not activated by implementing the base spell.

Read-only Astra review found no blocking principal-path defect. Deferred Phase 2:
legacy Clone uses zero returned injury damage on destruction, whereas AI's
health-delta expectation currently predicts collateral; fresh NH Clone is
inactive and Phantom Army's separate Integrity path is unaffected. Explicit
Time Stop pool-preservation, caster-bonus non-reapplication, full save/load and
rendered log/impact checks remain outside the initial focused evidence. Retain
that compatibility finding rather than treating the base spell as exhaustive
cross-system certification. Initial build 2773 and failed fixture retries are
preserved in the failure ledger. Client/test retry 28001 succeeds; final
incremental build 90769 succeeds. Binary SHA-256
`3ac2c0c602cb277c228164144ff86b2d448257b45cac526294c72cccdd7c09fd`;
reports `UP057-hand-of-fate-isolated-ai-retry5-focused.log`/`.xml`.
AI debugger confirms legitimate Order competition, not missing spell admission:
Hold the Line scores 1215 versus spell candidates 852.056 and 801.586. The
submission fixture therefore neutralizes Order coefficients, without changing
production preference. Next: Fate Dealer's two-draw hostile selection, then
the next missing Chaos identity; unresolved user-design questions remain queued.

### 2026-09-30 ordinary spell acquisition policy source/native verified

Source checkpoint `8e318e78431f8e14ffe7b39e96522ccb59dbdbcb` is pushed.
Full Windows run [36703167717](https://github.com/thegandalf196/vcmi/actions/runs/36703167717)
completed successfully on that exact head. Unexpired package artifact
`11093750773`, `New-Horizons-Windows-x64-8e318e78431f8e14ffe7b39e96522ccb59dbdbcb`,
is 750694392 bytes. It contains School/acquisition corrections, not Hand of Fate.
Package publication is not playable acceptance; no launcher/profile promotion.
The preceding Archmage run [36697665400](https://github.com/thegandalf196/vcmi/actions/runs/36697665400)
completed successfully on `fffd9b81329e06bda04ec48d2253f5f4a890e0ab`.
Its unexpired Windows x64 package is artifact `11090508152` (750686084 bytes),
with matching head in its name; that package does not contain the later School
or ordinary-acquisition corrections. No launcher/profile promotion.

UP-059 adds an optional saved ordinary-acquisition marker independently of
casting availability. Fresh Master Chain Lightning remains Solmyr's castable
specialty but cannot enter ordinary learning/Guild/scroll offers; fresh
Counterspell is inactive without removing historical countering execution.
Captured profiles without the marker retain their eligibility. Adventure
acquisition is unchanged. Guild generation, shared learning and House of Wisdom
generation/purchase admission and random reward default pools are wired.
Explicit named references retain existing roster/casting semantics. Client/test
build 73711 succeeds and native 27381 passes 42/42, zero skips, on
`e5a3ed12075a54ed827d1acb60c84b2b647263528ff33fc90eb17592f068f14e`.
Reports are `UP059-acquisition-final-focused.log`/`.xml`; earlier failed compile
and fixture runs remain in the failure ledger. Offline gates pass 76/76 and
module/diff checks pass; independent review has no blocker.
Counts stay unchanged: this repairs admission, not missing spell effects.
Broad acquisition/save-world journeys and graphical acceptance remain deferred.
Next missing combat identity is Hand of Fate (UP-057), whose mitigation policy
is resolved. No GUI, snapshot or launcher-profile promotion.

### 2026-09-30 corrected fresh School classifications

UP-058 now maps Implosion to Sorcery and Earthquake to Nature in newly captured
profiles without rewriting old saved rules. Both Linux targets build (74940),
final test rebuild 76420 succeeds, and four focused native cases pass 4/4,
zero skips, on `d492ad73bae4a628efb7f91dfdf49f18328722339a55bbebbbcff61d6b23f37f`.
Fresh acquisition/rank, old Havoc world/BattleStart persistence, shared actual
casting and the corrected Archmage AI submission are exercised. Offline gates
pass 75/75; mirror and diff checks pass, no review blocker. Counts remain
125/310 active perks, 58/67 combat identities and 84/93 ranks. This does not
complete Implosion's percentage/pull or Earthquake's full effects.
Next: UP-059 ordinary acquisition exclusions, then Hand of Fate (UP-057).
No launcher, gameplay profile or GUI changed.

### 2026-09-30 Archmage implementation and focused validation underway

Final checkpoint: client/test build 22317 and final test-only build 13005
succeed. Native 18779 passes 24/24, zero skips, on
`8e2222981acf90654d38166321ece81af245860deaf55a38680af0cc10dece52`.
The stale-dead request guard is verified, both authoritative spell levels and
actual detached-AI submission pass, and all failed attempts remain recorded.
Coverage advances to 125/310 active perks, 185 planned, Wisdom 7/3; ranks and
combat identities unchanged. Offline/mirror/diff checks pass; no review blocker.
This supersedes the earlier in-progress evidence below, not its failure history.
Next: UP-058 School assignments, then UP-057 Hand of Fate with the approved
secondary-recipient mitigation decision. No launcher or profile promotion.

Source delivery: `fffd9b813` is pushed and remote equality was verified with
a clean worktree. Windows run `36697665400` is queued on this exact source.
The preserved prior run `36691148552` succeeded on `1f8177b97`; its unexpired
Windows package is artifact `11087514647` (750678892 bytes). Preserve that
successful payload while the newer build runs; no graphical acceptance.
UP-058 now owns only fresh School data and focused fresh/old snapshot tests;
root retains generated module, documentation, builds and Git integration.

Independent runtime/AI workers implemented UP-055 and froze production files.
Accepted hero casts record exact saved levels 1–5; the first Level 4 or 5 uses
one shared discount after Wisdom/Prepared Caster, minimum one Mana. UI and AI
read the same cost. The per-side history survives rounds and current saves,
older loads default to zero, and lossy down-saves reject nonzero history.
Client build 43488 and test build 78105 succeed. Offline gates pass
74/74 and module/diff checks pass. Independent review has no production blocker;
the two fixture mistakes recorded in the failure ledger were corrected before
test compilation. Initial native execution passes seven cases then crashes on
a Defend request for a dead active stack. Gdb confirms the live-stack admission
hole before StartAction. A bounded authoritative guard, regression, and surviving
cross-round fixture are being repaired; completed coverage increase remains pending.
Broader Counterspell/resistance/Metamagic interactions, full save-world journeys
and playable acceptance remain Phase 2. Old pre-mask battles cannot reconstruct
completed levels from the start-of-cast history; the zero migration is explicit.
Next bounded missing-spell map: Chaos Hand of Fate (UP-057), without source
writes during the frozen build.

### 2026-09-30 Arcane Memory source verified; activation policy pending

The seven-file provenance/completion implementation builds client and test
targets (4257). Nine feature cases and two direct guards pass 11/11, zero skips,
on `7efa81f126a237daaf9a48bb0e47382b1de7aa9e26036a8e2de86df7f272b9bc`.
Both initial failures and successful repair evidence remain in the failure
ledger. Production activation remains planned until neutral Adventure learning
policy is answered. Explicit test-only activation preserves feature verification
without publishing an unresolved acquisition rule. Final build 89441 succeeds;
native 18008 again passes 11/11, zero skips, on
`1928e181a8d676e4e9fcf8a0c5dceff75c7c8c0f194de4d963fb6f1f1d7f7002`.
74 offline cases and module/diff checks pass; final review has no blocker.
Coverage remains 124/310 active perks, not 125 completed. No launcher promotion.
Next unblocked foundation: canonical Town Portal effect/shared AI policy (UP-056);
Archmage's map (UP-055) remains available. Five Adventure identities/acquisition
are registered, but all five retain missing canonical effect clauses, recorded
individually in UP-056. This is Phase 1 missing functionality, not Phase 2 polish.

Town Portal's bounded map confirms the existing deterministic squared-distance
resolver can be retained. Occupied-nearest cancellation must not become a
farther-town fallback. Shared runtime/AI destination and Movement policy is
missing; owner-versus-team towns and the legacy minimum Movement threshold are
now explicitly awaiting user clarification. Archmage UP-055 remains the next
unblocked implementation; do not stall the whole Phase 1 queue on these choices.

Historical correction evidence:

Source checkpoint `1f8177b97a5bcc81ff0fbe6b6846088c4deee770` is pushed,
with a clean worktree at delivery. Full Windows build `36691148552` is queued
for that exact source:
https://github.com/thegandalf196/vcmi/actions/runs/36691148552
Dispatch/queue is not build or package success. Preserve the earlier successful
Prepared Caster payload while this run is pending.

Repaired client 57887 and test retry 28356 build. The first isolated native
slice 94687 passes four of six cases, zero skips, on binary
`49c29fdd1feeba5b216e9092e6ae21d153187ac5d5af609f9c46044b9cf8d42c`.
The run exposes an incorrect charge-only implementation assumption: ordinary
scrolls are reusable, while the canonical perk learns from accepted scroll
casts without requiring consumption. Repair source classification and retain
ordinary scrolls; preserve authored charge costs for actually charged sources.
The second rejected Haste fixture action also needs diagnosis. Native reports
and the first fixture compile failure are retained in the failure ledger.
No verified coverage increment or feature-delivery claim is made.

The six-file runtime's pre-effect source snapshot remains necessary to avoid
Town Portal/Guild source substitution. Neutral Adventure acquisition through
Arcane Memory awaits clarification; fixed Guild unlocks remain a separate
canonical rule. The four legacy Tomes are deliberately excluded pending
authored replacements, not a four-to-six-school remapping defect. A bounded
read-only Archmage map is complete (UP-055); implementation has not started.

### 2026-09-30 Windows Prepared Caster package checkpoint

Full run `36680827103` succeeds on frozen `2b5a843d7d10ae68f8e53d40ee962fb27f4f72b9`.
Artifact `11082744152` is the 750666994-byte unexpired Windows x64 package;
its exact name is `New-Horizons-Windows-x64-2b5a843d7d10ae68f8e53d40ee962fb27f4f72b9`.
This includes Combined Arms, Mysticism and Prepared Caster, not subsequent
Meditation, Deep Knowledge or Arcane Reservoir. Build/package success is not
graphical gameplay acceptance. Preserve this terminal success and its payload;
dispatch the next full build at the next completed source checkpoint.

### 2026-09-30 Phase 1 native checkpoint — Wisdom Arcane Reservoir

The Expert perk adds 25 Maximum Normal Spell Points after Knowledge and
Intelligence rounding, without refilling current Mana or touching Buffer.
Saved active selection/current Expert rank gate it; existing rank-loss events
clamp Normal only. All ordinary capacity readouts and AI capacity consumers use
the same getter. The Tower building's Buffer grant is unchanged. No new saved
state, cache or polling was added.

Client build 7727 and test build 86291 pass. Native 40452 passes four new cases
plus 27 direct capacity guards, 31/31, zero skips. Binary SHA-256
`4c55d6c999d3a0e64d6982e5403e4f182f5ff6d89f78614a82e2b390e141c3b3`.
Reports: `NewHorizonsArcaneReservoir-capacity-guards.log`/`.xml`.
Offline gates pass 74/74 and mirror/diff checks pass; independent review has no
blocker. Coverage is 124/310 active perks, 186 planned, Wisdom 6/4. Ranks 84/93
and combat identities 58/67 remain unchanged. Integer saturation is reviewed;
the validated fixture cannot reach overflow, so no such runtime case is claimed.
Broader interactions, bespoke art and rendered/playable acceptance remain open.

Next: Arcane Memory (UP-054). Trace actual completion rather than treating an
adventure Boolean or initial packet as success, especially deferred queries.

Source delivery: `bccb3bd16` is pushed with matching branch identities and a
clean source checkpoint. Windows run 36680827103 still builds frozen Prepared
Caster `2b5a843d7`, not this newer capacity perk; no new package is claimed.
UP-054's completed map identifies a generic post-success adventure environment
notification plus the existing accepted combat charge helper as the shared
Arcane Memory boundary. No new saved counter is needed. Subsequent review
requires capturing the actual source before adventure effects: Town Portal can
otherwise teach the spell at its destination before the completion scan. That
repair is in progress. Neutral Adventure Spell permanent acquisition through
Arcane Memory also awaits user clarification against fixed Guild unlock rules;
see UP-054. Client session 10614 passes the initial slice, not the later repair.

### 2026-09-30 Phase 1 native checkpoint — Wisdom Deep Knowledge

The shared growth view raises only Wisdom's existing chance by ten percentage
points for a captured active selection/current rank: Advanced 30%, Expert 40%,
saturating custom chances at 100%. Actual rolls and growth-window percentages
use that same view. Fixed class growth, independent draw order/count and legacy
profiles are preserved. New selections affect later rolls, not the primary
roll preceding the current perk query. No new saved field or AI roll path.

Client retry 98557 and test build 8638 pass. Native retry 96534 passes four new
cases plus nine direct growth guards, 13/13, zero skips. Binary SHA-256
`c9b9cdfd304e9b9db3ef679da3d3d13352a73af892f519d88084d97c3dccac88`.
Reports: `NewHorizonsDeepKnowledge-retry1-growth-guards.log`/`.xml`.
First failed run 77666 and its fixture repair remain in the failure ledger.
Offline 74/74 and mirror/diff checks pass; independent review has no remaining
blocker. Coverage is 123/310 active perks, 187 planned, Wisdom 5/5; ranks 84/93
and combat identities 58/67 remain unchanged. Strategic acquisition valuation,
broader interactions, bespoke art and rendered/playable acceptance are deferred.

Next unblocked candidate: Expert Wisdom Arcane Reservoir's flat 25 normal
capacity, distinct from the Tower Buffer-Mana building (UP-053).

Source delivery: Deep Knowledge `a827bbb7b` and Meditation `d023766f9` are
pushed, with matching branch identities and a clean source checkpoint.
Windows run 36680827103 is still compiling frozen Prepared Caster `2b5a843d7`;
it does not contain these two newer perks. Preserve that live run. No new
Windows package or playable promotion is claimed for the current source.

### 2026-09-30 Phase 1 native checkpoint — Wisdom Meditation

Implemented additional daily Normal recovery from the previous day's unspent
Movement, with initial-day exclusion, additive regeneration, capacity cap and
unchanged Buffer. Pooled heroes use the pre-expiry Movement maximum before
daily refresh; no polling or new saved marker. AI heroes use the same passive
daily event. Strategic reservation of Movement remains Phase 2.

Client build 35691 links successfully and a follow-up build exits zero; test
build 88236 passes. Native 84667 passes all five new cases plus 22 capacity
guards, 27/27, zero skips. Binary SHA-256
`280e5b226f1cb9fb651e64ad0fc9067581c25c4c25793729d01d495054c99530`.
Reports: `NewHorizonsMeditation-capacity-guards.log` and `.xml` in the isolated
runner. Offline gates pass 74/74, mirror/diff checks pass, independent review
has no blocker. Coverage becomes 122/310 active perks, 188 planned, Wisdom 4/6;
ranks 84/93 and combat identities 58/67 are unchanged. Broader interactions,
bespoke art and rendered/playable acceptance are not claimed. No promotion.

Next: Deep Knowledge modifies the shared Wisdom level-up chance consumed by
authoritative rolls and hero-screen forecasts, preserving draw count/order.

### 2026-09-30 Phase 1 native checkpoint — Wisdom Prepared Caster

UP-050 adds the combat-lifetime accepted-hero-cast foundation, shared cost
discount and detached AI state. The first hero spell receives two Mana off
after Wisdom, minimum one; Overcharge surcharge and Empower eligibility remain
separate. Creature/rejected attempts and previews do not spend the discount.
The state persists across rounds, save/load and nested projections, with an
append-only version and downsave loss guard. Ordinary spellbook/affordability
already use the same callback. Generic perk offer/help exists; bespoke art does
not. Existing histories are not repurposed because they record action start.

Both Linux targets build (55809; final test-only rebuild 56500). All ten new
runtime/actual-AI cases pass, zero skips, on binary
`ea8e481c14da2395f288408bece79ae470d0d2ad9534398c57e1bb37f5e815a0`.
The expanded 31-case filter passes 30/31: one unchanged legacy-v2 synthetic
fixture retains v3 Quicksand `selectedPlacement` and is rejected during setup.
That helper migration, direct Adventure exclusion, broader interactions and
the approved old-load false boundary are tracked for Phase 2. Keep the failing
and succeeding reports. Offline checks pass 74/74; review has no production
blocker. Coverage increases to 121/310 active perks, 189 planned; Wisdom 3/7.
Ranks remain 84/93, combat identities 58/67. No launcher promotion.

Next unblocked slice: Meditation. Its daily map is complete, including first-
day exclusion and the tavern pool's Movement-before-Mana ordering. Use explicit
completed-day context and previous Movement; preserve Normal/Buffer and rest
precedence. Diplomacy and the recorded scope questions remain parked, not
silently decided. Source delivery and the next Windows batch are separate gates.

Prepared Caster source is committed and pushed as
`2b5a843d7d10ae68f8e53d40ee962fb27f4f72b9`; local/remote identities match,
with a clean worktree at that checkpoint. Full Windows run `36680827103` is
queued on that exact source, including Combined Arms and Mysticism; no new
package pass is claimed from dispatch. Preserve that handle. Meditation now
has separate runtime/test ownership. Pool eligibility uses a previous-Movement
maximum snapshot before bonus expiration without changing legacy daily
restoration ordering or adding saved state. Its active coverage is not yet
claimed.

### 2026-09-30 Windows Command package checkpoint

The preserved full Windows run `36672365779` finishes successfully on frozen
source `dc50b5353ceb86d8800eac9e162c69ad324ed4d6`.
Package artifact `11081176965`,
`New-Horizons-Windows-x64-dc50b5353ceb86d8800eac9e162c69ad324ed4d6`,
is available (750,646,843 bytes, not expired at verification). This proves
Windows build/package delivery for the Command efficiency checkpoint, not
Windows graphical acceptance. Combined Arms, Mysticism and Prepared Caster
postdate this frozen source and are not present in this package. Do not restart
the successful handle or describe it as containing the latest working tree.

### 2026-09-30 Phase 1 native checkpoint — Wisdom Mysticism

UP-049 implements the missing Basic perk through the existing daily recovery
getter and authoritative `SET_NORMAL`. Recovery is a floor of the greater of
5 or floor(10% normal maximum), fills only missing Normal and leaves Buffer
unchanged. Existing stronger regeneration and Mage Guild rest retain precedence.
Captured active selection/rank gate the effect, preserving planned snapshots;
no new persistent field, polling or scheduler. Generic AI acquisition and daily
application already exercise this passive; strategic acquisition ranking remains
Phase 2. Canonical help text is retained and bespoke art is Not done.

Linux client build 55027 and final test build 92352 pass; six new cases plus
30 directly relevant pool/capacity guards pass together, 36/36, zero skips.
The real daily packet, Wizard offer selection/save-load, planned snapshot,
rank removal, percentage floor/cap, Buffer and rest precedence are checked.
Binary SHA-256 `0b565de19b837c0f2a3bc476c59009f61c99f570ba15c507d3737df7912be080`.
Offline checks pass 74/74; mirror/diff checks pass. Independent review has no
blocking finding. Coverage is 120/310 active perks, 190 planned, Wisdom 2/8;
combat identities remain 58/67 and ranks 84/93. Broader interactions,
rendered/playable acceptance and art remain deferred; no launcher promotion.
The next unblocked candidate is Prepared Caster, with a shared first-accepted-
combat-spell state/cost map underway. Diplomacy still awaits the authored-free-
joining answer. Preserve Command Windows run `36672365779`.

Mysticism source is committed and pushed as `c03505830`; this is not a playable
promotion. Prepared Caster's read-only map is complete (UP-050). Its shared
cost callback already feeds the ordinary combat spellbook through
`CGameInfoCallback::getSpellCost`; no parallel UI calculator is needed. The
missing foundation is a combat-lifetime accepted-hero-cast state shared by
authoritative packets, saved sides and hypothetical AI. Per-round counts and
StartAction history are not substitutes. Define that API before parallel
runtime/AI edits; preserve creature/rejected-cast and old-save boundaries.

### 2026-09-30 next coverage slices — Diplomacy and Mysticism

UP-048's runtime and AI/UI maps plus independent policy review establish that
ordinary Diplomacy still uses legacy disposition. The canonical paid thresholds
are clear, but authored `COMPLIANT` free joins need a migration decision; the
user has been asked whether to preserve those exceptions. An explicit eligibility
marker avoids reinterpreting `HOSTILE`/`SAVAGE` disposition as a prohibition.
No Diplomacy activation or coverage increase is claimed. Existing accepted
joining/garrison removal behavior must not be silently redesigned.

Continue UP-049, Wisdom's missing Mysticism perk, through the existing daily
Normal-Mana recovery event. This is not polling, a new currency, or Buffer refill.
Separate focused principal-path evidence from playable/rendered acceptance.
The Command Windows run `36672365779` remains live on `dc50b5353`; preserve it.

### 2026-09-30 Phase 1 native checkpoint — Command component-specific perks

UP-044 implements Aggressive Commander, Defensive Commander and Veteran
Commander. This opens ordinary Advanced and Expert Command progression,
currently blocked by absent active Basic/Advanced perks. Runtime owns the
shared Order coefficient and focused server
fixture; AI owns its consumer trace and focused native fixture, with no
duplicate scaler. Keep rank efficiency and additive Warcasting points, add
20 efficiency points only to the matching Attack/Defense component, and leave
flat bases unchanged. Veteran adds +25 points only to Leadership-derived
terms, not to Leadership capacity. Root owns the
three registry activations, module mirror, test registration, inventory and
integration. Both Linux targets build; 11/11 focused runtime/progression/AI
cases pass with zero skips. Content/perk/inventory checks pass 74/74; mirror
and diff checks pass. Coverage is 58/67 combat identities and 118/310 active
perks; existing Command Order guards additionally pass 13/13, zero skips.
There are 192 planned perks, with Command 3/7 active/planned. Bespoke art is Not done;
generic neutral fallback is not art. Binary SHA-256:
`e228836aac3189c35ed63b803c2facd57ec22b5c006161537054ee860a13a2a3`.
No launcher promotion or broad suite after this bounded feature.

Production source review has no blocking finding: bonuses are source-specific
efficiency points, flat bases/capacity are untouched, AI uses the same helpers,
and the generic legacy bonus path excludes new perks. Deferred Phase 2
compatibility: legacy contextual Focus Fire still calls the public coefficient,
so a synthetic old-command/new-active-perk-registry hybrid could gain Aggressive
scaling; ordinary historical saved perk registries keep these perks planned.
Actual AI fixtures isolate each Order's shared coefficient consumer with a
legal Magic Arrow competitor; all-canonical-Order tactical ranking and AI
Warcasting interactions remain Phase 2. Runtime Warcasting/snapshot checks pass.
Source/native evidence does not establish rendered/playable acceptance.

Source delivery: committed and pushed as
`fcecc23d3d72ac6c67fd354bf8b2bfcb26234a5d`; remote identity verified.
Full Windows run `36672365779` is pending on documentation checkpoint
`dc50b5353ceb86d8800eac9e162c69ad324ed4d6`, containing that source.
It is queued behind the live Blink run `36670136812`; neither is restarted or
cancelled. Dispatch/queue state is not compile/package or playable evidence.
Next unblocked coverage slice: Command's Combined Arms, after the read-only
damage/admission/AI map. Confusion still awaits the two recorded design answers.

### 2026-09-30 Phase 1 in-progress slice — Combined Arms

Final native checkpoint: the bounded slice is implemented and independently
reviewed with no blocking finding. Both Linux targets build; final test-only
rebuild 11676 passes. Five focused runtime/actual-AI cases and 37 direct
Command/Focus Fire guards pass, zero skips, plus 74 content/perk/inventory
checks and mirror/diff checks. Binary SHA-256:
`9100b7e059bbe7822bc1b8df362b444a95e660f672ea40864ce35dc65bac2a5d`.
The exact 5,375 endpoint passes. Both actual-AI fixtures now explicitly isolate
other Order coefficients with legal Magic Arrow competition; Flank's army is
shooter-only. All-Order ranking, inherited Flank reachability/remaining-activation
valuation, broad interactions, bespoke art and rendered/playable acceptance
remain deferred. No gameplay scores were tuned to force fixture selection.
Coverage is now 119/310 active perks, 191 planned, Command 4/6 active/planned;
58/67 combat identities and 84/93 active ranks are unchanged. No launcher
promotion. Initial failures remain in the failure ledger and isolated reports.
The source map and earlier in-progress evidence below are chronological records,
not claims that the native gate is still pending.

Source delivery: `25bd4b08219fd9ff25cbf541a4b1c7f32bd164c1` is committed
and pushed with matching remote identity. All checkpoint source changes are
committed; no unrelated dirty files are left. UP-047 records the next Command
perk's recipient-scope question; while that and UP-046 remain unanswered,
continue an unblocked missing specification item rather than inventing rules.

Windows status: Blink run `36670136812` succeeds on frozen source
`d6f976a1b4b071768172c18003a942adc760f888`, downloadable artifact
`11079313586` (`New-Horizons-Windows-x64-d6f976a1b4b071768172c18003a942adc760f888`,
750649638 bytes). That package does not contain Command efficiency or Combined
Arms. Command run `36672365779` is now in progress, not a package pass yet.
Combined Arms Windows compilation and playable acceptance remain unverified;
preserve the existing job rather than restarting it for this new source slice.

UP-045 has bounded runtime and AI workers with separate file ownership; root
owns registry, validation and integration. Coverage remains 118/310 active
perks until the focused execution/build gate passes. Actual damage and AI share
`CBattleInfoCallback::calculateDmgRange`; canonical Flank uses the direct Order
damage payload, while Focus Fire currently uses a separate ranged-only premium
and penalty flag. Do not reuse that flag for melee. The direct damage payload
is currently integer-valued; preserve fractional half percentages through Lua
until final damage rounding, without changing serialized Order identifiers or
state unnecessarily. Flank's ranged extension excludes its flat base and
distinct-side additions. Focus Fire's melee extension excludes shooter-only
Target Caller additions and range/obstacle benefits.

Admission also needs coverage: `battleCanConfirmHeroCommand` currently requires
a legal shooter for Focus Fire. The perk must make its newly useful melee army
composition eligible without weakening target/owner/ordinary-unit validation.
Flank's `isMeleeAttacker` predicate already returns true for ordinary shooters
(`Unit.cpp:86`); the read-only map initially misinterpreted its name. No new
shooter-only Flank admission gap is claimed: preserve and test it. Actual side
recording already excludes ranged attacks in BattleActionProcessor; retain it.
AI's canonicalOrderHeuristic needs the same exact half-component helpers and
known-allied-perk checks; do not consult concealed opposing heroes. Validate
target scope, physical-only damage, legal perk progression, round expiry,
fractional damage, unchanged base/side bonuses and actual AI submission with
focused tests. No source or execution completion is claimed by this map.

Source integration checkpoint: runtime and AI workers are frozen; independent
review finds no remaining blocking production issue after repairing the
canonical-only AI gate. The first Linux build (90955) fails on raw-pointer
deduction for a shared callback; root repairs it and incremental build 3217
is running. Content/perk/inventory passes 74/74 and mirror/diff checks pass.
No native execution gate or coverage increase is claimed yet. The two actual
AI fixtures explicitly isolate competing Order coefficients and do not certify
all-Order ranking; the Flank fixture includes a melee ally, so selection is not
uniquely attributable to the new ranged heuristic. Add a hand-derived fixed
Angel endpoint before closing: NH suppresses passive hero Attack inheritance,
so creature Attack/Defense remain 20/20; 100 Angels at 50 damage plus the
7.5% half-snapshot bonus yield exactly 5,375, not the legacy-derived 17,125.
This checks fractional preservation beyond same-engine projection parity.

### 2026-09-30 read-only gap map — Commanding Presence

The Advanced Command perk is still planned/data-only. Shared
`moraleValAndBonusList` already supports a zero `MINIMUM_MORALE` floor;
authoritative activation and detached AI forecast consume that shared value.
Canonical Orders use state rather than broad stack bonuses; projected
`setHeroOrderState` does not currently change morale. A shared active-recipient
predicate is required before implementing the floor and AI valuation. Resolve
whether "currently affected" means every eligible stack covered by a
conditional standing Order or only its explicit recipients (especially Protect
and Second Wind). No edits, builds, tests, or activation are claimed by this
read-only map. Do not silently apply a whole-army aura to targeted Orders.

Read-only worker map complete. The differing canonical wording resolves the
component choice: Focus Fire's half includes its own flat base and Attack term;
Flank's half explicitly excludes the flat base. Preserve existing Focus Fire
snapshot values without a new save field where possible. Broadening admission
for melee-only Focus Fire is required to exercise the perk,
not permission to relax ownership, target or normal action restrictions.

### 2026-09-30 foundational gap map — Elemental Rebirth

Read-only Luna exploration confirms the Conflux Skill assignment exists, but
none of the three rank effects or ten perks has a runtime/AI implementation.
Do not count class assignment, metadata or art as completion. Base ranks need
a shared pre/post-death reaction for physical attack and spell-injury packets,
exact-health temporary Elemental spawning and a detached AI projection.
`CGameHandler::sendAndApply` already provides post-damage reaction seams;
`GameStatePackVisitor` has pre/post death tracking; `UnitInfo`/ADD already carries
temporary summon provenance. Original same-stack REBIRTH is not a substitute.
The missing UI hook is passive summon/result feedback, not another Hero Action.

UP-046 records a material question: does maximum aggregate HP mean battle-start
stack capacity or remaining creatures' capacity immediately before the fatal
hit? An asynchronous user question is pending. Later perks need serialized
Rebirth origin/original-HP and once-per-combat state, plus terrain candidate sets
that distinguish Adaptive Element from Perfect Convergence. No source changes
or coverage increase are claimed. Continue unblocked coverage while awaiting
the HP-basis decision rather than inventing an answer or stopping the whole goal.

### 2026-09-30 next-slice read-only map — Confusion and Confounder

UP-043 records the canonical Level-1/5-Mana forced-next-activation spell.
Runtime mapping completed without edits: BattleFlowProcessor automatic actions
and ordinary action validation provide execution; shared callback reachability
provides legal attacks/movement; CUnitState save/load and UnitChanges carry
pending/history state; hypothetical AI and PotentialTargets need a shared
expected-outcome path. Do not reuse Berserk's ally targeting or nearest-target
choice. Two user questions remain pending: impossible behaviors and the
Confounder sole-legal-result fallback; consumption when Morale/Berserk already
uses the activation. Preserve Time Stop's nonactivation behavior. No production
Confusion implementation or coverage increase is claimed. This ambiguity
does not block another unblocked Phase 1 item.

### 2026-09-30 Phase 1 in-progress slice — Chaos Blink and Blinkmaster

Source delivery: committed and pushed as
`d6f976a1b4b071768172c18003a942adc760f888`; remote identity verified.
Full Windows preview [run 36670136812](https://github.com/thegandalf196/vcmi/actions/runs/36670136812)
is live on that exact source (`preflight_only=false`). Dispatch is not a
Windows compile/package pass. Poll this run without restarting for a timeout;
no Linux launcher snapshot promotion. Hydra's preceding full Windows run
36665665686 succeeded and its artifact remains separate.

Final source/native gate: client/test targets build; the isolated refreshed
Blink filter passes 12/12 and focused immunity/Entangle guards pass 24/24,
zero skips. Final test binary SHA-256 is
`d5e161815ab6ab3ce33c82a43b9de49ebe5962d9fb7f32f071df1950653baa68`.
Actual AI submission and legal authoritative resolution pass with ordinary
Orders enabled; live position, health, Mana and RNG remain unchanged during
evaluation. No production scoring boost was used to repair the fixture.
Content/perk/inventory checks pass 74/74; UI source, mirror and diff guards
pass. Independent review has no remaining blocker. Coverage rises to 58/67
combat identities, Chaos 4/11, perks 115/310. Full save/load, wider status/
obstacle interaction, incoming ranged/Mirror AI valuation, tactical quality,
hover legibility and rendered/playable acceptance remain Phase 2. No launcher
promotion. Next unblocked missing identity: Confusion with Confounder.

UP-042 is the next unblocked missing canonical spell while Nature's Wrath and
Elemental Convergence await recorded design answers. Reuse teleport/relocation
authority and share legal radius/footprint geometry with UI and AI. Runtime,
client hover preview and bounded expected-value AI have separate worker-owned
files; root owns registration, original Provisional art and validation. The
content/perk/inventory suites pass 74/74 with Blink's school/cost/single-target/
no-mass and native asset-size assertions. This is registration evidence, not execution.
Preserve source checkpoint `ccd30f0ef` and live frozen Windows Hydra
run `36665665686`; no implicit launcher promotion or coverage increase.

Initial independent source review finds no blocker in the currently present
geometry, runtime/Lua, registration and client preview; AI and native fixtures
were not yet present and are not covered by that review. Phase 2 feedback
finding: an empty legal landing set is correctly rejected before cost, but
the client preview returns `nullopt` before its specific zero-destination
explanation, leaving generic invalid-target feedback. Keep this diagnostic
specificity and native-resolution hover-text length as deferred UI work.

Native-tester delegation was rejected by the agent service's thread limit;
reactivating the completed Luna UI worker was also rejected. Cancelling the
unused pending Verdant AI thread did not release capacity for a retry. Root
will therefore own focused native execution after the two implementation
workers freeze and both targets build; do not pretend a tester was spawned
or run stale binaries. The independent source reviewer did run.

The first incremental Linux client build (`vcmiclient -j8`, session 12600)
finishes with exit 0 after runtime/AI/client production files are explicitly
frozen. It compiles the helper, spell mechanics, Lua bindings, evaluator and
hover consumer and links the facade/client. Native fixtures are still being
completed in separate files, so this is not yet a focused execution pass.

Completed AI review finds no production blocker. Root repairs two validation
defects before retry: the RNG-saving fixture's accidental const pointer and
the equal-distance endpoint assertion's vector/hex-order mismatch. Retain the
failed test-build session 35688 in the release ledger. Phase 2 AI work:
incoming ranged pressure and hostile resistance/mirror outcome valuation;
current scoring is a bounded direct-position heuristic over exact endpoint
weights, not an exact full-combat expectation.

Latest continuation: clean build session 10235 links both client and test
targets. Binary `b59553d04e8f2984ba9b7049258e09100739980bdd4454b55057666cc17d4f8e`
passes all ten Blink rules/runtime cases and 24 focused existing immunity/
Entangle guards, zero skips. Both AI submission tests still select an Order,
including the revised shooter-escape fixture. The AI worker is resumed for
bounded ranking/fixture diagnosis; do not weaken the required actual Blink
submission or count this candidate as verified coverage. Content/perk/inventory
checks pass 74/74; UI source, module mirror and diff checks pass. Full Windows
Hydra run 36665665686 remains live; no restart or launcher promotion.

### 2026-09-30 Phase 1 source/native checkpoint — Hydra's Vitality

Source committed and pushed as `75c8aea71b8c4be48d561d727a897ee88d62c9fb`;
remote branch identity was verified and the worktree was clean. Full Windows
preview [run 36665665686](https://github.com/thegandalf196/vcmi/actions/runs/36665665686)
is queued on that exact source (`preflight_only=false`). Poll this same run;
dispatch is not a Windows compile/package result. Do not cancel/restart it
merely because an observation times out. No Linux launcher snapshot promotion.

Delivery update: full Windows run 36665665686 completed successfully. Client
compilation, runtime staging and packaging pass; downloadable artifact
`11076608841` (747899018 bytes) contains frozen source `75c8aea71`.
This establishes Windows compile/package delivery, not graphical gameplay
acceptance. The active Blink source changes are not in this Hydra artifact.

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

Next-slice read-only map: Elemental Convergence is unregistered, with a clear
Level-5/22-Mana exact-HP summon path (`250 + 5 × SP`) reusable from Trolls.
Elemental Conjurer's existing planned entry specifies +30% pool and +2
Initiative in the first battlefield round. Runtime can share a typed mapping
from resolved terrain/battlefield, Lua chosen-hex spawning and exact wounded
count; AI owns location enumeration/projected summon valuation; UI extends the
currently Troll-specific preview to dynamic creature/count/HP/footprint.
Design questions remain: Dirt/Sand/Swamp are absent from the terrain table,
magical overlay precedence is undefined, and Conflux's actual native Grass
conflicts with the table's Conflux-to-Magic example. Two non-blocking user
questions request Earth/Dirt+Sand and Water/Swamp defaults, plus magical-overlay
and Conflux-town precedence. Do not silently choose these or implement a
random/generic elemental substitute. Until resolved, select another unblocked
missing canonical item; preserve the clean Hydra delivery checkpoint.

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
