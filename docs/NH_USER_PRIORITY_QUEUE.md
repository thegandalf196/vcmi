# User-priority queue

User-established priority, 2026-09-24: persist newly assigned tasks here and
resolve them before resuming ordinary New Horizons implementation. Read this
file on every work resumption. Do not remove unfinished entries or equate an
implementation with a verified fix in the user's playable version.

Statuses: Open; In progress; Implemented (verification pending); Verified
(delivery pending); Resolved. Record blockers explicitly. Preserve resolved
entries and their validation/delivery evidence.

## UP-140 — Discipline Steadfast

Next independent read-only preparation: UP-141 Miracle Worker, below. It must
not mutate the frozen Steadfast candidate or replace its native acceptance.

Status: Verified (committed/pushed; playable delivery pending), 2026-10-02. Basic perk:
Morale penalties applied by enemy effects are reduced by1, to a minimum penalty
of0. Identify source/controller provenance and the shared live/detached Morale
calculation; do not reduce army composition, artifacts or friendly self-penalties
merely because they are negative. Production/config/activation remain unchanged
until root selects a faithful rule from evidence. Focused validation and minimum
AI hooks are required; no repeated map of already blocked Discipline perks.
Implementation checkpoint: root selected a limiter-applied unstacked query
cached under the existing bonus-tree version, with target-relative
`Bonus::appliedByEnemy` provenance captured on application. This is distinct
from dynamic aura `bonusOwner`. Duration-only refresh retains original value
and attribution; Hypnotize does not rewrite historical application hostility.
Four bounded Luna lanes own the query foundation, runtime, AI and focused
fixtures. Root owns binary/JSON/schema, registration, builds and Git. Same-key
friendly/hostile penalties must be transformed before winner selection.
Source is in progress; registry remains planned and counts are unchanged.
Source/fixture freeze checkpoint: independent review reports no remaining
blocking issue after preserving repeated Bonus pointer identity through live
attenuation and AI capture/refresh/aging. Runtime and detached paths retain
`ALWAYS` stacking and branch isolation. Both-target client/vcmitest build9276
is running with12 jobs; exact log is
`build/new-horizons-linux/testing/UP140-build.log`. Re-poll that handle before
running native acceptance or starting another build. Data/schema/inventory36/36
pass. Registration remains planned until native acceptance. Phase2 retains
the existing Hypnotize/inherited-aura ownership interaction, reflected/refresh
spell matrices and broader full-save integration. No playable promotion.
Build9276 is terminal failure: recorder's base interface lacks battleGetOwner.
Root corrected its constructor/member to the CBattleInfoCallback already
provided by live and projected mechanics. Retry/native acceptance are pending;
do not execute the stale test binary or mark activation from the initial build.
Exact retry handle29668 is live for both targets with12 jobs. Log:
`build/new-horizons-linux/testing/UP140-build-retry.log`. Re-poll that handle;
an observation timeout is not a reason to restart it.
Retry29668 is now terminal: the log reaches636/636 linking vcmitest and both
executables exist; no build process remains. A reused Luna tester owns the
sequential13-case principal and9-case adjacent native checks. No activation
or native-pass claim until those exact results return.
First native acceptance: principal13 runs9pass/4fail, adjacent9 runs4pass/5fail,
zero skips. Three principal expectations conflict with the active global Morale
cap; aura provenance needs investigation. Adjacent No Quarter fixtures use an
obsolete acquisition shortcut and fail the earlier-perk gate. Separate Luna
owners repair only the Steadfast and No Quarter fixtures; do not loosen production
validation or activate from partial passes. Rebuild/retest remains pending.
Aura tracing identifies a production initialization-order defect for packet-added
base-null stacks, not just a fixture expectation. Root reverses creature/army
attachment order so OwnerUpdater receives the owned stack context. Require
friendly and enemy native aura verification alongside the cap fixture repairs.
Fixture repairs are frozen, including legal double-wide friendly-dragon geometry.
Both-target rebuild76129 is live with12 jobs, logUP140-fixture-rebuild.log.
Re-poll that exact handle before executing14 principal cases and the focused
adjacent No Quarter/Standard Bearer filter; no parallel build or stale binary.
Latest checkpoint: rebuild76129 exits0. Principal14/14 passes in3.155s with
zero skips. Adjacent9/10 passes; remaining whole-battle roundtrip hits existing
Veteran damage-history serialization rejection (CStack binary omits CUnitState),
tracked Phase2 rather than silently dropping the failing result. Root activates
Steadfast, updates inventory and generated module:174/310 active,136 planned,
Discipline7/10; ranks84/93 unchanged. Data36/36, module drift and activated
both-target build pass. Frozen activated23-case bounded gate and review pending.
Purpose-made art Not done, generic UI Provisional; no immutable playable promotion.
Activated final gate passes23/23 in5.834s, zero skips. Reviewer reports no
blocking finding. Test binary SHA-256:
5413ec74489a3f1f5af9c1e7e132e77e639c78e79c78a6164b9d080cdb9afd4b.
Full-battle serialization failure remains explicitly deferred. Source commit/push
is next; rendered and immutable playable delivery remain separate.
Source delivered as be569afa4e2d9a3a4c1c47236bb86be3975f6340 on
origin/definitive-mvp; push exits0. Phase1 moves next to UP-142's accepted
effective-Order-lifetime rule and canonical integration. UP-141 still awaits its
casualty-rounding answer. No new local playable snapshot or Windows package is
claimed for be569afa4.
Map complete: shared battleGetMorale feeds live and detached AI. Generic Bonus
source/SID does not capture serialized applying side; Shield of Chaos can
penalize friend or foe, so blanket negative-Morale or SPELL_EFFECT attenuation
is wrong. Sorrow/Doom are hostile spell producers; No Quarter has a custom
marker but no issuer side. Fear uses FEARFUL rather than MORALE. No gameplay
wording ambiguity was found. Root must choose generic provenance/application
infrastructure, not activate a Sorrow-only subset; no source edit is yet claimed.

## UP-141 — Light Miracle Worker

Status: In progress (bounded read-only map), 2026-10-02. Missing Expert perk:
Resurrection restores25% more casualties than its normal calculated amount.
Trace casualty restoration, minimum AI prediction and shared live/detached
calculation, including the spell's casualty ceiling and living-target rules.
Do not substitute ordinary surviving-creature healing for casualty output.
No source edits, activation, build or coverage claim from this map. Steadfast's
running build and principal native verification remain the immediate priority.
Map finds the shared heal.lua preview/application path and CHealth casualty
ceiling. Survivor healing precedes casualties. Asked whether25% scales residual
casualty-restoration HP or the resulting integer creature count (floor); those
produce materially different outcomes for partial restored creatures. Await
that narrow clarification before implementing, not a global healing multiplier.

## UP-142 — Command Commanding Presence

Status: Verified (source/native; playable delivery pending), 2026-10-02. Advanced perk:
friendly stacks currently affected by one of the hero's Orders treat negative
Morale as0 for that Order's duration. Map current Order recipient/lifetime
representation and shared live/detached Morale path. Preserve simultaneous
different Orders and target membership, do not grant an unconditional army-wide
Morale floor or invent an extra action. No edits/activation during Steadfast's
frozen build. UP-141 awaits casualty-output clarification; UP-140 acceptance
remains the immediate delivery priority.
Map complete: all eight Orders use round-scoped state, but recipient benefits
can be consumed or broken earlier (Charge, Protect, Second Wind). Asked whether
Commanding Presence follows that effective benefit lifetime or recipient
membership until round end. User resolved2026-10-02: end the Morale floor when
that recipient's Order benefit is spent or broken, not merely at round end.
User's subsequent reply to question `call_ZE8GputCEgupMjebv9Ly6VXg`
reaffirms this same ruling. No new round-long protection or design change is
introduced; the canonical Commanding Presence row already incorporates it.
Record the accepted clarification in Pending Changes until canonical integration.
Shared battleGetMorale
covers live and detached AI. Existing state represents only one Order per side;
Double Command's missing multiple-Order foundation remains explicit and must
not be disguised as full Command coverage.
Implementation checkpoint: accepted clarification is integrated into the
canonical Command row and registry help; Pending Changes marks it integrated.
Canonical SHA-256 ccaa84fcd322b1e011ab5cac8094195f198b499026f5f78005b1a1a4eab93d21.
Separate Luna runtime and native-fixture owners implement the shared effective
recipient predicate and Morale floor without polling/action changes. Root owns
registration, metadata, builds, docs and Git. Status remains planned until native
acceptance; no coverage increase or playable claim from specification integration.
Runtime source is frozen in shared CBattleInfoCallback. Review catches Focus
Fire's Combined Arms melee eligibility missing the actual damage path's
SPELL_LIKE_ATTACK exclusion; root aligns that branch and reuses the existing
shooter-recipient predicate. A focused fixture guard is required. No new state
or polling; multiple-Order representation remains independent missing work.
Frozen production client build52957 is live with12 jobs, log
build/new-horizons-linux/testing/UP142-client-build.log. Fixture owner may edit
only its new unregistered test file; no overlapping source/build. Re-poll52957
before test-target registration/build and do not infer native success yet.
Client52957 exits0. Nine-case fixture is registered; serialized test build98920
is live with12 jobs, logUP142-test-build.log. Re-poll that handle. Review repairs
fixture-only assumptions about Charge movement and shooters' melee eligibility
under Flank; do not narrow correct production behavior to match a faulty test.
Rebuild the changed fixture after98920 terminates before native acceptance.
Test build98920 and frozen incremental rebuild exit0. Principal56838 runs9
cases:2 pass,7 fail, zero skips; positive Angel/army Morale invalidates the
fixture's assumed net-1. Preserve UP142-principal.log/XML. Fixture owner repairs
the negative baseline without weakening production; registration stays planned.
Fixture rebuild15520 exits0. Principal retry18653 passes9/9 in21.568s, zero
skips, with negative-before/zero-during/negative-after checks against the
configured Morale lower cap. Root activates the perk and refreshes module/UI
inventory. Both-target21780 exits0; data36/36 and module drift pass. Coverage
175/310 active,135 planned, Command5/10; ranks84/93 unchanged. Activated23-case
gate39487 is running; re-poll it before commit. No playable promotion. Phase2
retains Protect control changes and Flank/Formation Fighting interactions;
multiple-Order state is still separate missing Phase1 coverage.
Activated gate39487 passes23/23 in25.382s, zero skips. Independent final review
reports no blocker. Test binary SHA-256:
c29e58c08a615bcf3406d43e6cca7c1a402b45dc96b8174243b12d4eaed49906.
Source commit/push follows; graphical/playable delivery remains separate.
Source delivered as401f80384451e0522ff8df8f035901863c03025a on
origin/definitive-mvp; push exits0. Work moves next to the unblocked Bloodrage
threshold/cap foundation. No new Linux launcher snapshot or Windows package is
claimed for this commit.

## UP-143 — Bloodrage threshold perks

Status: Verified (committed/pushed; playable delivery pending),2026-10-02.
Unrelenting, Berserker and the prior Fury Unbound slice are implemented and active.
Snapshot46666 builds both Linux targets; principal retry64160 passes7/7 in2.554s,
zero skips. Activated both-target build succeeds; focused70764 passes31/31
in6.987s with zero skips. Data36/36/module drift/UI source guard pass. Current
coverage179/310 active,131 planned; faction48/90; Bloodrage5/10; ranks84/93.
The player-scoped enemy-AI failure is repaired without changing its six original
behavior tests. Test binary SHA-256:
cf67616ee55e5c617473e91238bd34ee66c0a8fef56eb65131e42181def5d981.
Phase2 retains broader control/status/save, hidden-enemy hero and Shroud-cache
interactions. Purpose-made artwork is Not done and generic UI Provisional.
No immutable playable snapshot or Windows acceptance is claimed.
Source delivered as b99c49c32aff8beb8f0b615edc845d55435784c9 on
origin/definitive-mvp; push exits0. Windows notice preflight37049324047 is
confirmed in_progress on this exact source. Check its terminal result before
dispatching the next full Windows build; do not claim it is a playable package.
Notice preflight37049324047 is terminal success. Full Windows build37049519240
is confirmed queued on b99c49c32aff8beb8f0b615edc845d55435784c9:
https://github.com/thegandalf196/vcmi/actions/runs/37049519240 . Track that exact
run through terminal state; a queued dispatch is not Windows compile acceptance.

Next Bloodrage design question: First Blood and Slayer each individually grant
two increments. Asked whether their overlap on the first Elite/Champion death
grants2,3(additive extra increments),or4; await that narrow stacking answer rather
than silently choose. Blood Scent, Rage Through Pain and Avatar of Rage remain
unblocked missing specification items. This does not block the whole Phase1 goal.

2026-10-02 next implementation slice: Unrelenting and Berserker. Root selects
generic unit-environment dynamic Speed and retaliation hooks, shared by live and
detached units. Threshold uses the current controller's saved cap, never a fixed
20/30 value. Speed does not raise separately defined Initiative. Berserker's
allowance stays outside the ordinary retaliation cache so control/eligibility
loss cannot preserve it; spent retaliations are not refunded. Separate Luna
runtime and fixture owners, with read-only AI review. Registration remains
planned pending builds and focused native acceptance; counts remain177/310.
Runtime is frozen; Astra review finds no blocker. Serialized12-job client
build66372 is live, log `UP143-threshold-client-build.log`. Re-poll that handle
before test-target registration/build; fixture work remains unregistered and
independent. Broader control/status/save matrices are deferred to Phase2.
AI review confirms movement radius and retaliation allowance are read dynamically
in isolated branches. Existing battle-form Initiative snapshots retain precedence:
Unrelenting changes Speed, not separately defined Initiative. Phase2 finding:
the existing unit-ID-only ReachabilityMapCache can retain controller-sensitive
Shroud ghost-walk geometry after hypothetical Hypnotize; that cache is not the
Bloodrage movement radius and this slice does not claim to repair it.
Client66372 exits0, reaching268/268 and linking vcmiclient. Native acceptance
awaits the frozen new fixture and serialized test build; do not run stale tests.
Serialized vcmitest baseline build49398 is live for the changed shared headers,
log `UP143-threshold-test-baseline-build.log`; the new fixture remains unregistered
until it freezes and this build terminates. No native execution before the
subsequent fixture registration/build succeeds.
Six-case fixture is frozen; root adds the direct GameSettings include identified
by independent review before registration. Data/schema/inventory36/36 pass
before activation. Principal native acceptance is still pending; source review
does not substitute for it.
Baseline49398 exits0; both-target fixture build54931 succeeds. Principal30137
passes5/6, zero skips. Detached defender Berserker fails after the branch crosses
the threshold, despite correct per-side progress. Registration stays planned.
Root coordinates read-only AI/fixture diagnoses before selecting a faithful
repair; do not change the expected principal behavior to conceal the failure.
Diagnosis confirms the player-scoped BattleProxy hides the defender hero. Root
selects authoritative per-side resolved Speed/retaliation bonus snapshots instead
of a spectator-only fixture or a global hidden-hero bypass. Hypothetical branches
copy these mechanic values; current control and saved cap still determine benefit.
Append one serialization feature, reject lossy older writes before bytes, validate
0/1 values and required rank, and reset older-format bonuses to0 to preserve
their prior inactive behavior. New save verification is required before activation.
Snapshot repair and seventh savecase are frozen. Reviewer finds no blocker.
Serialized12-job both-target rebuild46666 is live, log
`UP143-threshold-snapshot-build.log`. Re-poll this handle before executing the
unchanged six behavior cases and new binary case. No activation yet.

Current implementation slice2026-10-02: Fury Unbound's shared live/detached
Morale floor and UP-144's resolved cap. Friendly eligibility uses the current
controller, consistently with Commanding Presence and other faction effects;
the base Bloodrage damage query must use the same side rather than original
unit side after Hypnotize. Unrelenting/Berserker remain missing next slices,
not counted from shared foundations. Separate runtime, AI and fixture owners;
root owns serialization feature, UI cap binding, activation, builds and Git.
No new polling, actions or counter. Keep registration planned until native gates.

Status: In progress (bounded read-only map), 2026-10-02. Map missing Unrelenting
(+1 Speed at half the current Bloodrage cap or higher), Berserker (one additional
retaliation at that threshold), and Fury Unbound (negative Morale floor0 while
any increment is active). Trace authoritative state, current control, detached
AI and shared attribute queries. Do not invent counters or per-update scans.
Root must assign non-overlapping implementation ownership after reviewing the
map; no activation or coverage claim yet. Steadfast acceptance remains first.
Map complete: serialized per-side rank/increment already drives live and
hypothetical deaths. Unrelenting needs the shared Speed/Initiative seam and
cache invalidation; Berserker needs CRetaliations allowance/spending; Fury
Unbound fits shared battleGetMorale. Root must resolve original-side versus
current-controller eligibility consistently with the existing Bloodrage damage
path before assignment, and preserve future cap modifiers. No edits/tests from
mapping are evidence of these perks being implemented.

## UP-146 — Simultaneous different Orders foundation

Status: Verified (committed/pushed; playable delivery pending),2026-10-02. The user's approved
rule keeps different Orders active for their normal durations when a perk allows
more than one in a round. The current one-optional-Order-per-side model is missing
foundational Phase1 coverage and blocks Double Command. Map authoritative
issuance/consumption/expiry, every shared live/AI consumer, client required hooks,
and save/wire compatibility before selecting a collection model. Do not merely
retain two labels while only the latest effect operates. Root owns architecture;
three independent read-only lanes cover runtime, AI/shared effects and saves.
Focused simultaneous damage/mitigation, independent consumption/expiry, detached
branch isolation and legacy/current save gates are acceptance requirements.
No source activation or coverage increase is claimed from mapping alone.
Selected foundation: one authoritative bounded per-side Order collection,
command-keyed state mutations, independent effect consumption, latest-order
compatibility projection, append-only versioned collection serialization, and
pre-byte rejection of lossy old-format writes. Runtime/transport, core state,
shared effects/AI are separate Luna ownership lanes; root owns UI consumers,
version/preflight, existing fixture migration, builds and delivery. Current-round
same-Order issuance remains prohibited; collection updates grant no action.
Source is not yet frozen or built. Focused native acceptance and independent
review remain mandatory before claiming this foundation complete.
Production freeze checkpoint: reviewer reports no remaining blocking issue after
both packet visitors require unchanged issuance and monotonic progress before
mutation. Client build23496 is running with12 jobs; log
`build/new-horizons-linux/testing/UP146-client-build.log`. Re-poll that handle
before another build or native acceptance. New bounded fixtures may finish while
this client-only target builds; no further production edits during the build.
Client23496 exits0. Root adjusts two existing help strings after the build to
describe eligible Hero/Order actions accurately. The subsequent serialized
both-target fixture build must include that bounded UI change; native acceptance
is still pending, and no stale test binary is being used.
Both-target baseline build20796 is live with12 jobs. Exact log:
`build/new-horizons-linux/testing/UP146-test-baseline-build.log`. Re-poll that
handle before registering/building the unregistered main fixture or executing
native acceptance. The packet fixture is frozen and included; the main fixture
may be written independently without entering this build.
Baseline20796 exits0. Root registers the frozen six-case main fixture; incremental
both-target build42111 is live with12 jobs, log
`build/new-horizons-linux/testing/UP146-fixture-build.log`. Re-poll it before
native acceptance; the candidate now includes both packet and live/AI fixtures.
Fixture42111 exits1 on two standalone SideInBattle default constructors; root
supplies explicit null callbacks only in the isolated serialization fixture.
Retry96338 is live with12 jobs, logUP146-fixture-build-retry.log. The original
failure log is retained; do not run native tests until this retry succeeds.
Retry96338 exits0. First principal13014 passes19/20 in32.516s, zero skips.
The client-visitor fixture uses the isolated wire helper's BattleID7 instead of
the live ID; root corrects all three contextual packets without relaxing any
assertion or production check. Rebuild62682 is live (UP146-visitor-fixture-build.log).
Retain the initial failure log/XML and re-poll this build before native retry.
Rebuild62682 exits0; principal retry75974 passes20/20 in31.867s, zero skips.
This includes the accepted Commanding Presence lifetime, independent coexistence,
legal action allowance/repeat gates, branch isolation and current/legacy saves.
Adjacent87780 is running the bounded existing Order/persistence/Vengeance filter;
log/XMLUP146-adjacent. Source/UI guard7/7 and diff check pass. No perk activation
or immutable playable promotion is claimed; Double Command still needs its hook.
Final bounded evidence: principal20/20 passes in31.867s, zero skips. Adjacent87780
passes38/46 in12.558s: Order/Iron Discipline/persistence37/37 pass; eight unchanged
Vengeance cases stop at missing earlier-perk fixture setup, recorded in
NH_RELEASE_FAILURES.md for Phase2. Both targets build, UI source guard7/7 and
diff check pass. Reviewer reports no remaining blocking source finding. Binary
SHA-25642573c71f48dcd943238666c0e44772ca2999eec148aec0b9d7ff1d654fd4865.
The simultaneous-Order foundation is complete enough for Phase1; counts stay
180/310 perks,84/93 ranks,49/90 faction perks. Double Command's missing trigger
is the next dependent coverage item. Commit/push is next; no GUI or promotion.
User reaffirmed the Commanding Presence decision on2026-10-02: the Morale floor
ends when the recipient's Order benefit is spent or broken. With simultaneous
Orders, retain that floor only while at least one still-effective Order benefits
the recipient; consuming one Order must not consume or erase another. This
clarification is already canonical under UP-142, not a new round-long exemption.
Source delivered asf57f58a84c8d82d49c9b5f555b12eb08f62e4585 on
origin/definitive-mvp; push exits0. Earlier Windows37049519240 completed
successfully onb99c49c32aff8beb8f0b615edc845d55435784c9, not this source.
New-source notice preflight37060224004 is in progress onf57f58a84. Preserve
and poll that exact run through terminal before dispatching the full Windows
package build. No launcher snapshot or GUI delivery is claimed from source push.
Notice37060224004 now exits success. Full Windows37060422101 is in progress
on7a90085cb0d96a9b379bf4afc83a2fe66354bf41, a documentation-only checkpoint
after the gameplay commitf57f58a84. Preserve/poll that exact full run, do not
launch a replacement while it remains live. No new Windows package is claimed
until compilation and packaging actually succeed.
Full Windows run 37060422101 completed successfully at 2026-10-02T21:29:11Z
on 7a90085cb0d96a9b379bf4afc83a2fe66354bf41: compilation and packaging passed.
It includes UP-146 coexistence, not the still-uncommitted UP-147 implementation.
Windows graphical acceptance and local launcher promotion remain separate.

## UP-147 — Command Double Command

Status: Verified (source/native and pushed; Windows build in progress),
2026-10-02. Implement the
canonical Expert perk: the first time per combat the hero spends a Hero Action
on an Order, immediately issue an additional different Order. UP-146 supplies
independent coexistence, not this trigger or its once-per-combat state. Reuse
authoritative typed allowances and shared live/AI seams; preserve the restriction
against the same Order twice in the sequence. Map the immediate choice/continuation
and failure/cancellation behavior before implementing it; do not silently turn
the canonical immediate sequence into an arbitrary deferred round-long action.
Required registration, save-state, minimum AI and existing UI hooks, builds and
focused legal-trigger/once-budget/no-repeat tests precede activation. Independent
art and broad cross-system matrices do not block this Phase1 execution path.
Root resumed the three independent maps after UP-146 delivery: authoritative
trigger/continuation, client/AI choice flow, and focused save/fixture acceptance.
The existing typed ledger has no payload-restricted immediate Order continuation;
granting an ordinary round-long ORDER allowance alone would not implement the
canonical timing. In particular, an initial Second Wind must not start its
Creature Activation before the additional Order choice resolves. Target-selection
cancellation and an empty legal-choice set must not produce a stuck combat.
Registration remains planned and coverage counts are unchanged during this map.
Map completed. The canonical UI rule explicitly forbids an Activate/Decline
perk prompt; independent review confirms that a mandatory ordinary Orders
chooser is faithful without a new design decision. Cancelling target selection
returns to that chooser; no legal different Order ends the opportunity on the
authority and resumes the deferred flow. The actual HERO allowance receipt,
not heroCommandUsed, supplies the first-use trigger. Separate Luna lanes now
own runtime/core, AI projection/use, and a new focused fixture. Root owns UI,
append-only feature version, registration, builds and final review. Do not
activate or increase coverage before the complete production path builds and
passes focused native acceptance.

Frozen source checkpoint: runtime, AI and five native cases are frozen. Independent
review found a deferred Second Wind scheduling hazard; root moved its scheduling
before unrelated continuation returns and reviewer confirmed the blocker repaired.
Shared branch nextRound now rejects unresolved continuation before ledger reset.
Client source guards11/11 and diff check pass. Serialized12-job build37865 is
running for vcmiclient and vcmitest, logUP147-build.log. Re-poll that same build;
do not execute a stale test binary or activate from static checks alone.
User reaffirmed the existing UP-142 spent/broken Commanding Presence lifetime;
no new round-long exemption or canonical amendment is needed.
Build37865 is terminal exit1 on the new fixture's IBattleInfo/concrete snapshot
type mismatch and absent act helper. Runtime/AI/client objects compiled so far;
do not infer both-target success or run the stale binary. Independent source
review also found the mandatory AI mode still entering the ordinary queue
forecast/early-victory decline; preserve the pending-round guard and bypass only
that ordinary forecast. Separate owners repair the fixture and AI source, and
add one actual evaluator-submit case before serialized rebuild/native acceptance.
Retry build 68259 is running for both targets with 12 jobs; log
UP147-build-retry.log. The AI forecast guard is repaired and independently
source-reviewed. Five server cases and one actual AI-submit/server-accept case
are frozen. Its defender first spends a real Hero Action on Haste while owning
the active stack, then the fixture reanchors the attacker before triggering
Double Command. This prevents an unused enemy Hero grant from masking the old
forecast bug. Re-poll this exact build before native execution or activation.
Retry 68259 exits 0: both Linux targets build. Principal native session 86481
is running six cases, logs/XML UP147-principal. Registration remains planned
until its actual terminal result; no source or graphical acceptance is inferred
from the successful compile. Phase 2 retains generic hypothetical packet replay,
rendered chooser QA and broader continuation combinations.
Principal 86481 is terminal: 3/6 pass, zero skips, 95.212s. Actual AI submission,
legal acquisition and no-choice exhaustion pass. Two invalid-target fixtures
used UINT32_MAX, rejected by the action factory before submission; the tester
replaces them with representable nonexistent IDs without changing rejection or
no-spend assertions. The remaining failure validates anchor health while binary
stack descriptors are still uninitialized. Runtime ownership now separates
structural decode checks from full alive/controller checks after initialization;
strict write-side and old-format loss guards remain. The fixture must describe
descriptor persistence honestly: CStack binary omits runtime unit state and
CGameState does not save ongoing battles. No fake midbattle resume or health
initialization is added to make acceptance green. Preserve original principal
artifacts; rebuild before retry. Coverage and registration remain unchanged.
Boundary repair is frozen: descriptor-only validation on decode and before
BattleStart initialization; full liveness/current-controller validation after
initialization and before writes. The fixture uses one honest descriptor
roundtrip, retains independent live AI branches, and checks missing-anchor
rejection. Both-target build 47418 runs with 12 jobs; retain/poll
UP147-build-boundary-retry.log before executing the repaired native cases.
Build 47418 exits 0 for both targets. Post-build atomicity review finds grant-ID
exhaustion must be rejected before consuming HERO or clearing projected effects.
Root adds server/visitor prechecks; separate AI and fixture owners add the matching
preparation guard and unchanged-state assertion. This small state-integrity fix
requires an incremental rebuild before native retry, not a new broad suite.
Pre-mutation grant checks and the unchanged-state assertion are frozen and
independently reviewed without a remaining blocker. Incremental both-target
build 82381 is running with 12 jobs, log UP147-build-atomic-retry.log. The 30
focused registry/inventory/client checks pass; native acceptance remains pending.
Incremental build 82381 exits 0 for both targets. Principal native retry 30525
is running the same six cases, logs/XML UP147-principal-boundary-retry. The
original failures remain retained; no activation before this terminal result.
Principal retry 30525 passes 6/6, zero skips, 99.078s. Double Command is enabled
in source registration and the generated module; the inventory marks its generic
interaction Provisional and purpose-made art Not done. Data/client checks pass
30/30 and module drift passes. Activated both-target build 47633 exits 0. The
final adjacent native gate 99320 runs 47 cases including Commanding Presence,
coexistence, packet persistence and typed action/spell allowances. Counts from
the actual registry are 181/310 active, 129 planned; Command 6/10. Faction perks
remain 49/90 and ranks 84/93. No graphical or immutable playable promotion.
Final activated native 99320 passes 47/47 in 134.777s, zero skips. Both Linux
targets build; generated-module drift, data/client 30/30 and independent review
pass. The canonical spent/broken Commanding Presence lifetime is included in
the gate. Original failing logs/XML remain preserved; no blocking issue remains
for this Phase 1 slice. Commit and push this coherent implementation next, then
run the Windows notice preflight before the full build. UP-148 is next.
Source delivered as 51340a3d48607a096acd1dcf2975bafdcfc03ef7 on
origin/definitive-mvp; push exits 0 and the worktree was clean. Verified test
binary SHA-256: 48b70cc162325509a0cd8cdf522a72e966a5a57b51038ce5f1f2e650e8296d34.
Notice preflight 37071300435 runs on that source. An accidental noncompiling
preflight dispatch through the expensive full workflow (37071223589) was
cancelled before compilation; preserve its run identity, do not confuse it with
the intended full build or restart it. Dispatch the actual full build only after
notice success and terminal cancellation. No launcher snapshot has changed.
Notice 37071300435 is terminal success and 37071223589 is terminal cancelled.
Full Windows build 37071436091 is running on source 51340a3d4. Poll that same
run through terminal; observation timeouts do not justify a replacement build.
Source/native Phase 1 acceptance is complete; Windows graphical/playable delivery
is not inferred from dispatch. UP-148 remains the next implementation item.

## UP-148 — Command Battle Plan

Status: Verified (source/native; playable delivery pending),2026-10-02. Command
Basic perk: once per combat, immediately before the first Creature Activation
of round1, issue one Order without spending that round's Hero Action. Map the
opening flow boundary, per-side choice anchor, typed receipt, save state and
minimum human/AI hooks while UP-147 is compiled and validated. No production
edits or activation during the frozen Double Command build. Root must resolve
the timing/controller contract before assigning implementation; focused legal
acquisition, opening timing, retained HERO budget and once-use evidence are
required. UP-147's retry/native acceptance remains the immediate priority.
Map complete: the canonical pre-combat UI explicitly opens the Orders chooser.
Insert after onTacticsEnded initializes round1 and its HERO ledgers, before
activateNextStack performs regeneration/Morale/automatic turns. Use a nonactivation
HERO_COMMAND anchor, saved per-side once-use/pending context and a dedicated
ORDER-only source; this must not trigger Double Command or consume the normal
HERO budget. Both eligible sides need their own opening choice before the first
real activation, then initiative is recomputed. Deterministic side ordering and
automatic exhaustion when no legal anchor/Order remains need root architecture,
not an invented delayed round-long action. No source activation from this map.
Root architecture approved after UP-147 delivery: a generic saved pre-combat
Order state resolves Battle Plan entitlement at battle setup, then deterministic
attacker/defender choices after tactics and round 1 initialization. Dedicated
BATTLE_PLAN Order receipts leave HERO intact and cannot trigger Double Command.
Publish pending state before the temporary HERO_COMMAND anchor notification;
do not run Creature Activation effects, Morale, regeneration or movement resets.
No legal anchor/Order ends the opportunity authoritatively, without carrying it
into later rounds. Runtime/core, AI and focused native fixtures are independent
Luna lanes; root owns existing chooser interaction, version, CMake, activation,
builds and delivery. Independent architecture review finds no blocker. Keep
Battle Plan planned until both targets and focused native acceptance pass.
Runtime, AI and fixture source are frozen. Independent source review finds no
blocking issue; focused data/client guards34/34 and diff checks pass. Root's
serialized12-job client/vcmitest build95660 is running, log
`build/new-horizons-linux/testing/UP148-build.log`. Re-poll that handle before
native acceptance; do not execute a stale binary or activate from source checks.
Second Wind remains unavailable at opening under its existing spent-activation
prerequisite. Phase2 records exhausted grant-ID handling in prospective preflight
(throws without partial mutation), broader opening interactions and rendered QA.
No playable snapshot promotion or Windows acceptance is claimed.
Build95660 is terminal failure: the local prospective view inherits unimplemented
pure BattleProxy methods. The runtime owner is repairing its read-only adapter;
preserve the failed log and retry only after source freeze. No native acceptance
or activation is inferred from the source review.
Read-only adapter repair is frozen. Root's both-target12-job retry43682 is live,
log`build/new-horizons-linux/testing/UP148-build-retry.log`. Re-poll43682 before
native acceptance or any other build; all delegated source lanes have completed.
Retry43682 is terminal failure: the read-only adapter requires a complete
BattleLayout return type. Root added its defining header; both-target12-job
retry26167 is live, log`build/new-horizons-linux/testing/UP148-build-retry2.log`.
Re-poll that exact handle, preserving earlier failed logs. Native tests and
registration remain pending.
Retry26167 exits0,635/635, linking both targets. Principal native99345 is running
the four server cases and one actual AI submission/server-acceptance case; logs
are`build/new-horizons-linux/testing/UP148-principal.log/.xml`. Registration stays
planned until those results establish the principal paths with zero skips.
Principal99345 passes5/5 in13.180s, zero skips. Root activates production
registry/module/inventory, then removes fixture-local activation overrides.
Activated both-target build75589 exits0; native40531 passes30/30 in45.567s,
zero skips, including Battle Plan5, Commanding Presence9, coexistence5 and
allowance ledger11. Data/client34/34, module drift and final independent source
review pass. Coverage182/310 active,128 planned; Command7/10, ranks84/93 and
faction49/90 unchanged. Test binarySHA-256:
f26cef48474dc3b5f892cfb820d38c03a8ac9772cd3fdea227f2cea95267ece0.
Original build failures remain retained. Commit/push is next; no launcher
snapshot, Windows acceptance or rendered chooser acceptance is inferred.
Source delivered as52c4f89a636923260ea0ac8d4e1a2c79aab76bda to
origin/definitive-mvp; push exits0. Windows notice37076319236 is in_progress
on that source. Earlier full Windows37071436091 is still in_progress on
51340a3d4; preserve/poll it before dispatching the next full build. No new
package or local snapshot is claimed.
Windows notice37076319236 subsequently succeeds. Full Windows37071436091
completes successfully on51340a3d4 (Double Command source). Root then dispatches
full Windows37077420212 on37dd359b871852bd43c56c46fe020b76c75da441,
which includes Battle Plan; this new run is confirmed in_progress. Preserve and
poll that exact run; no Battle Plan Windows acceptance is inferred from dispatch.

## UP-149 — Command Iron Will

Status: Awaiting design answer (map complete),2026-10-02. Canonical Basic perk:
friendly stacks affected by an end-round-expiring Order retain that Order through
their next Creature Activation. Map shared live/detached aging and recipient
consumption while UP148 builds. Do not revive spent Charge, broken Protect or
completed Second Wind benefits. Determine the saved per-recipient lifetime seam
before implementation; do not reduce the feature to an army-wide expiry extension.
No source changes, build, activation or coverage claim from this preparation.
Map complete: carry must begin at normal round expiry, preserve unspent/unbroken
recipient progress, and last through (not merely until the start of) the next
genuine Creature Activation. Live and detached Order paths have direct round
gates beyond the central benefit predicate; those require a shared effective
lifetime query. Continuations do not finish an activation; Wait/Defend finish it
when their normal action path does. A Time-Stopped recipient can carry across
several rounds while the same Order is reissued. Asked whether new same-command
issuance replaces that older carry or preserves separate nonstacking instances;
await this narrow lifetime decision before implementation. UP148 acceptance
continues independently.

## UP-150 — Command Crisis Command

Status: Awaiting design answer (map complete),2026-10-02. Missing Advanced perk: once per
combat, when a friendly stack is completely destroyed, immediately issue one
Order without consuming the Hero Action. Trace authoritative casualty events,
current-controller allegiance, action-resolution boundary and saved once-use
state. The free choice must not be invented as an ordinary round-long action or
trigger Double Command. Identify interruption/retaliation/ongoing-activation
requirements before implementation; minimum human and AI hooks are required.
Parallel read-only runtime and AI maps do not change production sources or
coverage. UP149 awaits its same-command carryover answer; no blocked rule is
silently decided. Root retains builds, integration, registration and delivery.
AI/UI map complete: expose a shared read-only pending-Order choice context rather
than another repeated client/AI boolean union. Crisis must retain responder side,
choice anchor and distinct interrupted activation/action context; the destroyed
stack's current controller need not own the active creature. Mandatory chooser
and legal nonpositive Order ranking are reusable, but activeStack is currently
a turn callback, not an off-turn response API. Saved entitlement must drive
detached branches, without hidden opponent-hero perk inspection.
Runtime finds BattleAttack/StacksInjured as hit-bearing destruction sources.
The current action finishes retaliation and automatic post-attack effects before
onActionMade handles later continuations. Asked whether Crisis opens after that
complete action resolves (before subsequent continuations/activations), or
interrupts individual hits. Await the timing answer before implementation; do
not silently weaken "immediately" or expose a chooser inside packet visitors.
Runtime map complete: capture controller before BattleAttack/StacksInjured
lethal hits; rebirth survivors do not constitute complete destruction. Unlike
Bloodrage, Crisis wording does not exclude summoned or cloned stacks. Ghost
cleanup is not the trigger. Outside-action deaths also arise in opening spells,
turn triggers and round-transition damage, so action-only draining is incomplete.
The saved reaction must resume the original continuation exactly once; do not
switch active stacks without recording that context. No source/activation claim.

## UP-151 — Command Seize Initiative

Status: Awaiting specification-conflict answer (map complete),2026-10-02. Missing Expert perk:
the first HERO-paid Order once per combat makes the latest-scheduled friendly
stack that has not completed its normal Creature Activation the next friendly
stack to activate after the current activation ends. Map shared live/AI initiative
selection and saved once-use/queue override while UP149 and UP150 await narrow
answers. Preserve enemy ordering and normal-activation eligibility; no extra
activation, HERO refund or secondary ORDER-receipt trigger may be invented.
No source changes or activation from this map.
Shared queue seam is CBattleInfoCallback::battleGetTurnOrder; Flow takes only
its first entry, so any override must occur before truncation for execution,
UI and detached AI consistency. Move into the next friendly slot without moving
enemy entries. Existing moved flags are reset by some extra activations and
cannot reliably prove normal-activation completion; a generic per-unit marker
is needed. HERO-paid receipt projection is the once-use trigger seam; dedicated
Battle Plan/Crisis/Double follow-up grants must not trigger it.
Root audit finds a material canonical conflict: the detailed perk row describes
moving a pending normal activation, the Morale paragraph5013 categorizes Seize
as extra, and UI5407 explicitly distinguishes moved normal from extra activations.
The current queue includes an unfinished active unit; selecting it can generate
an extra activation instead of moving an existing future one. Asked whether
Seize only moves an existing activation (excluding that current-unit repeat),
or may grant an additional activation to the current stack. Do not silently
adopt the map worker's extra-activation interpretation. Coverage is unchanged.

## UP-152 — Discipline Esprit de Corps

Status: Retired duplicate of UP130,2026-10-02. Root's registry scan initially
selected this planned perk without matching the earlier UP130 map. That existing
entry already awaits mixed-faction versus Undead-presence penalty scope. Do not
repeat its map or treat it as unblocked. No source or activation was performed.

## UP-153 — Battlecraft Passing Lines

Verified source/native checkpoint: both-target9087 and fixture retry38200 build
successfully. Principal retry13004 passes6/6 in4.330s; adjacent87077 passes10/10
in2.280s, zero skips. First4pass/2fail artifacts are preserved; fixture repairs
pin the actual detached copy and capture the movement activation token before
battle flow advances. Registry/module/inventory are active; data/inventory19/19,
drift and final independent review pass. Coverage183/310 active,127 planned,
Battlecraft3/10; ranks84/93 and faction49/90 unchanged. Test binary SHA-256:
`386e58b7065922baa459741a35985108654292f31d5af4dce372ac59257fa191`.
No immutable playable promotion or full tactical AI certification. The recorded
Phase2 deferrals remain open. Existing Windows37077420212 now succeeds on
older37dd359b8 (Battle Plan included; Passing Lines excluded). Commit/push next.
Delivered source: `7aaa48c1be92db6056973dfd4a3e6ad9164302c5` is committed and
pushed to origin/definitive-mvp; identity/privacy checks pass and the source
worktree is clean. Cheap notice37081984549 succeeds on that exact revision.
Full Windows37082097577 is confirmed queued on the same revision; preserve and
poll that job rather than dispatch a replacement. Linux source/native acceptance
does not imply Windows graphical acceptance or launcher snapshot promotion.
Full Windows37082097577 subsequently reaches confirmed in_progress on7aaa48c1b.

Status: In progress (bounded implementation map),2026-10-02. Canonical perk: friendly
stacks may move through hexes occupied by friendly stacks, provided movement ends
in a legal empty position. Implement shared movement/pathfinding eligibility,
authoritative destination/path validation, client preview and detached AI hooks.
Do not pass through enemy stacks, physical obstacles or illegally occupy friendly
hexes at movement end. Current controller, double-wide footprints and ordinary
movement-trigger behavior must remain correct. Preserve Ghost Walk semantics;
this is not flight or teleportation. UP149/150/151 and UP130 retain their existing
clarification blockers. No source, activation or coverage claim yet.
Separate runtime/shared, AI/client-consumer and focused-fixture read-only maps
are assigned. Root owns architecture, registration, integration, builds and Git.
The ordinary movement UI should consume shared reachability rather than a new
visual control. No new artwork or graphical execution is in scope.
Implementation architecture selected: transient reachability parameters carry a
friendly-occupied transit mask, resolved from the mover's current controller and
visibility-aware hero access. No duplicate saved capability is introduced.
Original accessibility remains strict for endpoints; physical obstacles are not
relaxed. Runtime, direct AI forecast consumers and a new bounded native fixture
have separate file owners. Ordinary hazards must still trigger during transit,
without committing an illegal occupied intermediate stop. Coverage remains
182/310 until build and focused execution establish acceptance.
Pre-implementation review requires legal segment endpoints at both hazard and
gate boundaries. The existing Ghost Walk occupied-transit exception suppresses
hazard segmentation and is not suitable for Passing Lines. The obstacle helper's
`passed` argument excludes already handled tiles; it does not process crossed
tiles. Focused acceptance must exercise an actual authoritative movement request
across a friendly footprint with a Fire Wall, not merely call the trigger helper.
Existing Ghost Walk interaction hardening remains a separate Phase2 finding.
Source is frozen with six registered native cases. Registry/module activation is
staged for validation, not counted as accepted coverage yet. Data/inventory
checks pass19/19; module drift and whitespace checks pass. Independent runtime,
AI and fixture review finds no blocking issue. Both-target12-job build9087 is
live, log `build/new-horizons-linux/testing/UP153-build.log`.
Phase2 deferrals: consecutive occupied-footprint interaction matrices,
double-wide siege gates/moats, compound hazards, broader control changes and
full tactical AI selection. Current AI evidence is shared/detached reachability,
not tactical-choice certification. No saved-state addition or playable snapshot
promotion is included. Existing Windows37077420212 is still confirmed compiling
older37dd359b8; preserve it rather than start another full build.

## UP-154 — Battlecraft Tactics deployment coverage

Verified source/native checkpoint: core37002 and repaired both-target10000/39337
exit0. Principal retry24146 passes8/8 in23.514s; adjacent11237 passes10/10
in17.054s, zero skips. Data/inventory19/19, module drift and final source review
pass. Coverage184/310 active perks,126 planned; Battlecraft4/10, ranks84/93
and faction49/90 unchanged. Registration/module/inventory are active. Preserve
the exit143 baseline and original7/8 principal artifacts. UI constructor crash
is repaired, and valid movement remains asserted before fixture blockers.
Rendered/actualAI handoff, broader siege layouts and malformed post-opening
phase hardening remain Phase2. Descriptor roundtrips do not prove full midbattle
resume; no immutable playable promotion. Source commit/push is next.
Source is committed/pushed as`a85f2e44e303effe166badb5765422f4eeb6585a`;
push exits0. Notice preflight37086103464 is queued on that exact source.
Existing full Windows37082097577 remains confirmed in_progress on older
Passing Lines7aaa48c1; preserve/poll it, then dispatch the newer full build after
the cheap notice gate passes and the current full job reaches terminal state.
Do not claim Windows compile/package acceptance from notice or native Linux tests.
CI continuation: notice37086103464 is terminal success on Tacticsa85f2e44e.
Older full Windows37082097577 is still live, now in packaging after compile;
it does not contain Tactics. Wait for its terminal result before dispatching the
newer full build, preserving that job and avoiding duplicate heavy compilation.
Older full37082097577 reaches terminal success on Passing Lines7aaa48c1.
After notice success, full Windows37086471771 is dispatched/queued on
`b954d071f2b7b0d32d8a47088e3939a742863def`, which adds only delivery notes over
Tacticsa85f2e44e. Re-poll this specific run; no newer compile/package acceptance
until terminal success. No local snapshot is promoted.
Full37086471771 subsequently terminates in failure before compilation: the
package regression source guard still expects local `tacticsMode` rather than
the production global `deploymentPhase` spell block. The91-case package gate
has one failure. A bounded guard/mutation repair is assigned; preserve this run,
record its lesson, and require repaired preflight before the next full build.
Guard repair is committed/pushed as0721ee12b7f9db7250f25bc6dc2f0d8b3a6fd1ac.
The focused resource wrapper5/5 and complete package preflight91/91 pass locally;
all three global-deployment mutants are rejected. Cheap notice37087398608
reaches terminal success on that revision. A replacement full build is dispatched
only after those gates and the earlier full job's terminal failure; it does not
include the still-uncommitted Defend prerequisite or imply graphical acceptance.
Replacement full run37087488369 is confirmed in_progress on0721ee12b;
preserve and poll that run rather than dispatching duplicate compilation.

Status: Bounded read-only preparation,2026-10-02. Canonical Basic perk extends
the army's deployment area two additional battlefield rows forward, subject to
scenario and siege restrictions. Map current deployment setup, authoritative
relocation legality, human/AI consumers, both-side sequencing and focused native
fixtures. Preserve scenario restrictions and Hero/Creature action budgets; do
not substitute legacy opposed-rank subtraction for two independent entitled
armies. Root chooses architecture before source edits. Passing Lines commit
and delivery remain the immediate integration checkpoint. No activation or
coverage increase from this map; ordinary design blockers remain recorded.
Maps complete without source edits. Legacy setup subtracts opposing reposition
bonuses and selects only one side; it cannot express two independent NH armies.
Human and AI receive only the initial tactics callback. Authoritative gaps must
be repaired in this slice: END is not bound to the current deployment side, and
movement's zone guard is only an assertion rather than release validation.
Root architecture direction: resolve independent per-side entitlements/ranges,
save explicit deployment progression and publish phase switches. Use deterministic
attacker-then-defender sequencing (an architecture choice, not a new gameplay
exception), and start opening effects/round1 exactly once after both finish.
Retain layout.tacticsAllowed and ordinary siege wall/gate/footprint legality;
do not invent an additional blanket siege prohibition. Reuse the existing
deployment interface and AI handler, extending their side-switch notification.
The legacy range defines its base row as1; the canonical extension is two rows
forward, not opposed Skill-rank subtraction. Native acceptance must cover both
sides, scenario-disabled deployment and forged side/out-of-zone requests.
No implementation, registry activation or coverage increase from these maps.
Implementation begins with three isolated Luna lanes: shared state/packets,
authoritative flow/validation, and human/AI deployment handoff. Root owns the
generic `BattleDeploymentState` header, one append-only serialization feature,
type registration290, metadata/configuration, builds and Git. Distances and
completion flags infer the current attacker-then-defender phase; existing scalar
tactics fields are synchronized projections. No polling, extra action or custom
visual control is added. Registration remains planned and coverage183/310 until
focused build/native acceptance. Server lane becomes the bounded native tester
after its implementation freezes, avoiding overlapping test-file ownership.
Shared runtime is source-frozen: independent deployment snapshots, typed phase
updates, scalar projections and pre-write compatibility guards are present.
Root rejects independent snapshots with no entitled side and aligns available
deployment destinations with the entire creature footprint. Server and human/AI
handoff lanes are still integrating; no build/native acceptance or registry
activation is claimed. The previous confirmation-only turn made no coverage
progress; current source inspection and footprint correction resume UP-154.
Existing Passing Lines Windows run37082097577 is confirmed live on7aaa48c1;
preserve that run rather than dispatching a duplicate while it compiles.
Tactics registration/module/inventory activation is staged for the principal
fixtures; corrected data/inventory gate passes19/19 and module drift check passes.
Counts remain183/310 verified until native acceptance. Serialized12-job frozen
core build37002 is live, log`build/new-horizons-linux/testing/UP154-core-build.log`.
Human/AI sources remain editable outside this target; the tester writes only its
unregistered fixture. Re-poll37002 before starting another compile, then freeze
all client/AI/test sources for the combined client/native build. Shared fixture
setup now preserves real independent deployment instead of clearing its scalar
distance; the new cases must use actual END actions, not synthetic beginCombat.
Core build37002 exits0. This proves the shared target compiles, not client/native
acceptance. Human/AI freeze and the unregistered fixture remain pending before
the combined build. No source build or registry flag alone increases coverage.
Human/AI lane is now frozen. Baseline combined build42019 is live with12 jobs,
log`build/new-horizons-linux/testing/UP154-client-baseline-build.log`; the new
deployment fixture remains unregistered while its owner writes it. Final source
review runs read-only. Re-poll42019 before fixture registration or another build;
no native acceptance, coverage increment or playable promotion yet.
Root/follow-up review found a blocking AI-deployment constructor-order defect:
tacticPhaseStarted(false) calls blockUI before stacksController exists. Repair
is queued after42019 is terminal: move that call to deploymentPhaseChanged's
inactive-local branch. Initial constructor blocking already occurs after controller
initialization. Do not run the baseline binary before recompiling the repair.
Baseline42019 is terminal exit143 at386/542, without a reported compiler error;
process inspection confirms no surviving cmake/ninja/compiler child. Do not
describe this interrupted build as success or infer its termination cause.
The constructor-order repair is now applied and the frozen eight-case fixture
is registered. A new combined incremental build must finish before native use.
The fixture exercises authoritative requests and detached packet replay, not a
client TacticsHandler callback queue; rendered/actual-AI handoff evidence remains
Phase2. Source registration remains staged, verified counts unchanged.
Repaired fixture build10000 is live with12 jobs, log
`build/new-horizons-linux/testing/UP154-fixture-build.log`. Re-poll that handle
before another compile or principal native run.
Build10000 exits0 for both targets. Principal35799 runs8 cases:7pass/1fail,
zero skips in23.519s. The movement case cannot find a reachable legal acceptance
destination after assembling its rejection blockers; other assertions pass.
Retain the original log/XML and diagnose fixture geometry without weakening
movement rules or acceptance. The Luna fixture owner has this bounded repair;
no coverage increment or source/native-complete claim yet.

## UP-155 — Battlecraft Overwatch implementation map

Status: Bounded read-only preparation,2026-10-02. Canonical Basic perk: a
Waiting shooter makes one automatic50%-damage ranged reaction against the first
enemy that voluntarily moves into its range before its delayed activation,
provided that enemy is a legal target; once per round. Map authoritative movement
segments, ranged target legality, reaction resolution and consumed/round state,
plus detached AI representation. Do not implement while UP-154 source/build
ownership is frozen. Root resolves architecture after the map; no perk activation
or coverage increase from exploration. Tactics build/native acceptance remains
the current delivery priority. No numerical redesign or bespoke art is requested.
Read-only map complete: voluntary-path reactions must check traversed hexes,
not just endpoints. Shared battleCanShoot supplies legality, while Counterfire
provides the50%-reaction and published per-unit round-marker pattern; do not
reuse its consumed marker. Ordinary moveStack also handles return-after-strike
and gating, so movement cause must remain explicit. Native CStack descriptor
serialization omits runtime unit state; do not claim full save support from
detached/JSON copies. Asked whether player-chosen Teleport/Blink count as
voluntary movement; await that genuine wording choice before implementation.
Tactics acceptance remains unblocked and takes priority.

## UP-161 — Learning Field Study

Status: Verified (committed/pushed; playable delivery pending), 2026-10-03. Advanced perk grants +25%
additional Experience for defeating enemy heroes or wandering armies whose Army
Value exceeded this hero's army at battle start. Map battle-start raw Army Value,
opponent-kind eligibility, winner/casualty XP publication and ordinary Learning
composition, persistence and AI visibility. No edits while UP160 builds. Do not
compare surviving armies or perceived hero-adjusted strength, include unrelated
guardian battles, or replace the authored condition with a generic XP bonus.
Root chooses architecture after the map; no activation/count from preparation.
Map complete: snapshot each actual side army's raw getArmyStrength at setup,
not Diplomacy-perceived or hero-adjusted strength. Existing SideInBattle saves
identities but has no start-value snapshot; append versioned state with old-read
defaults. Qualifying opponent has a fighting hero or map Obj::MONSTER identity;
exclude other guards/town/garrison armies. Winning hero's battle XP is composed
in BattleResultProcessor::endBattle, then calculateXp applies the existing
HERO_EXPERIENCE_GAIN_PERCENT total (100+Learning rank). A conditional25 percentage
point contribution follows that existing composition; only the non-draw winner
receives the grant. Ordinary postbattle XP display and generic AI perk selection
already consume the result; no separate action/UI currency is needed. Root will
partition setup/state, result award and isolated result/AI fixtures after UP160
acceptance. No edits or activation from this read-only map.
UP160 acceptance is complete. Root now partitions three Luna lanes: shared
battle snapshots/setup; generic XP composition plus winning-result consumer;
isolated authoritative result fixture. Side snapshots use optional raw starting
Army Value (unknown on old saves, zero remains meaningful) and a wandering-army
classification, appended under BATTLE_INITIAL_ARMY_VALUE. Old loads do not
reconstruct initial strength from surviving armies. Only the actual non-draw
winner with active Field Study gets25 additional percentage points through the
existing XP formula; equal/weaker enemies and other guards are excluded. Generic
postbattle XP display/receipt and AI acquisition remain ordinary consumers.
Registry stays planned until principal build/native evidence; no new count yet.
Production lanes are frozen. Root added outer BattleInfo/BattleStart older-write
pre-byte guards in addition to SideInBattle's direct guard. Core-only vcmi
build29456 is live with12 jobs; log testing/UP161-field-study-core-build.log.
Independent isolated result and AI-acquisition fixtures are outside that target
and may finish without mutating compiled sources. Re-poll29456 before another
build or CMake registration; no client/native acceptance or active count yet.
Core29456 exits1 because BinaryDeserializer rejects direct uint64_t values.
Root assigns a bounded wire-only repair: retain optional<uint64_t> in memory,
serialize optional low/high uint32_t words with no truncation or range cap.
Fixture adds zero/max-domain roundtrips; unknown legacy snapshots remain unknown.
No principal native execution or registration activation occurred. Retry only
after that repair is frozen; preserve the original build log.
Wire repair is frozen. Core retry6495 is live with12 jobs, log
testing/UP161-field-study-core-build-retry.log. The legal Advanced Nullkiller
offer fixture is frozen; the isolated server fixture remains unregistered.
Re-poll6495 before CMake registration or combined client/native build. No native
run or new coverage is implied by source implementation or this compile.
Core retry6495 exits0. Final production review finds no blocker. Root starts
combined client/test baseline build with12 jobs while the new server fixture
remains unregistered; all compiled production and existing AI-test files are
frozen. Register the new frozen fixture only after this build is terminal,
then incrementally build its target before runtime use. Core success is not
principal-path or client/native acceptance; registry stays planned.
Baseline57072 exits0 for both targets. Frozen nine-case result fixture is
registered, then build16347 exits1 on three local fixture API/include errors:
query ownership, missing local stackAt helper and unused CHero-dependent helper.
The fixture owner repairs only that file; production APIs remain unchanged.
Preserve the failed log and rebuild after freeze before running11 focused
result/AI cases. No native acceptance or Field Study activation yet.
Older Windows37091363403 succeeds on213b4a35e. After Investor notices pass,
new full Windows37094808848 is live on21dbb224b; dirty Field Study is excluded.
Fixture retry48428 exits0. The11-case principal gate exits139 after two hero
victory cases pass, during the wandering-army case; remaining cases are not
accepted and no XML is emitted. Keep registry planned. The designated tester
traces that one case with a batch debugger before any broader rerun or edit.
Retain the failed native log; source/build alone cannot close this crash.
The isolated debugger reproduces a fixture-side dangling access: neutral victory
removes the battle synchronously, unlike hero-vs-hero result dialogs; the XP
assertion then reads the removed battle. Backtrace is retained as
testing/UP161-field-study-monster-backtrace.log. Authorize only a fixture repair
capturing expected inputs before completion; preserve actual XP receipt checks.
No production lifecycle change or activation follows from this diagnosis.
Fixture-only lifetime repair is independently reviewed with no blocker.
Both-target rebuild31335 exits0. Isolated wandering-army retry passes1/1;
full principal gate passes11/11 in4.059s, zero skips, including actual XP receipt,
strict eligibility, snapshot roundtrips and legal AI acquisition. Logs/XML:
UP161-field-study-lifetime-single and UP161-field-study-lifetime-native.
Root activates Field Study after this evidence:187/310 perks,123 planned,
Learning3/10;84/93 ranks and49/90 faction perks remain unchanged. Generated
module/check and data/inventory19/19 pass; activated both-target build exits0.
Final activated gate passes11/11 in3.697s, zero skips; independent review finds
no blocker. Binary SHA-256:
84b396ec5c21d9abc9ecb1a8209a4494aad37f92af1f2a6cb9f735500e996605.
Full-game resume, unusual result/ownership
transitions and comparative AI valuation remain Phase2. Purpose-made art is
Not done; generic UI is Provisional. No immutable playable promotion.
Source committed/pushed as4c41c8aa0273b44fa538908a5ea017fc131bf0a0.
Notice37095711525 passes on that source. Full Windows37094808848 still runs
on preceding Investor21dbb224b; do not claim it verifies Field Study or restart
it merely because a later source commit exists.

## UP-169 — Bloodrage Rage Through Pain

Status: Source/native verified and active (committed/pushed; playable delivery pending),2026-10-03. First time a friendly stack
falls below50% maximum HP, it gains one personal Bloodrage increment for the
rest of combat. Map shared live/detached damage application, saved unit state,
current-controller eligibility and existing rank/cap/threshold consumers. Do
not increment the whole army or limit the trigger to physical damage without
authored authority. Root chooses architecture; no activation/count from mapping.
The previous No Escape cycle is committed/pushed as9f59f66eb; notice37098685825
passes and full Windows37098764803 is live on that exact source. Preserve it.
Rage Through Pain is per stack, not an army-wide first proc. Shared unit damage
must record the crossing once and retain the earned increment through healing
and ordinary round/activation changes. The current CStack binary omits broader
CUnitState; explicitly persist the new field rather than treating packet JSON
roundtrip as proof of game-save representation. No activation/count yet.
Root chooses an event-driven shared damage crossing using one pre-hit maximum
HP reference and strict below-half comparison. A saved per-side selected-perk
snapshot supplies the current controller's rank increment; the earned per-unit
value is independent of the shared side meter. Effective combined damage and
Unrelenting/Berserker/Fury thresholds use the normal current-side cap. Earned
state is retained through healing, ordinary activation/round changes and death;
alive/ghost/current-controller eligibility still gates benefits. One append-only
binary feature will persist side profile and the new CStack field, with legacy
zero defaults and earlier-writer loss rejection. No periodic normalization.
Separate Luna owners implement shared/runtime/persistence, detached AI and an
isolated native fixture; Astra independently reviews. Root owns accepted-hit
combat feedback, builds, registration/data, integration and Git. The log hook
reuses BattleAttack/StacksInjured's targeted event path, not a battle-wide scan.
Registry stays planned and coverage188/310 until principal acceptance.
Runtime, detached AI and four-case fixture are frozen. Root registered the
fixture and started one combined vcmiclient/vcmitest build with12 jobs,
session52291; log testing/UP169-rage-through-pain-baseline-build.log under
build/new-horizons-linux. Re-poll this handle before native acceptance; do not
restart it on an observation timeout. Pre-build review caught and repaired
fixture-only retaliation prevention on victims instead of outgoing hitters.
The fixture also rejects oversized and fractional JSON increments. Final
outer-packet-guard review is pending; no native or activation claim yet.
Frozen final Astra review reports no remaining BLOCKING finding. Outer battle,
attack, injury and unit-update old-version guards precede payloads; CStack
initialization preserves the explicit increment. Broader historical CUnitState
binary restoration and rare controller/form/revival matrices remain Phase2.
Build52291 is still running; native acceptance and activation remain pending.
Continuation checkpoint: handle52291 is confirmed live beyond515/727 with no
reported compiler error. Baseline registry/inventory19/19 pass using python3;
the initial python command was unavailable and its log is retained separately.
Direct registry recount confirms188 active/122 planned and84 active/9 planned
ranks. Ledger's stale Estates and Learning rows are corrected to5/5 and3/7.
Existing DirectDamageMechanicsTest.cpp:700 emits a non-blocking dangling-else
warning; no unrelated fixture/source change is made during this build. Full
Windows37098764803 remains live on9f59f66eb, excluding dirty UP169.
Combined baseline build52291 now exits0; the new fixture compiled and vcmitest
linked. A reused tester owns the four-case private-profile native gate with
outputs UP169-rage-through-pain-native.log/XML. No stale-binary acceptance,
registry activation or coverage increase is claimed before its results.
Principal native acceptance exits0:4/4 pass in1.186s, zero skips. Baseline
test binary SHA-256 fc1b4c90470cb164641e06ffc4be91220bedfb03776d788b212fba43a956e4d9.
Root activates Rage Through Pain, regenerates the curated module and updates
the asset inventory. Direct recount is189/310 active perks,121 planned;
faction51/90 active,39 planned; Bloodrage7/10; ranks84/93 unchanged. Activated
data/inventory19/19, module drift check and both-target incremental build pass.
Final production-active native gate and source checkpoint are pending. No
immutable playable promotion or rendered approval is claimed. Purpose-made
art remains Not done and generic UI is Provisional; Phase2 retains the broad
full-CUnitState binary gap and controller/form/revival interactions.
Final production-active gate passes4/4 in1.183s with zero skips; fixture reads
the active registry without its synthetic map override. SHA-256 is unchanged.
Final independent review accepts the activation delta with no BLOCKING issue.
Root proceeds to the coherent source commit/push; no full-game or rendered
acceptance is implied by the focused gate.
Source delivered as025ea810a740cff134d115dd7fab78cf232cca6d on
origin/definitive-mvp; push exits0 with the approved author/committer identity.
Matching notice preflight37101230223 is live. Full Windows37098764803 remains
live on earlier9f59f66eb; preserve it and do not dispatch a competing full run.
No local immutable playable snapshot has been promoted by this checkpoint.

## UP-171 — Shroud Evasive Shroud preparation

Status: Source/native verified and active (commit pending),2026-10-03. After making a flanking attack,
the attacker receives15% physical damage reduction until its next activation.
Reuse the authoritative flanking classifier, normal physical cap, activation
expiry and detached AI preview. Do not reinterpret the trigger as a hit on the
victim or invent a hero action. Root chooses architecture after the map; no
runtime edits, activation or coverage from preparation. UP169 build52291 and
principal acceptance remain the immediate integration priority.
Map complete: reuse the direct primary flanking-hit completion in
BattleActionProcessor::makeAttack, with eligibility captured before the hit
packet and a surviving-attacker refresh after application. The ordinary melee
retaliation follows that seam, so protection can apply to it. Canonical wording
does not require positive damage. A1500-basis-point physical-reduction bonus
uses the normal global cap and existing UNTIL_NEXT_CREATURE_ACTIVATION expiry
and serialization. Candidate-local AI can reuse No Escape's effect preview;
selected BattleExchangeVariant replay also needs the transition, since replay
does not generically copy newly added preview bonuses. No genuine design
ambiguity was found. Root will choose ownership/implementation after UP169's
principal acceptance, rather than mutate sources during the frozen build.
UP169 has now passed active native acceptance and is committed/pushed. Root
selects the mapped shared flanking predicate and refreshable1500-basis-point
bonus. Capture eligibility before applying the accepted primary hit; apply to
the surviving attacker before ordinary retaliation. No new polling, action or
binary feature is needed. Runtime owns NewHorizonsShroud.{h,cpp} and
BattleActionProcessor.cpp; AI owns AttackPossibility.cpp and
BattleExchangeVariant.cpp; tester owns a new unregistered Evasive fixture.
Root owns registration, builds, data/activation, integration and Git. Registry
remains planned and counts stay189/310 until the principal gate passes.
Live helper/server sources are frozen: qualification is captured once for a
direct primary flank, and surviving-attacker protection is applied before
ordinary retaliation with quantitative grant/refresh feedback. AI and the
isolated fixture remain in progress. Root identified the damage-cache lifecycle
requirement: a cache built during protection must not reuse reduced values
after expiry. AI ownership expands to AttackPossibility.h for bounded target-ID
history, including initial cache capture and parent-chain queries. This does
not depend on an unrelated Order forcing recalculation. No build or activation
yet. UP169's matching notice37101230223 has completed successfully.
UP171 runtime/AI and three-case fixture are frozen. Root registers the fixture
and starts one combined client/vcmitest build92831 with12 jobs; log
build/new-horizons-linux/testing/UP171-evasive-shroud-baseline-build.log.
Re-poll that exact handle before native acceptance; no parallel or stale-binary
run. Cache history is captured at initial population and queried through parent
caches. The fixture includes actual flanking/retaliation protection, front/ranged
negative cases, candidate/selected-replay isolation, narrow Bonus persistence,
same-strike nonstacking refresh and genuine TURN_QUEUE activation expiry.
Final source review is running; activation and counts remain unchanged.
Build92831 is terminal failure: the generic selected-exchange helper invokes
detached bonus methods on CUnitState rather than StackWithBonuses. Sole AI
owner repairs this concrete receiver without expanding shared-state APIs.
Failure log is retained; no stale test run, activation or coverage increment.
The AI receiver repair is frozen: getForUpdate supplies the mutable branch-local
StackWithBonuses. Root starts serialized both-target retry76200 with12 jobs;
log testing/UP171-evasive-shroud-retry-build.log. Re-poll this handle before
running the three-case native gate. Source review remains pending.
Retry76200 exits0 for both targets; tester owns the three-case native gate with
UP171-evasive-shroud-native.log/XML. Final review finds no remaining blocker.
Root corrected an overrestrictive review prompt: canonical Cleave is a separate
direct melee strike and Evasive has no authored Cleave exception, so a direct
qualifying Cleave remains eligible in live/AI/replay. Secondary collateral is
still excluded by the shared classifier. Broader Cleave/preemptive ordering
coverage is Phase2, not a claimed executed matrix or gameplay amendment.
Previous full Windows37098764803 succeeds on No Escape9f59f66eb. Matching notice
37101230223 succeeds on Rage Through Pain025ea810a; root dispatches the next
full Windows build on that committed source, not the dirty Evasive candidate.
New full Windows37102336709 is confirmed live on025ea810a. The first Evasive
native gate runs3cases:2pass/1fail, zero skips,5.463s. The target dies after
three actual attacks, preventing the live-retaliation assertion; selected AI
projection, refresh/real-expiry and narrow Bonus checks do not indicate a
production failure. Sole tester repairs fixture survival bounds; activation
and counts remain unchanged. Preserve original native log/XML and rebuild
before retrying; no altered production coefficients or stale-binary claim.
Fixture survival repair is frozen:3,000 peasants/20 Angels and current primary
damage plus unprotected-retaliation bounds control the observation interval.
Root starts serialized both-target fixture rebuild99526 with12 jobs; log
testing/UP171-evasive-shroud-fixture-rebuild.log. Re-poll before native retry;
principal live/AI/log assertions and negative controls are retained.
Rebuild99526 exits0. Repaired principal3/3 passes in5.480s, zero skips;
production activation follows, with data/inventory19/19, module drift and
both-target incremental build passing. Final production-active3/3 passes
in5.730s, zero skips, without the fixture's planned-only override. Binary
SHA-256:3d302ce731c2f278dfc30093d4a3e6767b95c3ebe7da0efde8810a7f00a3ab09.
Direct recount:190/310 active perks,120 planned; faction52/90,38 planned;
Shroud3/10, ranks84/93 unchanged. Retain both failed and repaired logs/XML.
Broader Cleave/preemptive ordering, control and full combat-save restoration
remain Phase2; purpose-made art Not done and generic UI Provisional. Final
activation review reports no blocking finding and confirms those registry
counts. Source commit/push is next, not a playable promotion.
Source is now committed/pushed as04a6ecdd68f10d26fb35fab0f1fda8c9529096c3;
push exits0 and the worktree is clean at that checkpoint. Matching Windows
notice37103081203 passes on that exact source. Full Windows37102336709 remains
live on preceding025ea810a; preserve it, with no competing full build. The
Evasive source checkpoint is not a Windows package or local playable promotion.

## UP-172 — Shroud Ambusher

Status: Source/native verified and active (commit pending),2026-10-03. Canonical Basic perk:
the first flanking attack made by each friendly stack in a combat deals+20%
damage. Map shared live/detached damage, accepted-hit consumption, per-stack
battle/save representation and minimum AI projection. Do not substitute one
trigger per army, every flank, a turn-local timer or an inert registration.
Root chooses architecture after evidence; no edits/activation/coverage from
this preparation. Preserve UP171's frozen acceptance and source checkpoint.
Map finds no genuine design ambiguity. Root selects a per-stack spent marker:
ONE_BATTLE duration, NONE type, SECONDARY_SKILL source/Shroud SID and a unique
stacking key. Existing saved Bonus representation and detached branch-local
bonus mutation preserve once-per-combat state without polling or new unit fields.
Shared flanking damage adds20 while unspent. Capture accepted primary-flank
eligibility before hit; consume after application before retaliation, including
zero damage and a dead attacker. Ranged/collateral/front attacks do not consume;
direct qualifying Cleave and retaliation retain the canonical classifier.
Runtime owns Shroud helpers/shared damage callback/BattleActionProcessor, AI
owns AttackPossibility/BattleExchangeVariant, tester owns one new unregistered
fixture, reviewer checks architecture/source. Root owns builds/registration/Git.
Registry remains planned and coverage190/310 unchanged until focused acceptance.
Runtime/AI are frozen. Runtime review finds no blocker; the dead-but-existing
stack accepts its spent marker and ordinary cleanup does not erase it. AI
candidate/direct/replay paths consume locally, and current-controller plus
parent-cache attacker history avoid stale first-hit premiums. Root starts the
serialized client build40160 with12 jobs, log
build/new-horizons-linux/testing/UP172-ambusher-client-build.log. Re-poll that
handle before another build. Tester may edit only its unregistered new fixture;
native acceptance, registration and coverage remain pending.
Client40160 exits0. Independent frozen AI review also reports no blocker:
candidate/selected/direct strikes consume once and collateral is excluded;
visible ownership and cache histories preserve branch-local prediction.
Await only the focused fixture before test registration/build and native gate.
The bounded principal fixture is frozen/registered. It exercises legal Basic
acquisition, front/ranged non-consumption, two actual direct strikes with the
first premium spent before the second, an independent second friendly stack,
candidate/selected AI branch isolation, actual Bonus-marker roundtrip and named
quantitative combat feedback. Root starts both-target test build9218 with12 jobs,
log testing/UP172-ambusher-test-build.log. Re-poll before native execution;
no independent exact-formula, full-save or rendered claim is inferred.
Combined9218 exits0; current test binary contains the registered fixture.
Independent final source/fixture review finds no blocking issue. Tester owns
the principal filter, with UP172-ambusher-native.log/XML retained. No activation
until that current-binary accepted-action result is inspected.
Principal1/1 passes with zero skips (0.354s test), including actual first/repeat
strikes, per-stack independence, candidate/selected AI isolation and named+20%
feedback. Root activates the registry/allowlist/inventory and generated module;
data/inventory19/19, module drift and both-target incremental build pass. Final
production-active1/1 passes, zero skips (0.346s test), without its planned-only
override. Native binary SHA-256:
5c9706054ccbc4f59f040e7ed901498fa3878aa0d9a3e471fdd063b83aba36e9.
Direct recount191/310 active perks,119 planned; faction53/90,37 planned;
Shroud4/10 and ranks84/93 unchanged. Marker Bonus persistence is executed;
whole-combat-save restoration and broader control/order/form/clone interactions
remain Phase2. UI Provisional, purpose-made artwork Not done, no rendered or
immutable playable promotion. Final activation review/source checkpoint next.
Final independent activation review finds no blocker and confirms the counts.
Root proceeds to the coherent source commit/push; no package/runtime-GUI
acceptance is inferred from that source checkpoint.
Source is committed/pushed asdb96e718b3de383cf6c8cd8296b347ac0edfed89, push
exits0 and the worktree is clean at the checkpoint. Matching Windows notice is
dispatched on definitive-mvp; capture its exact handle before delivery claims.
Full Windows37102336709 remains live on025ea810a; no competing full dispatch.
Matching notice37104183936 succeeds on exactdb96e718b. Compile/package progress
continues separately from source acceptance and does not certify Windows GUI.

## UP-173 — Shroud Shadow Assault

Status: Verified (source/native; playable delivery pending),2026-10-03. The first
flanking attack against each enemy stack ignores25% Creature Defense. Trace
shared Creature-Defense calculation, accepted per-target consumption, marker
persistence and AI branch/replay requirements. Do not replace this with Hero
Defense reduction, a bonus on every flank, or one use per attacker. No source
edit/activation/count from mapping. UP172 frozen build/native acceptance and
coherent source checkpoint remain the immediate priority.
Map complete: shared flank classifier and existing meleeDefenseIgnorePercent
apply25 percentage points to Creature Defense only, composing with Armor
Piercer/Charge under the existing cap. Capture accepted nonsecondary primary
hit before packet application, then mark the target after application even if
dead; another target retains its own first-flank allowance. Existing saved Bonus
representation and AI branch mutation avoid new unit-state fields or polling.
Keep the attacking/controller side in marker identity so one side does not
consume the other side's eligibility after control changes. Candidate/replay
and defender-keyed cache history need the corresponding transitions. No new
source edit/activation/count is claimed yet.
UP172 is accepted and committed. Root selects distinct attacker/defender-side
stacking keys on the target-carried hidden ONE_BATTLE/NONE marker, keeping
current-controller first-enemy allowance independent between sides. Existing
meleeDefenseIgnorePercent composes25 with Armor Piercer/Charge and only reduces
Creature Defense. Shared prediction reads do not spend; accepted primary-hit
application marks the target even if dead or no damage is dealt. Runtime owns
Shroud helpers/shared damage/BattleActionProcessor, AI owns AP/BEx, tester owns
one unregistered fixture and reviewer audits architecture/source. Root owns
registration/builds/Git. Registry stays planned; coverage191/310 unchanged.
Runtime is frozen and independently reviewed without a blocker. Root finds an
AI cache-key mismatch during implementation: cached damage is keyed by unit IDs,
not controller side. Therefore any target with recorded Shadow Assault history
must bypass that cache after a control change, even when the new side lacks the
perk. Sole AI owner fixes the parent-history predicate to ignore side for cache
validity while keeping actual spent-marker eligibility side-specific. No broad
control-matrix claim or gameplay amendment follows from that correction.
Runtime/AI are now frozen and both independent reviews find no blocking issue.
Root starts serialized client build10661 with12 jobs; log
build/new-horizons-linux/testing/UP173-shadow-assault-client-build.log. Re-poll
the exact handle before another build. Tester may edit only the unregistered
new fixture; no native acceptance, activation or coverage increase yet.
Client10661 exits0. The current production runtime/AI library links successfully;
test registration/build awaits the isolated fixture freeze. Retain the build log
and do not execute the previous test binary as Shadow Assault acceptance.
Root pre-build fixture review catches a fatal-assert macro in a value-returning
helper and a Castle defender incorrectly used for a Dungeon-locked perk. The
sole fixture owner repairs typed failure handling and selects a distinct second
allowed Dungeon hero; production faction/offer validation remains unchanged.
No failed native run or test-build failure is claimed from that source finding.
The repaired focused fixture is frozen/registered; final independent source
review finds no blocker. Both legal acquirers are distinct Dungeon heroes and
the helper uses typed failure handling. Root starts serialized both-target test
build99818 with12 jobs, log testing/UP173-shadow-assault-test-build.log.
Re-poll that handle before native acceptance. The initially observed AI header
signature concern was transient; root confirms the frozen declaration/definition
both take only defenderId. No production contract change was needed.
Combined build99818 exits0. Principal native1/1 passes, zero failures/skips,
test0.358s, wall0.67s. Logs testing/UP173-shadow-assault-native.log/XML;
binary SHA-256 eb13b6ef7f9c69e416031ce74750cb7e7960eea303c1a551ade54c19dd84add1.
Root enables the exact perk, data allowlist and honest UI/art inventory, then
regenerates the module. Production-active native acceptance remains required;
no immutable playable or rendered acceptance is claimed.
Activated data/inventory19/19, module drift and both-target incremental build
pass. Production-active native1/1 passes, zero failures/skips, test0.353s,
wall0.66s; the fixture bypasses its planned-only override. Binary SHA remains
eb13b6ef7f9c69e416031ce74750cb7e7960eea303c1a551ade54c19dd84add1.
Final independent activation review finds no blocker and recounts192/310 active
perks,118 planned; faction54/90,36 planned; Shroud5/10 and ranks84/93. Broad
control/form/clone/full-save and rendered-delivery validation remain Phase2.
Root proceeds to coherent source commit/push, not a playable promotion.
Source committed/pushed asbc979fdcde8f2447a57f06b8687045c42f406c8a; push exits0.
Matching Windows notice37105388534 is dispatched on that exact source. Existing
full Windows37102336709 remains running on025ea810a; no competing full build.

## UP-174 — Shroud Deep Flank

Status: Awaiting narrow design clarification,2026-10-03. Canonical row4793:
friendly ranged attacks against a target currently attacked from at least two
distinct melee sides gain half the current Shroud flanking bonus. Read-only
map finds FLANK Order target-specific accepted-hit side history and a shared
occupied-footprint directional mask; neither settles this independent perk's
meaning. Clarify current positional contacts versus previously accepted hits;
the historical interpretation also needs an explicit round/battle reset.
Do not invent that lifetime or require an active FLANK Order. Half rank bonuses
are12.5/20/30%, with existing fractional damage payload support. Shared ranged
damage and AI callbacks are mapped; historical semantics would additionally
need saved target state and branch-local AI transitions. No source activation,
build or coverage increase from this map. Shadow Assault acceptance remains
the preceding completed checkpoint.

## UP-175 — Shroud Night Prowler

Status: Verified (source/native; playable delivery pending),2026-10-03. A stack using Ghost Walk to pass
through an enemy stack's occupied hexes gains10% damage on its next attack
that activation. Map actual accepted movement path, enemy occupancy/controller,
next-attack consumption, activation expiry and shared AI movement/damage paths.
Do not grant the bonus for ordinary movement, friendly occupancy, merely ending
adjacent, or attacks in later activations. Deep Flank UP174 awaits its positional
versus actual-hit-history clarification. No source activation/count from mapping.
Map complete, no material design ambiguity. Root selects two existing melee/
ranged PERCENTAGE_DAMAGE_BOOST bonuses of10, Shroud Skill source, unique keys,
and STACK_ACTIVATION|UNTIL_ATTACK duration. Apply only after an actually committed
non-flying, non-deployment Ghost Walk segment crosses a currently hostile living
footprint, before an associated attack. Existing accepted-hit and activation-end
expiration handle consumption and unused opportunities. Shared callback route
predicate feeds independent AI candidate/replay projection, branch isolation and
cache invalidation. Runtime, AI and isolated fixture have separate Luna owners;
Astra reviews architecture/source. Root owns registration/builds/Git. No polling,
new unit field or gameplay schema is intended; coverage192/310 remains unchanged
until native acceptance and production activation.
Independent architecture review finds no blocker; it requires first-strike AI
consumption of both subtype bonuses and actual committed crossing, not endpoint
inference. Full Windows37102336709 now succeeds on025ea810a. Matching notice
37105388534 succeeds on Shadow Assaultbc979fdcd. Latest committed documentation
checkpoint3e0e96df6 gets its own notice before a subsequent full build; dirty
Night Prowler implementation is not included in that committed-source delivery.
Latest-head notice37105938548 succeeds on3e0e96df6; root dispatches full Windows
37106017377 on that exact committed revision after the preceding full build
is terminal. It includes Evasive/Ambusher/Shadow Assault, not dirty UP175.
Capture this same handle's terminal result before replacing its delivery lane.
Runtime source is frozen in Shroud helpers, shared callback and authoritative
movement hook. Independent review finds no blocker: typed bonuses apply after
an actually committed hostile crossing and before the associated attack. Root
starts only the frozen shared vcmiMain target while independent AI/fixture
ownership remains active; no full client/test or coverage claim follows yet.
Exact core build53687 uses12 jobs and log
testing/UP175-night-prowler-core-build.log. Re-poll this same handle; do not start
a second build while it is live.
Core53687 exits0. Root's pre-freeze AI inspection catches unconditional per-
candidate pathfinding even for heroes without Night Prowler, and missing pending
defender-effect projection. Sole AI owner gates route work before pathfinding and
completes preemptive/retaliation/whole-hit-set consumption. This is a source
readiness correction, not an executed native failure or a coverage increase.
AI source is frozen; exact-route prediction is gated before pathfinding and
consumption now follows each striker's complete hit set. Root starts a serialized
client build on frozen runtime/AI while the isolated unregistered fixture owner
finishes its readiness corrections. No native test executes on stale bytes.
Client handle17500 uses12 jobs, log testing/UP175-night-prowler-client-build.log.
Independent AI review finds two blocking compile surfaces after dispatch:
BEx lacks its local pending-bonus helper, and several candidate mutations call
removeUnitBonus on CUnitState instead of branch-local StackWithBonuses. Retain
the first build result; the sole AI owner repairs only after it is terminal,
then root rebuilds and retests rather than treating this as native acceptance.
Client17500 is terminalexit1. The retained log confirms four invalid candidate
mutation receivers; the missing BEx helper is a separate source-review finding.
Root assigns sole-owner repair through getForUpdate's StackWithBonuses, not a
new CUnitState method. The repeat UP171 constraint is recorded in release lessons.
Fixture source-only corrections use const BattleHex values, a non-flying mover,
the real log wording and persistent Backstab for isolated repeat-hit baselines.
The bounded AI receiver/scope repair is frozen and independently reviewed with
no remaining blocker. The isolated three-case fixture is frozen and registered:
accepted crossing/first versus follow-up damage/AI branches; unused move-only
expiry with friendly/adjacent/flying negatives; typed current Bonus roundtrip.
No invented old-writer rejection is claimed for these existing duration bits.
Root proceeds to serialized both-target retry and principal native acceptance.
Exact retry90975 uses12 jobs, log testing/UP175-night-prowler-retry-build.log.
Re-poll this same handle before a native run or another build.
Retry90975 exits0; client and vcmitest link, with the new fixture compiled at
221/317. The designated tester now runs only the three Night Prowler principal
cases in the private native profile. No activation/count until that gate passes.
Principal native exits0:3/3 pass, zero skips, total1.110s and suite0.825s.
Logs testing/UP175-night-prowler-native.log/XML. Binary SHA-256:
537d5121058c8e16be5a5c1eab738ca0a4d9177a63984128650e3e3e9ac1c785.
Accepted crossing/first-strike/unused expiry and minimum AI route/replay branches
work. Root activates the exact perk and data allowlist, regenerates the module,
and records honest Provisional UI/Not done art. Activated native gate remains
pending; no immutable playable or rendered acceptance is claimed.
Activated data/inventory19/19, module check and both-target incremental build
pass. Production-active native exits0:3/3, zero skips, total1.110s,suite0.833s;
its planned-only registry override is bypassed. Binary SHA remains
537d5121058c8e16be5a5c1eab738ca0a4d9177a63984128650e3e3e9ac1c785.
Final independent activation review finds no blocker and recounts193/310 active
perks,117 planned; faction55/90,35 planned; Shroud6/10 and ranks84/93 unchanged.
The flying negative is a shared predicate check, not a flown movement action.
Broad hazard/control/form, full-save and rendered-delivery checks remain Phase2.
Root proceeds to coherent source commit/push; no immutable playable promotion.
Source committed and pushed as003cd49cd869249aa4c96faf408f00e495f7fdd3.
Matching Windows notice37108021258 is terminal success on that exact revision.
Full Windows37106017377 remains live on3e0e96df6665926db35b2c35f768dc4772222ffc
and therefore excludes Night Prowler. That full run subsequently completed
successfully. Root dispatched full Windows37108695052 on003cd49cd869249aa4c96faf408f00e495f7fdd3;
it is queued at dispatch and includes Night Prowler but not dirty UP178 source.
Re-poll this exact new handle; notice success is not compiled-package acceptance.

## UP-177 — Dungeon Portal of Summoning shared recruitment

Status: Verified (source/native committed/pushed; playable delivery pending),2026-10-03. Canonical row3283
requires a weekly choice of one owned external dwelling. Dungeon recruitment
must expose that dwelling's current stock and deduct from the same stock;
the Portal never creates or duplicates troops. Current CGameHandler weekly
Portal generation selects a creature randomly and creates a separate growth
pool; ordinary recruitment deducts only the recruiting object's pool. Missing
Phase1 work: saved source selection, authoritative source-linked deductions,
selection/recruitment UI and minimum AI selection. Focused acceptance must
recruit through both locations and prove that each observes the same remaining
stock. Do not claim completion from a renamed building or a copied pool.
No source changes or coverage increase from this read-only audit.
Authority map complete: weekly setPortalDwelling creates an independent extra
town recruitment row, while RecruitCreatures already carries actual dwelling
ID, row, creature and quantity and deducts source stock. Save a Portal source
identity rather than a pool mirror; validate built/owned Portal access and
destination before reusing source cost/stock publication. Multiple source rows
and upgraded IDs already have ordinary request representation. Portal selection
UI and minimum AI selection still need a bounded map. Ownership loss must not
permit recruitment; no extra midweek choice or cross-town shared choice is
silently introduced. Root will establish the building-scoped selection rule
before implementation; no unrelated source mutation during UP178 acceptance.
Root selects building-scoped persistent source identity and last-selection
absolute week, with one authorized replacement per week per built Portal town.
Recruitment must carry explicit Portal-town context while retaining the actual
source dwelling as the stock/cost target. Validate owned built town, matching
saved source, still-owned eligible external dwelling, and a destination army
in that town. Without Portal context, retain ordinary local-visit checks: mere
source ownership must never authorize arbitrary remote recruitment. State and
wire changes require appended serialization compatibility. No foundational
blocker was found; implementation awaits completion of UP178 acceptance.
UP178 is now committed/pushed. Three bounded Luna lanes implement Portal
authority/state/request validation, town source selection/recruitment UI, and
minimum AI buying. Root owns append-only version/type registration, focused
fixture integration, builds and Git. Source selection persists across rollover
until a legal weekly replacement. Named packs SelectPortalDwelling and
SetPortalDwellingSource carry authority and replication; RecruitCreatures
retains the real source ID with explicit optional Portal-town context. No
stock mirror, arbitrary remote recruitment or coverage acceptance from edits.
Three production lanes are source-frozen, but review catches a synchronous GUI
ack wait that can deadlock the interface mutex. UI owner replaces it with an
asynchronous replicated-state event and safe window-lifetime revalidation.
AI owner repairs an undefined scheduler local, missing active-rule gates and
unconditional legacy-row exclusion. Authority context validation otherwise
passes material review. Focused native fixture creation is independently owned;
no build, coverage increase or usable-UI claim yet.
AI bounded repairs are frozen. Core-only vcmi build43329 runs12 jobs; exact log
testing/UP177-portal-core-build.log. Only isolated fixture files and client-only
deadlock repair may change while this target compiles. Root registers fixtures
and builds client/tests after that handle is terminal. Re-poll rather than
restart the live core build or run stale native bytes.
Core43329 exits0 at207/207. Root changes the new selection callback to return
its ordinary request ID, enabling exact-ID PackageApplied dispatch to the
current castle window without synchronous GUI waiting. Authority-only target
vcmiservercommon build99958 runs12 jobs, logUP177-portal-authority-build.log;
client-only repair and isolated fixture creation remain in progress. Do not
claim a full client/test build from the core or authority target alone.
Authority99958 exits0. Client79950 exits1 at the castle UI: three callback
locals incorrectly declare shared_ptr<CCallback> as auto pointers. The sole UI
owner repairs those declarations without restoring synchronous GUI waiting.
Both isolated fixtures are frozen (five authority/save cases and four AI
candidate cases). Root starts a serialized client/test retry with12 jobs,
logUP177-portal-client-test-retry-build.log. Focused data/inventory19/19,
generated-module drift and diff whitespace gates pass; native acceptance is
still pending and Portal is not yet counted complete.
The exact retry handle is34651. Re-poll this existing build until terminal;
do not restart it on an observation timeout or run the stale test executable.
Retry34651 is terminal exit143 at272/374 with no compiler error recorded;
read-only process inspection confirms the cmake/ninja process is absent. The
cause of the termination is not established. Root resumes the incremental
client/test build (completed objects retained), with a separate
UP177-portal-client-test-resume-build.log. Preserve the interrupted log and
require a successful fresh link before native execution.
Exact resume handle75438 is live; root remains sole build owner.
Resume75438 exits0 at103/103, linking vcmiclient and vcmitest. Both new
fixtures compile successfully. The designated Luna tester runs the nine-case
Portal principal filter in the existing private native profile, then the small
recruitment/BuyArmy adjacent subset only if principal passes. No stale binary,
coverage acceptance or playable promotion is inferred from compilation.
Principal9/9 passes in3.987s; adjacent recruitment/Muster/BuyArmy8/8 passes
in4.074s, zero skips and both exit0. Logs/XML are
testing/UP177-portal-{native,adjacent}.{log,xml}; fresh vcmitest SHA-256:
084fb8e102f7ec99f2bac6abcd42a90a8f9a5fb746db81ef6a504b95f2aec3a2.
Actual Portal/local purchases deduct the same real stock/cost and receive troops;
weekly choice, forged-context/ownership/Leadership rejection, full adventure
save/load, old defaults/loss guards and AI candidates pass. Independent final
review finds no blocker. Data/inventory19/19 and module drift pass. This closes
the missing building principal path, without changing194/310 perk or84/93 rank
counts. Phase2 retains rendered UI/ack behavior, broader ownership transitions
and full AI-turn scheduling. Coherent source commit/push is next; no promotion.
Source is committed/pushed asbd4f08c49483a1f62ab7955d0167ae6f2e041596.
Matching notice37120294892 succeeds. Full Windows37118407677 remains live
one6fd45213318b7a3b7812e4bd7ade712af404a8d and does not include Portal; do
not dispatch a competing full build while that exact handle is running.

## UP-181 — Logistics Mountaineer

Status: Source/native verified; commit/push and playable delivery pending,2026-10-03.
Initial map: Missing Advanced perk: rough and
mountainous passable terrain imposes no additional movement penalty. Map
canonical terrain identities, saved-rule eligibility, shared human/server/AI
movement-cost calculation and existing terrain fixtures. Do not grant passage
through impassable rock or globally remove other difficult-terrain penalties.
Root owns terrain semantics/activation/builds; no implementation or coverage
claim from this map. Do not repeat the already completed Roadmaster/Wayfarer map.
Map complete: TurnInfo's saved-rule-gated terrain exemption feeds the common
human/server/AI movement-cost path; ROCK remains impassable independently of
cost. Core data defines ROUGH and SUBTERRANEAN but no MOUNTAIN terrain/tag.
Asked whether mountainous means Subterranean or only Rough should qualify.
Do not waive Lava/other terrain costs by analogy or repeat the shared-path map.
User resolved terrain identity: Rough and Subterranean. Canonical text and
registry description now agree. Shared-cost production and legal-acquisition
human/AI fixtures are frozen; build/native acceptance and activation pending.
Root's serialized core build51743 is live with12 jobs; log
testing/UP181-UP182-core-build.log. No native acceptance or activation yet.
Core51743 exits0. Serialized client32699 is live with12 jobs, log
testing/UP181-UP182-client-build.log. Focused data/inventory19/19 and generated
module drift pass. Both new perks remain planned pending fresh native evidence.
Client32699 exits0. Test15320 exits1: the new direct-header fixture exposes
BattleDeploymentState's missing direct BattleHex.h dependency for BFIELD_WIDTH.
Root makes the header self-contained; repaired test build18902 is live with12
jobs, log testing/UP181-UP182-test-repair-build.log. Final incremental freeze
check is required before running tests. This is a compile failure, not runtime
acceptance, and no perk is activated yet.
Repaired18902 exits1 at the new runtime fixture: MasteryLevel is a namespace,
not a type. The fixture owner repairs the helper parameter; product code remains
unchanged. Resume incrementally after fixture freeze, not from a clean build.
Fixture correction is frozen; resumed test19165 is live with12 jobs, log
testing/UP181-UP182-test-resume-build.log. No native execution on stale binaries.
Resumed19165 exits0. Final frozen both-target98551 exits0, recompiling33 final
dependencies and linking client/tests. Designated tester now runs12 principal
deployment/Mountaineer cases, then adjacent Tactics/Redeployment/Logistics if they
pass. Production registration still planned pending those gates.
Principal12/12 passes, zero skips,2.818s; adjacent deployment3/3 and Logistics3/3
pass, zero skips,6.424s/1.975s. Combined adjacent6/6 also passes7.874s. Logs:
testing/UP181-UP182-native.*, UP181-adjacent.*, UP182-adjacent.*, and
UP181-UP182-adjacent.*. Binary SHA:
68ddef848092cde5f5499d29175416e74228985b47a339d32be64ee4092c4fa1.
Root activates exact Grand Tactics/Mountaineer registry and allowlist; data and
inventory19/19 pass. Generic UI is Provisional; purpose-made icons Not done.
Fixtures now distinguish original active registration from planned-only override;
final fixture rebuild and production-active12-case rerun remain required.
Final fixture build31761 exits0. Production-active native12/12 passes, zero skips,
2.618s; XML proves all four Grand Tactics and two Mountaineer cases see active
registry status with no activation override. Binary SHA:
22315f6c31d82de5b1caef29f33354cfc2ae0317ed422cbc0300995b176c5087.
Logs testing/UP181-UP182-active.*. Perks196/310,114 planned; Battlecraft6/10,
Logistics6/10; ranks84/93 and combat60/67 unchanged. Source/native verified;
rendered/actual full AI deployment and playable delivery remain separate.

## UP-182 — Battlecraft Grand Tactics

Status: Source/native verified; commit/push and playable delivery pending,2026-10-03.
Initial map: Missing Expert perk: reveal enemy
deployment before this hero finalizes ordinary deployment. Map the existing
Tactics/Redeployment shared deployment phase, authoritative hidden-state/access
policy, human confirmation flow and minimum AI hook. Preserve ordinary scenario
and siege deployment legality; do not substitute a separate perk action or
merely activate a tooltip. Root owns architecture; no edits or coverage claim
from this map. Report only genuine contradictory sequencing requirements.
Map complete: all enemy stacks are already rendered; existing initial phase
ordering is hardcoded attacker then defender. Grand Tactics requires sequencing,
not a new secrecy/reveal action. Asked for the both-holder tie rule and whether
the later Redeployment move is included. A holder without Basic Tactics should
still use the ordinary one-row area, not gain the two Tactics extension rows.
Root selects the unblocked prerequisite: generic saved initial-first-side
ordering in BattleDeploymentState, defaulting to attacker for old/current
ordinary battles. Preserve final-relocation order, authoritative transitions,
callback routing and old-format loss guards. This foundation does not activate
Grand Tactics or claim its complete coverage before the design answers.
User resolved both-holder ties to normal attacker-then-defender order and scope
to initial deployment only. Canonical text and registry description now agree.
Generic saved ordering and setup source are frozen; actual authoritative
deployment fixtures, build/native acceptance and activation remain pending.
Independent source review found a missing outer BattleStart downgrade guard;
root added it before payload, matching state/BattleInfo/deployment-update guards.
Current core build51743 does not constitute fixture/native or UI acceptance.
Four actual deployment fixtures are frozen, including exact immediately-prior
save-version BattleStart zero-byte rejection. Independent final review finds no
blocking issue; broader control/rendered handoff interactions are Phase2 deferrals.
UP181's shared evidence above also covers this perk: active native12/12, zero
skips, independent review no blocker and Battlecraft6/10. No rendered or playable
acceptance is inferred from native movement/deployment tests.

## UP-178 — Warcasting Master Synthesis

Status: Verified (source/native committed/pushed; playable delivery pending),2026-10-03. Canonical Expert perk replaces the
first Warcasting bonus consumed in combat with50% /50 percentage points.
Map shared spell/Order preview, accepted action consumption, battle-long
history, detached AI and saved state. Normal readiness must exist; the perk
does not manufacture empowerment on the first unempowered action. Do not
reset the first-consumption history at round boundaries or count typed bonus
actions as ordinary Hero Actions. Root owns architecture/registration/builds;
no source activation or coverage increase from mapping.
Map complete: no principal-path ambiguity. Root selects generic battle-long
positive-readiness consumption history in AlternatingHeroActionState, shared
hero-aware effective bonus resolution, and an append-only saved feature.
Runtime owner covers spell/Order preview and accepted consumption; AI/UI owner
covers detached Order valuation and visible hero status; fixture owner covers
legal Expert selection and focused actual action/state acceptance. Root owns
serialization version, registration, builds and integration. Coverage remains
193/310 until production activation after native acceptance. Asked whether
Perfect Rhythm doubles Master Synthesis's replacement50 to100 or leaves50;
Perfect Rhythm remains planned, so this future interaction is not silently
implemented or claimed verified by the standalone Master Synthesis slice.
Production source is frozen. Source review found typed/free action preview
leakage; shared eligibility now excludes these actions from both normal and
synthesized empowerment, matching accepted consumption. Legacy non-shared
Focus Fire and spell paths retain their prior eligibility. Root adds inner and
outer state/packet loss guards for the appended consumption history. Serialized
client build37491 is live with12 jobs, log
testing/UP178-master-synthesis-client-build.log. Re-poll that handle before a
test build; fixture editing is isolated from this client-only target. No stale
native execution, activation, or coverage increase from source freeze.
Client37491 exits0 at317/317. Data/inventory19/19 and generated-module check
pass while Master Synthesis remains planned. Independent production review
finds no blocking issue; principal fixtures/native gate remain pending.
Focused fixtures are frozen: three actual action cases cover legal Expert perk
offers, Spell and Order first-consumption50, later30, exact Spell HP loss,
typed exclusions, unused expiry and detached branch isolation. Four value-state
cases cover consumption, expiry/clear, copying, current roundtrip and old-version
loss guards; the prior zero-empowerment expectation now retains consumed history.
Serialized vcmitest build6811 is live with12 jobs, log
testing/UP178-master-synthesis-test-build.log. Require a final incremental build
after this fixture freeze before native execution. No coverage activation yet.
Test build6811 exits0 at339/339. Final frozen both-target incremental64587
exits0, recompiling the final server fixture and linking vcmitest. Independent
final source review finds no blocker. Designated tester now runs only seven
MasterSynthesis cases, then the relevant existing Warcasting/state subset if
principal passes. No stale binary or production-active evidence is assumed.
Principal native acceptance passes7/7, zero skips, exit0,1.364s; fixture XML
records the planned registry before its explicit test override. Adjacent gate
passes58/64, zero skips,10.967s: all new cases pass. One old readiness assertion
expects combat-long consumption history to disappear with expiry, and five
older fixtures bypass earlier-tier perk prerequisites. A bounded fixture owner
repairs those cases without weakening production prerequisites; independent
review checks the failure classification. Registry remains planned pending the
repaired adjacent gate and a subsequent production-active rerun. Exact evidence:
testing/UP178-master-synthesis-{native,adjacent}.{log,xml}.
Fixture-only repairs are frozen: legal Basic Spellward before Advanced Tactical
Weaving, legal Basic Sorcery Overcharger before Countermage, and cleared
readiness retaining consumed history. Independent review finds no material
blocker and confirms the hidden-enemy Countermage assertions remain intact.
Serialized both-target incremental57489 runs12 jobs; log
testing/UP178-master-synthesis-fixture-repair-build.log. Re-poll the same handle
before the designated tester's adjacent rerun. No activation yet.
Repaired incremental57489 exits0. Adjacent-repaired gate passes64/64, zero
skips,11.141s, exit0, including every new Master Synthesis case. XML records
planned status before the fixture override. Rebuilt binary SHA-256:
b206d126311f098c5964bc25a2b3e170e9b553eea4a62b97c75ff1286440d4ba.
Root activates the exact registry/allowlist and records Provisional generic UI,
Not done purpose-made art. Generated module, focused data gates and a fresh
production-active rerun remain required before coverage/delivery acceptance.
Activated data/inventory19/19, generated-module check and both-target incremental
build pass. Production-active native passes7/7, zero skips,1.316s, exit0; XML
confirms all three server fixtures see active status and bypass the planned-only
override. Logs testing/UP178-master-synthesis-active.{log,xml}; binary SHA
remainsb206d126311f098c5964bc25a2b3e170e9b553eea4a62b97c75ff1286440d4ba.
Independent final review finds no blocker and recounts194/310 active perks,
116 planned; Warcasting6/10, faction55/90 and ranks84/93 unchanged. Perfect
Rhythm stacking, full battle-save restoration, broad interactions and rendered
UI are deferred. Root proceeds to a coherent commit/push, not local promotion.
Source committed and pushed ase6fd45213318b7a3b7812e4bd7ade712af404a8d.
Matching Windows notice37111101650 succeeds on that exact revision. Full
Windows37108695052 remains live on003cd49 and excludes Master Synthesis;
do not dispatch a competing full build while that exact run remains live.
Full37108695052 subsequently succeeds on003cd49. Root dispatches full Windows
37118407677 one6fd452 after matching notice success; queued at dispatch. It
includes Master Synthesis, not the dirty Portal implementation. Re-poll that
exact handle, rather than creating a competing full job.
Full Windows37118407677 now succeeds on exact e6fd45213318b7a3b7812e4bd7ade712af404a8d.
This build includes Master Synthesis but excludes the later Portal source and
current uncommitted Grand Tactics/Mountaineer work.

## UP-186 — Dark Conversion canonical execution gap

Status: Verified source/native; playable delivery pending,2026-10-03.
Historical audit and correction trace follows. Runtime previously
offers a player/AI choice and converts Skeletons from every casualty tier. The
canonical rule instead requires automatic conversion from eligible Core-tier
casualties only. Active registration is not faithful completion of this rule.
Correct production authority without restoring invalid remains or magical
casualties lacking Corpse Preservation; retain unconverted Skeletons and atomic
Leadership/slot admission. Human and AI winners must use the same automatic
path, with no conversion-choice query. Focused category/remainder/admission and
post-battle evidence are required. Preserve historical choice tests as evidence
of the superseded runtime, not current acceptance. No activation count increase
is claimed: the data row was already active.
Production and fixtures are frozen. Client35092 exits0. Root both-target
12-job build70772 is live, logUP186-frozen-build.log; re-poll this exact handle
before native execution, do not restart on an observation timeout. Independent
review reports no blocking finding. Planned principal12-case gate covers shared
formula, real human/computer result paths and atomic admission; adjacent9 covers
Corpse Preservation and ordered cohorts. Data/inventory19 and UI source guard
pass; native acceptance and commit/push remain pending. No playable promotion.
After the environment transition,70772's handle is missing and a process check
confirms no surviving build/compiler. Its log ends77/257 without linking; this
is an interrupted build, not acceptance. Resume the same incremental target
withUP186-resumed-build.log; do not execute the stale test binary.
Resume9620 exits0 (180/180). Tester remained pending initialization after the
environment transition; root explicitly cancelled that assignment and ran the
focused native gate directly. Principal12 runs11pass/1fail, zero skips,3.270s;
retainUP186-principal.log/XML. The computer-winner fixture hits its ten-dialog
limit with an ordinary HeroLevelUpDialog still open, not NecromancyChoice.
Root increases only that bounded fixture drain to64, preserving no-choice and
actual army assertions. Production is unchanged; retry22923 is live, log
UP186-fixture-retry-build.log. Adjacent tests wait until principal acceptance.
Retry22923 exits0 but principal retry still11/12 (19.373s): increasing the drain
does not repair the fixture. Trace identifies missing onAdvInterfaceReady in the
compact computer case; unprompted level-up packets are never emitted/applied.
Root adds both simulated controller-ready signals, matching the admission
fixture's existing setup, and restores the original ten-dialog bound. No
production validation change. Ready-build71025 is live, logUP186-ready-build.log.
Final acceptance:71025 exits0. Principal12/12 passes2.383s; adjacent9/9
passes1.778s, zero skips. Data/inventory19/19, module consistency and result-text
guard pass. Independent frozen production review finds no blocker. Final binary
SHA-25670900e308674b933b1ba3835d5a78085aad55bbc5af83e85fd7f785086c9b5ae.
No new registry activation:197/310 active,113 planned remains unchanged; this
repairs already-active Dark Conversion's specification fidelity. Broader
interactions, actual full-AI play and rendered delivery remain Phase2/acceptance.
No local playable promotion. Next is UP184's approved Wight conversion.

## UP-184 — Necromancy Soul Harvester

Status: Completed source/native,2026-10-03; playable delivery not claimed.
Historical implementation trace follows. Implement the canonical
Advanced perk's automatic conversion of complete groups of six Skeletons
generated from eligible Elite casualties. Map category-specific generation,
atomic multiple-output admission, post-battle feedback and minimum AI hooks.
The specification names Wight but its faction roster classifies Wight as Core;
do not silently select a different Elite output. Check and flag this conflict.
Acceptance requires faithful category filtering, retained remainders, actual
raising, capacity rejection without partial mutation, registration and focused
native evidence. No activation or coverage claim from exploration.
Map complete: use captured battle category rules and eligible per-creature
counts; do not infer tier from legacy creature levels. Wight is Core in both
the canonical roster and runtime category data. Asked whether to retain the
explicit named Wight or use an Elite output; no replacement chosen. Soul's
implementation waits on that answer while UP186 repairs its Core conversion
dependency. Preserve global base rounding and classify only source-tier
generated whole Skeletons for tier-specific conversions.
User explicitly chose the named Wight. Canonical and registry descriptions now
state that Wight remains Core-tier and only the input casualties are Elite-tier.
The output ambiguity is resolved; the perk remains planned pending actual
implementation after UP186's focused acceptance boundary.
Implementation starts on committed e8f2cb4b5. Root selects the existing global
base floor with separately floored Elite input and automatic six-Skeleton Wight
groups; Core Zombie conversion remains independent and all remainders remain
Skeletons. Capture explicit battle category rules and provenance-filtered
casualties. Extend the authoritative result with Wight count and guarded wire
representation, atomically admit all three outputs, and show actual result
counts without frontend calculation. Three bounded Luna lanes own runtime,
result-text/components and focused fixtures; root owns version/enclosing guards,
activation, builds and Git. No coverage claim until native acceptance.
Previous notices37135635152 succeed on e8f2cb4b5; previous full Windows build
37127577580 succeeds on756d225818. Neither includes this new Soul source.
Production runtime/UI/version integration is frozen; independent Astra review
reports no blocking source finding. Soul is registered active for principal
validation, not yet accepted as completed coverage. Data/inventory19/19 and UI
result guard pass. Root client-only 12-job build95124 is running, with log
UP184-client-build.log; focused fixtures are still being completed independently.
Full Windows37136224312 runs committed e8f2cb4b5, not these uncommitted edits.
Wight outputs append under NEW_HORIZONS_NECROMANCY_WIGHTS; older readers default
zero, and unsupported nonzero outputs reject before result/outer payload writes.
No local playable promotion or rendered acceptance is claimed.

Client95124 exits0. Focused fixtures are frozen against the active production
registry with no activation override. Root test build53850 runs12 jobs, log
UP184-test-build.log. Independent final review has no blocker. Deferred Phase2:
the combined category case checks group remainders but not fractional carry
between category pools; broad full-AI play and rendered acceptance also remain.
Native focused execution waits for this freshly rebuilt vcmitest binary.
Test53850 exits1 on a fixture-only `final` declaration incompatible with Google
Test's generated subclasses. Tester removes only that qualifier and freezes
again; root resumed incremental build15042, logUP184-test-retry-build.log.
Production sources remain unchanged. The regression lesson is recorded in
NH_RELEASE_FAILURES.md; no stale-binary native acceptance is claimed.
Final acceptance: retry15042 exits0. Luna tester principal20/20 passes4.193s
and adjacent9/9 passes1.718s, zero skips. All five battle cases record active
production registry/no override; four select Soul normally after Basic Dark
Conversion and the negative control does not select it. Actual army/result
counts, atomic rejection, direct/outer version reset and zero-byte downgrade
guards pass. Final binary SHA-256:
cf6fe68c13be8424f92e519508ddca19e1d6bb5d9f31f072b11fd553e6bc63f8.
Data/inventory19/19, module check, UI guard and independent review pass.
Coverage197->198/310 active,113->112 planned; faction56->57/90, Necromancy4->5/10.
Broader interactions, fractional category carry, actual full-AI play/rendered
acceptance remain Phase2. Dedicated art is missing. No playable promotion.
Next is UP185 Master of Bones; full Windows37136224312 remains e8f2cb4b5 only.

## UP-185 — Necromancy Master of Bones

Status: Completed source/native,2026-10-03; playable delivery not claimed.
Historical implementation trace follows. Map the canonical
Expert perk's upgraded Skeleton output and the condition that the appropriate
Necropolis upgrade is available to the player. Identify existing ownership,
building/upgrade APIs, result representation and minimum AI consumers; flag
genuine availability ambiguity before editing production. This preparation
does not displace UP184 or claim implemented coverage.
Map complete: owned towns expose built upgrade dwellings and their actual
offered creatures; Skeleton's configured upgrade is Skeleton Warrior. The
natural availability interpretation is a currently owned, built appropriate
upgrade, not foreign ownership or a merely buildable upgrade. A new explicit
Skeleton-output form in the result will be needed for mixed upgraded-Skeleton
and Zombie output, with matching wire protection and UI consumption. This
remains the next bounded coverage candidate after UP186, not current source.
Implementation starts on committed12431082e after UP184 acceptance. Root selects
current owned Necropolis towns with a built appropriate upgrade dwelling; mere
buildability or foreign ownership cannot grant upgraded output. Resolve the
configured Skeleton upgrade at post-battle authority time, apply it only to
remaining Skeleton output, and retain independent Zombie/Wight conversion and
atomic Leadership/slot admission. Three bounded Luna lanes own runtime, result
UI consumption and focused fixtures; root owns serialization/version/packet
guards, activation, builds and Git. No coverage claim before native acceptance.
The new explicit skeletonCreature result field uses NONE for base/legacy output
and the actual upgraded CreatureID when applicable, including mixed rewards.
Notice37137524285 succeeds on12431082e; full Windows37136224312 still runs
preceding e8f2cb4b5. No local playable promotion is inferred from either.
Production runtime/UI/root guarded-wire integration is frozen. The form is
appended under NEW_HORIZONS_NECROMANCY_SKELETON_FORM and requires positive
Skeleton output; older records reset NONE, unsupported direct/outer writes
reject before payload. Generated/conversion labels remain base Skeleton
equivalents; delivered labels/components use actual output form. Registry is
active for acceptance, not yet completed coverage. Data/inventory19/19,
module consistency and result guard pass. Root client build57879 runs12 jobs,
logUP185-client-build.log. Reviewer follow-up failed with a thread-limit error;
team inspection and fresh bounded Astra reviewer spawn succeeded. Tests remain
independently in progress; no stale-binary acceptance or playable promotion.
Client57879 exits1 on an interface/concrete Creature upgrade-access mismatch in
the new helper. Runtime owner repairs only the lookup; independent reviewer
confirms the same compile blocker and otherwise reports coherent semantics.
Preserve UP185-client-build.log and record lesson in NH_RELEASE_FAILURES.md.
Do not execute the prior binary as new-source acceptance.
Runtime repair uses the concrete creature registry, preserving the configured
upgrade intersection. Astra reviewer confirms no remaining source blocker.
Root incremental client retry43912 runs12 jobs, logUP185-client-retry-build.log.
The independent runtime worker now maps only Death Lord/Grave Knowledge's
weighted casualty seam read-only while this accepted-source build remains frozen.
Client retry43912 exits0. Data/inventory19/19, generated module and result guard
pass. Focused tests cover ordinary Expert selection plus owned built/unbuilt,
foreign built and absent upgrade availability; root is waiting for their freeze
before compiling vcmitest. Independent final fixture review is read-only.
Fixtures frozen. Root test build65198 runs12 jobs, logUP185-test-build.log.
Final fixture review has no blocking finding; building construction/capture
refresh is explicitly deferred rather than certified by the prepared-town
fixtures. Wait for this exact build before executing native tests.
Final acceptance: test65198 exits0. Luna tester principal26/26 passes5.386s and
adjacent9/9 passes1.707s, zero skips. Four map-town cases record production active,
no override, ordinary BasicCP->AdvancedSoul->ExpertMaster selection and actual
army output; owned built upgrades apply, owned unbuilt/foreign built/absent do
not. Mixed-output form/atomicity and direct/outer version reset/rejection pass.
Binary SHA-256b5612702c235e3d66403429999fe6838558e13635680337d701ace6e3ba276c9.
Data/inventory19/19, generated module/result guard and independent review pass.
Coverage198->199/310 active,112->111 planned; Necromancy5->6/10; faction57->58/90.
Construction/capture roster refresh, broader interactions and full-AI/rendered
acceptance remain Phase2. Dedicated art is missing; no playable promotion.
Next prepared slice: Death Lord/Grave Knowledge weighted eligibility, recorded
in the sprint register. Existing full Windows37136224312 remains e8f2cb4b5 only.

## UP-187 — Death Lord and Grave Knowledge special casualty conversion

Status: Completed source/native, 2026-10-03; playable delivery not claimed.
Historical implementation trace follows. Implement the two missing
Advanced Necromancy perks from captured, provenance-filtered original-form
casualties. Death Lord converts Construct/Elemental inputs at one quarter of
the normal rank/Bone Collector rate; Grave Knowledge reclaims Undead at a fixed
20%. Mechanical, summoned, cloned and destroyed remains do not qualify;
ordinary magical casualties still require Corpse Preservation. Preserve the
ordinary living pool's floor and separately floor each special pool, then
combine category contributions before automatic Dark Conversion/Soul Harvester.
Soul Harvester retains the explicitly approved Core Wight output.
Three bounded Luna lanes own runtime, packet-driven result text and focused
fixtures. Root owns the appended version boundary, direct/enclosing guards,
activation, serialized builds and Git. Acceptance requires actual army outputs,
perk-absent and old-capture negatives, atomic admission, category/rate tests and
wire roundtrips/rejection. No coverage increase or playable delivery is claimed
before focused acceptance; broad interactions remain Phase 2.
Client13126 exits0. Data/inventory19/19, generated module and result UI guard
pass; independent Astra source review has no blocker. Focused fixtures remain
in progress, so no stale vcmitest run is accepted. Full Windows37136224312
completed successfully on e8f2cb4b5; dispatch the next full only after this
coherent checkpoint is committed and matching notices pass. No playable promotion.
Fixtures are frozen after correcting the old-writer setup and ensuring actual
Golem/Vampire magical casualties. Root test build86643 runs12 jobs, log
UP187-test-build.log. Canonical Ossuary clarification changes source identity;
registry hash and generated module were updated, data/inventory19/19 pass again.
Wait for this fresh binary before native acceptance; no broad suite is required.
Test86643 exits0. Principal32/32 passes6.689s, zero skips; adjacent11/12
passes with one new Grave Knowledge Vampire spell-submission failure, before
its casualty assertions. Preserve UP187-adjacent.log/XML. Tester diagnoses
initiative/window setup before any repair; no weakened production validation or
full acceptance claim. Actual new principal cases record active/no override and
normal Basic-perk then Advanced selection. Native completion remains pending.
Final acceptance: fixture-only retry17335 exits0. Principal32/32 passes6.716s
and adjacent12/12 passes2.607s, zero skips; original failure remains preserved.
Production active/no override and normal Basic-perk then Advanced selection are
recorded, alongside actual army output, magical/Disintegrate capture and direct/
enclosing current/old wire behavior. Binary SHA-256:
212ea29fb37c2f95a844e452174c6b5db40da917d08d432abf4b57cacd77d07c.
Data/inventory19/19, generated module/result guard and independent review pass.
Coverage199->201/310 active,111->109 planned; Necromancy6->8/10;
faction58->60/90. Broad interactions/full AI play/rendered acceptance remain
Phase2, dedicated art remains missing. No local playable promotion.
Next UP188 Ossuary; UP189 awaits the named high-tier output.

## UP-188 — Necromancy Ossuary destination fallback

Status: Read-only preparation, 2026-10-03. Implement the canonical nearest
owned Necropolis fallback for raised creatures the hero cannot admit, preserving
atomic multi-output planning and authoritative town-garrison mutations.
The existing planner combines slot and Leadership failures into one empty result;
asked whether Ossuary covers both causes or only unavailable army slots. Do not
silently choose that gameplay scope. Existing nearest-town precedent uses squared
two-dimensional distance over the owner's town list; no global town scan is
needed. Town garrisons remain seven-slot armies without Hero Leadership caps.
UI/result destination identity and guarded representation will be needed.
This mapping does not activate the perk or displace UP187 native acceptance.
User resolved the scope: both Leadership limits and unavailable army slots
trigger the fallback. Canonical Markdown and registry descriptions now include
both; the perk remains planned pending source/native implementation. Follow
the town's normal visible upper-army destination, not a hidden town-only army
when a garrison hero exists; do not transfer to its merely visiting hero.

## UP-189 — Necromancy Lord of the Dead

Status: Read-only preparation, 2026-10-03. Map the missing Expert perk's
pre-conversion replacement of12 base Skeletons after a qualifying living
Champion army. Check whether its faction-defined high-tier Undead output is
actually specified/bound before implementing; do not silently choose a creature.
One bounded Luna explores only this species/ordering seam while UP187 native
acceptance remains the active source checkpoint. No activation or coverage claim.
Map confirms no output binding in the canonical row, perk registry or category
data. Necropolis's Champion line is Bone Dragon/Ghost Dragon, both Undead;
asked which form should be the explicit Lord of the Dead output. Do not infer
upgrade availability or substitute a species without resolution.
User selected Bone Dragon. Canonical Markdown and registry descriptions now
name that output explicitly; the species ambiguity is resolved. Runtime remains
planned pending pre-conversion accounting, atomic output/admission and native
acceptance. This clarification does not add a coverage item by itself.

## UP-183 — Necromancy Corpse Preservation

Status: Completed source/native,2026-10-03; playable delivery not claimed.
Historical implementation trace follows. Missing Basic perk: ordinary magical
damage casualties remain eligible for Necromancy unless an effect explicitly
invalidates remains. Current runtime reads the perk but the coverage audit
reports no eligibility effect. Map casualty provenance from actual damage
through BattleResult/Necromancy, explicit corpse-destruction exclusions and
minimum AI/value seams. Do not treat disintegrated casualties as eligible or
limit the implementation to an inert registration flag. Root owns architecture
and activation; no source changes or coverage claim from mapping.
Map complete: ordinary magical deaths already qualify without the perk and
the selected flag is only copied into the result summary. Explicit unusable
remains from Disintegrate are correctly separate. Asked whether to exclude
ordinary magical casualties without the perk or retain the baseline and redesign
the redundant perk. A meaningful gating implementation would require saved
per-casualty damage provenance (including restoration/form consistency), not
an inert flag activation. Do not change baseline eligibility silently.
User explicitly approved excluding ordinary magical casualties without Corpse
Preservation. Disintegrate remains excluded even with the perk. Integrated this
decision into the canonical Markdown and registry description. Runtime is still
unchanged and the perk remains planned: next implement saved casualty provenance,
restoration consistency, authoritative result filtering and focused real-damage
tests. Do not claim this documentation decision implements the perk.
Follow-up trace confirms common Lua spell damage currently reaches health as
OTHER, despite native damage paths carrying explicit SPELL/PHYSICAL provenance.
Both visible and original Battle Form health need the actual damage nature;
Disintegrate destruction remains independent. A new genuine ambiguity is partial
Resurrection after mixed physical/magical deaths: current aggregate restoration
does not identify which casualties returned. Asked whether restoration takes
most recent, physical-first or magical-first casualties. Do not silently choose
an allocation, activate an inert perk, or claim the no-resurrection case is full
coverage. Continue the unblocked UP181/182 acceptance meanwhile.
User resolved restoration allocation: most recent usable casualties first.
Integrated into the canonical Necromancy section. Restore in reverse casualty
order, retain damage nature for remaining corpses, and assign the new cause on
subsequent death. Explicit destroyed remains remain non-restorable. This resolves
the design blocker; a saved ordered casualty ledger is now the next foundation,
not a scalar magical-death counter with arbitrary restoration allocation.
Root selects ordered usable casualty cohorts with damage nature and temporary
restoration identity. Permanent restoration removes newest usable deaths;
one-battle restoration keeps their prior cause/order for expiry, while re-death
replaces the old identity with the new cause. Battle Form original-health ledger
owns provenance; the transformed health view is only the HP projection. Legacy
snapshots cannot reconstruct prior causes: retain unknown prior deaths
as OTHER (legacy eligibility), never fabricate magical provenance. New damage
receives explicit classification. Save/network loss guards must preserve ordered
state. Implementation starts after UP181/182's frozen acceptance/commit boundary.
UP181/182 source was committed/pushed as1c2b7cf2c5d7839f2dd6f15f2d93ec337191501f.
Matching Windows notices37123346422 succeed. Full Windows37123447269 is live on
that exact revision; it includes Portal/Grand Tactics/Mountaineer, not UP183's
new dirty source. Re-poll that live handle, do not dispatch a competing full build.
UP183 implementation is delegated with bounded ownership: health/CStack/ordered
provenance, explicit Lua damage ingress, and focused actual-cast fixtures. Root
owns authoritative result filtering, version/outer guards, registration and builds.
Existing binary battle descriptors omit general CUnitState: do not append a
casualty-only sidecar and claim it restores matching health/resurrection. JSON
health/state packets preserve full provenance; binary descriptors fail closed on
nonrepresentable provenance until real full combat-state serialization exists.
Ordinary adventure saving remains supported. This is not a new midbattle-save
feature or a claim of existing ongoing-battle save support.
Core1826 and client18663 pass; test50692 is compiling. Follow-up independent
review confirms one blocking legacy-JSON regression: omitted optional original-
form health reaches the new validator as null. Root repaired null-as-absent
handling while retaining non-object rejection; a focused legacy-snapshot fixture
is being added. The ongoing compile is not a frozen final-candidate claim:
rebuild affected targets after this repair before native execution. Do not run
the tester against the earlier binary.
Frozen all-target77992 passes after the null fix; binary SHA-256
8ca510882e75aa39e0f7ed685c1ae747e383dd9096f499cf3cf609ec596be317.
Principal9 runs with zero skips: pure health4 pass, battle fixtures5 fail.
Retain UP183-principal.log/XML. Fixture-only causes include damage's in/out value
being actual HP consumed (not remaining damage), removed initial troops counted
as dead, injected troops lacking original-army result baseline, and wrong-side
spell timing after a shot. Owner is replacing injected troops with real prebattle
armies and legal action timing, preserving actual filtered raising assertions.
No activation or accepted coverage yet; tester stops before adjacent execution.
Final acceptance: fixture retry48299 passes after repairing34931's nonexistent
getter. Principal9/9 and adjacent15/15 pass, zero skips,1.751s/1.740s. Registry
is active; generated module and active both-target build pass. Production-active
9/9 passes1.794s with all five XML properties active and override false.
Data/inventory19/19 and module drift pass after repairing an inventory-column
mix-up. Independent review passes; the legacy-null defect is repaired and its
omitted-field/malformed-field regression assertions pass. Final binary SHA-256:
001072515cdc1f22f068c038ffc242c304cfb4b84fe780c3128b37bd4650a77a.
Coverage196->197/310 perks, planned114->113; Necromancy3->4/10, faction55->56/90.
Ranks84/93 and spells60/67 unchanged. Broad restoration/form interactions and
midbattle persistence remain Phase2; art Not done, generic UI Provisional.
No local playable promotion. Windows37123447269 succeeds on the prior1c2b7cf2c
source, not this new slice. Root proceeds to coherent commit/push.

## UP-180 — Spellcraft Counterpressure

Status: Bounded read-only preparation,2026-10-03. Missing Advanced perk:
after an enemy hero casts a spell affecting the hero's army, the next spell
before the end of the next round gains20% on its Spell Power-derived component.
Map actual affected-target provenance, accepted cast timing, shared numerical
consumers, saved state and detached AI. Preserve flat bases, spell costs and
action economy. Portal's frozen build/native acceptance remains priority; no
product edits, registration activation or coverage claim from this map. Report
any genuine trigger/consumption ambiguity rather than silently narrowing scope.
Map complete: BattleSpellCast affectedCres records resolved eligible recipients,
not necessarily a changed effect (a no-op Dispel may still appear). Asked whether
the trigger requires an actual stack change or merely a valid non-resisted
recipient. Negated casts skip beforeCast and have no affected recipients;
creature casts and rejected requests must not arm the perk. Use independent
side-scoped R+1 readiness, snapshot the shared SP-term coefficient before accepted
own-cast consumption, and copy/consume readiness only in the detached AI branch.
If actual changes are required, reuse effect packet recording rather than infer
them from targeting. Do not fold readiness into Warcasting or repeat this map.
No production edit or coverage activation until the trigger boundary is resolved.

## UP-179 — Chaos Reality Warp and Reality Breaker

Status: Bounded read-only preparation,2026-10-03. Missing canonical Level4
combat identity swaps all transferable temporary magical buffs and debuffs
between one friendly and one enemy stack, preserving remaining durations.
Orders, intrinsic/permanent/equipment effects, terrain, summon identity,
transformations and explicitly non-transferable effects do not move. Effects
with an illegal recipient remain on their original stack. Reality Breaker
permits any two legal stacks instead of the friendly/enemy pair. Map the whole
effect representation, paired targeting, accepted authority and minimum AI;
do not substitute a bonus-only swap if other transferable effects use saved
unit state. Master Synthesis's frozen build/native acceptance remains priority.
No source edits, activation or coverage increase from this preparation.

## UP-176 — Shroud Vanish

Status: Bounded read-only map,2026-10-03. Destroying an enemy with a flanking
melee attack permits movement up to half Speed, without another attack. Map
accepted kill classification and existing movement-only follow-up state,
authoritative legality/action economy, required UI and AI. Do not substitute
an extra full activation or force automatic movement. Night Prowler's frozen
build90975/native acceptance remains the immediate priority; no edits/activation
or coverage claim from mapping. Record any genuine rounding/stacking ambiguity.
Read-only map is complete. Existing Pursuit supplies a saved, authoritative
same-activation move-or-decline continuation with movement-only UI/AI, but its
unused-approach allowance is not Vanish's half-Speed allowance. Existing half-
Speed rules floor positive integers. Accepted direct nonsecondary flank/kill
must be captured before/after the hit packet; broad destroyedEnemy includes
collateral and is insufficient. Asked whether retaliation kills also grant a
follow-up, and whether simultaneous Pursuit/Vanish allowances use their maximum
or sum. Own-activation question explicitly includes a direct Cleave strike.
Do not silently inherit Offense ownership or schedule an extra full activation.
No source edit/activation/count from the map; retain the existing continuation
seams for implementation after the narrow rulings.

## UP-170 — Shroud No Escape

Status: Source/native verified and active,2026-10-03. A target suffering a flanking
melee attack loses2 Speed until its next activation. Reuse actual accepted
flanking classification, timed effects and shared AI projection. Do not apply
to ordinary ranged attacks or unclassified attacks. Root chooses implementation
after the bounded map; no activation/count from exploration.
Map establishes an unblocked full path: shared battleIsShroudFlankingAttack
classifies rear physical melee, excludes ranged/collateral, and includes a
retaliation only when it itself qualifies. Capture eligibility before accepted
damage; apply-2 Speed to the surviving direct target using the existing
UNTIL_NEXT_CREATURE_ACTIVATION duration and nonstacking refresh. Existing saved
bonus representation and HypotheticBattle expiry are reused, with no new polling
or action. Separate Luna owners implement runtime/helper, candidate-local AI,
and an isolated unregistered fixture. Root owns registration, builds and Git.
Registry remains planned until principal native acceptance; counts unchanged.
Dead-target/resurrection status interactions remain explicit Phase2 follow-up.
Frozen runtime and candidate-local AI both compile: serialized root build42759
exits0 for vcmiclient and vcmitest. Log:
build/new-horizons-linux/testing/UP170-no-escape-baseline-build.log.
Independent review finds no blocking runtime/AI defect. Eligibility belongs to
the attacking stack's current-controller hero, not the victim's hero; detached
preview uses visible heroes and keeps refreshes inside its candidate branch.
Principal fixture remains pending; no activation or coverage increment yet.
Visible feedback includes the actual reduced Speed value and an explicit combat
log entry. The generic creature-window bonus list can display this description,
but groups Speed bonuses and may show another modifier's description instead.
Guaranteed separate status labeling is a Phase2 UI follow-up, not claimed here;
there is no dedicated Speed tooltip or purpose-made perk artwork.
Windows run37094808848 completes successfully on Investor21dbb224b. It does not
include Field Study or this dirty No Escape work. The next full build requires
a passing notice preflight for its exact committed source.
Four-case principal fixture is registered; both-target build83393 exits0.
Independent fixture review blocks acceptance: blockRetaliation on the victim
does not suppress its response. Correct the fixture to prevent retaliation on
the attacking stacks and assert surviving negative controls before native
acceptance. This is a fixture-control defect, not a production failure.
Initial native gate runs4 cases in8.101s:2 pass,2 fail,zero skips. The log
confirms live No Escape triggered, but automatic queue progression activates
the fast Angel victim before the post-action assertion, correctly expiring the
bonus. Repair the observation interval: spend the victim's real activation
first and retain an unacted reserve, then test refresh before its next genuine
activation. Do not change production duration to satisfy a stale observation.
Fixture-only const/interface compile repairs precede both-target retry3 build33849
exit0. Principal retry passes4/4 in8.112s, zero skips. Root activates production
registration/module/allowlist/inventory only after acceptance. Data/inventory
19/19 and module drift pass; activated both-target build exits0. Final native
gate passes4/4 in8.145s, zero skips, using the active registry without synthetic
override. Independent final review finds no blocker. Coverage188/310 perks,
122 planned; faction50/90 and Shroud2/10; ranks84/93 unchanged. Native SHA-256:
a9cb4afb3fd1184af1e2825e6f55791a3d9b8a57a4353bcc5a0f002fa0fcb02e.
Full-game resume, unusual activation/resurrection interactions, hidden-enemy
valuation and separate status labeling remain Phase2. Purpose-made art is Not
done; generic UI is Provisional. No immutable playable promotion.

## UP-164 — Learning Master Teacher

Status: Blocked on Mentor-prerequisite answer (map complete),2026-10-03. Expert perk extends Mentor to
the first two different lower-level allied heroes met each week, awarding500
times the mentor's level to each. Map existing weekly meeting provenance,
authoritative XP award, saved state, rank/prerequisite gates and minimum AI
hooks. Reuse Mentor's existing trigger; do not introduce periodic polling or
grant both ordinary and upgraded XP on the same meeting. Root chooses exact
state representation after mapping; no activation/count from preparation.
Map complete: current Mentor reuses authoritative exchange/town hooks and a
single weekly marker. Two different recipients need saved recipient identities,
not merely a second counter. Expert progression allows other Basic/Advanced
Learning perks; canonical wording names Mentor without explicitly requiring
its selection. Asked whether Master Teacher works independently or requires
selected Mentor. Await that prerequisite answer before activation/implementation.

## UP-165 — Learning Archivist preparation

Status: Blocked on UP-054's existing Adventure-scroll policy,2026-10-03. Acquiring a spell scroll
permanently teaches its spell immediately when legally eligible. Map artifact
acquisition/transfer settlement and existing shared spell-learning policy.
Inspect UP-054's pending neutral Adventure acquisition ruling before choosing
work; do not activate a combat-only subset that silently drops authored scope.
No edits or coverage claim from exploration; root chooses implementation after
the map and records a shared blocker rather than repeating an unresolved ask.
Map complete: direct gifts use NewArtifact, map pickup uses PutArtifact, and
hero transfers use BulkMoveArtifacts. A complete authoritative postacceptance
hook must cover all three, excluding same-hero rearrangement. ChangeSpells and
canLearnSpell provide ordinary receipt/persistence/AI visibility; no extra saved
counter is needed. Neutral Adventure spells have separate Guild unlock rules
and the pending UP-054 policy determines legal scroll learning. Do not implement
or activate a combat-only subset; no duplicate question is issued.

## UP-166 — Estates Prospector preparation

Status: Blocked on Gold-mine scope answer (map complete),2026-10-03. The first owned mine visited
by the hero each week grants+2 of its common resource or+1 of its rare resource,
according to normal output type. Map authoritative visit/ownership events,
weekly saved hero provenance and existing AI/tooltip consumers. Check canonical
resource classifications before inferring Gold behavior. No source activation
or coverage claim from this preparation; prefer event-driven state over scans.
Map finds campaign selectors classifying Wood/Ore as common and Mercury/Sulfur/
Crystal/Gems as rare; Gold is neither. Asked whether Gold mines are excluded
without spending the weekly use or have a separate Gold reward. SAME_PLAYER at
visit entry is the eligible owned-mine event; capture remains Land Surveyor's
separate hook. Existing last-use property/save pattern and selected-hero mine
hover text are reusable. AI needs a one-shot hero/week value, not a change to
recurring mine income. No implementation or activation before the scope answer.

## UP-167 — Armorer Unyielding preparation

Status: Blocked on missing displacement foundation (map complete),2026-10-03. Friendly stacks Defending or
affected by Hold the Line cannot be forcibly displaced by non-magical effects.
Map actual displacement producers and shared live/AI legality, reusing effective
Order lifetime and Defending state. Do not blanket-disable magical relocation or
ordinary voluntary movement. No source edits/count from preparation; root chooses
the full event-path implementation after mapping.
Map confirms the existing Deep Bulwark finding: no canonical nonmagical
forced-displacement producer exists in current source. Ordinary moveStack is
voluntary movement and spell relocation is magical, so neither is a faithful
acceptance path. Defending and effective Hold the Line predicates already exist;
do not activate inert protection or invent an unrequested knockback mechanic.
Keep planned pending that foundation; no new design question is necessary.

## UP-168 — Estates Magnate preparation

Status: Blocked on ownership/stacking answers (map complete),2026-10-03. At week start, the most
recently visited owned town from the previous week produces+500 Gold per day
for the next7 days; no qualifying visit means no effect. Map existing town
meeting provenance and weekly income publication, saved state and shared
AI/tooltip consumers. No arbitrary town choice, polling or retroactive first-week
bonus. Root chooses event-driven architecture and safe file ownership after
mapping; no activation/count from preparation.
Map complete: HeroVisitCastle is the entry event; current residence clears on
leaving and is not historical provenance. Save the latest qualifying town per
hero and consume/reset it at week boundaries. Publish a saved active town-income
snapshot through NewTurn, with prospective week-start receipts like Investor.
CGTownInstance::dailyIncome is shared by server receipts, town/kingdom UI and
Nullkiller; no periodic map scan is needed. Day0 has no prior-week visit.
Asked whether ownership is required both at visit and week start, whether capture
ends the active bonus or transfers it to the new owner, and whether different
Magnate holders stack at the same town. Await these payout-affecting decisions
before implementing; do not silently select a recipient or stacking rule.

## UP-162 — Learning Eagle Eye preparation

Status: Bounded read-only preparation,2026-10-03. After combat, learn the
highest-level eligible Level1–3 spell cast by the enemy hero, breaking equal-level
ties by first cast. Map existing accepted hero-cast history, postcombat learning
policy and publication, rank/perk gates, saved battle history and AI receipt.
No source edits while Field Study owners/builds are active. Reuse shared learning
legality; do not grant removed/unavailable spells, bypass learning-school ranks,
include creature spells or choose a later equal-level cast. Root chooses the
implementation after this bounded map; exploration does not increase coverage.
Map complete: accepted HERO_SPELL StartAction appends IDs to saved ordered
usedSpellsHistory; creature casts are excluded. Existing canLearnSpell handles
school acquisition, roster/map bans and already-known spells. battleFinalize's
legacy Eagle Eye path is winner-only, random and may grant several spells;
replace its selection with highest eligible Level1–3/earliest tie, not a new
history counter. Existing BattleResultsApplied/ChangeSpells publishes learned
spells and informational UI; generic active-perk AI selection is sufficient.
Asked whether losing heroes surviving retreat/surrender also learn, or only
the winner, or every participant including removed heroes. Canonical wording
does not explicitly restrict victory; do not silently import legacy winner/unit
gates. Await that scope answer while UP161 acceptance remains unblocked.

## UP-163 — Learning Scholar preparation

Status: Bounded read-only preparation,2026-10-03. When allied heroes meet,
each teaches the other their highest-level legally learnable unknown spell;
ties use canonical spellbook order, once per hero pair per week. Map the
existing exchange/town-meeting hooks, shared acquisition legality, paired
weekly history and replicated spell grants, with basic save/AI consumers.
No production edits during Field Study's frozen builds. Preserve asymmetric
eligibility (one hero may learn while the other cannot) and per-pair, not global
weekly, accounting. Root will select architecture after the bounded map.
Map complete: existing useScholarSkill is called by allied heroExchange and
town visitor/garrison meetings; it currently grants all legal spells both ways
under legacy level limits. Reuse canLearnSpell and ChangeSpells; add authoritative
per-pair weekly provenance (Mentor's per-hero marker cannot represent this).
Stored spellbooks use stable SpellID order, while rendered books sort partly by
localized names. Asked whether one Scholar holder enables both directions,
whether a meeting with no possible transfer consumes the weekly use, and whether
stable stored SpellID order defines canonical tie order. Await those decisions
instead of implicitly importing legacy behavior; Field Study remains unblocked.

## UP-160 — Estates Investor

Status: Verified (source/native; playable delivery pending), 2026-10-03. At the start of each week,
snapshot the hero owner's current treasury: Estates daily income for that week
increases by50 Gold for each full5,000 Gold, capped at250 daily Gold. Map the
existing weekly publication, hero income, saved hero state and shared AI quote.
Do not recalculate against treasury on every income/render/AI update, apply
weekly interest instead of daily income, or grant the perk retroactively at
midweek selection. Root chooses architecture after mapping. Required evidence:
legal acquisition, exact threshold/cap, weekly refresh, current owner, daily
income receipt, persistence and minimum shared AI visibility.
Map complete; root chooses a typed NewTurn per-hero weekly snapshot plus a saved
hero daily-Gold value, default0. Weekly refresh includes clearing inactive or
unowned old values and seeds day0->day1 without a special first-day payout.
Sample pre-packet treasury, consistently with Financier; the new week's first
regular receipt uses the prospective snapshot, not the old week's value.
Income retains ordinary current-owner handicap and AI-income policy; the bonus
is hero-bound for that week. Shared dailyIncome feeds Nullkiller without a second
treasury calculation. Runtime owns hero/turn packet/visitor/processor files,
tester owns an isolated server fixture, AI worker owns only the existing Estates
AI fixture; root owns serialization version, CMake, activation and integration.
Production and fixtures are source-frozen. The existing TavernHeroesPool daily
loop clears expired Investor snapshots at week start before skipping unused
heroes, preventing stale bonuses after a later rehire. Five server cases and
three new AI cases are staged; rank income is measured separately from Investor.
Data/inventory19/19, module drift and diff checks pass. Combined client/test
build81506 runs with12 jobs, log testing/UP160-investor-build.log. Registration
remains planned and coverage185/310 unchanged. Do not run a stale native binary.
Review finds one fixture-only blocker: the old-format pre-byte hero assertion
serializes a pointer, whose metadata is emitted before the hero guard. After
81506 terminates, change only that guard test to serialize *firstHero and retain
the separate pointer roundtrip. Do not weaken the zero-byte object guard or
claim graph-level atomic serialization. The current candidate is not native
accepted; build retry after that bounded fixture repair before the14-case
Investor/Estates-AI/Financier gate. No production blocker found by review.
Build81506 terminates with exit1: the new fixture has a redundant namespace
close and missing defining ObjectTemplate/bonus updater/propagator includes for
hero serialization. The fixture owner repairs those and the pointer-guard test
without changing production or dropping persistence checks. Original build log
is retained; no native acceptance or active coverage yet. Rebuild both targets
once the repair is frozen, then run the14-case focused gate.
Fixture repair is frozen: reuse FullGameSnapshotTypes.h, remove the redundant
closing namespace and serialize *firstHero for the guarded-payload assertion.
Pointer roundtrips and persistence checks are retained. Combined retry45920
is confirmed live with12 jobs, log testing/UP160-investor-build-retry.log.
Package preflight91/91 passes. Re-poll45920 before native execution or another
build; stale binaries are not acceptance. Registration remains planned.
Retry45920 terminates with exit1 on the new AI fixture's mutable town list.
The quote needs a const PlayerState view, not a production API change. The AI
owner repairs only the fixture; the server fixture now compiles. Hold native
execution until a further serialized both-target retry exits0. Preserve both
failed logs; registration and verified coverage remain unchanged.
Combined retry2 40823 exits0 for both client and native-test targets, with12
jobs; log testing/UP160-investor-build-retry2.log. The frozen candidate's14-case
Investor/Estates-AI/Financier gate is running. No stale binary is used. Keep the
registry planned until the principal gate completes; no playable promotion.
Principal gate runs14 cases:13 pass,1 fails,zero skips in131.136s. The sole
failure compares standalone copied-hero income to a live-hero rank-income
baseline. CMemorySerializer::deepCopy does not rebuild the full bonus graph;
CBonusSystemNode exports restored bonuses only for loadingGamestate. Diagnose
using the copy's own baseline and preserve explicit active-perk, saved snapshot
and exact250 income-delta assertions. Full-game resume remains Phase2, not
acceptance implied by this isolated hero roundtrip. Preserve failed log/XML.
The bounded copied-hero assertion is repaired; retry3 both-target build exits0
and the single failed case passes1/1,zero skips in10.700s. Earlier13 passing
cases remain unchanged. Investor registry/module is now active; data/inventory
19/19, module drift and package91/91 pass. Activated build exits0 and five-case
native gate runs against the frozen source. Final Astra review finds no blocker;
full-game resume, unusual owner/rehire paths, rendered delivery and comparative
AI valuation are Phase2. Coverage186/310 perks,124 planned,Estates5/10;
ranks84/93 and faction perks49/90 unchanged. No snapshot promotion or GUI run.
Final activated Investor gate passes5/5,zero skips in68.870s. Both native logs
and XMLs retain the initial failure and bounded successful retry. Phase1
principal implementation is accepted; next missing unblocked item is UP161
Field Study. Source commit/push follows, with no playable-delivery claim.
Investor source is committed/pushed as21dbb224b972668054b6b07bf50908229408a8fd;
Windows notices37093465685 succeed on that source. Full Windows37091363403
remains live on older213b4a35e; do not describe it as Investor validation.

## UP-159 — Battlecraft Rapid Response

Status: Bounded read-only preparation, 2026-10-02. Once per round after an
enemy Creature Activation ends, the waiting friendly stack scheduled latest
in the current initiative order takes its delayed activation next. Map the
authoritative activation-end boundary, initiative selection, consumed-round
state, save representation and detached AI projection. This reorders an
existing delayed activation; it must not grant another activation or consume
the opportunity for an invalid recipient. No source edits while UP-158's
combined build is frozen. Return concrete seams and genuine design ambiguities;
root selects architecture before implementation and activation.
Map complete: use true completed-activation boundaries in onActionMade, not a
blanket activateNextStack hook. Select the reverse-most eligible friendly waiter
from battleGetTurnOrder's current-round queue, preserving initiative/tie rules.
WAIT and same-activation Pursuit/ranged/Gating continuations are not completions.
The unresolved timing choice is whether Rapid Response precedes immediately
earned new activations (Morale, Quartermaster, Second Wind) or follows them.
Interrupting those needs typed saved resumption rather than discarding an earned
activation. Ask the user; no registration change until that choice is resolved.
Binary CStack serialization omits existing runtime Wait state; a new per-side
used-round marker alone cannot establish full midbattle save fidelity.

## UP-158 — Battlecraft Redeployment

Status: Verified (committed/pushed; playable delivery pending),2026-10-02. Advanced perk: after
both armies complete initial deployment, retain the hero's normal deployment
interface for exactly one final relocation of a friendly stack to another legal
deployment hex before the first Creature Activation. Reuse the independent
deployment descriptor and authoritative whole-footprint movement guards; do not
grant a separate perk/Hero Action. Map stage transition, one-move consumption,
saved/packet representation and minimum human/AI handoff. Root chooses the
generic architecture before edits. Other mapped Battlecraft perks await their
recorded narrow rulings; no source activation or coverage increase from mapping.
Map complete and bounded implementation assigned. Root extends the generic
descriptor with separately versioned final-relocation ranges/completion flags;
all initial phases precede final phases, attacker then defender. A final-only
hero receives the normal base range1; Tactics extends that range to3. Existing
scenario restrictions and formation-enabled setting still apply. Runtime owns
setup/guards/accepted-action transition, UI/AI owns existing phase consumers,
tester owns a new isolated fixture. An accepted position-changing WALK consumes
the opportunity automatically; END passes; no-op/invalid moves do not consume.
Opening effects and first activation wait for all phases. Preliminary descriptor
review finds no blocker; parent serialization pre-byte guards and activeDistance
projections are mandatory. Registration remains planned, verified184/310.
Production runtime and existing human/AI phase consumers are frozen. Review
repairs same-controller initial-to-final UI selection; AI skips unchanged
destinations and passes if an alive request causes no displacement. Server
rejects unreachable/no-op final destinations before StartAction and retains the
opportunity after a surviving zero-displacement outcome. One proposed trap case
combines two Advanced Battlecraft perks and is not legally selectable; do not
forge that selection to claim principal evidence. Dead-before-displacement and
broader trap/callback interactions are Phase2. Four focused native cases use
legal progression with a fixture-local planned-to-active registry override;
production registration remains planned until acceptance. Root registers the
fixture and begins one serialized12-job combined build; no stale native run.
Combined95627 terminates with exit1 at TacticsHandler.cpp: the new descriptor
query needs IBattleInfo's direct defining include, not its forward declaration.
The AI owner has this bounded repair. Data/inventory19/19, module drift and
package preflight91/91 pass. Preserve the failure log; native acceptance and
activation remain pending. Full Windows37087488369 is still live on older
0721ee12b; the Defend-source notice37088119439 has succeeded.
Direct include repair is frozen. Serialized combined retry56408 is confirmed
running with12 jobs, log build/new-horizons-linux/testing/UP158-redeployment-
build-retry.log. Re-poll that exact handle before native acceptance or another
build; observation timeout is not terminal. All delegated source/fixture/review
lanes have completed. Required next gate: four Redeployment cases plus eight
Tactics deployment and three Defend lifetime cases in the active private profile,
with zero skips. Activate/register module and inventory only after principal
acceptance, then commit/push; verified184/310 remains unchanged meanwhile.
Retry56408 terminates with exit0 at517/517. Focused native acceptance passes
15/15 in25.735s, zero failures/skips, using the private active module profile.
All four Redeployment cases, eight Tactics deployment and three Defend lifetime
cases pass. Production registration is now active; module/inventory synchronization
and final focused checks follow. Coverage185/310,125 planned; Battlecraft5/10.
No graphical handoff, full resume, rare trap/death or actual AI certification is
claimed from this gate. No snapshot is promoted.
Final activation gate passes4/4 in1.564s, zero skips; data/inventory19/19,
module check and package91/91 pass. Both-target incremental build exits0.
Independent activation review finds no blocker. Root integrates the coherent
source checkpoint; Windows37087488369 still runs on older0721ee12b.
Source is committed/pushed as27ae52f378984c8be70bf0dbf0b4ac483f92a0db;
the worktree is clean at that checkpoint. Notice preflight37090616619 is queued
on that exact source. Preserve the live older full Windows37087488369 and
dispatch the new full build only after it terminates and the new notice passes.
Older full37087488369 succeeds; notice37091288150 succeeds on delivery-notes
source213b4a35e. New full37091363403 is queued on213b4a35e, excluding UP160.

## UP-157 — Battlecraft Pre-emptive Strike

Status: Bounded read-only preparation,2026-10-02. Missing Advanced perk: the
first melee attack each round against a Defending friendly stack triggers a
50%-damage pre-emptive attack without consuming normal retaliation. Map accepted
attack sequencing, effective Defend lifetime, existing Bulwark reaction seams,
per-recipient round state and shared detached AI forecast. Do not implement a
post-hit retaliation substitute or reuse an unrelated consumed marker. Root
chooses architecture after evidence; no source activation or coverage increase
from preparation. UP156's focused native prerequisite remains the immediate
validation priority; no overlapping file ownership or additional build.
Map complete: reuse authoritative pre-hit attack sequencing and damage resolution,
but allocate an independent per-recipient round marker. Bulwark's existing marker
resets on Defend and cannot silently consume Battlecraft's once-per-round award.
The detached per-attack projection and Defend heuristic both require parity;
JSON/network copies alone do not establish full binary-save preservation.
Asked whether overlapping Battlecraft and Bulwark sources produce two independent
strikes or one strike at the higher percentage. Await that composition ruling
before implementation; the Defend prerequisite remains unblocked.

## UP-156 — Battlecraft Battlefield Mastery

Status: Bounded read-only preparation,2026-10-02. Implement the canonical
Expert perk: the first friendly stack each round to Wait or Defend receives
double the normal Battlecraft rank bonus for that action. Preserve the existing
Wait one-shot/round expiry and Defend lifetime; do not double Entrench, Reserve
or unrelated effects, grant extra actions, or add polling. Map authoritative
accepted-action allocation, current-controller semantics, shared live/detached
damage consumers and save/packet state. Root owns architecture and chooses the
minimal event-driven representation before implementation. Overwatch awaits its
Teleport/Blink clarification and is not silently redefined. Tactics is already
source/native verified and pushed; Windows jobs remain separately monitored.
No activation or coverage increase from this preparation.
Prerequisite map confirms a base lifetime defect: afterNewRound clears the
Defending flag and exact stance provenance before the canonical next activation,
even though its STACK_GETS_TURN bonuses remain. Root selects a bounded repair:
preserve those three values at round rollover; existing initialization and
afterGetsTurn remain their clearing boundaries. Wait and per-round reaction
resets are unchanged. Runtime source is frozen in CUnitState.cpp; an isolated
native fixture follows in parallel. Mastery allocation itself remains planned;
verified coverage184/310 is unchanged by this prerequisite repair.
Review blocks the initial three-reset-only repair: willMove uses !defending,
so retaining that dual-purpose flag would prevent the next normal activation.
Baseline25126 builds successfully but is not accepted native evidence. Root
chooses the existing authoritative UNIT_DEFENDING tag as persistent stance,
not a redundant flag: defended() reads the action flag or the tag; rollover
clears the action flag but retains stance provenance; existing next-activation
bonus removal and afterGetsTurn expire both. The AI Defend candidate adds that
same tag only on its clone. Isolated ownership/source freeze precede retry.
Revised runtime and AI sources are frozen. Review identifies a newly introduced
Second Wind eligibility risk if persistent `defended()` is used as proof of this
round's completed action. Its callback now checks the current-round raw Defend
flag instead; the native fixture must distinguish prior-round stance from a
current-round Defend. Actual queue selection remains a required acceptance gate.
Frozen production client retry84116 is running with12 jobs; log
build/new-horizons-linux/testing/UP156-defend-client-retry.log. Re-poll that exact
handle before registering/building the independent fixture; no stale native run.
Client retry84116 exits0, linking the corrected shared library and client.
Independent source review finds no remaining blocking issue after the Second
Wind consumer repair. Native actual-queue/lifetime acceptance is still pending;
extra-activation/Stasis expiry and broader vanilla interactions remain Phase2.
Combined fixture98647 fails on a test-only rank parameter; the repaired fixture
also retains a slower reserve to prevent an accidental double round advance.
Retry27682 builds both targets successfully. Focused native37434 passes16/16
in4.453s with zero skips: three new real-queue/lifetime/Second Wind/Wait cases,
eight Battlecraft rule/runtime cases and five Reserve cases. Existing duration
tags carry the stance without new saved fields; AI clone tagging remains local.
Test binary SHA-256:
2d7b257e890330470463df4420eaba27f2c5178b3dd35402520296f8a82d2e28.
Prerequisite is source/native verified; Battlefield Mastery remains planned and
coverage184/310 is unchanged. Client pose across rollover, extra-activation/Stasis
expiry and broader vanilla/save interactions are Phase2; no snapshot promotion.
Prerequisite source is committed/pushed as5f79306283cdb241db1679ea88de7cfe7c1473de;
worktree was clean after push. Notice37088119439 is monitored on that revision.
Full Windows37087488369 remains live on older0721ee12b and excludes this repair;
preserve it and do not infer repair delivery from the older Windows job.
Mastery map also exposes a genuine machine-eligibility wording gap; asked whether
an ineligible War Machine consumes the award. Do not invent that exception.

## UP-145 — Bloodrage Blood Scent

Verified source/native checkpoint: fixture rebuild84207 exits0; principal
retry91133 passes5/5 in1.713s, zero skips. Active registry/module/inventory now
represent Blood Scent; data36/36, drift and activated both-target build pass.
Focused activated62923 passes36/36 in8.312s, zero skips. Coverage180/310 perks,
130 planned; faction49/90; Bloodrage6/10; ranks84/93 unchanged. Test binary SHA-256
fe5286f43e521d400d201c518081f32bf94a001ed1fe20076b5bceb1ce696ac5.
Original3/5 failure artifacts remain preserved. Broader control/status/save and
rendered feedback are Phase2; no immutable playable promotion. Commit/push next.
Source delivered as0a0914e1ce8ab1f22f5aa977e8284ceb6b6ff1c3 on
origin/definitive-mvp; push exits0. Current Windows37049519240 remains confirmed
in_progress on older b99c49c32; it does not include Blood Scent. Preserve and poll
that run, then preflight/build the newer commit without claiming CI acceptance
from the native Linux gates. No launcher snapshot is promoted by this commit.

Next read-only map: Avatar of Rage's25% Creature Defense penetration belongs in
the shared target-defense stage, not Hero Order mitigation, with a resolved
per-side snapshot and saved-cap/current-controller gating. Asked whether Blood
Scent's attack-local cap attainment should activate Avatar for that attack;
await the narrow composition answer before implementing Avatar. Blood Scent's
own implementation remains unblocked. No Avatar source/activation from the map.

Status: Verified (source/native; delivery pending),2026-10-02. Implement the canonical
Basic perk's temporary one-increment increase when the attacked enemy is strictly
below50% maximum stack HP, bounded by the current Bloodrage cap. It must use the
shared physical-damage path for live and detached AI, current controller, and
authoritative resolved mechanic state rather than inspecting hidden enemy heroes.
No persistent increment, threshold Speed/retaliation change or polling is granted
by an attack-local bonus. Separate read-only runtime and AI/save maps precede root
architecture; focused boundary, cap, control, branch and save evidence is required.
Registration remains planned and coverage179/310 until execution/build acceptance.
Runtime/AI/serialization source is frozen. Saved low-health increment is0 or the
rank's5/8/12; the shared attack-only overload preserves the ordinary counterquery.
Current binary saves preserve both side values; older lossy writes reject before
bytes and old loads default0. Native fixture is independent and unregistered.
Serialized12-job client build50746 is live; exact log
`build/new-horizons-linux/testing/UP145-blood-scent-client-build.log`.
Re-poll that handle before test-target registration/build. No activation yet.
Client50746 exits0,317/317, linking vcmiclient. Serialized vcmitest baseline
build25076 is live, logUP145-blood-scent-test-baseline-build.log, while the new
fixture remains unregistered; re-poll25076, then register/freeze and
rebuild its exact source before native execution. Data36/36, module drift and
existing UI source guard pass. No native or playable acceptance yet.
Baseline25076 exits0,320/320. Five-case fixture is frozen/registered; serialized
both-target build40698 is live, logUP145-blood-scent-fixture-build.log. Re-poll
it before executing the principal filter. Source review's dead-attacker guard
was corrected before client compilation; native acceptance remains pending.
Both-target40698 exits0. Principal61899 runs5 cases:3 pass,2 fail, zero skips
in1.740s. HP boundary/cap/rank/save cases pass; payload cases incorrectly expect
Bloodrage to multiply the already attribute-raised damage by1.05, while existing
Lua adds its percentage to the raising factor. The independent fixture owner
must verify/repair the deterministic reference, not change production damage math
or weaken the intended attack-local result. Original principal log/XML retained;
registration stays planned until repaired exact-source execution passes.

## UP-144 — Bloodrage Endless Bloodshed

Status: Verified (source/native; delivery pending), 2026-10-02. Principal66256
passes4/4 in1.559s, zero skips. Fury Unbound and Endless Bloodshed are active
after legal offers, live/detached72->80 cap saturation, Morale/current-control
and cap serialization checks. Client91439/test68195 and both-target18196 pass;
data36/36, module drift and UI source guard pass. Coverage177/310 active,
133 planned, Bloodrage3/10, faction46/90; ranks84/93 unchanged. Activated
adjacent gate has completed; see retry evidence below. No playable promotion.
UP-143's Fury portion is implemented, not its remaining Speed/retaliation perks.
Activated69374 has40/41 pass, zero skips; rankless legacy fixture's NH typed
Hero Action setup is incompatible with its requested old format. Root applies
a bounded fixture-profile repair without weakening save guards or changing
assertions. The exact-source rebuild6389 exits0; activated retry20229 passes
41/41 in29.684s, zero skips. Evidence: `UP144-activated-retry.log`/`.xml`.
Original failure artifacts remain preserved; production save guards are unchanged.
Source delivered as ca1898435d61d664e8d95016924a11dc0b61c125 on
origin/definitive-mvp; push exits0. Exact test binary SHA-256:
3bf63e6fc70bc57bbc5b12d8fbc5c505a39b6dec172a704dc4e5c9126aca515d.
No immutable playable promotion or Windows acceptance is claimed.

Implementation selected alongside Fury Unbound, which opens legitimate
Advanced progression before this Expert perk. Snapshot the resolved cap per
side, share it across live/AI/UI, and append one serialization feature with
rank-only legacy fallback and rejection of lossy older writes. Counts remain
175/310 active,135 planned; no coverage or playable claim until focused gates.
Runtime and detached AI are frozen; pre-build review finds no blocker. Root
starts the serialized12-job client build with logUP144-client-build.log. New
unregistered fixture may finish independently; no production edits or competing
build. Native execution and activation remain pending.
Exact live client-build handle91439 must be re-polled before registering the
test file or starting vcmitest. Source review finds no blocker; UI source guard
passes against the shared saved cap. The generic panel design is unchanged.
Client91439 exits0, reaching317/317. Principal fixture source is still finishing;
register/build the test target only after its freeze. No native-pass claim from
the client compile or source guards. Data36/36 and module drift pass.
Four-case fixture is frozen/registered; independent final review has no blocker.
Serialized12-job vcmitest build68195 is live, logUP144-test-build.log. Re-poll
that exact handle; no native execution or competing build until terminal.

Status: In progress (bounded read-only map), 2026-10-02. Expert perk increases
Bloodrage's maximum damage cap by20 percentage points. Trace saved battle rank,
live/detached kill progression and generic resource maximum display; this cap
foundation must support threshold perks without separate contradictory limits.
No implementation/activation from mapping alone. Keep changes independent of
Commanding Presence's callback/fixture ownership; root selects architecture.
Map complete: resolve an active selected Expert perk at battle setup and snapshot
the resulting cap (60->80) per side. Expose one cap getter to live deaths,
detached projections, UI and future half-cap perks. Add append-only serialization
feature with old rank-only fallback and rejection of dropping a nonbase cap.
The12-point Expert increment stays unchanged. No design ambiguity; normal perk
progression's missing Advanced Bloodrage prerequisite must also be addressed,
not bypassed by silently force-activating a different perk in the product.

## UP-139 — Havoc Demolitionist

Verified structural-foundation checkpoint, 2026-10-02: both-target retry4772
exits0; principal35313 passes10/10 in2.669s, adjacent27391 passes6/6 in1.369s,
zero skips. Python36/36 and generated-module drift pass. Reviewer reports no
blocking finding. Runtime6 cases include obstacle-only casts, Spell Lock and
double-wide geometry, fort/unit split, global both-side damage, markerless-v3
fallback and detached/live parity. AI3 cases prove signed fort valuation,
geometry retention and a paid AI spell under a validated zero-effect Order
fixture profile, not normal-profile tactical superiority. Test binary SHA-256:
ee004df30d8ebb25f768042b1c76e1f915851e134f754dab94e4fcff180f5467.
Phase2: obstacle-clearing valuation, normal-profile AI choices, broader immunity
interactions and feedback localization. Fixed-landmark destructibility and
structural perk stacking remain unresolved Phase1 design choices, not waived
coverage requirements. Demolitionist/Meteorologist remain planned; counts stay
173/310 active,137 planned. No graphical or immutable playable promotion.
Earlier paragraphs below are checkpoint history, not current gate status.
Structural foundation committed and pushed as e538921a4; remote branch identity
matches. The worktree is clean after that commit. This is source delivery, not
playable promotion. The unresolved design choices still block perk completion.

Source implementation checkpoint: the optional structural producer, Lua binding,
two spell registrations and geometry-aware signed AI fortification valuation
exist. Root registered isolated runtime/AI fixtures and refreshed the generated
module; 36 focused data/schema/inventory checks pass. Independent review found
and repaired creature-filter-dependent impact metadata; native compile and
principal runtime verification remain pending. This is not perk activation,
full structural coverage, playable delivery or a numerical-balance claim.
Client build20497 is running with12 jobs against the frozen production source.
The isolated runtime fixture is still completing its moat/Spell Lock setup
repair and is not part of that client target. Re-poll20497 before starting the
test build; do not run the stale native binary or infer a build result.
Client20497 exits0. Runtime/AI fixtures are now frozen, including valid moat,
Spell Lock and outside-primary double-wide geometry. Root starts the serialized
vcmitest build with12 jobs; principal native execution remains pending.
Exact live test-build handle is48092. Pre-build review repairs are frozen;
client20497 is terminal success. Run NewHorizonsHavocStructuresTest.*,
NewHorizonsHavocStructuresAITest.* and the saved-v3 typed opt-in parser guard
only after48092 exits0. Supplemental content inventory56/59 failures come from
the old five-Mass-spell catalogue omission and are deferred in the failure ledger.
Final static AI-fixture review corrects incompatible disabled-Order setup and
an immunity/geometry assertion. The AI fixture compiled before this repair in
48092, so re-run vcmitest build after48092 terminates before native acceptance.
Only that new fixture changed; production stays frozen.

Status: In progress (read-only map), 2026-10-02. Missing Basic perk adds50%
damage to destructible objects/fortifications only for Havoc spells already
able to affect them. Map existing structural paths and AI; do not invent new
spell targets. Production, registration and coverage remain unchanged.
Map finds a foundational coverage gap: Meteor Shower and Armageddon lack their
canonical scenery/fortification effects. Only Nature Earthquake currently has
a spell structural producer; do not boost that or unit damage to fake Havoc
coverage. Implement the specified Havoc structural paths before activating
Demolitionist/Meteorologist. Binary obstacle destruction has no numeric HP
quantity to boost. Structural stacking and tunable formula scope need root
canonical review, not a claim that the perk is already functional.
Implementation contract: optional saved-v3 structures block, omitted older
snapshots retain their old behavior. Data prototypes use50% raw coefficient-aware
spell damage against forts for Meteor Shower,100% for Armageddon. Ordinary
scenery removal is binary; absolute scenery, moats and magical obstacles are
not ordinary scenery. No new polling or gameplay counter. Runtime/AI/fixture
ownership is separated; root owns data/schema, registration, build and Git.
Asked additive+75% versus multiplicative+87.5% for the two structural perk boosts;
base spell effects proceed while perk stacking/activation awaits the answer.
Asked whether fixed absolute landmarks are destructible; the engine's absolute
tag expresses placement, not destructibility. Runtime initially preserves that
category pending review, while implementing usual scenery and actual fort HP.
Do not claim the classification question is resolved or activate blocked perks.

Next bounded coverage candidate: Havoc Cataclysm remains planned. Read-only
mapping may proceed while the structural foundation compiles: identify the
shared +20% Armageddon SP-component gate and ordinary magical-obstacle removal
classification, with minimum AI hooks. No activation, production change or
coverage claim is authorized from that map alone; resolve scope before writing.
Mapping confirms this is existing UP-111, not a new uncovered item. Its hidden
magical-obstacle/moat filter remains the previously asked design choice; the
shared coefficient hook and detached obstacle removal already exist. Do not
repeat that map or implement only its damage clause as the entire perk.
Principal81936 passes6/6 runtime structural cases but fails1 parser and3 AI
cases (10 total, zero skips). The typed-percentage parser is repaired; AI owner
is diagnosing candidate lifecycle and actual action choice. Builds20497/48092
and fixture rebuild43129 passed. Source is not accepted/committed from this
partial native result; follow the focused repair through rebuild/retest.

## UP-138 — Havoc Conductor

Status: Resolved (duplicate selection), 2026-10-02. Read-only inspection proves
Conductor is already active, with a shared damage multiplier and focused
ordinary/Master Chain tests. No new implementation or coverage increase is
claimed. Do not re-explore this implemented perk merely to add more tests;
select the next genuinely planned item from the live registry.

## UP-137 — Havoc Mine Layer

Verified (delivery pending): client27766 and test22177 build successfully.
Principal51245 passes10/10 in2.899s, zero skips: legal acquisition,3/4/5
counts, detached AI, authoritative placement/damage snapshot, atomic rejection,
existing runtime and AI guards. Registration is active; generated-module and
activated gates are next. Purpose-made artwork and playable promotion are not
claimed. Broader GUI/placement interactions remain Phase2.
Activated retry70019 passes10/10 in2.919s, zero skips. Client activation build
exits0; data/schema/inventory35/35, module drift and independent activation
review pass. Earlier paragraphs below are checkpoint history, not current status.
Source committed and pushed as779289300; remote branch identity verified.
This is not immutable playable promotion or graphical acceptance.

Status: In progress (bounded map), 2026-10-02. Land Mine creates one additional
mine with the active Havoc Mine Layer perk. Trace the shared mine-count and
placement path, live/detached caster gates and focused verification. Root owns
registration/build/Git. No source activation or coverage increase from mapping.
Map complete: Mechanics::getNewHorizonsLandMinePatchCount is already consumed by
client placement, obstacle Lua and AI. Add1 after the canonical2-to4 base cap;
server validation currently recomputes the bare count and must use this shared
accessor too. Land Mine itself has authoritative placement/trigger and AI tests.
No new saved state or polling is needed; preserve non-hero/legacy gates.
Production owner is authorized only for the named Havoc constant, shared
ISpellMechanics count accessor and server validator count line. All build/native
processes are terminal. Bastion regions stay frozen; its fixture and the new
isolated Mine Layer fixture have separate writers. Registry remains planned.
Production is frozen in the two scoped cpp regions; private constants leave
the public header unchanged. Independent review has no blocking finding: UI,
Lua, AI and both server checks use the same accessor, including five targets.
Client27766 is live with12 jobs. Re-poll it before another build/native run;
principal verification and registration remain pending.
Client27766 exits0. Test72269 is now compiling with12 jobs, including the
frozen repaired Bastion fixture. The unregistered Mine Layer fixture may finish
independently; do not change production or CMake during72269.

## UP-136 — Armorer Defiant

Status: Blocked on retaliation-denial scope, 2026-10-02. Read-only map complete:
No Quarter applies a non-magical NO_RETALIATION debuff, but innate blocking,
Long Weapon geometry, Shroud flanking and ranged retaliation use separate gates.
Asked whether Defiant covers both intrinsic attack mechanisms and applied
debuffs, and whether blocking No Quarter also blocks its linked Morale penalty.
Use actual accepted suppression, current control and round-local side state;
do not implement a No Quarter-only subset as the entire perk or repeat the map.

## UP-135 — Armorer Bastion

Verified (delivery pending): final fixture rebuild92361 exits0; principal45892
passes8/8 in2.618s, zero skips. Legal offers, Defend/Hold the Line, first-hit
reduction/expenditure, normal next-round renewal, spell-like exclusion and
detached live-state isolation/JSON defaults pass. Registration is active;
activated gates remain next. Earlier entries below are checkpoint history.
Retain Phase2 findings already listed; no GUI/artwork/playable acceptance.
Activated build28218 exits0 for both targets. Combined67346 passes18/18
in5.197s, zero skips, including Mine Layer. Data/schema/inventory35/35 and
module drift pass; source integration is ready for normal commit/push.
Committed/pushed6f848c9a8. Windows notice preflight37018538339 queued on that
source; poll its exact handle before a full build. No playable promotion.
Notice37018538339 passed. Full Windows37018692299 queued ondf94df8ec;
re-poll that exact build. No new platform/package acceptance is claimed yet.
Terminal evidence, 2026-10-02: full Windows37018692299 completed successfully
on df94df8ec267c0ab07c0833bc1dd67a1c8c6d9ca. This proves that checkpoint's
Windows workflow, not the later Havoc commit or Windows graphical gameplay.

Retry48708 passes6/8 in2.622s, zero skips. Two fixture cases still fail:
post-action baseline prediction reports1 versus actual3825, and a next-round
actor action is rejected. The fixture owner is investigating while preserving
production validation and meaningful assertions; registration remains planned.

Status: In progress, 2026-10-02. Implement Expert Armorer Bastion:
while Defending or covered by Hold the Line, a stack's first physical creature
attack received each round deals30% less final damage. Map the existing
per-stack first-hit/round lifecycle and physical damage pipeline; preserve
spell damage exclusion, final-damage ordering and current-controller perk gates.
Runtime, detached AI and focused fixture work have separate ownership. Require
production, legal selection, principal compile/native evidence and registration
before increasing coverage. No GUI or playable promotion is inferred.
Runtime and the four-case principal fixture are frozen; independent review finds
no blocking issue. The server preserves constructor-derived spell-like attack
classification. AI implementation and one isolated detached parity case remain
in progress; root registered the fixture, but no build/native pass is claimed.
Phase2 retains explicit absorbed/lethal hits, controlled ownership and stacking
with Immovable. Coverage stays171/310 until the focused gates pass.
Runtime and AI are now frozen and independently reviewed without blockers.
Client build92791 is live with12 jobs; re-poll that exact handle before test
build or native execution. The isolated detached fixture may finish independently
but no production edits are permitted during compilation. Phase2 also retains
Defend heuristic valuation when Hold the Line already grants baseline Bastion:
baseline first-hit discounts are repeated in the forecast, underpricing Defend.
Client92791 exits1 on a Counterfire state-interface read; the owner corrected
it through acquireState and refroze. Both-target retry79589 is live with12 jobs.
Five principal cases now include actual detached AttackPossibility/exchange
spending and live-state isolation. Independent corrective/fixture review has no
blocker. Do not run native until79589 is terminal successful.
Both-target79589 exits0. Native64640 reports4/8 pass in2.607s, zero skips;
fixture repairs are in progress for repeated spent actions/Defend lifetime and
the player0 projection hiding the defending hero. Production stays frozen,
registration remains planned, and no native/build handle is presently live.
Fixture repairs are frozen and independently reviewed: distinct unused actors,
an actual validated Defend, a slow reserve, and the spectator mechanics oracle
preserve the assertions. Test72269 is live; re-poll it before native retry.
Spectator parity is not proof that player-scoped AI sees hidden enemy perks;
that visibility/valuation assertion remains Phase2.

## UP-134 — Spellcraft Extend Spell

Status: Blocked on duration scope clarification, 2026-10-02.
Next missing Advanced Spellcraft perk:
once per round the first temporary hero spell lasts one additional round.
Read-only duration/accepted-cast/detached-state map while UP-133's bounded
fixtures are written. Identify real lifecycle prerequisites and scope conflicts
before implementation; no activation or coverage increase is claimed.
Mapping is complete. BaseMechanics::adjustEffectDuration is shared by ordinary
and custom Lua round-based durations. A pre-cast snapshot plus accepted-cast
per-side round allowance is required; actual effects follow BattleSpellCast
application, and detached AI needs a copied/advanced allowance. Asked whether
temporary terrain and summons qualify alongside creature enchantments. Time
Stop uses action-bound stasis rather than round duration and must not gain an
invented round. Accepted Counterspell-negated consumption is also unresolved,
as in the already pending accepted-cast design clarification. Do not repeat the
map or add permanent polling.

## UP-133 — Spellcraft Precise Casting

Status: In progress (broader area scope clarification pending), 2026-10-02.
Implement the canonical Advanced perk:
conventional area spells centered on an occupied friendly hex exclude that
stack, while explicitly indiscriminate spells cannot benefit. Map authoritative
target filtering and detached AI with separated ownership. Require legal perk
selection, principal targeting verification and focused compile/native evidence
before activation or coverage claims. No GUI or playable promotion is inferred.
Controlled Blast supplies the existing shared Lua center-identity gate for
Fireball, Inferno and Meteor Shower. Implement and verify those unambiguous
cases without activating the perk prematurely. Asked whether Precise Casting
also excludes Time Stop stasis and Earthquake's immediate field damage while
leaving terrain unchanged. Canonical "conventional area spell" does not settle
this broader scope; do not silently narrow the completed perk to three spells.
The bounded production helper is now in source; independent Astra review finds
no blocker. Client48085 and test18427 build successfully. Existing shared-path
Controlled Blast regression89309 passes6/6 in2.658s with zero skips, covering
legal offers/save, friendly/current-control/double-wide centers, Armageddon and
AI parity. These are regression evidence, not Precise Casting principal proof;
isolated fixture build90773 now passes. Principal96284 passes7/7 in2.238s,
zero skips: legal Basic/Advanced offers, accepted live/detached Fireball,
unselected and planned gates, current-control double-wide Meteor Shower,
Armageddon and BattleAI viable central-target filtering. Registry stays planned
because broader scope awaits clarification; coverage remains171/310 active.
No GUI or playable promotion is claimed. Do not repeat the completed targeting
map or principal three-spell tests in place of resolving the outstanding scope.
Verified subset committed and pushed as7e02b092f. Independent fixture review
has no blocker; Phase2 retains direct Inferno/hover assertions and actual AI
utility ranking. No new save state or serialization version was needed.

## UP-132 — Spellcraft Cross-School Formula

Status: Blocked on multi-school/Counterspell clarification, 2026-10-02. Next UP-023 missing
Basic Spellcraft perk: after casting from one school, the next spell from a
different school before the end of the next round gains10% to its Spell
Power-derived numerical component. Map completed-cast history, saved/detached
state and shared numerical consumers without changing production bytes while
UP-131's test build is live. Preserve flat bases, costs, action economy, rejected
casts and canonical school identity. Root owns architecture/state/activation,
builds and Git. No implementation or activation is inferred from the map.
Mapping is complete: existing completion flags and level mask lack spell/round
provenance; StartAction history is not an accepted-cast substitute. Add compact
accepted source identity/round state at BattleSpellCast, copy/advance it in
detached AI and reuse shared coefficient-only scaling after policy resolution.
Current configured spells include multi-school membership, so the different-
school relation is a real scope question. Asked whether it requires disjoint
school sets or any new school, and whether accepted Counterspelled casts arm
the source. Do not silently resolve either or repeat this map.

## UP-130 — Discipline Esprit de Corps

Status: Blocked on existing composition-scope clarification, 2026-10-02. Continue UP-023
Phase1 missing Basic Discipline coverage: reduce army-composition Morale
penalties by one without changing enemy-effect penalties or granting positive
Morale to a composition without a penalty. Map the shared army-composition
calculation, saved perk gates, live/detached AI and principal native fixture.
Root owns architecture, registration, builds, docs and Git; independent Luna
maps are read-only until ownership is assigned. No activation or coverage
increase is claimed from mapping. No GUI or playable promotion.
Mapping reconfirms the earlier sprint finding: mixed-faction and Undead-presence
penalties are separate, and the unanswered scope choice must not be resolved by
root implementation direction. No source implementation is authorized until
that answer arrives. Temporary-army AI projections also need receiver context.

## UP-131 — Discipline Unbreakable

Status: Verified (playable delivery pending), 2026-10-02. Unbreakable is active.
Client52523, test10838 and repaired fixture52313 build successfully. Principal
retry10314 passes10/10 in3.330s; activated both-target98579 and native69637
pass10/10 in3.303s, zero skips. Data/schema/inventory35/35, module check and
independent frozen review pass. Coverage170->171/310, Discipline5->6/10.
Phase2 retains multi-round AI valuation and broader stochastic interactions;
generic UI Provisional, bespoke art Not done; no GUI or playable promotion.
Source committed/pushed asff18ed6b9. Windows preflight37006272158 now passes.
Full Windows37008135705 is queued on8c5f5ec87, containing Broad Muster and
Unbreakable; compile/package remains pending. Older full37000555568 completed successfully on
7331e1056, including compile, recursive package audit and artifact upload;
it does not contain Broad Muster or Unbreakable. Broad Muster preflight
37002243267 is now terminal cancelled; do not treat it as a pass.
Native evidence is the frozen pre-commit candidate, not an
immutable promoted package. Windows compile/package acceptance remains pending.

Original scope: Continue UP-023
Expert Discipline coverage: ignore the first negative Morale trigger against
the army each round. Reuse the established Rally suppression event while keeping
Rally's once-per-combat allowance distinct, preserving current-controller and
Twist of Fate ordering. Require authoritative trigger/reset behavior, saved and
detached state, legal Expert acquisition and focused AI/native evidence. Root
owns architecture, registration, versions, builds, docs and Git. No activation
or coverage increase is claimed before principal validation; no GUI/promotion.
Production and AI source are frozen. Four concurrent workers plus root were
confirmed for runtime, AI, focused fixture and independent Astra review. The
review finds no provisional blocking issue; it defers multi-round AI valuation.
Data/schema/inventory35/35 and module drift checks pass while registration
remains planned. Append-only state compatibility is present; actual trigger,
save and detached principal gates and compilation remain pending.
Production-only client build52523 is live with12 jobs while the isolated new
fixture is completed. Its file is not yet in the test target. Freeze production
bytes through this build; then register/build the fixture serially and run the
focused Unbreakable/Rally gates. No native execution during compilation.
Client52523 exits0. The new six-case fixture is registered and frozen; test
build10838 is live with12 jobs. Root corrected packet-enable and deterministic
Twist assumptions before compilation rather than weakening production rules.
All workers are terminal. Re-poll this build handle before any native run;
focused filter is NewHorizonsUnbreakableTest.*:NewHorizonsRallyTest.*.

## UP-126 — Recruitment Recruiter's Contacts

Status: Blocked on multirow pool clarification, 2026-10-02. Next UP-023 Advanced Recruitment perk:
once per week, visiting an owned external dwelling with an empty recruitment
pool adds one normal week's growth. Map existing growth/ownership/visit hooks,
weekly persistence and minimum AI/log/UI paths before implementation. Root
owns architecture/state versioning and builds; read-only mapping while UP-124's
frozen principal candidate compiles. Preserve existing Muster allowance; this
is a distinct perk trigger, not another Muster use. No activation/coverage claim.
Mapping is complete: same-owner visits reach the dwelling hook; normal weekly
growth and SetAvailableCreatures are reusable. A separate persisted per-hero
weekly cooldown and empty-dwelling AI eligibility/value are required. Asked
whether a multirow dwelling must be entirely empty before all rows refill, or
whether an empty row can trigger a partial refill. Do not silently choose.

## UP-127 — Recruitment Drill Sergeant

Status: Blocked on merged-cohort clarification, 2026-10-02. Canonical Basic perk
grants hero-direct Core/Elite recruits+1 Morale for their first combat within
seven days. Recruitment/battle/expiry seams are mapped, but same-creature recruits
merge into existing stacks and ordinary split/join does not preserve stack-local
bonuses. Asked whether the whole resulting stack receives the bonus or only the
newly recruited cohort. Do not silently grant old creatures a cohort-only bonus
or weaken transfer persistence. No implementation or activation is claimed.

## UP-128 — Recruitment Broad Muster

Status: Verified (playable delivery pending), 2026-10-02. Broad Muster is active.
Both Linux targets build40839; principal54272 passes18/18 in3.701s and
activated82143 passes18/18 in3.704s, zero skips. Data/schema/inventory35/35,
module drift and static UI guards pass. Independent runtime/wire/fixture and
AI/UI reviews have no blocking findings. Coverage169->170/310 active;
Recruitment5->6/10. No saved gameplay counter or polling; append-only wire
fields preserve solo compatibility. No GUI or playable promotion. Source
committed/pushed as0f2d8cac8. Native gates are frozen pre-commit candidate
evidence, not an immutable playable package. Windows preflight37002243267 is
queued on that source behind full37000555568; the running older job is preserved.

Original scope: Next unblocked Basic Recruitment perk: generated
Core Muster recruits may be split between two Core dwellings in the same town.
Map the authoritative atomic allocation, shared weekly allowance/target locks,
exact split interaction and minimum AI path before implementation. Preserve
the current rank/perk amount; rejected allocations must not consume the use or
mutate either pool. Root owns architecture/config/build/Git; Luna is read-only.
No activation or coverage increase is inferred from the map. Mapping found no
material specification blocker. Append optional second creature and first-row
allocation to the existing request with an append-only wire feature; old solo
requests remain unchanged. Server derives total, requires two distinct Core
rows and positive exact-sum amounts, validates both overflows, then sends one
marker and one combined stock update. Native scrollable allocation choices
must name both destinations and amounts. AI may choose a split when Leadership
admission makes it more useful, otherwise retain solo. Runtime, UI, AI and
native fixture have separable ownership. Volunteer Network contributes only
once to a derived total, but do not fake simultaneous legal Basic perk choices
in the principal native fixture; test hypothetical modifier composition in the
shared helper if needed. No new saved gameplay counter is required.
Runtime, UI and AI workers are live with separate ownership. Fourth native
worker activation was rejected by the service; root owns that bounded fixture
and serialized build gate instead. Perk stays planned until native acceptance;
this is actual delegation, not an activation or coverage claim.
All three production workers are terminal and source is frozen. Root added
legal-rank actual split/negative/overflow/save/wire fixtures and a localized
two-dwelling note, updating the curated CMake text list as well as the module.
Static UI/module checks and data/schema/inventory35/35 pass. Runtime/wire
review has no blocking finding; AI/UI review and both-target build40839 are
live. No native/activation evidence is claimed until that build and focused
execution pass. No GUI launch or playable promotion.
Final AI/UI review has no blocking finding. Phase2 retains long-label native
row fit and actual UI/AI query execution; AI split valuation omits existing
dwelling stock, Gold affordability and shared free army slots. The external
negative fixture rejects at visit validation rather than isolating the later
no-external-split check. Do not expand Phase1 into an exhaustive matrix here.

## UP-129 — Deterministic Diplomacy foundation

Status: Mapping complete; consolidated with blocked UP-048, 2026-10-02. Missing Version1.0 foundation for all three
Diplomacy ranks and ten perks: eligible neutral joins use deterministic
25/50/75% Army Value thresholds and normal recruitment Gold costs. Map current
encounter eligibility, saved rules, exact pre-commit feedback, Leadership
admission and adventure AI consumers while the Broad Muster candidate is
verified. Do not revive random joining or bypass hostile/scripted exclusions.
Preserve the accepted-join/garrison lifecycle until its remainder semantics are
explicitly decided, as UP-048 already requires. This queue does not authorize
an invented partial-neutral persistence rule. No activation/coverage claim.
Supplemental mapping confirms the shared pure evaluator can serve server visit
feedback and AI through existing BlockingDialog queries, without a new request.
Scripted visits already retain their own control path. Authored COMPLIANT free
joins versus the normal-Gold rule remain the existing unanswered UP-048 choice;
raw Army Value versus legacy perceived/hero strength must remain explicit.
Leadership-surplus dismissal/neutral-source AI handling needs a separate
lifecycle decision, not an automatic rewrite. Do not repeat this map again.
The existing authored-free-join question was renewed on2026-10-02 after mapping;
no answer or authority to override map semantics is inferred.

## UP-125 — Four-worker concurrency

Renewed authorization verified, 2026-10-02: global configuration, AGENTS.md and
the orchestration skill already permit four subagents excluding root. This
session exposes five total concurrency slots. No lower file setting was found
in the root check; no redundant configuration edit or gameplay change is needed.
Independent read-only worker audit confirms no lower or contradictory override;
the user-level AGENTS.md is empty. Configuration verification is complete.

Latest user request rechecked, 2026-10-02: global capacity remains four;
the repository `.codex` file is empty, and no profile/project agent-limit
override was found. A fresh Luna spawn and completed-worker follow-up both
succeeded. Added the four-subagent shared-capacity and reuse/error-reporting
policy to the orchestration skill itself. No numeric setting change was
needed; this check does not claim four simultaneously running agents.

Status: Resolved, 2026-10-02. User authorizes four concurrent workers. Inspected
the local agent configuration: max_concurrent_threads_per_session is already4.
Fresh spawn and a follow-up to an unavailable historical explorer were rejected;
follow-ups to two completed workers still in the current team succeeded.
Team inventory now confirms four running workers plus root: external runtime,
external UI, AI and native fixture. Persisted bounded four-worker/reuse policy
in AGENTS.md. No configuration increase or unrelated-thread interruption was
necessary. Runtime setting changes are not falsely claimed.
Policy committed and pushed as42ed09b7e. Concurrency was verified through the
actual agent API/team inventory, not merely by editing a configuration file.

## UP-124 — Recruitment External Recruiter

Status: Verified (playable delivery pending), 2026-10-02. External Recruiter is
active; both Linux targets build. Principal15376 passes11/11 in2.877s and
activated81048 passes11/11 in2.899s, zero skips. Data/schema/inventory35/35,
module drift and Muster UI wiring pass; independent source/fixture reviews have
no blocking finding. Coverage168->169/310 active, Recruitment4->5/10.
Existing saved markers/packets are reused. Full natural visit/window/AI run,
full-army merging, mixed rows and restored queries are Phase2 deferrals.
Bespoke icon remains Not done, UI Provisional; no GUI or playable promotion.
Source committed/pushed as6cb08a8cb. Native gates are frozen pre-commit candidate
evidence, not a promoted immutable package. Windows preflight36998928632 passed
on6cb08a8cb; full37000555568 was dispatched on7331e1056 (same functional source,
later queue/sprint documentation). It does not contain the dirty Broad Muster
candidate. Full Windows compile/package acceptance remains pending.

Original scope: Continue unblocked UP-023 Basic perk coverage:
the hero can spend the weekly Muster use at an owned external Core dwelling
instead of a town, adding two Core recruits there. Map shared weekly allowance,
dwelling ownership/category/pool validation, authoritative acceptance, required
adventure interaction and minimum AI hooks. Preserve the town path, Leadership
admission and rejected-action non-consumption. No alternate weekly counter or
frontend state mutation. Root owns architecture/config/build/Git; Luna maps
before bounded implementation and focused native gates. No GUI/promotion.
The completed map confirms existing hero/dwelling weekly markers and stock
packets suffice. Runtime and native-recruitment UI workers have disjoint file
ownership. Preserve free original tier-1 external recruitment through a shared
dwelling cost method, not a client-only displayed discount. Bind external
Muster to the exact active visit and keep Leadership admission authoritative.
The service rejected a fresh third worker and an unavailable-explorer follow-up;
reusing two completed workers now runs AI implementation and native fixture
work in parallel with runtime and UI. Root owns the serialized build/test gate.

Windows preflight36992596028 succeeded on source9d8c5f4d4. This is preflight
evidence only, not a Windows compile/package or playable delivery.
Full Windows build36994237037 on6ca967db6 failed in Discipline source-ID
initialization under MSVC. Brace initialization repairs that parse ambiguity
and is committed/pushed as453828742; a succeeding Windows build is still pending.
The failed run contains Spellward, not the uncommitted External Recruiter.
All four workers finished and the candidate is frozen: runtime, native
recruitment controls, minimum AI query/purchase hook and deterministic fixture.
Root integrated localization/module generation and updated the static UI guard,
which passes; module drift and diff checks pass. Perk stays planned until the
principal native gate succeeds. No build/native or coverage increase is claimed.
Next: serialize the vcmiclient+vcmitest build with12 jobs, run Recruitment
Muster and Nullkiller2 Muster helper tests with the New Horizons test profile,
repair material failures, review, then activate/register and recheck. Both Linux
targets now build (final44293 exits0). Principal37505 ran11 cases:9 passed,
two fixtures failed because Advanced/Expert perks were selected without their
required earlier tiers. Repair legal acquisition preconditions, not production
enforcement; strengthen the free-recruitment case with actual zero resources.
Independent Astra source review reports no blocking production finding. No GUI,
playable promotion or source commit is claimed for this candidate yet.

## UP-123 — Chaos Pandemonium and generic debuff counting

Status: Blocked on debuff-count/perk clarification, 2026-10-02. Continue UP-023 Phase1 missing combat identities
after Spellward's verified pushed slice9d8c5f4d4. Canonical Level5 Pandemonium
deals D×(20+0.25×SP) to every stack, including allies, where D counts active
DEBUFF-tagged effects; raw statistics and permanent creature traits do not count.
Map a reusable classification/counting path for magical and physical statuses,
effect identity/deduplication, immunity/defenses, forecast/UI and detached AI.
Expert Pandemonium Master adds25% damage per counted debuff. Do not substitute
Armageddon, a hardcoded spell list or a data-only activation. Root owns the
generic architecture, registration, state versioning if required, builds and
coverage. Workers are read-only until ownership is partitioned. No GUI/promotion.
Both maps are complete. Existing physical-affliction groups and stored Poison
can supply a shared derived tagged-effect view without new counters. Explicit
effect metadata is required: Shield of Chaos has neutral spell flags but timed
negative Morale/Luck, and No Quarter is a non-spell temporary Morale penalty;
permanent Undead Morale must remain excluded. Count logical effects rather than
each Bonus payload (Disease has a marker plus two penalties). A generic opt-in
must cover future creature effects, with versioned Bonus metadata if added.
The saved integer coefficient/divisor10 cannot exactly express0.25×SP; use a
shared rational formula rather than rounding to0.2 or0.3. Global preview must
show per-stack count/damage before commitment, including allies and zero count.
Asked whether repeated stackable applications of one debuff count once or
separately, and whether Pandemonium Master's25% accumulates with D or strengthens
each damage contribution by25%. Neither interpretation is activated or canonical.
No source edits, spell registration or coverage increase is claimed by mapping.

## UP-122 — Warcasting Enchanted Command

Status: Blocked on Order-recipient clarification, 2026-10-02. UP-023 Advanced perk while
Spellward's frozen repair builds. An allied recipient of an Order empowered
by Warcasting gains+1 Morale until its next activation. Map actual recipient
sets, captured empowerment, next-activation cleanup and detached AI consumers
before choosing the smallest shared implementation. Require legal Advanced
acquisition, empowered/unempowered guards, correct recipients and duration,
actual accepted Orders and detached parity. No polling or new duplicated state.
Root owns architecture/data/build/Git; Luna is read-only during the frozen build.
Mapping is not implementation or completed coverage. No GUI/promotion.
Read-only map confirms captured HeroOrderState::warcastingBonusPercent is the
trigger, not post-action readiness. Existing UNTIL_NEXT_CREATURE_ACTIVATION
bonus expiry is mirrored by detached AI. The recipient question overlaps
UP-047: Protect's pair and Second Wind's selected stack versus every troop in
their broad declared coverage. Asked one shared scope question; do not infer
an unrelated whole-army aura. No source changes or activation occurred.

## UP-121 — Warcasting Combat Casting

Status: Blocked on penetration composition, 2026-10-02; read-only mapping
while UP-120's frozen candidate builds.
Canonical Advanced perk: a hostile spell empowered by Warcasting ignores15%
of the target's Magical Damage Reduction. Map captured Warcasting eligibility,
shared penetration composition, collateral/delayed consumers, legal Advanced
progression and focused native/AI seams. No source edits or activation during
the UP-120 build. Identify consequential ambiguity rather than inventing a
stacking rule. Root owns architecture/configuration/build/Git. Mapping is not
implementation or completed coverage; finish Spellward's gate first.
The15% trigger is authored and existing captured Warcasting state is reusable.
Existing runtime takes the strongest penetration; canonical text gives each
effect's fraction but does not explicitly settle simultaneous composition.
Asked the user whether20% and15% combine independently to32%, add to35%, or
retain only20%. This shared answer also affects future Overwhelming Formula
and existing Spell Penetration/Focused Pairing/Annihilator combinations. Do not
activate Combat Casting by silently choosing one; Spellward is independent.

## UP-120 — Warcasting Spellward

Status: Verified (playable delivery pending), 2026-10-02. Spellward is active;
build80192 repairs detached parity and principal24023 passes21/21 in5.858s.
Activated build12348 exits0; native60120 passes22/22 in6.000s, zero skips,
including projected-only control flips without changing live stacks.
Data/schema/inventory35/35 and module drift check pass. Independent Astra
review has no blocker. Coverage167->168/310 active,143->142 planned;
Warcasting4->5/10. No new saved state or polling. Bespoke art remains Not done,
generic presentation Provisional. No GUI or playable promotion.
Source slice committed and pushed as9d8c5f4d4; build/native evidence above is
pre-commit frozen-candidate evidence, not a promoted immutable playable package.

Original UP-023 Basic perk candidate while
Mire Shaper awaits its cap decision. Friendly stacks receive10% less magical
damage; this replaces old Resistance, not hostile-spell rejection. Map the
canonical multiplicative reduction/cap, existing inherited perk bonus lifecycle,
authoritative and detached damage, and legal Basic offer/native seams. Root
owns semantics/registration/builds/Git; Luna maps before bounded ownership.
Require exact unprotected and combined-protection damage, nondamaging spell
preservation, inactive/rank-loss guards and minimum AI parity. Do not add
polling, mirrored state or spell resistance. No GUI or playable promotion.

Architecture checkpoint: do not put this defense only in the original hero's
static bonus DAG. Current controlling hero must govern friendly protection,
including control changes and summoned/gated stacks. Resolve that hero through
the existing battle callback, supply10% as an independent source to shared
magical reduction before its95% cap/penetration, and include recipient collateral
and scripted creature damage. This is on-demand damage resolution, not polling
or a new persistent state field. Native worker owns an isolated fixture.

Focused native21882 found detached AI damage220 instead of live198; other20
cases passed. Proxy hero visibility discarded the opposing hero's protection.
A narrow computed-defense override forwards the projected unit to the subject
callback, preserving projected ownership and hidden hero information. Build80192
is validating that repair; registry remains planned until parity passes.

## UP-119 — Nature Mire Shaper

Status: Blocked on design clarification, 2026-10-02. Continue UP-023 Phase1 coverage with Advanced
Nature Mire Shaper: Quicksand creates one additional patch. Map the shared
count formula and base cap, exact sequential placement, Lua validation and AI
consumers before assigning ownership. Root owns semantics/configuration/builds
and coverage; Luna owns bounded exploration and implementation. Require legal
Advanced acquisition, count at low power and the base cap, actual authoritative
paid placement, inactive/legacy guards and detached AI evidence. Do not add
polling or saved counters. UI and spell help must agree with the required count.
No GUI or playable promotion; bespoke perk art remains independently tracked.
Read-only map confirms the shared quicksandPatchCount feeds Mechanics, Lua,
server exact-count validation, placement UI and AI. No extra state is needed.
The earlier Quicksand checkpoint explicitly preserved a cap ambiguity: does
Mire Shaper allow six patches, or is five an absolute maximum? Asked the user;
do not activate or claim coverage before that answer. Root's initial after-cap
interpretation is a recommendation, not authority. Workers are freezing at a
safe checkpoint. Existing spell and legacy profiles remain unchanged.

## UP-118 — Earthquake foundation and Geomancer

Status: Verified (playable delivery pending), 2026-10-02. Earthquake's field
and selected siege paths and Advanced Geomancer are implemented and active.
Final build80978 exits0; final native91000 passes63/63 in8.411s, zero skips.
Data/schema/inventory35/35 and module drift check pass. Independent Astra
review has no blocking findings. Coverage166->167/310 active perks,144->143
planned; Nature6->7/10. Combat identity count remains60/67 plus five Mass
variants: Earthquake was already catalogued, but its principal behavior now
has evidence. No GUI, playable promotion or final-art acceptance.
Phase2 retains wider save/Charge/Pursuit/return-movement interactions, special
Metamagic-event forecast modifiers and optional destructible scenery handling.
Canonical Earthquake has selected-area siege structural damage and a radius2
field mode dealing30+0.8×SP to grounded stacks, then creating3-round Fractured
Ground that adds1 movement point per entered hex without reducing Initiative.
Flying travel ignores the extra cost. Advanced Geomancer adds25% structural
damage and one Fractured Ground round. Map both current paths, saved state,
movement/accessibility, previews and AI before assigning exclusive runtime
ownership. Do not treat the existing spell identity as completed behavior or
activate the perk from metadata. Root owns architecture, config, builds and
coverage. No GUI/promotion; focused validation and Phase2 deferrals.

Historical consumer integration checkpoint: field damage/terrain and deterministic selected
siege sections are implemented through the saved-v3 marker and real Lua effect.
Legacy profiles retain Catapult behavior. Structural damage is an explicit
Phase1 tunable100 HP per section (Geomancer125), because no absolute amount is
authored. Movement budget is distinct from physical travel in server and AI
Charge paths; return movement checks weighted affordability. Geomancer remains
planned until focused actual casts pass. The first Python gate's6 legacy-fixture
conversion errors were repaired without relaxing old schemas;35 data checks now
pass. Client/test build86453 is running. Independent Astra source review found
no blocker. Borrowed Quicksand field art is Not done, not final Fractured Ground
art; optional destructible scenery remains deferred because no destructibility
marker exists. No playable promotion or graphical acceptance is claimed.

Bounded foundation checkpoint: generic spell-created obstacle movementCost is
in source with JSON/network and append-only binary representation, zero-cost
legacy defaults, overlap maximum and newly entered footprint charging. Flying
reachability is unchanged. Root repaired a pre-validation double-count of the
surcharge and avoids footprint work when no terrain cost exists. Client54585,
test-target92767 and focused fixture build82811 exit0. Native72881 passes12/12
in3.287s, zero skips: seven new weighted-cost/state cases and five existing
detached obstacle guards. No complete spell/perk coverage is added. An additional independent reviewer
spawn was rejected by the service thread limit; root owns direct review.
This does not complete Earthquake or activate Geomancer. Before either consumer
is enabled, separate weighted movement budget from actual traveled hexes in
the server movement result (Charge/Pursuit), add authoritative field creation
and feedback, and implement selected-area siege structural damage. Existing
hero Earthquake currently uses legacy1-point damage against structural HP because
the Catapult callback only supplies structuralDamage for a unit caster.

## UP-117 — Nature's Wrath foundation and Worldroot

Status: Mapping, 2026-10-02; next UP-023 missing combat identity while the
frozen UP-115/116 candidate builds. Canonical Level5 Nature spell chains through
at most17 distinct stacks by nearest unvisited proximity, deals Nature damage
to enemies and ordinary survivor-only healing to allies, starts at110+2×SP,
and retains93% power per jump. Worldroot adds two valid stacks and10% to the
Spell Power-derived term. Map existing chain path, target defenses, healing,
shared prediction/AI and preview infrastructure; identify unspecified chaining
range/tie/eligibility rules rather than guessing. Read-only mapping is not
implementation, activation or completed coverage. Root owns final semantics.

Read-only map complete: existing Lua chain resolution has no jump-distance
limit and uses the engine's deterministic closest-hex tie policy. Damage and
survivor-only healing can share a custom effect and detached castEval, but the
current affected-stack preview loses hop order. Asked for the missing range,
healthy-ally/blocked-stack conduction, and resisted-hit continuation policies.
Do not activate or silently infer those rules; retain mapping for the next
implementation slice after answers. Worldroot's explicit two-extra-stack rule
means19 maximum; its10% modifier affects only the Spell Power term.

## UP-115 — Light Sanctuary Keeper

Status: Verified (playable delivery pending), 2026-10-02. Sanctuary Keeper is
active with exact source-linked+2 Morale snapshots, non-stacking recast,
non-perk recast cleanup, Wait/Defend preservation and movement/attack/Dispel
removal. Saved-v2 and materialized detached/live guards pass. Real BattleAI
selects Sanctuary and the authoritative processor accepts the paid cast.
Client90317 and final both-target10531 exit0. Principal20512 passes25/25
in6.559s; activated76413 passes30/30 in7.833s, zero skips. Data/schema/inventory
34/34 and module check pass. Independent review has no remaining blocker.
Perks164->166/310 across UP-115/116; Light8->9/10, Nature5->6/10.
Failures/repairs are persisted. Phase2 retains negative-Morale-only tactical
selection, specialty and wider save/modifier interactions. Generic UI is
Provisional; bespoke art Not done. No GUI or playable promotion.

Original UP-023 Phase1 missing-specification continuation:
Canonical Basic perk: a friendly stack protected by Sanctuary gains+2 Morale
while Sanctuary remains active. Map the cast marker, action/removal lifecycle,
existing bonus limiters and detached AI projection before choosing the smallest
shared implementation. No extra saved counters or update polling. Require legal
Basic acquisition, actual cast, exact+2 snapshot, refresh without stacking,
movement/attack/Dispel removal, inactive/legacy guards and detached/live evidence.
Root owns architecture/registration/build/Git; workers own disjoint runtime and
fixture slices. No GUI/promotion or new art. Wider interactions belong to Phase2.

## UP-116 — Nature Venomancer

Status: Verified (playable delivery pending), 2026-10-02. Venomancer is active:
whole stored integer Poison Base gains20%, including fixed20; Basic SP100
stores92 and ticks92/138/184. School/Spellcraft/Empower composition, legal
Basic offers, inactive/v2 guards, materialized detached/live parity and actual
paid AI-selected cast pass. Toxic Spines retains its independent reflected-loss
formula; its fixture now legally selects Basic perk then advances Bulwark to
Advanced for nonzero reflection. Same UP-115 principal/activated/build/data
gates pass; neither new saved fields nor per-update polling were added.
Coverage166/310 active,144 planned. Broader interactions remain Phase2;
neutral fallback art Not done, generic UI Provisional. No GUI/promotion.

Original independent UP-023 Phase1 missing-specification slice:
Canonical Basic perk increases Poison's Base Poison value by20%. Map the
Nature spell's Poison cast-time snapshot, tick progression, School/Spellcraft scaling
and detached AI before implementation. Physical Toxic Spines must not inherit
this spell-casting perk (the resulting Poison is still a bodily affliction).
Require legal Basic acquisition, exact boosted base and
all three ticks, stored-once scaling, inactive/legacy guards, physical Poison
exclusion and focused production/native/AI evidence. No numerical redesign,
new polling, GUI or playable promotion. Keep file ownership separate fromUP-115.

## UP-112 — Shadow Blood Drinker and Painweaver

Status: Verified (playable delivery pending), 2026-10-01. Both Basic perks are
active. Final both-target68123 exits0; principal6616 passes23/23 in6.246s and
activated33834 passes29/29 in7.838s, zero skips. Data/inventory19/19 and module
drift check pass. Coverage159->161/310; Shadow6->8/10. Legal offers, actual
clipped75% healing, survivor-only repair,20% SP-only Hex snapshots, inactive/
v2 guards and detached/authoritative injury parity pass. Independent review
has no remaining blocker. Build/fixture failures and repairs are persisted.
Phase2 retains strategic AI nonselection, reflected paired-spell semantics,
recipient-healing preview and wider modifier/save interactions. No GUI or
playable promotion; generic UI provisional, authored art Not done.

Read-only mapping checkpoint: Blood Drinker already has a dormant 75% hook in
`scripts/spells/lifeDrain.lua`; it uses actual clipped damage and ordinary healing.
Require selected-perk native coverage before activation, not duplicate runtime
code. Painweaver must modify Hex's cast-time Spell Power term only; its existing
bonus snapshot carries the result through delayed triggers and detached AI.
Extending the generic damage-perk helper alone does not reach Hex's custom Lua
formula. No new save state is expected. Maps are evidence, not completed coverage.

Implementation checkpoint: Three bounded Luna workers owned Life Drain
coverage, Hex runtime/coverage, and detached AI fixtures in disjoint files.
Root owned registration, build/native validation and integration. Continue
UP-023's missing Phase1 coverage
after the pushed Havoc slice. Basic Blood Drinker changes Life Drain's friendly
healing from60% to75% of actual damage dealt. Basic Painweaver adds20% only to
Hex of Pain's Spell Power-derived damage component. Map actual damage/overkill,
paired targeting, delayed Hex state, shared prediction and AI consumers before
implementation. Do not scale fixed bases, invent healing from theoretical
damage, restore genuine casualties through ordinary healing, or reapply a
stored damage bonus on each trigger. No activation or completed coverage from
mapping. Root owns semantics and integration. Acceptance: legal Basic offers,
exact authoritative effects, inactive guards, detached/live parity and focused
build/native/data evidence. No GUI or playable promotion.

## UP-114 — Distinct perk-granted Mass spell entries

Current continuation verified, 2026-10-02: distinct Mass Slow is active. Temporal
Field grants a permanent virtual spell source with a physical Spellbook; it
cannot be ordinarily learned. Saved-v3 family scaling applies60% after the
ordinary cap and specialty, preserves duration, charges triple listed Mana
before Wisdom, and replaces one shared Initiative status. Repeat casting,
both refresh directions, both immunities, Spell Lock and detached/live parity
pass. Old snapshots retain their toggle/budget; new profiles reject it.
Client33547 and final both-target53442 exit0. Principal7002 passes22/22 in5.821s;
activated47843 passes36/36 in9.512s, zero skips, including actual AI selection
and server acceptance, Communion and Heavenly Gale guards. Data/schema/
inventory34/34 and module drift check pass. Independent review has no remaining
blocker. Distinct variants4->5/5; active perks remain164/310 because Temporal
Field was already active. Failures and repairs are recorded. Phase2 retains
broader save/modifier and rendered interaction checks; no GUI or promotion.
UP-114 is native verified, playable delivery pending. Next unblocked missing
coverage: Light's Basic Sanctuary Keeper (Sanctuary-linked +2 Morale).

Current continuation verified, 2026-10-02: Mass Regeneration and Advanced
Verdant Communion are active. Saved-v3 physical-book virtual grants, living ally
scope (excluding clone/phantom/siege/undead/nonliving/mechanical/locked/immune),
triple listed cost, ranked rate snapshots, future wounds, survivor-only healing,
family refresh and already-mutated detached state pass focused native checks.
Both-target55569 exits0; principal79005 passes26/26 in7.453s and activated81701
passes30/30 in8.697s, zero skips. Real AI selection and server acceptance pass
after fixing empty candidate destinations to emit the protocol's NO_LOCATION
sentinel. Data/schema/inventory33/33 and module check pass. Independent review
has no remaining material blocker. Coverage163->164/310, Nature4->5/10, distinct
variants3->4/5. Build/test failures and repairs are recorded. Phase2 retains
broad save/modifier interactions and diagnosis of round advance with the
synthetic eligibility roster; the bounded minimal refresh roster passes.
No GUI or playable promotion. Distinct Mass Slow/Temporal Field is next.

Latest continuation verified: Mass Bless and Advanced Litany are active.
Bless-family capped School scaling, Benediction, triple listed cost before
Wisdom, ally scope, both immunities, ordinary-source exclusion and virtual grant
revocation have focused evidence. Ordinary and Mass Bless explicitly replace
one family status; prior Bless refresh and Curse removal agree in detached and
authoritative paths. Client23367 and both-target20799/28088 exit0. Repaired
31806 passes55/55 in10.977s; activated5126 passes55/55 in11.867s, zero skips.
Data/schema/inventory32/32 and module check pass; independent final review has
no material blocker. Coverage162->163/310, Light7->8/10, distinct variants2->3/5.
The stale Bless description assertion now passes and is no longer a deferred
failure. Phase2 retains broad save/load, AI selection and modifier interactions.
No GUI or playable promotion. Mass Regeneration/Verdant Communion is next;
distinct Mass Slow remains missing. UP-114 remains open.

Status: Partially verified (playable delivery pending), 2026-10-01. Mass Curse
and Mass Sorrow plus Expert Grand Malediction are active. Saved-v3 perk-only
virtual grants require a physical Spellbook and do not mutate durable knowledge.
Base-family statuses refresh one effect; both ordinary and variant immunities
apply. Effect application now supports previously-mutated detached units.
Final both-target37060 exits0; principal99435 passes48/48 in7.091s and activated
21991 passes48/48 in7.326s, zero skips. Data/inventory/schema32/32 and module
drift check pass. Coverage161->162/310; Shadow8->9/10; distinct variants0->2/5.
Independent final review has no material blocker. Restrict this slice to100%
until Mass Slow's60% consumer exists. Older-profile fixture adapters exclude
new metadata rather than interpreting it under v1/v2. Phase2 retains wider
save/map-ban/counter/dispel interactions and one known stale Bless tooltip-text
assertion, explicitly excluded from the final filter. No new persistent state,
polling, GUI execution or playable promotion. Mass Bless/Litany is next;
Mass Regeneration and distinct Mass Slow remain missing. UP-114 stays open.
Read-only map complete: use ordinary SpellID action transport and the existing
spell-source discovery/cast-admission seam, not another action flag or toggle.
No generic perk-to-spell source exists yet. Ordinary-acquisition exclusions
already exist but direct scroll sources also need the canonical perk-only gate.
Shared base-family handling is necessary: Slow's scale is keyed to its old
boolean mode, and Regeneration's single-target validation and wound markers
are keyed to the base ID. Merely duplicating JSON entries would be incorrect.
Current Temporal Field also has a once-per-combat ledger incompatible with the
canonical permanent spell option; preserve old saved behavior deliberately,
not as the new runtime rule. Root must choose family/grant and saved-profile
architecture before splitting content, UI and AI ownership. No edits or tests
were performed by the mapper; coverage remains0/5 distinct entries.
Canonical Magic proficiency and casting variants requires distinct spell entries,
not toggles or automatic Expert transformations: Mass Bless, Mass Curse, Mass
Sorrow, Mass Regeneration and Mass Slow. Perk grants govern availability;
ordinary learning sources must not grant these entries. Each costs three times
the base listed Mana before Wisdom; Mass Slow alone uses60% of the base magnitude.
Map the existing Mass Slow transport/AI/UI and generic spell-grant seams before
choosing architecture. Grand Malediction depends on Mass Curse/Sorrow. Root owns
the shared architecture and registration; no coverage claim from source searches.
Acceptance: distinct selectable entries, proper grants/removal, cost/effect parity,
eligible mass targeting, ordinary-acquisition exclusion, saved state and minimum
AI hooks with focused build/native evidence. No GUI or playable promotion.

## UP-113 — Shadow Plaguebearer

Read-only mapping checkpoint: design ambiguity blocks this perk alone. Neither
the canonical text nor runtime defines the normal propagation limit to which
the perk adds one. Current infections each last three rounds, spread to one
neighbor per processed activation, and reset spread attempts in descendants;
there is no enforced chain-wide cap. Resolve whether the intended limit is
per infection, per propagation path, or across the original cast before coding.
Marker-local metadata can represent a path allowance; a total-cast budget needs
shared lineage state. Do not invent a cap or activate the perk from this map.
An asynchronous clarification asks the user for the normal limit's scope and
number; continue independent Blood Drinker/Painweaver coverage meanwhile.

Status: Read-only map, 2026-10-01. Missing Advanced Shadow perk: Plague may
propagate one additional time beyond its normal limit. Map the shared chain
limit, caster/source provenance and lifetime, status representation and AI
forecast before choosing state ownership. Preserve ordinary Plague potency,
targeting and propagation rules; do not silently increase damage or introduce
unlimited recursive spread. Acceptance: legal Advanced offer, exact baseline
versus perk propagation limit, accepted cast and real propagation, inactive
guards, save/replica sanity where needed and focused build/native/data checks.
Root owns architecture, serialization and shared integration. No activation
or coverage increase from a map.

## UP-111 — Havoc Cataclysm

Status: Read-only map, 2026-10-01. Next missing Expert Havoc perk while the
UP-109/110 candidate builds and remains frozen. Canonical: Armageddon gains
20% to its Spell Power-derived damage component and destroys ordinary magical
obstacles as well as physical ones. Map both clauses, obstacle exclusions,
shared cast/prediction and detached AI paths before assigning implementation.
Do not silently reduce this to a damage bonus, destroy permanent moats or
fortifications without specification authority, or activate from a map.
Root owns semantics and integration; no production writes during the current
build/native gate. Acceptance: legal Expert offer, unchanged flat base, exact
SP-only bonus, authoritative obstacle removal and exclusions, detached/live
parity, inactive guards and focused build/native/data evidence.
Read-only map is complete. Current Armageddon's damage-only Lua effect also
lacks its baseline physical-obstacle cleanup; implement that clause as well,
not merely the perk multiplier. The existing removeObstacle packet path is
shared with detached forecasts. Ordinary scenery has a clear USUAL class;
SPELL_CREATED also includes some moat representations, so it is not a safe
blanket deletion category. The user is asked whether ordinary hazards/barriers
include hidden Land Mines while all moats/permanent siege structures survive.
Root must settle that filter before implementation. Hidden-obstacle visibility
in AI projections is preserved; fortification damage is a separate clause.
No source implementation, activation or coverage increase is claimed.

## UP-110 — Havoc Pyromancer and Cryomancer

Status: Verified (playable delivery pending), 2026-10-01. Adjacent missing Basic Havoc coverage,
independent from Controlled Blast targeting if file ownership can be separated.
Pyromancer adds15% to the Spell Power-derived damage of Fireball, Fire Wall and
Inferno; Cryomancer adds20% to Ice Bolt and Frost Ring. Preserve flat bases and
shared School/Spellcraft math; include Fire Wall's stored hazard damage and
detached AI forecasts rather than changing only instant casts. Root owns
architecture and assigns implementation only after the modifier/path map is
complete. No new serialized state unless evidence requires it; no activation
or coverage claim from mapping. Acceptance: legal Basic offers, exact
SP-only scaling with unchanged bases, live casts/hazards, inactive guards,
shared predictions/AI and focused build/native/data checks.
The completed map identifies a damage-only coefficient shared by cast mechanics
and spellbook estimates; do not increase raw Spell Power or the general
coefficient, which would also strengthen Ice Bolt's slow and durations. Fire
Wall snapshots the cast damage in its existing obstacle state and must not
apply the perk again on contact. A bounded Luna worker owns the modifier and
hazard fixture; root owns integration and accepted-offer/AI evidence. Registry
activation and completed coverage await focused verification.
Verified checkpoint: client38230, repaired both-target48589 and v3-fixture
build10278 exit0. Repaired principal5598 passes20/20 in5.977s; activated19887
passes28/28 in8.153s, zero skips. Both Basic perks are active in canonical and
bundled registries. Data/inventory19/19 and module drift check pass. Flat bases,
actual casts, prediction and exact Fire Wall snapshot/trigger are verified.
Coverage156->159/310 active,154->151 planned; Havoc6active/4planned. No new
saved state or polling. Phase2 retains wider coefficient/defense interactions,
proxy/reflection cases and legacy hybrid-fixture audit. Authored art Not done,
generic UI provisional; no GUI or playable promotion.

## UP-109 — Havoc Controlled Blast

Status: Verified (playable delivery pending), 2026-10-01. Continue UP-023 missing Phase1 coverage while
Divine Mandate and Elemental Rebirth remain at their recorded item-level design
gates. Canonical Advanced perk: when Fireball, Inferno or Meteor Shower is centered
on a hex occupied by a friendly stack, exclude that stack from spell damage.
Other stacks in the area are unchanged. Frost Ring already has a safe center;
Armageddon remains indiscriminate. Map shared spell targeting/effect resolution
and detached AI forecasts, saved active-perk eligibility and legal native offers
before assigning bounded ownership. Root owns architecture, registration,
CMake/docs/build/native/Git. No GUI/promotion. Acceptance: accepted centered
casts, exact protected-center versus adjacent/enemy damage, inactive and excluded
spell guards, minimum AI use/projection and focused build/native/data evidence.
No implementation/activation/coverage increase is claimed by a source map.
Runtime and fixture maps are complete. Root selected one shared effect-target
filter in unitEffect's range transform, exposed through the existing Mechanics
Lua proxy. It resolves the original center occupant and current controlling
side, including either hex of a double-wide stack. This covers authoritative
casts, detached AI projections, highlights and damage previews without changing
area geometry or introducing saved state. Separate Luna workers own the proxy/
script and principal acquisition/cast fixtures; root owns the AI parity fixture.
Precise Casting remains a separate planned perk. Reflected-cast inheritance and
wider status interactions are recorded for Phase 2, not broadened implicitly.
Client38230 and repaired both-target48589 exit0. Principal73570 passes13/17
with zero skips; four Controlled Blast setup failures come from an invalid
hybrid v2 fixture retaining selectedPlacement. The owner is switching only
these new/modified current-feature cases to savedV3Formula; assertions remain
unchanged. Production, AI parity, legal acquisition/save-load and Pyro/Cryo
damage/hazard cases already pass. Activation remains held pending repaired run.
Repair verified: v3-fixture build10278 exits0, principal5598 passes20/20 and
activated19887 passes28/28, zero skips. Selected current-controller center
protection for all three spells, either double-wide footprint, adjacent friendly
collateral, isolated hover, Frost Ring/Armageddon guards, real query/save-load
and detached/accepted AI parity pass. Controlled Blast is now active in canonical
and bundled registries; data/inventory19/19 and module check pass. No new state.
Independent source/fixture review has no remaining blocker. Broad reflected-
cast/status/save interactions remain Phase2. Generic UI is provisional and art
Not done; no rendered/playable acceptance or snapshot promotion is claimed.

## UP-108 — Divine Mandate rank foundation

Status: Read-only map, 2026-10-01. UP-023's missing faction rank effects outrank
further hardening of completed perks in Phase1. Canonical Castle rank: after a
Hero Action casts a Light Spell, immediately issue one Order, or after a Hero
Action issues an Order, immediately cast one Light Spell; once/twice/three times
per combat at Basic/Advanced/Expert. This is a precise paired exception, not a
second general Hero Action currency. Map accepted action admission/resolution,
current saved side state, UI continuation and AI consumers before architecture
or implementation. No production edits during Land Surveyor's frozen build.
Root owns semantics, action economy, persistence/version, ownership boundaries
and integration. Report genuine opt-in/expiry/cancellation ambiguities; do not
silently recreate the former forced Metamagic pending-action lock. Mapping does
not activate any rank or count a mechanic. Acceptance needs accepted paired
actions, Light-only restriction, usage limits, save/replica sanity and minimum
human/AI access with focused compile/native checks.
Read-only maps are complete. Reuse the typed per-side action allowance ledger
with school-restricted Spell grants, not Metamagic's sequence-specific state or
retired forced-action lock. Accepted Order StartAction and accepted BattleSpellCast
are the commit hooks; shared callbacks, ordinary Orders/Spellbook consumers,
generic Faction Skill statuses and detached AI projections all need matching
admission. Canonical UI expressly forbids Activate/Decline prompts. Two item-
level questions are pending: expiry on another accepted combat action versus
round end, and spending usage on completed pair versus opportunity creation.
Do not silently assume the ledger's normal round expiry resolves “immediately.”
No production implementation/activation/count yet; this gate does not block
independent missing coverage.

## UP-107 — Estates Land Surveyor

Status: Verified (playable delivery pending), 2026-10-01. Continue UP-023 Phase1 missing Basic perk
coverage after Financier's focused verification. Canonical: the first mine
captured by this hero each week immediately produces three days of normal
output. Map the authoritative capture-success event, owner transition, per-hero
weekly expenditure, resource replication and minimum AI/native seams. Do not
trigger from merely visiting an already-owned mine or from an unsuccessful
capture. Root owns architecture, save/version integration, activation, CMake,
docs/build/native/Git. No GUI/promotion. Acceptance: legal Basic offer, accepted
capture and correct output, once/week and next-week behavior, inactive guards,
saved/replicated expenditure and focused build/native/data evidence. Mapping
alone does not activate the perk or increase coverage.
Root architecture reuses the single CGMine::flagMine capture-success path for
ordinary and abandoned mines, including victorious guarded capture. The capturing
hero is threaded through that path. After ownership changes, three times the
mine's actual normal dailyIncome (including its ordinary bonuses/handicap) is
granted once per hero per absolute week. A versioned last-use-week hero field
is replicated by the existing SetObjectProperty packet; no new packet hierarchy,
callback bridge or polling scan is needed. The marker is authored before the
resource receipt and does not invalidate the bonus graph/Mana capacity. Root
owns append-only save/wire gates; mine and minimal native-fixture writers have
separate file ownership. This is implementation in progress, not activation.
Production is frozen and independent review reports no blocker. Hardcoded English
capture feedback is deferred polish; it is not artwork/rendered acceptance.
Client-only build11819 is running while the separately owned test fixture is
finished. Do not register/reconfigure test CMake or start a second build/native
process before that handle exits. Active coverage remains155/310.
Client build11819 exits0 (`UP107-client-build.log`). Principal fixture is being
repaired before registration for adjacent accepted movement, neutral-owner income
sampling and direct dependency includes; these are source-review findings, not
a claimed failing native run. No build/native process remains live at this point.
Frozen fixture independently reviewed without blocker; root bounds movement and
routes around prior captured mines rather than traversing their garrison visit.
Baseline13332 and both-target30265 exit0. Principal87442 passes3/3 in1.709s;
activated61224 passes18/18 in7.206s, zero skips. Actual accepted capture/resource
receipt, weekly limit/renewal, saved marker and serialized property replay are
verified. Data/inventory19/19 and module drift check pass. Land Surveyor is
active; coverage156/310,154 planned; Estates4/6. Phase2 retains independent
holders, guarded/abandoned execution, old-format gates, broader fan-out/AI
strategy. English feedback is deferred localization. No GUI/promotion; generic
UI provisional and art Not done. No build/native remains live.

## UP-106 — Estates Financier

Status: Verified (playable delivery pending), 2026-10-01. Independent UP-023 missing
Expert coverage while unresolved Logistics/Luck choices remain item-level
blockers. Canonical perk: at the start of each week gain1% current Gold treasury
as interest, capped at1000 Gold. Map and reuse the existing weekly income/resource
aggregation and active saved-perk gate, including the treasury snapshot used
for all eligible heroes. No daily polling or redundant per-week stored state if
the authoritative calendar event already owns the once-weekly trigger. Separate
Luna maps cover production and legal-offer/native/resource receipt evidence.
Root owns architecture, activation, configuration, CMake/docs/build/native/Git.
Acceptance: legal Expert offer, actual weekly resource packet/treasury gain,
integer/cap/ordinary-day/inactive guards, minimum AI receipt, focused successful
build/native/data gates. Coverage remains154/310 until verified; no GUI/promotion.
Runtime source is frozen in NewTurnProcessor.cpp. Root contract uses one
pre-NewTurn treasury snapshot, floor(max(0, Gold)/100), capped1000 per active
holder, after ordinary income/handicap adjustments; the existing weekly event
includes day0→1 and supplies cadence without redundant saved counters. Separate
fixture ownership covers legal Expert offers and real packet/treasury receipts.
Independent Astra review finds no blocker and no new deferred defect. Both-
target build71297 is live with12 jobs (`UP106-shared-build.log`); re-poll that
handle, do not run native tests or launch a competing build while it is live.
Shared build71297 exits0; native96952 passes12/12 relevant Estate Network,
Tax Collector and existing AI income/receipt tests, zero skips in4.367s
(`UP106-shared.log`/`.xml`). This proves adjacent income regressions, not the
new Financier principal path; registration/counts remain unchanged pending
the isolated frozen fixture. No native or build process remains live.
Focused fixture build25033 failed on the mastery namespace used as a type;
owner repair uses MasteryLevel::Type. Both-target21766 exits0. Principal39424
passes3/3 in58.108s, then activated95915 passes15/15 in61.975s, zero skips.
Data/inventory19/19 and module check pass. Financier is now active; coverage
155/310,155 planned; Estates3/7. Independent source and fixture reviews have
no blocker. The planned-rule fixture proves offer exclusion, not suppression of
an already-selected planned holder; selected-holder rank-loss suppression and
broader calendar/save/client fan-out/AI weekly forecasts remain Phase2 evidence.
Generic offer/description UI is provisional and authored art remains Not done.
No GUI or snapshot promotion; playable delivery remains separate.

## UP-105 — Luck Perfect Fortune

Status: Read-only map, 2026-10-01. Independent UP-023 missing-coverage candidate
while Logistics items await explicit decisions. Canonical Expert perk: the
first eligible attack made by the hero's army each combat triggers positive
Luck automatically. Map shared eligibility, current-controller army ownership,
once-per-combat saved/replicated expenditure and detached AI forecasts; do not
silently redefine eligibility or substitute a chance boost for the guarantee.
Root retains architecture, persistence/version/network, activation, build/native
and Git. No implementation or coverage increase yet. Focused acceptance needs
legal perk offers and actual attacks, one guaranteed eligible strike, subsequent
ordinary Luck, inactive/immune guards and shared AI/save-state sanity.
Resumption audit finds the existing UP-081 source map and pending No Luck
immunity decision. This duplicate selection is superseded by UP-081; do not
repeat its map or implement around that unresolved boundary. UP-106 Financier
is selected instead. No new Perfect Fortune implementation is counted.

## UP-104 — Logistics Pursuit March

Status: Read-only map, 2026-10-01. Independent UP-023 missing-coverage candidate
while UP-103 awaits its item-level stacking decision. Canonical Advanced perk:
after winning combat recover10% maximum daily Movement, once per day. Map the
authoritative victory reward, surviving winning hero, saved/replicated daily
expenditure and minimum AI/native seams before root assigns safe ownership.
No new implementation/activation/count is claimed. Root retains semantics,
state/version/network integration, CMake/config/docs/build/native and Git.
Acceptance: legal perk offer, accepted victory and exact recovery, once/day and
next-day behavior, loss/inactive guards, persistence and focused native evidence.
Runtime map complete: BattleResultProcessor::battleFinalize is the authoritative
reward point after BattleResultsApplied and before hero removal. Current-mode
movementPointsLimit supplies land/sea capacity; SetMovePoints replicates recovery.
Castle Gate supplies a saved last-use-day/packet pattern. AI ChainActor consumes
remaining Movement, but AIGateway::heroMovePointsChanged is currently a no-op;
check an event-driven path invalidation rather than adding a polling scan.
Item-level question asked: whether recovery caps at daily maximum and whether
a zero-recovery victory spends the daily allowance. No production implementation
while that materially different rule remains unresolved. A declared winner
with surviving units is the eligible hero; do not silently narrow wins to only
NORMAL results when the opponent's retreat/surrender still declares a winner.

## UP-103 — Logistics Rapid Embarkation

Status: Open; design-choice blocker, 2026-10-01. Continue UP-023 Phase1 missing
perk coverage after pushed1b3088ec9 and a clean worktree. The canonical Advanced
perk makes embarking/disembarking cost10% of maximum daily Movement. Map the
complete boarding charge, source/destination pool conversion and admission;
do not merely discount the adjacent step while retaining the old all-remaining
charge. Separate Luna maps cover production and legal-offer/native/AI seams.
Root owns semantics, architecture, configuration, CMake, build/native and Git.
Preserve ordinary travel, blocked landing, boats/airship distinction, existing
free-boarding effects and saved planned-registry gates. No GUI or promotion.
Acceptance: legal perk acquisition, exact forecasts versus accepted boarding/
deboarding spending, insufficient-Movement rejection, inactive guards, minimum
AI route consumption, successful build and focused native/data gates. Coverage
remains154/310 pending verified activation. Item-level ambiguities do not block
other independent missing specification work.
Item-level design question asked: Navigation halves boarding costs, while Rapid
Embarkation specifies10% maximum daily Movement. Does their combination remain
fixed10% (Navigation retains sea-capacity benefit), or halve again to5%? Do not
silently select one stacking rule. Continue read-only maps; postpone production
activation until resolved, and use another unblocked missing item if needed.
Runtime map complete: CPathfinderHelper::getMovementCost supplies admission;
CGHeroInstance::movementPointsAfterEmbark supplies total debit and proportional
source/destination pool conversion. Apply any fixed fee in source-pool units
before that conversion, and preserve SAIL-only transitions, ordinary WATER,
blocked/coastal landing and the existing airship exclusion. TurnInfo can cache
saved active-perk eligibility once; no new serialized state is required. Human
and Nullkiller paths already share these routines and perk invalidation hooks.
The source map is not implementation evidence; status stays planned.

## UP-102 — Logistics road and terrain movement perks

Status: Verified (playable delivery pending), 2026-10-01. Continue UP-023
Phase1 missing perk coverage after pushedbc39d04a7 and a clean worktree.
Roadmaster reduces normal road movement cost by an additional25%; Wayfarer caps
passable-terrain cost at125% of base clear-terrain cost. These provide missing
Advanced/Expert Logistics progression and must apply through the shared movement
calculation used by authority, player path prediction and AI, not a frontend-only
discount. Preserve blocked terrain, movement modes, ordinary road/terrain rules,
diagonal/end-of-day behavior and old-save activation gates. Map formula ordering
and minimal actual-movement/native fixtures before assigning ownership. Root owns
architecture, activation, registration, CMake/docs/builds/Git; no GUI or promotion.
Acceptance: legal perk offers, exact road/capped terrain forecasts and accepted
movement spending, absent-perk/ordinary mode guards, shared AI path usage, focused
build/native gates and deferred integration findings. Counts stay152/310 until
verified. Existing item-level design questions remain independent blockers.
Shared map complete: CPathfinderHelper::getMovementCost feeds authoritative
admission/spending, player CPathfinder and Nullkiller's AI pathfinder. Root chooses
the canonical single-final-ceiling policy: cap the terrain multiplier at5/4 after
Pathfinding, before roads and explicit travel multipliers; Roadmaster applies3/4
to the road factor before that same final ceiling. Do not integer-round at an
intermediate cap or discount the already-rounded cost. Cached TurnInfo flags are
derived once from saved active perk/rank data, not queried for every path node.
No new gameplay state/serialization is needed; old saved registries are not
silently rewritten. The Luna cost mapper now owns the bounded shared helper/
TurnInfo/CPathfinder production edit and pure formula tests; an independent
consumer map prepares accepted-movement and AI evidence. Root retains activation,
build/version integration, documentation and Git.
The runtime/pure-formula source is frozen. The consumer map confirms existing
HeroPerkChosen path invalidation reaches both human and Nullkiller caches; no
parallel UI/AI cost implementation is required. An independent Astra reviews
the shared candidate while a Luna owns an isolated legal-offer/accepted-movement
fixture. Root starts only the frozen shared build; the not-yet-created fixture
is not registered prematurely. Registration remains planned pending native gates.
Shared build46311 exits0; native66894 passes21/21 pure formula and existing
movement/boarding/Water Walk/Fly/legality cases, zero skips in3.521s. Independent
Astra source review reports no blocker. This is shared-source evidence, not
Roadmaster/Wayfarer accepted-offer completion. Separate Luna fixture owners now
cover the real movement path and the isolated Nullkiller projected-route path;
neither edits production/config/CMake or runs competing builds/native.
The accepted-movement fixture is frozen and registered. Root corrected draft
expectations before execution (adjacent versus multi-step cost and the active
terrain cap); no production rule was weakened. Both-target build76132 is live
with12 jobs (`UP102-movement-fixture-build.log`). AI fixture ownership remains
separate and its unfinished source is not registered. Re-poll the same build
handle; no native execution while it is live.
Build76132 exits0; native72673 passes23/23, zero skips in4.249s, including
two legal-offer/forecast/accepted-movement cases (`UP102-movement-fixture.log`
and `.xml`). AI source is now frozen and registered; root repairs its source-
terrain setup before execution, without changing the production formula.
Both-target build20420 is live (`UP102-ai-fixture-build.log`). Full activation
and coverage still await that focused AI route/cache gate.
Final gate: both-target20420 exits0; activated28363 passes25/25, zero skips
in4.827s (`UP102-activated.log`/`.xml`). Legal Scouting→Roadmaster→Wayfarer
offers, literal forecasts and accepted spending, saved-planned/blocked guards,
and actual Nullkiller projected routes after cache invalidation pass. Data/
inventory19/19 and module drift check pass. Both registry copies are active;
coverage152→154/310, planned158→156, Logistics5active/5planned. Binary SHA-256:
`72dcd031ee08bc4342b2a472372608965f97c6f18cc46e7e82a2d7d8d898cfc2`.
Independent production review has no blocker. Phase2 retains client visitor
fan-out rather than direct interface-hook execution, wider multi-day/mode/perk
interactions and full old-save loading evidence. No new serialized state; no
GUI, artwork approval or playable snapshot promotion is claimed.

## UP-101 — Quartermaster extra war-machine activation

Status: Verified (playable delivery pending), 2026-10-01. Continue UP-023 Phase1
coverage with the canonical Basic War Machines perk: once per combat, while
the Ammo Cart survives, the first allied war machine other than the cart to
complete an activation immediately receives an additional activation at 50%
effectiveness. Two independent Luna maps cover shared/server lifecycle and
UI/AI/fixture seams. Root owns architecture, registration, persistence/version
integration, focused builds and Git. No substitute automatic second shot: this
must be a genuine activation, including applicable damage, healing and siege
output. Acceptance requires a legal saved perk offer, accepted principal actions,
once-per-combat/cart-survival guards, shared output predictions and minimum AI
use. Coverage remains151/310 until implementation and focused gates pass.
Field Workshop's destroyed-target scope remains pending independently; do not
silently resolve it or block all other missing implementation work on it.
Consumer map complete: Tent forecasts cap healing by missing HP, so apply 50%
to raw Siege output before that cap, not to the forecast result. Actual Tent
healing enters `BattleActionProcessor::doHealAction`; human HEAL preview uses
`getFirstAidHealValue`. Ballista uses the shared damage-script payload; Tent and
Catapult bypass that calculator. Catapult raw structural output is converted in
`luascript/api/callback/ServerCallback.cpp::catapultAttack` after hit quality and
before packet application. Its existing UI preview is empty, and AI selects a
legal non-destroyed part without evaluating structural damage. Tent AI currently
chooses by missing HP; use the shared reduced-output forecast where relevant.
Root category interpretation follows the canonical distinction between war
machines and defensive structures: Ballista, Catapult and Tent qualify; Ammo
Cart and turret stacks do not. Use current-controller hero/side ownership.
Architecture direction: side-owned saved/replicated once-per-combat expenditure
and active extra-activation identity/output, with a dedicated genuine turn reason.
Do not duplicate the allowance in transient unit fields that CStack's binary
serialization omits. Detached AI battle copies must retain the same state.
Completion trigger belongs after same-activation continuation returns in
`onActionMade`: Master Gunner's first shot must not trigger Quartermaster before
its second shot or explicit decline ends that activation. Spend before dispatch,
refresh actual activation lifecycle, and preserve the reduced output through
Hero Actions and Master Gunner continuations. Clear it at real completion;
exclude Morale recursion and duplicate ordinary queue turns. Principal fixtures
should use legal perk offers and accepted Ballista/Tent/Catapult actions; direct
CatapultAttack injection alone is insufficient accepted-action evidence.
Runtime map is complete. Root corrected one mapping inference: current
`CUnitState::afterGetsTurn` resets moved/cast flags only for Morale; the full
waiting/moved/Morale reset is in `afterNewRound`, not automatic for every genuine
turn reason. Quartermaster needs an explicit safe action-resource reset, without
claiming the existing path already provides it or pretending it is Morale.
Wait is not activation completion; its delayed activation must retain the
reduced-output identity rather than prematurely spend/clear a second lifecycle.
Master Gunner's second shot remains 60% of this activation's 50% output (30% of
ordinary output), with independently chosen targets and no extra allowance.
Prepared ownership: runtime writer shared state/callbacks/pack/server/output;
consumer writer detached AI copy/projections and client status/preview; tester
isolated new native fixture. Root owns append-only version/type registration,
CMake, config/module/inventory/docs, serial build/native gates and Git. No
production source or coverage increase is claimed by this completed map.
Implementation delegation started: independent Luna runtime and consumer owners
are active. The third fixture spawn was rejected by the service thread limit;
assign it when a slot frees without duplicating source ownership. Root appends
one save feature for the generic reduced extra activation and owns build/type
registration. Keep Quartermaster planned until the principal action gates pass.
The rejected third spawn was recovered by assigning the completed Luna mapper
the isolated fixture task through a follow-up; four agents including root are
now active. The tester owns only NewHorizonsQuartermasterTest.cpp. Confirmed
consumer APIs share side state, activation output percent, raw scaled Tent
healing and raw scaled Catapult structural output; ordinary client state
application requires no new frontend-specific packet event.
Fixture scope correction: Quartermaster and Master Gunner both require Basic,
and the approved one-per-tier progression cannot legally select both for one
hero. Preserve that model; do not rewrite perk requirements or bypass offers to
manufacture a combined principal fixture. Quartermaster's accepted-action gate
uses its legal offer alone. A detached generic percentage-composition check may
prove 50% times60%, but is not evidence of a playable two-Basic-perk hero.
Consumer source is frozen. An actual Astra reviewer is now inspecting the
candidate; runtime and isolated fixture remain under their exclusive owners.
Phase2 retains future-lookahead consumption of the copied reduced identity;
principal current-branch forecasts must already match reduced output.
Runtime, consumer and six-case fixture sources are frozen. Independent Astra
review reports no remaining blocker after fixing terminal battle lifetime,
lightweight Catapult proxy dereference and the missing Fire Wall activation hook.
Root integrated a small production-AI Tent selection check after the tester
follow-up was service-rejected; its returned action is submitted authoritatively.
Both-target build88648 is running with12 jobs (`UP101-build.log`); preserve its
live handle and do not execute native tests alongside it. Quartermaster remains
planned and coverage151/310 until the six focused cases pass. No GUI, artwork
approval or playable promotion is claimed.
Build88648 exits1 on the AI heal amount's mutable-reference contract. Root uses
a fresh per-target mutable copy, retaining the failed run and unchanged formula/
fixture expectations. No native execution or activation yet; repaired build
will reuse the same build tree and12-job limit after terminal failure is confirmed.
Repaired build66614 is confirmed live through its original CMake/Ninja processes
after the tool lost that session handle. A replacement observer monitors the same
process; no competing build or native run was started. Preserve the repaired log
and obtain terminal build evidence before the principal gate. The preceding
implementation cycle was progress; this checkpoint is a verified process wait.
The repaired build finishes both links and the subsequent target-freshness check
exits0. Principal73624 runs six cases with zero skips: five pass; the siege case
fails activation setup before structural-output checks. A new bounded Luna
fixture owner diagnoses that failure. Registration stays planned and coverage
unchanged until the repaired principal gate passes.
Final gate: fixture build21374 exits0. Repaired principal47670 passes6/6 in2.277s;
activated88418 passes22/22 Quartermaster/Master Gunner/Engineer/Piercing/Surgeon
cases in8.107s, zero skips. Data/inventory19/19 pass. Quartermaster is active;
coverage151→152/310, planned159→158; War Machines5active/5planned. Binary:
`c0cad3f2435ba0886c286ce5bb311170cbec7a58b06af60fa2d57e96e3ade5d8`.
The siege setup now survives opening tower shots without weakening output checks.
Independent production review has no blocker. Deferred Phase2: simulated future
activation consumption, zero-rounded Catapult fallback, broader Wait/Order/
controller-transfer interactions and full binary battle snapshots. Perk-specific
art remains Not done. No GUI, snapshot promotion or playable acceptance.

## UP-100 — Field Workshop machine and fortification repair

Status: In progress; read-only architecture map, 2026-10-01. UP-023 missing
Advanced War Machines perk: the Tent may target allied war machines or friendly
fortifications, repairing with its normal Siege-scaled healing output. Both
target families are required; do not activate a machine-only substitute. Root
selects this unblocked candidate after pushedadfabbc46 and a clean worktree;
coverage151/310 remains unchanged. Separate Luna maps cover authority/shared
output/persistence and UI/AI/real-siege fixture seams. Root owns architecture,
ownership, registration/version integration, focused builds/native and Git.
Acceptance: legal saved perk offer, accepted Tent machine repair and defended-
town structural repair, exact shared output/current-max cap, hostile/full-health/
absent-perk guards, ordinary troop-heal preservation and minimum AI selection.
No art, GUI launch or playable snapshot promotion in this slice.
Scope question is pending: surviving damaged targets only vs rebuilding destroyed
machines/fortifications. Structural HP can represent restored walls, but tower
destruction also removes its shooting unit; positive HP alone cannot reconstruct
that unit. Occupied breaches likewise need a rebuilding policy. Continue mapping
the unambiguous damaged-target paths; do not silently count a partial repair
implementation as complete or fabricate destroyed-target behavior.
Maps complete: share Tent eligibility/output across the callback, authoritative
`doHealAction`, UI, AI and automatic-control admission. The latter skips Tents
when its ordinary troop-only candidate list is empty *before* checking manual
control, so it must include repair targets even with guaranteed Basic control.
`getFirstAidHealValue` is a target-capped cloned heal, not raw Siege output;
repairs need the full output before applying their own missing-HP cap. Machine
eligibility must remain local to Field Workshop; do not globally loosen
`CStack::canBeHealed`. Prioritize structural part routing on tower hexes, which
also contain turret stacks. Existing unsigned CatapultAttack subtracts HP and is
not a repair packet: add a generic authoritative structural-HP update with
shared live/detached application, explicit wire/version compatibility, and a
post-apply sprite refresh (siege wall images are cached). Existing structural HP
already lives in SiegeInfo's saved payload. A rebuilt turret would additionally
require its removed shooter unit to be restored; all-destroyed detached battles
also currently lose the canonical-structural mode inferred from positive HP.
Retained fixture leads: Surgeon real Tent/legal offers and Fortification Engineer
real town/validated Citadel setup. Require actual accepted STACK_HEAL to wall hex,
not merely direct structural packet injection, plus machine repair/AI selection.
No production changes, build or activation are claimed by this mapping checkpoint.

## UP-099 — Master Gunner selectable second Ballista shot

Status: Verified (playable delivery pending), 2026-10-01. UP-023 Basic War Machines perk: two
Ballista shots per activation, second60% normal damage and independently selected
target. Read-only map confirms the generic extra-attack loop only repeats one
submitted target at full damage, so it cannot satisfy this rule. Root selects a
saved/replicated same-activation ranged follow-up allowance and dedicated turn
reason, preserving activation serial/lifecycles through first-shot continuation.
Pending follow-up permits a normal validated SHOOT or safe decline; invalid
requests must retain it. Shared actual/preview damage and minimum AI selection
must honor60%, with legal offer and accepted two-target native evidence before
activation. Root owns architecture, version integration, config/docs/CMake/build/
Git; workers have separate runtime, UI/AI and fixture ownership. No GUI/promotion
or artwork change. Coverage remains150/310 until verified.
Actual delegation is running: a Luna runtime writer owns shared unit/callback/
packet/server and damage-script files; a separate Luna owns AI/client interaction
files; the tester owns only a new isolated fixture. Root owns the single append-
only save feature/version gate and all registration/build/Git integration. No
build starts before required source owners freeze; no active-perk count yet.
Root integration now contains the append-only version and BattleInfo sidecar
declarations/tail. Runtime must guard nonzero pending state in both standalone
unit updates and nested attack-state packets, not just the active-stack reason.
The damage projection must honor copied pending state independently of live
active-unit identity; action authorization remains separate. These are source
requirements, not yet compilation/native evidence.

Integration review: the isolated four-case fixture is frozen and registered;
AI/client source has its pending-shot controls and shared estimates. Root requested
an explicit AI Shoot fallback if ordinary evaluation picks Wait/movement despite
a legal follow-up. Runtime authority/activation flow remains under implementation;
no build, activation or coverage increase yet. Phase2 retains first-shot two-target
lookahead, external extra-attack bonus stacking, combat-log localization, and full
binary battle-snapshot coverage (the pre-existing Veteran history guard still
fails closed). Unit JSON and continuation-packet evidence must not be represented
as full binary battle-save verification.

Production and fixture owners are frozen; independent Astra review finds no
principal-path blocker. AI now independently selects a legal hostile second
target rather than declining because its ordinary evaluator chose Wait/movement.
Both-target build76640 runs with12 jobs (`UP099-build.log`); preserve its live
handle. No native execution alongside this build and no activation yet.
Build76640 exits1 on two raw field reads through the callback Unit interface.
Root repairs those cleanup reads to the shared pending-state query; the failure
is retained in `NH_RELEASE_FAILURES.md`. Repaired both-target20641 is running
with12 jobs (`UP099-repaired-build.log`), no native/activation yet.
Build20641 exits1 on the fixture's missing HypotheticBattle declaration; root's
first header-name correction14515 also exits1. Source lookup identifies its
actual owner `StackWithBonuses.h`. Both failures are retained; corrected
both-target89421 runs with12 jobs (`UP099-header-repaired-build.log`). No test
assertions were weakened; registration remains planned.
Both-target89421 exits0. Principal88930 passes3/4, zero skips in1.445s;
only the ratio baseline fails after accepted Defend changes the target's Defense.
The fixture owner checks same-state normal/follow-up sampling before the repaired
gate. Invalid-target retention, explicit decline, rank-loss spending and no-perk
actual-shot guards pass. Master Gunner remains planned until all four cases pass.
Final gates supersede the in-progress chronology: both-target76128 exits0;
repaired principal71745 passes4/4, zero skips in1.450s with the same60% assertions.
Activated74243 passes16/16 Master Gunner/Engineer/Piercing Bolts/Surgeon cases,
zero skips in5.022s; data/inventory19/19 pass. Master Gunner is active;
coverage150→151/310, planned160→159, War Machines4active/6planned. Test binary:
`11b4dc190f413736f8868e88e654fb27276a81f87b8b652ab6b2ac49fbdebecb`.
No GUI, art approval or snapshot promotion. Phase2 retains Second Wind
interleaving, extra-attack stacking, controller-transfer compatibility, initial-
shot multi-target lookahead, localization and full binary battle-save breadth.

## UP-098 — Fortification Engineer (continuation evidence)

Breachmaker's first map identifies a genuine adjacency gap: current structural
HP and enum/hex identity exist, but no fortification-neighbor relation does.
The user is asked neighboring outer-wall sections with the central keep excluded
vs including the keep by nearest-section distance. Preserve this decision gate;
do not silently treat enum order as geometry or implement overflow without it.

2026-10-01 continuation: source checkpoint407788932 is pushed and the worktree
is clean. This was progress, not an idle wait. Two read-only Luna maps prepare
Breachmaker structural overflow and Master Gunner's independently selectable
second shot. Root will select the next complete unblocked rule from evidence;
no multiplier-only or same-target-only substitution is permitted. Coverage stays
150/310 until the next principal path is implemented and verified.

Next-item preparation: a read-only Luna maps Precision Bombardment's specific
Catapult wall/gate/tower targeting and existing control/AI paths while UP-098
builds. No implementation overlap or activation is authorized by that map.
Map complete: Basic War Machines already supplies100% Catapult direct control;
existing CATAPULT UI and BattleAI submit specific attackable wall/gate/tower hexes.
The Lua ability retains structural hit chances and randomly redirects misses.
Precision Bombardment remains planned and unreferenced by production. Its literal
selection benefit overlaps existing rank behavior; do not invent guaranteed hits
or remove existing rank control without a design decision. Retain the shared
attackable-part validator, CATAPULT action and real fortified-town fixture leads.

Status: Verified (playable delivery pending), 2026-10-01. UP-023 Expert War Machines perk: when defending
a fortified town, defensive towers use125% of the hero's Siege rating and may
be manually targeted. This standalone rule is selected while Counter-Battery's
targeting overlap is mapped and Battlefield Medic awaits persistence clarification.
Root contract: shared current-controller/defending-fortified-town eligibility;
existing tower damage output evaluated at floor(125% Siege), not125% total damage;
deterministic manual control bypasses legacy RNG and uses existing validated shot
UI. No new persistent state. One Luna owns callback/header/flow; another owns an
isolated real-siege fixture. Root owns CMake, registration, review and gates.
Require accepted manually chosen tower shot, exact shared forecast/output,
eligibility exclusions and focused native build before activation. No GUI launch,
new art or playable promotion in this slice; coverage remains149/310.
Production is frozen and independently reviewed without a blocker. The shared
query requires a living nonghost actual tower slot, original/current defender,
fortified defended town and active saved perk; both boosted damage and manual
control use it. Rating arithmetic is widened, floored and clamped before the
existing saved output formula. Detached battle proxies retain town context.
Client build is starting on frozen production while the separate unregistered
fixture uses a real town and validated fortification construction. No activation.
Client43691 runs with12 jobs (`UP098-client-build.log`); preserve its live handle.
Do not register/change CMake or run native concurrently with that build.
Client43691 is terminal exit0. The fixture is present with four cases using a
real Castle-faction town and validated Citadel construction; final freeze,
CMake registration and combined/native gates remain pending.
Fixture review caught a missing `skills` registry level before native execution;
the fixture owner corrected it and refroze. Root registered the four cases and
started the serialized both-target12-job build (`UP098-build.log`). No activation
or coverage change yet. Ordinary-control activation breadth remains Phase2.
Final gates: both-target19393 exits0. Principal2955 passes4/4, zero skips in
1.624s (`UP098-principal.log`/`.xml`), including an accepted manually selected
real Citadel tower shot and exact pre-defense Siege output. Activated75235
passes12/12 Engineer/Piercing Bolts/Surgeon cases, zero skips in3.960s
(`UP098-activated.log`/`.xml`). Data/inventory19/19 pass. Engineer is active;
coverage149→150/310, planned161→160; War Machines3active/7planned. Binary:
`87d29702e613cd333db104a2266b8dd2231dc2a7416e15e1a03e7e94dbead788`.
No new save state, GUI, artwork approval or playable snapshot promotion. Phase2
retains broader controller-transfer and no-perk automatic-activation evidence.
Independent final activation/fixture review finds no remaining blocker. Root
will integrate this verified source checkpoint with a normal commit/push.

## UP-097 — War Machines Expert targeting and damage

Status: Read-only implementation map, 2026-10-01. Piercing Bolts50a85e3bf is
pushed and the worktree was clean on resumption. Battlefield Medic remains mapped
pending post-combat persistence clarification. A Luna maps Counter-Battery's
deliberate enemy-machine targeting and+50% final damage alongside Fortification
Engineer's explicit manual defensive-tower targeting and125% hero Siege. Do not
register only a damage multiplier while omitting required targeting. Root owns
the architecture/targeting contract and selection of the next unblocked full perk.
Keep ownership, target validation, forecasts and minimum AI behavior shared;
no new art, GUI launch or playable promotion in this implementation loop.
Read-only map complete: ordinary enemy war-machine targets already pass the
shared shot validator/UI, but unattended towers always prefer non-machines.
Counter-Battery needs its+50% final damage and a pinned targeting decision, not
only registration. The user is asked automatic machine preference with manual
control reserved for Fortification Engineer vs Counter-Battery granting manual
tower control too. No Counter-Battery implementation until clarified. Minimum
AI map includes shared damage and AttackPossibility's dynamic cache policy.

## UP-096 — War Machines Piercing Bolts

Status: Verified (playable delivery pending), 2026-10-01. UP-023 Advanced perk: Ballista attacks ignore50%
of the target's Creature Defense. Surgeon checkpoint424ed5a02 is pushed and the
worktree was clean on selection. Root chooses an ephemeral shared damage-script
payload contribution for physical ranged Ballista attacks using the current
controlling hero's active perk. Preserve ordinary Creature Defense ignore
composition and separate hero-Defense mitigation. One Luna owns callback/payload/
Lua; another owns an isolated real-shot fixture. Root owns CMake, registration,
review, build and focused evidence. Require no-perk/ineligible behavior and
prediction/actual/AI consistency before activation; no new persistent state,
art, GUI or promotion is needed for this source slice.
Production is frozen: a distinct script payload field is set only for physical
ranged Ballista attacks whose current controller has the active saved perk. Lua
adds the independently floored50% contribution to existing target-Defense bypass,
capped at total Defense; Frenzy's own-Defense trade and hero-based PDR are unchanged.
Independent Astra review is assigned; the separate native fixture is still being
written. Registration remains planned, coverage148/310 unchanged.
Independent production review has no blocker and confirms the same calculation
serves actual, UI and detached AI. Client build70423 is running with12 jobs
(`UP096-client-build.log`) on frozen production source while the unregistered
fixture is written. Do not alter CMake or run native tests during that build.
Client70423 is terminal exit0. The native fixture is still in progress; its
registration, combined target build and principal real-shot gate remain required.
The four-case fixture is frozen and registered. Combined42241 runs both targets
with12 jobs (`UP096-build.log`); independent final fixture review is assigned.
Preserve the exact live build handle; no native run until terminal success.
Combined42241 exits0 for both targets. Principal18354 passes4/4 in1.560s with
zero skips, including accepted shot/forecast and detached parity. Both production
and fixture reviews have no blocker; actual controller transfer is deferred to
Phase2. Registry/module are active and regenerated; data/inventory19/19 pass.
The small activated regression batch is running before commit/count finalization.
Activated21661 is terminal exit1:9/11 pass, including all4 Piercing Bolts and4
Surgeon cases. Two existing Archery fixtures directly select higher-tier perks
without prerequisite perks and throw before exercising their mechanic. Failed
batch evidence is retained in NH_RELEASE_FAILURES; independent classification is
assigned. Do not call the whole batch green or weaken progression to accommodate
old fixture setup. Record nonblocking fixture repair for Phase2.
Independent Astra classification confirms both fixture setup defects occur at
unchanged prerequisite validation before damage assertions; no UP-096 blocker.
Fix their legal preceding selections in Phase2 without dropping assertions.
Principal4/4 and activated4/4 new cases prove this bounded feature; full11-case
batch remains9 pass/2 fail. Data/inventory19/19 pass. Coverage148→149/310,
planned162→161; War Machines2/8, ordinary Expert progression opens. Binary:
`bcd78c12f52089a2b50a24b8628c58eb82373dd4b9da4095d9446504b7cae427`.
No art approval, GUI or playable promotion. Next Medic map is retained in Sprints;
after-combat restoration persistence is asked, not silently chosen.

## UP-091 — Reserve and Standard Bearer coverage

Status: Reserve and Standard Bearer verified (playable delivery pending),
2026-10-01. UP-023 missing Basic Battlecraft
Reserve: a stack gains +2 Speed only during its delayed activation after Waiting.
Missing Advanced Discipline Standard Bearer: adjacency to at least one other
friendly stack grants +1 Morale, not one bonus per neighbor. Root owns activation
and shared architecture; independent read-only maps identify lifecycle/AI seams.
Require actual ordinary interaction, current-controller ownership, live and
detached state parity, lifecycle/immunity boundaries and focused native gates.
Do not activate or count either before validation. Entrench is already active;
the current 1/1 baseline pass confirms it is not a missing item to reimplement.
Esprit de Corps remains a separate scope question, not a blocker for these items.

Reserve root contract: use a generic nonnegative per-unit activation movement
bonus, not an until-next-turn SPEED bonus that persists beyond this activation.
Grant only on the delayed waited TURN_QUEUE activation for the current controller;
preserve through Hero/spell/pursuit continuations, clear at the existing terminal
Creature Activation EndAction signal and on reset/round/removal. Do not change
Initiative. Detached Wait forecasting must arm the same +2 before reachability.
Current binary BattleInfo snapshots omit CUnitState, so append a version-gated
unit-ID/value sidecar for this field rather than silently losing it or rejecting
all current saves. Legacy defaults zero; nonzero downgrade must reject before
writing. One Luna worker owns state/runtime/AI files; new tester spawn and previous
tester reuse were service-rejected, so the completed Standard Bearer mapper slot
is reused for the isolated Reserve fixture. No feature activation/coverage yet.

Standard Bearer map: existing UNIT_ADJACENT limiter is creature-specific and lacks
friendly ownership; sibling death/control cache invalidation and detached copied
limiters make a direct reuse stale. Preserve ordinary recipient Morale immunity,
but any living currently friendly supporting stack qualifies. A dynamic battle
context query must use candidate positions/control, not live original-bearer
limited bonuses. Serialize work after Reserve because CUnitState/AI ownership
overlaps; the map is retained without pretending this is implemented.

Reserve source is frozen. Independent reviewer spawn and previous-reviewer reuse
were service-rejected; root reviews the frozen diff without inventing approval.
Root hardened detached activation-end cleanup against a missing active unit.
Phase2 forecast finding: BattleExchangeEvaluator refreshes delayed reachability
after makeWait, but its Wait-choice loop still starts from the already-built
possible-attack catalogue. Actual delayed AI activation sees the granted movement;
regenerating every newly reachable Wait candidate is separate planner integration.

Both-target build25950 exits1 (`UP091-build.log`): the isolated fixture has an
unqualified CUnitState and an invalid Unit-to-CStack const_cast. Existing Luna
owners are assigned bounded repairs: fixture namespace/ID lookup and legal local
active perk offer; production compiled sidecar helpers to remove incomplete-type
warnings and a UnitChanges older-version nonzero-state guard. The independent
reviewer spawn is again service-rejected. No native pass or coverage activation.

Reserve acceptance checkpoint: both-target repaired64222 and final controller
build34777 exit0. Native55349 passes16/16, then activated native69809 passes16/16,
zero skips in4.778s (`UP091-activated-verified.log`/`.xml`), including five Reserve,
seven Battlecraft and four Rally cases. The principal accepted Wait → delayed
extra-reach move → immediate expiry works; current-controller detached Wait,
branch isolation, unchanged Initiative, sidecar/UnitChanges and immunity guards
pass. Binary SHA-256
`9fe6ca9152d6e666c651efbea2617ee173a5770b6c8100b571befa07030e6cce`.
Data/inventory19/19 pass. Both registry copies active; coverage143→144/310,
planned167→166, Battlecraft2active/8planned. Root reviewed production; independent
Astra review remained service-unavailable and is not claimed. Wider Wait-choice
attack-catalogue regeneration and the pre-existing full CUnitState binary-snapshot
contract remain Phase2 findings. Purpose-made art Not done; no playable promotion.
Next: implement the retained Standard Bearer dynamic adjacency/Morale map.

Standard Bearer implementation started: root chooses a contextual battle Morale
query and a generic raw-before-cap adjustment, preserving ordinary immune/MAX/MIN
semantics and existing non-battle behavior. The current BattleProxy returns itself
and its virtual unit enumeration already merges candidate states; no broader
enumeration rewrite is needed. One Luna owns shared lib/server calculation, a
second owns AI valuation and existing client Morale refresh. The third tester
spawn and old tester reuse were service-rejected; root owns the isolated fixture.
No registration/coverage claim before focused validation. No new art or layout.

Standard Bearer source is frozen. Independent Astra review finds no BLOCKING
issue in production/fixture. Four cases cover legal Advanced selection, accepted
supporter movement through real negative/positive Morale gates, nonstacking,
raw-before-cap/MAX/MIN/immunity, current controller and candidate branch changes.
Deferred Phase2 verification: explicit double-wide rear-hex adjacency and supporter
death/resurrection. Sorrow/Doom valuation uses the existing detached context for
both unit values; those spells do not change adjacency/control. No coverage yet.

Standard Bearer acceptance: both-target68249 and repaired42607 exit0.
Principal82873 passes4/4; activated native74455 passes39/39 with zero skips in
10.603s (`UP091-standard-bearer-activated.log`/`.xml`), including four new cases
and focused Battlecraft/Reserve/Rally/Sorrow/Doom/Shield of Chaos/Crusade gates.
Binary SHA-256
`f12c0d80bf4aa73ec033bfc80c6b68aa0bb36fed2fd7e92665e2a646ce10d261`.
Data/inventory19/19 pass. Source and fixture-repair Astra reviews have no blocker.
Both registry copies are active; coverage144→145/310 active, planned166→165,
Discipline3active/7planned. Existing Morale panel uses the contextual value and
refresh detects sibling-dependent changes; this is a source/compile hook, not
graphical acceptance. Art Not done; no playable promotion. Explicit double-wide
rear-hex and supporter death/resurrection cases remain Phase2 verification.

## UP-092 — Hold Fast activation lifetime

Status: Verified (playable delivery pending), 2026-10-01. UP-023 missing Advanced
Discipline perk: Defend or Hold the Line grants protection from negative Morale
until the next Creature Activation begins. Read-only map identifies authoritative
Defend effect publication and Hold the Line's captured recipient anchors in
BattleActionProcessor. Existing STACK_GETS_TURN survives rounds and is present at
the bad-Morale gate, but also expires on HERO_SPELLCAST continuations and misses
Second Wind HERO_COMMAND starts. Therefore do not reuse it unmodified or globally
change unrelated legacy bonuses. Root direction: generic activation-begin expiry
with live/detached parity and a versioned bonus-duration contract; grant a normal
MINIMUM_MORALE=0 timed effect via authoritative Defend/Order paths. Test genuine
queue/Morale/Second Wind starts, Hero/spell continuations, round boundaries and
legal command recipients. Timed grants follow the ordinary buff lifecycle;
control-change and broken-anchor interactions must be recorded, not mistaken for
a permanent army-wide immunity. No feature activation or coverage claim yet.

Two Luna workers own generic duration/save/live-detached expiry and authoritative
Defend/Order grants respectively. A new tester spawn was service-rejected; an
available completed tester was successfully reused with isolated fixture ownership.
Root owns CMake, registration, focused serialized builds and integration. The
preceding scope-confirmation turn changed no source; this continuation resumes
the next safe implementation item. No native acceptance or coverage change yet.

Generic duration source is implemented: append-only bit14 and save feature,
parser lookup/schema/docs and live/detached genuine-activation expiry. Independent
Astra duration review finds no blocker and confirms pre-activation Morale ordering.
Grant/fixture work remains in progress. Purify's explicit temporary-duration mask
does not include the new duration; the present beneficial secondary-skill grant
is unaffected. Record extension for future negative spell consumers in Phase2.

Production and six-case fixture are frozen. Independent Astra production review
finds no blocker. Root/tester repaired source-review fixture mistakes before the
first build: protected moraleVal already includes the floor, -1 could be offset
by Archangel/Discipline bonuses, copied Time Stop bonuses need selector removal,
and the Second Wind capability query belongs on the battle callback. Both-target
build77264 is live with12 jobs (`UP092-build.log`); revalidate this exact process
handle on continuation, not a lock or elapsed time. Do not restart on observation
timeout. No native pass, registration activation or coverage change yet.

Acceptance checkpoint: repaired80348 and final controller2758 both-target builds
exit0. Principal85726 passes7/7; activated69879 passes28/28, zero skips in8.612s
(`UP092-verified.log`/`.xml`), including Hold Fast7, Reserve5, Rally4, Standard
Bearer4, Battlecraft7 and one actual Second Wind damage/activation regression.
Binary SHA-256
`a20a31dee29b913dec0a59c64554e318093c9555858513839ec70aa6700d9bab`.
Data/inventory19/19 pass; independent reviews have no remaining blocker.
The 5/6 initial native result exposed canonical Defend→Second Wind eligibility
and original-side bookkeeping defects. Production now recognizes canonical
Defend completion and current-controller activation/start/end; the seventh case
verifies actual hypnotized Defend/Second Wind and detached isolation. Both registry
copies active; coverage145→146/310, planned165→164; Discipline4/6. Purpose-made
art Not done; no GUI/promotion or playable acceptance. Phase2 retains future
negative-duration Purify consumers, control changes during an activation and
cross-perk Morale forecast correlations.

## UP-093 — Discipline Fearless

Status: Verified (playable delivery pending), 2026-10-01. UP-023 Advanced
perk: immunity to explicitly non-magical fear, not negative Morale. Read-only map
finds FEARFUL creature/commander ability bonuses and one authoritative turn-start
roll before the fear trigger packet. No Dread spell or spell-sourced fear exists
in current content. Classify source contributions before aggregation/publication;
do not erase future spell fear or confuse the transient fear flag with immunity.
Root must pin the source-aware helper, current-controller ownership, minimum AI
hook and focused native evidence before activation. Existing source metadata is
available; the result packet itself has no provenance. No coverage change yet.

Root classification contract: positive CREATURE_ABILITY contributions to FEARFUL
are the current explicitly non-magical turn-start fear family. This does not
classify every creature ability as non-magical. Preserve zero/negative caps and
SPELL_EFFECT, OTHER and unclassified contributions. Commander requirements have
no mapped runtime consumer; do not invent one in this slice. One Luna owns the
shared query, authoritative trigger and minimum AI hook; another owns an isolated
native fixture. Suppressed fear must not consume Twist of Fate or extra RNG.
Require real turn-start, mixed-source, current-controller and detached-state
evidence before activation. The user confirmed UP-089's explicit adverse-roll
scope again; that scope is already recorded in the canonical Luck section.

Production and five-case fixture are frozen; independent Astra runtime and
fixture reviews find no BLOCKING issue. Root repaired fixture-root indexing and
Unit/CStack helper assumptions before compilation and strengthened the protected
Twist case to stochastic50% fear. Both-target build36048 is live with12 jobs
(`UP093-build.log`). Revalidate that process handle rather than restarting on an
observation timeout. Same-stacking-key cross-source fear, seeded-bias/Twist-aware
AI forecasting and a direct unchanged-RNG-state assertion remain Phase2 findings.
No registration activation or coverage claim before focused native evidence.

Acceptance checkpoint: both-target36048, frozen follow-up and repaired24535
builds exit0. Principal13527 passes5/5; activated30226 passes27/27, zero skips
in9.008s (`UP093-activated.log`/`.xml`), including Fearless5, Hold Fast7, Rally4,
Standard Bearer4 and Twist runtime7. Data/inventory19/19 pass. Binary SHA-256:
`275f9ef5ddf86b424924369988ccb25fbd0dff0b9bf6e6ecc0b444df8438ead5`.
Independent production/fixture reviews have no blocker. Initial4/5 was a fixture
visibility error, repaired without exposing opposing heroes. Source and embedded
module registries active; coverage146→147/310, planned164→163; Discipline5/5.
Combat feedback describes a prevented check, not a realized RNG trigger. No new
state/save feature is needed; existing perk persistence applies. Phase2 retains
future same-key source stacking, nominal AI chance/history correlation and direct
RNG-state evidence. Art Not done; no GUI/promotion/playable acceptance.

## UP-094 — Remaining Discipline contract maps

Status: Design clarification pending, 2026-10-01. Read-only next-item evidence.

Next-item map, Heroic Spirit: blocked on activation wording, not on Fearless.
The positive-Morale roll occurs before the immediate Morale Creature Activation;
UNTIL_NEXT_CREATURE_ACTIVATION would expire the grant immediately. User asked
whether the extra retaliation should survive that immediate activation and expire
on the following activation. Do not silently change generic expiry. Retaliation
totalCache also latches observed bonus capacity until round reset; a timed bonus
alone cannot revoke unused capacity at activation expiry. Root must choose an
activation-scoped allowance contract after the design answer, with live/detached
parity. Read-only mapper evidence; no implementation or coverage claim.

Veteran Cohesion read-only map: authoritative BattleAttack/StacksInjured pre/post
health observation covers ordinary physical, spell and Poison damage. User asked
whether the50% denominator is initial full stack capacity or surviving-creature
capacity. Record the answer before implementing; do not invent a low-health
trigger that cannot ordinarily occur. One-shot state must survive healing and
resurrection, copy into detached branches and use explicit battle-save support.
No source/count change; this question does not block other missing features.

## UP-095 — War Machines Surgeon

Status: Verified (playable delivery pending), 2026-10-01. UP-023 Basic perk: First Aid Tent
healing removes one physical affliction, in priority order Poison, Disease,
Bleeding, then other eligible physical afflictions by application order. One Luna
maps the existing authoritative Tent/Cure status path, current-controller
ownership and AI prediction read-only. Root owns the shared cleansing contract,
registration and focused real-healing evidence. Do not broaden this to magical
Dispel, cleanse every affliction, or register before the principal path works.

Read-only map complete: `BattleActionProcessor::doHealAction` centralizes real
Tent casts and Siege output; `battleGetOwnerHero(tent)` supplies current control.
Stored physical Poison needs a UnitChanges state update; Disease uses a timed
spell-effect group removed by SetStackEffect. Existing Cure allowlist only covers
Poison/Disease and sorts SpellID, not application order. No Bleeding producer or
generic physical-affliction eligibility/application-order representation exists.
This is an implementation-foundation gap, not permission to classify all magical
groups as physical or call a two-affliction subset complete. Build a shared
selection/removal contract before registration; minimum AI consumer is
`CBattleAI::useHealingTent`, which currently only picks the most wounded stack.
No source/count change. Root owns the next foundation choice and focused evidence.

Foundation contract: an effect-neutral PHYSICAL_AFFLICTION bonus marker carries
explicit kind and applicationOrder in existing JsonNode bonus parameters. Its
source/sid identifies the removable effect group; do not infer physical eligibility
from arbitrary negative magic. Poison, Disease and Bleeding precede other marked
groups, which use application order. Stamp order at effect application, preserve
it on refresh and replicate it in the authoritative effect packet. No polling or
per-frame scan is introduced. Stored physical Poison remains a separate descriptor.
One Luna owns marker/parser/schema/save plumbing, one owns shared live/detached
selection and lifecycle, and one owns an isolated native fixture. Root owns packet
integration, CMake, production consumers, build and activation. The marker plumbing
is implemented but unverified; a pre-cast numeric-range issue found in root review
was repaired before build. No Surgeon activation or coverage change yet; a marker
foundation alone does not implement Bleeding or the real First Aid Tent consumer.

Independent runtime review found a blocking detached-copy gap before build:
the existing projection filter captures spell/Order sources only, so a parent-local
generic non-spell affliction can survive child removal through recreated bonus
pointer identities. The runtime owner is repairing capture of exact explicitly
marked source/sid groups, including their underlying effects, without freezing
unrelated attributes. A focused parent/child removal/refresh regression is assigned.
The real Tent and AI consumer worker owns only BattleActionProcessor/BattleAI;
registration remains planned until actual healing evidence passes. Marker parser
and outgoing-packet review have no remaining blocker; data/inventory19/19 pass.
No build has started while the runtime candidate is being repaired.

Tent and AI consumer source is frozen and independently reviewed without a
blocker: exactly one shared selection after actual friendly living Tent HP gain,
authoritative group/stored-Poison removal, named feedback and current-controller
AI target search. Foundation fixture has12 cases including parser, persistence
and parent/child full-group removal/refresh; no native pass is claimed. Follow-up
review cleared full-group removal but found marker-only removal followed by
recapture/aging losing remaining non-spell effects. Root extends runtime ownership
to StackWithBonuses.h for narrowly retained branch-owned captured group identities;
they preserve projection provenance, not eligibility. Add the marker-only and
grandchild regression before freeze/build. The real Surgeon fixture is separately
assigned and will be registered only after it exists and is frozen. Coverage is
unchanged; no build, activation, commit or playable promotion is claimed yet.

Production and13-case foundation fixture are now frozen. The private detached
source/sid history repair is independently cleared: capture, suppression,
refresh, aging and descendant copies preserve underlying effects after marker
removal without treating history as affliction eligibility. Both-target build
31895 is live with12 jobs (`UP095-build.log`); revalidate that process handle on
continuation, never restart from elapsed time or a log alone. No native pass or
Surgeon activation yet. The unregistered actual-healing fixture is being written
separately; it is not part of this frozen build candidate. No GUI or promotion.

Build31895 is terminal exit1, not a live wait: PhysicalAffliction.cpp needs the
direct BonusList.h include rather than a forward declaration. Root repairs the
include and records the failure in NH_RELEASE_FAILURES; no assertions or gameplay
scope are weakened. Retry and focused native evidence remain required.
Retry88256 is live with12 jobs (`UP095-build-retry1.log`); preserve and re-poll
this exact handle on continuation. No native test runs concurrently with build.

Retry88256 is terminal exit1 in the foundation fixture (missing JsonBonus.h,
ambiguous marker-removal overload and nonexistent STACKS_ATTACK). The tester
repairs all three without weakening assertions; production source stays frozen.
The four-case actual Surgeon fixture is independently reviewed, repaired and
now registered for the next combined build. Require13 foundation and4 actual
healing cases to pass before activation; synthetic generic Bleeding statuses
exercise removal, not a claim that a production Bleeding damage source exists.
Combined retry72892 is live with12 jobs (`UP095-build-retry2.log`). Re-poll that
exact handle, then run the focused native filter only after terminal build success.

Retry72892 is terminal exit1: the Surgeon fixture lacks direct definitions for
CGameHandler, BattleProcessor and SetStackEffect. The tester owns the include-only
repair; assertions and production behavior remain unchanged. Rebuild before the
17-case principal gate; no activation or playable acceptance is claimed.
The include-only repair is frozen. Retry67115 runs the combined targets with12
jobs (`UP095-build-retry3.log`); preserve its handle until terminal completion.
Retry67115 is terminal exit0 for both targets. Principal native90035 is now
running the13 foundation and4 actual-healing cases (`UP095-principal.log`/`.xml`).
Activation remains pending its terminal evidence; no GUI or promotion.
Principal90035 is terminal exit139 in the first mock-based foundation case.
GDB74245 identifies a null UnitInfoMock unitType during acquireState assignment,
not an accepted Surgeon healing failure. The tester repairs valid fixture creature
setup/lifetime without bypassing the state-copy path. No activation; rerun the
17-case gate after a successful incremental build.
The valid-creature fixture repair is frozen. Incremental80241 builds both targets
with12 jobs (`UP095-build-retry4.log`); native retry must wait for terminal success.
Incremental80241 exits0. Principal retry4916 exits1:13 foundation cases pass,
all4 Surgeon cases fail in setup on a legacy capability-version/warMachineShop
mismatch. The tester repairs current-schema fixture setup without deleting rules
or weakening assertions. No perk activation until actual healing passes.
The fixture now retains canonical capability v4 instead of forcing legacy v3;
shop/progression data and all healing assertions remain intact. Incremental24147
runs both targets with12 jobs (`UP095-build-retry5.log`).
Incremental24147 exits0; principal retry37773 passes15/17. Stored-Poison cleansing
and no-perk healing pass. Remaining fixture preconditions are healthy-target
healing forecast and Tent auto-skip without a wounded friendly recipient. The
tester verifies and repairs setup while preserving principal/negative assertions.
The priority forecast now follows wounding and still requires40 HP and four real
heals. A separate wounded legal friendly stack prevents Tent auto-skip in the
negative-target case. Incremental64786 runs both targets (`UP095-build-retry6.log`)
with12 jobs; independent fixture-delta review is assigned before acceptance.
Final64786 exits0 for both targets. Principal29476 passes17/17 in1.997s; activated
59354 passes34/34 in6.552s with zero skips, including relevant timed projection,
Cure, Purify and Toxic Spines regressions. Data/inventory19/19 pass; Surgeon is
active and the embedded module is regenerated. Independent final fixture review
has no blocker. Coverage147→148/310, planned163→162; War Machines1/9. Binary
`beb89e7e361cdd3f42e9b664a8b3de5d9b816b6d1662410896ca39a76d273e1d`.
Bleeding producer remains separate content work; generic marked Bleeding removal
is exercised. Phase2 retains packet-wide preprocessing rollback for later-unit
errors, broader control-change interactions, producer-duration consistency and
combat-log localization. No GUI, art approval or playable promotion claimed.

## UP-090 — Implement Discipline Rally

Status: Verified (playable delivery pending), 2026-10-01. UP-023 missing
Basic perk: once per combat, cancel the first negative Morale trigger affecting
a friendly stack. Preserve current-controller army ownership, ordinary Morale
immunity, genuine activation flow, save/replication and detached AI state.
Do not implement it as a reroll or as a chance multiplier. A canceled negative
result must not also spend Twist of Fate, matching existing suppression precedence.
Root owns the shared state/packet/API contract and registration; a worker may
map the narrow live Morale and AI seams without changing the frozen Twist fixture.
Acceptance: legal Basic perk selection, actual first-trigger cancellation,
subsequent/next-round triggers unchanged, side/save/packet isolation, combat
feedback and focused native/AI evidence. No coverage claimed at selection.

Map confirms one authoritative bad-Morale gate and no existing Rally state.
Root selects an independent side-long enabled/used suppression state and a
monotonic dedicated transition packet, not a strike or reroll snapshot. The
callsite draws once, cancels a realized negative result when Rally is available,
then otherwise passes that cached first result to Twist's resolver before any
final redraw. This preserves the exact original first RNG draw and excludes
already-canceled results from Twist expenditure without expanding the generic
resolver API. Deterministic negative triggers may be canceled by Rally; ordinary
immunity/no-trigger leaves the allowance untouched. Detached AI must copy/spend
candidate-local state without pretending all negative stacks become immune.
Its current per-unit Morale heuristic has no first-trigger ordering model;
broader cross-stack/multi-round correlation belongs to Phase2. Future coexistence
with unimplemented Unbreakable requires explicit suppression precedence before
that Expert perk is added; it does not block Rally alone. No source activation.

Shared state/packet source is frozen with its own append-only save feature and
type288. Root wired the authoritative cancellation before cached-first-draw Twist
resolution, ordinary activation and hero-named feedback. Detached AI copies its
own allowance and adjusts only one prospective Morale event, leaving the rest of
the duration exposed. Four status-spell valuation paths use that bounded helper;
cross-stack realized-trigger ordering remains a Phase2 forecast limitation.
The fixture worker owns only the new Rally test; an Astra reviewer inspects the
frozen production slice. Registration remains planned until focused build/native
gates pass. No completed coverage or playable promotion claimed yet.

Independent Astra production review found no blocker. Its two fixture findings
were addressed before build: seeded50% bad Morale on a hypnotized recipient now
tests cancellation before eligible Twist, and AI horizon2 assertions show first
delta-0.35 then spent delta-0.70 with sibling/live isolation. Four fixture cases
are frozen. Serialized both-target build93251 is running with12 jobs
(`UP090-build.log`); inspect this handle on resumption, never restart merely
because an observation times out. Reviewer follow-up was service-rejected;
the original review stands and root inspected the strengthened fixture.

Build93251 exits0 for client and tests. Native3559 passes4/4 principal cases;
after activation, native7731 passes47/47 with zero skips in13.611s
(`UP090-activated-verified.log`/`.xml`). Binary SHA-256
`f012740b9bf1a26fc50ea0a16a8fa4ae9b759401e3c972d812ff8d47ed5b1d2b`.
Data/inventory19/19 pass; both registry copies are active. Coverage142→143/310
active, planned168→167; Discipline2active/8planned. Broader AI first-trigger
ordering and cross-stack/multi-round probability correlation remain Phase2.
Future Unbreakable precedence must be decided before that perk is implemented.
Purpose-made art is Not done; no GUI, snapshot promotion or playable acceptance.

## UP-089 — Implement Luck Twist of Fate

2026-10-02 repeated user reply retains the explicit scope recorded below.
Canonical wording already agrees; no design or runtime change is required.
Latest confirmation: “Use that explicit scope.” This is confirmation of the
existing rule, not authorization to expand the qualifying roll types.

2026-10-01 user reply reconfirms the already-integrated adverse-result scope:
negative Luck, negative Morale, failed resistance against hostile spells, and
successful hostile chance abilities; exclude damage variance, failed beneficial
procs, and random target/form selection. The canonical Luck section already
records this decision; no competing amendment or runtime scope change is needed.

Latest continuation checkpoint: verified scripted slice is pushed as9a339f8c4;
worktree was clean on resumption. Previous goal turn was progress, not an idle
wait. A new Luna spawn was service-rejected; an existing tester follow-up succeeded
with exclusive runtime-fixture ownership for the late Hand of Fate collateral
gate. Root owns registration/coverage and will not activate until that principal
path is verified. No GUI/promotion or completed coverage change yet.

Status: Verified (playable delivery pending), 2026-10-01. UP-023 missing Expert Luck
perk: reroll the first random combat roll each combat whose result is negative
for the hero's army; deterministic effects cannot be rerolled. Map existing
authoritative random-roll and adverse-result classification before choosing a
generic once-per-combat interception. Do not silently reduce the rule to only
negative Luck or invent a damage-roll threshold. Root owns scope/architecture,
serialization and final semantic decisions. No implementation while Chain of
Fortune's frozen candidate builds. Acceptance: specification-defined roll types,
current-controller/side expenditure, exactly one reroll, deterministic exclusion,
replicated/save state, principal focused native and AI evidence.

Read-only map complete: no generic adverse-outcome/reroll layer exists. Luck,
Morale, ability procs, hostile spell resistance and reflection use different
random paths; the harmed side is not universally the RNG actor. Canonical wording
does not classify failed benefits, damage variance or random target/form choices.
The user approved this scope: negative Luck/Morale, failed hostile-spell resistance
and successful hostile chance abilities, excluding damage variance, failed
beneficial procs and random selections. Do not implement an invented threshold or
silently narrow to bad Luck. The canonical document records this classification
and the harmed army's expenditure; implementation follows after UP-087 gates.

Architecture map complete, read-only. Proposed root contract: an authoritative
resolver takes affected side, draw callback and explicit adverse predicate;
consume allowance before one final redraw. Keep classification outside the RNG
actor/stream keys. Existing side fortune state can store enabled/used, but a
generic side-state packet is needed for Morale/spell transitions, unlike the
attack-only fortune payload. Root must finalize controller ownership, reflected
spell polarity and fixed effective proc chance before assigning callsites.
Map identifies negative Luck/Morale, Fear, hostile discrete damage/on-hit procs
and failed hostile resistance; no manual-control, damage-variance or random
selection interception. AI uses branch-local state; wider cross-category
probability correlations belong in Phase2. No implementation/coverage claimed.

Root contract selected: store a separate AdverseCombatRerollState on each side,
not within strike fortune snapshots. This prevents later BattleAttack packets
from overwriting an allowance spent by a hostile proc or spell. A generic
authoritative BattleProcessor resolver draws once, asks the harmed side's state
to consume only a stochastic adverse outcome, publishes the transition before
one final redraw, and provides combat feedback. Shared state/version/packet
ownership is delegated separately from server/spell callsites. Registration
remains planned until the full approved scope and focused native/AI gates work;
this infrastructure adds no completed-perk coverage on its own.

Shared implementation is frozen; root added the generic authoritative resolver
and detached branch-local state copy. A first tester spawn was service-rejected
by its thread limit, then succeeded once the shared worker finished. The reviewer
spawn and existing-reviewer follow-up were also service-rejected; retry after the
fixture freezes, otherwise record missing independent review without inventing
approval. Registration is still planned and coverage unchanged.

Runtime API map identifies ServerCallback (not only SpellCastEnvironment) as the
spell bridge; its EffectPacketRecorder must forward. Resistance currently draws
for all battlefield units before reflection and actual effect-target collection;
do not spend Twist for untargeted units or a subsequently reflected original
cast. Use actual prepared recipients/current controller after final reflection.
Freeze fractional proc rounding once for both draws. Successful Mirror is adverse
to the caster's army as a hostile redirect proc; the separate random recipient
selection remains excluded. These contracts await runtime wiring, not more broad
exploration.

Frozen infrastructure checkpoint: six fixture cases exercise local legal Expert
perk setup, state/packet current and legacy codecs, deterministic/favorable
non-consumption, final adverse result without recursion, side/round persistence,
spent state before nested redraw, server spell-environment bridge, and actual
hypothetical packet visitor/nested-copy isolation. Reviewer retry succeeded after
fixture completion; independent review is running. Both-target build1364 is live
with12 jobs (`UP089-infrastructure-build.log`). Revalidate that exact handle on
resume; do not restart because an observation times out. No native pass, commit,
coverage increase or playable promotion is claimed yet.

Independent infrastructure review completed with no blocking finding. Deferred
direct assertions: resolver's invalid-side fallback and malformed current-version
state deserialization. The implemented validation remains present; do not expand
this infrastructure gate into broad certification. Actual gameplay interception
and AI valuation are still required before counting Twist. Build1364 remains the
serialized gate; focused execution follows it.

Next runtime slice is assigned to one Luna worker with exclusive attack/Morale
processor ownership, held read-only until build1364 and its infrastructure tests
finish. All affected sides use current-controller lookup; original unitSide is
retained only for existing RNG stream keys. Existing Providence/Second Chance
suppression takes precedence, so a cancelled negative result cannot spend Twist.
Root will expose frozen favorable-proc chance and weighted-curve stochastic
classification helpers. The parallel spell-worker spawn was service-rejected;
assign it when a slot opens. Its fixed contract preserves original MR first draws,
then spends only on actual prepared hostile recipients after final reflection.

Infrastructure verified: both-target1364 exits0; native73236 passes32/32, zero
skips in8.536s (`UP089-infrastructure-build.log`, `UP089-infrastructure.log`/`.xml`).
Six new infrastructure cases plus26 focused Luck regressions pass. Binary SHA
`adefcb23c6001b687c0f425d29dafbc69ff9fbe749edbb31063a5c86275b08b8`.
Data/inventory19/19 pass; independent infrastructure review has no blocker.
This releases the frozen candidate for runtime wiring but does not activate the
global perk or add completed coverage. Counts remain141/310 active,169 planned.

Verified infrastructure is committed/pushed as2220d6f5d. Root added live weighted
bad-Luck/Morale stochastic classification and a frozen favorable-proc chance
preparation seam; existing favorable rolls reuse that exact rounding. Attack/
Morale worker is released to its two owned processors. Spell-worker retry was
again service-rejected; its full approved scope remains queued, not omitted.
No full-perk build/native evidence or completed coverage is claimed at this stage.

The user explicitly reconfirmed the four-category adverse scope on resumption.
Attack/Morale wiring is frozen for root review; the bounded spell worker is now
running with exclusive BattleSpellMechanics ownership. A concurrent actual-runtime
test-worker spawn was rejected by the service thread limit; retry after the spell
worker completes. Canonical scope is unchanged, and global activation remains
planned until actual runtime and minimum AI evidence pass their focused gates.

Spell worker froze its bounded two-file slice without build/tests. Ordinary
prepared hostile recipients and Mirror have source wiring, but root review found
a blocking timing gap: Chain Lightning's `transformByChain` consults `wouldResist`
during target preparation, and Hand of Fate's random collateral consults it later
during application. Resolving only after `collectTargets` does not cover those
actual recipients correctly. Before activation, root must move resolution to the
actual resistance-consumer decision with cached legacy first draws, frozen chance,
current-controller hostility, and once-per-recipient processing. Do not discard
the approved scope or count the incomplete spell slice as completed coverage.
Runtime source remains unverified; no build, commit or promotion of it is claimed.

Root selected authoritative lazy resistance resolution at actual consumer queries,
with per-recipient cached final decisions and scope-bound callback/RNG lifetime.
The repair worker owns only spell-mechanics files. Root added first-attack negative
Luck forecast awareness in the shared callback: a stochastic adverse probability
is squared while the side's reroll is available, after existing suppression rules.
Conditional future-roll correlations remain a Phase2 valuation finding, not a
claim of exhaustive AI forecasting. Parallel tester retry was service-rejected.

Lazy resistance source is frozen: `wouldResist` shares a once-resolved recipient
cache with ordinary filtering, chain routing and late collateral; scoped callback
cleanup covers exceptions and predictive evaluation suppresses authoritative
resolution. Root integrated the detached AI callback's local packet transition
and first-event hostile MR forecasts. After new tester spawns were again rejected,
an idle Luna follow-up succeeded with exclusive new-test-file ownership. Production
compile starts separately while that unregistered test file is written; no source
owner may change the frozen production candidate during this gate.

Production compile77876 exits0 (`UP089-runtime-build.log`). Existing focused
Luck/infrastructure native59072 passes32/32, zero skips in8.445s
(`UP089-runtime-regressions.log`/`.xml`); binary SHA-256
`e1196ff56aa5e28adc2240fc7598099266a0d654b5a781abac1cec2bd0b2d7c2`.
Data/inventory19/19 also pass. New actual-runtime cases remain unregistered and
unbuilt pending the tester's frozen source; this gate proves regressions only,
not the full approved adverse-result scope. Coverage/registration stay unchanged.

Callsite audit found another required runtime slice before global activation:
scripted Destruction/Transmutation still use generic actor-only combat chance,
and Death Stare uses a binomial kill roll. These are successful hostile chance
abilities too, not excluded damage variance. Add an explicit harmed-recipient
script bridge preserving frozen chance and legacy RNG, and classify Death Stare's
positive kill result as adverse with exactly one final full redraw. Ordinary
random damage/target selection remain excluded. This is missing implementation,
not a Phase2 excuse to narrow scope; the current native pass does not cover it.

Runtime dependency checkpoint verified: both-target4456 exits0
(`UP089-chain-fixture-build.log`); final native34416 passes35/35, zero skips
in9.458s (`UP089-runtime-verified.log`/`.xml`). Binary SHA-256
`e6bd7c8ccd8ee258a953e1e4103005def3be6210b51ca3d7e56d5a7efba5b852`.
Three new cases verify actual primary MR during chain preparation (including
unchanged secondary-hop HP), negative-Luck forecasts before/after expenditure,
and local hypothetical resolver isolation. Independent Astra source review has
no production blocker; its weak chain assertion finding is repaired and reviewed.
Initial missing-header and unstarted-round failures remain recorded.

Do not activate or count the perk yet. Next required slice is the scripted
hostile-ability bridge, followed by focused actual negative-Luck/Morale, hostile
proc/suppression and late-collateral evidence. Existing deterministic/state tests
pass but do not substitute for these principal callsite cases. Broader multi-event
AI valuation and reflection interaction matrices remain Phase2 integration work.
No GUI, playable promotion or art completion is claimed.

Verified bounded runtime/AI checkpoint is pushed as1b57c9ac1; worktree was clean
on resumption. Root selected the scripted extension: explicit harmed-recipient
boolean proc bridge with one frozen favorable chance, plus a capped binomial
count bridge whose positive result is adverse and whose entire reroll is final.
Current controller determines the suffering army; original actor army retains
its RNG stream. Inert/immune/friendly effects must not spend an allowance, and
legacy first draws must be preserved. One Luna owns the bounded callback/server/
Lua/script implementation; a parallel test-worker spawn was service-rejected.
Registration and coverage remain unchanged pending full scope and focused gates.

Root added the new boolean proc seam's detached AI implementation in its owned
StackWithBonuses files: freeze the projected effective chance once, classify by
current actor/recipient controllers, and spend only local branch state through
the existing resolver. Lua count resolution will use that same generic local
resolver. Predictive stochastic outcome quality remains the existing midpoint
model; it must not fabricate a favorable reroll. No build/native claim yet.

Resumption reconfirms the user-approved explicit scope without changing the
canonical rule. Script implementation is frozen; root aligned invalid/invincible
recipient guards in the authoritative, Lua-count and hypothetical paths. A Luna
tester now owns an isolated scripted-runtime fixture. The concurrent Astra
reviewer spawn was service-rejected and will be retried after the tester finishes.
Root's four additional actual Luck/Morale/proc/suppression cases are unverified.
Both-target build18304 is running with12 jobs (`UP089-scripted-build.log`);
do not execute native tests until it exits or count this perk as complete yet.

Build18304 failed on narrower callback/Unit C++ method names; the service rejected
the bounded repair follow-up, so root repaired that API mismatch directly.
Both-target retry23124 exits0 (`UP089-scripted-build-retry1.log`). Native26641
passes39/39, zero skips in10.901s (`UP089-scripted-regressions.log`/`.xml`),
including all four new actual Luck/Morale/suppression/Death Blow cases. Binary
SHA-256 `a19116a05068cdb05e067c624335c5f3deec38f8e232358af3cd82ca076ee9d5`.
Data/inventory19/19 pass. The tester's three real scripted-ability cases remain
unregistered/unbuilt; this regression checkpoint does not complete the full perk.

Scripted fixture is now registered and verified: both-target50122 exits0
(`UP089-scripted-fixture-build.log`); principal native67689 passes3/3 in1.444s.
The real Lua entry points exercise Destruction success→failed final redraw,
exact full capped Death Stare count redraw, and immune-target non-consumption.
Final combined native6674 passes42/42, zero skips in12.110s
(`UP089-scripted-verified.log`/`.xml`); binary SHA-256
`a18f4d8ed6cc97c933fa9ae37f1b5ab41b0b1be0559f28ac3e07d5416809cdd5`.
Independent Astra scripted review remains unavailable after repeated spawn
rejections, including after tester completion; root reviewed the bounded diff
but does not claim independent approval. Full-attack script event collection,
broader controller/immune/proc matrices and conditional AI valuation remain
Phase2 evidence. Late Hand of Fate collateral is the next principal Phase1
gate before full-perk activation. Coverage remains unchanged; no promotion.

Full Phase1 checkpoint: the late Hand of Fate case passes after retaining a
genuine caster-side escort and normal initiative admission. Current-controller
resistance expenditure is verified without rerolling recipient selection.
Twist is active in the registry/module and aligned with the inventory; art
remains Not done. Both-target31690 exits0; final native95364 passes43/43, zero
skips in12.421s (`UP089-activated-verified.log`/`.xml`), binary SHA-256
`67ba01cfdc050aade2741bee5187d9e2d870ba93b06ffe13c3aaa4bf7b6d3d19`.
Data/inventory19/19 pass. Independent Astra activation review now succeeds and
finds no blocker; broader reflection/controller/cross-category ordering and
conditional forecast breadth remain Phase2. Coverage141→142/310 active perks,
planned169→168; Luck6active/4planned. Ranks84/93 and combat60/67 unchanged.
No GUI, immutable playable promotion or art approval. Next unblocked slice is
UP-090 Rally; its bounded map and suppression-before-Twist contract are recorded.

## UP-088 — Implement Luck Opportunist

Status: Read-only implementation map, 2026-10-01. UP-023 missing Basic Luck
perk: after positive Luck on an attack, retain the stack's current Creature
Activation for movement only, up to2 hexes using remaining movement, with no
additional attack. Map existing Pursuit/Skirmisher activation continuations,
positive strike aftermath and authoritative movement validation before selecting
architecture. Preserve action/activation identity, Time Stop and reaction
ordering; no extra activation or attack may be fabricated. Root owns shared
architecture and final semantic decisions. No code changes while Gambler builds.
Acceptance: an actual positive trigger exposes a legal bounded move, no attack
or reused allowance, round/activation cleanup, principal AI/native verification.

Map complete: Pursuit already supplies a saved/copied/replicated movement-only
allowance, continuation reason, bounded shared path range, authoritative move/
attack validation, generic client controls and an AI movement chooser. Its
current trigger/flow is lethal melee/WALK_AND_ATTACK, so Opportunist must add
actual positive-Luck and ranged paths without creating a new activation. The
shared attack path also handles out-of-turn reactions; a user question asks
whether "remains open" restricts this perk to the stack's own activation.
No implementation or coverage increase yet. Keep the answer explicit rather
than silently excluding reactions solely because Pursuit is easier to reuse.

## UP-087 — Implement Luck Chain of Fortune

Status: Verified (delivery pending), 2026-10-01. UP-023 missing Advanced Luck
perk: once per round after a friendly positive Luck trigger, the next friendly
stack to attack gains+1 Luck for that attack. Map existing shared side history,
authoritative strike packets, reactions and detached AI replay; preserve normal
Luck caps/immunity and current-controller ownership. Determine whether existing
code defines the pending recipient and round expiry before selecting architecture.
Gambler is verified and pushed as680d142c5. Root owns architecture,
registration, serialization, integration and verification. Acceptance: first
positive trigger arms at most one pending+1 benefit, correct next-attack
consumption, side isolation, save/replication and principal native/AI evidence.
Any genuine recipient or carry-over ambiguity must be surfaced, not guessed.

Map complete: shared side state, chanceLuck, existing BattleAttack fortuneState
and per-round lifecycle supply the authoritative/save/replication seams; detached
AI already has branch-local pre-consumption outcomes and ordered replay. Caps
and No Luck remain enforced by the shared callback. No extra canonical clause
defines whether the same stack's second strike may receive the bonus or whether
an unconsumed benefit survives the round boundary. Two user questions are
answered: the recipient must be a different friendly stack. User directed the
round policy to follow the wording; once per round limits triggering, not the
lifetime of an unused benefit, so it carries until the next different stack
attacks. Canonical Luck now records both decisions. A No Luck attack's
consumption policy must be reconciled with this recipient rule. No implementation
or validation was performed by the read-only worker; this map adds no coverage.

Root implementation decision: keep one pending source unit ID and a separate
round-trigger flag in the existing shared Luck state. A different stack's next
attack consumes the pending benefit before its own positive outcome may arm
another; No Luck/caps do not preserve an already consumed attack benefit.
Same-stack follow-ups retain it. Round reset clears only trigger expenditure,
not the pending gift. A carried gift remains one+1, not an accumulating token
stack when the same source triggers again. Existing BattleAttack fortuneState
replicates/saves the transition; append-only NEW_HORIZONS_CHAIN_OF_FORTUNE
defaults older state inert and rejects lossy downgrade/disabled history.
Runtime logging is frozen; AI and a separate fixture have exclusive workers.
Independent review is active. Registration is staged, not completed coverage;
counts remain140/310 until build and principal native gates pass.

Frozen source checkpoint: all three implementation/fixture workers completed,
and independent review has no remaining blocking finding. The shared callback
already reads branch-local fortune through BattleProxy::getBattle returning
this; speculative duplicated Luck formulas were rejected before integration.
Loaded pending-source provenance is validated against recorded positive Luck.
Six focused cases include actual native arm/consume, same-stack shots, round
carry/reset, controlled reactions/No Luck, current/legacy packet state, malformed
state guards, and certain/UNKNOWN candidate plus selected replay isolation.
Data/inventory19/19 and diff checks pass. Both-target build74505 is running
with12 jobs (`UP087-build.log`); native execution is pending. Counts remain
140/310, not141, and no commit/promotion is claimed yet. Broad perk/reaction
matrices and playable combat-log acceptance remain Phase2 findings.

Final gate: both-target3912 exits0; native73716 passes26/26, zero skips in6.779s
(`UP087-repaired-build.log`, `UP087-verified.log`/`.xml`). The failed24/26 run
is retained in the failure register; both errors were fixture setup, repaired
without production rule changes. Independent repair review has no blocker.
Data/inventory19/19 pass. Coverage141/310 active,169 planned; Luck5/5.
Source/native complete; art and playable promotion/acceptance remain pending.

Committed and pushed as0e403406d0da2df58efbf037267d160268ba74da. HEAD and
origin/definitive-mvp match; working tree clean after that push. The launcher
snapshot is unchanged, so this source commit is not a playable-delivery claim.

## UP-086 — Implement Luck Gambler

Status: Source/native verified; playable delivery pending, 2026-10-01. UP-023 missing Advanced Luck
perk: the first friendly attack each round gains+3 Luck for that attack; if
positive Luck does not trigger, its attacker suffers-2 Luck until its next
activation. Map first-strike side history, post-roll penalty and activation
expiry through existing authoritative/replicated and detached AI lifecycles.
Keep current-controller ownership and normal Luck immunity. Root owns shared
architecture and configuration; no code edits before Second Chance freezes and
the map is reviewed. Acceptance: first attack only, positive/non-positive
outcomes, genuine activation expiry, shared AI prediction/branch isolation,
save representation and focused gates. Serendipity's round1 question remains
pending, not silently replaced by an assumption.

Map complete: add an independent Gambler side flag and round-long first-attack
expenditure to shared Luck state; use current controller for the first-strike
bonus and include reactions. No Luck still prevents the+3 but consumes the
first attack and qualifies for the non-positive penalty. Store the-2 on the
unit through an ordinary LUCK bonus/SetStackEffect, not a side-owned recipient
set, so it follows controller changes. STACK_GETS_TURN supplies the normal
expiry seam; root must check Second Wind/HERO_COMMAND genuine activation
before relying on it, because existing nextTurn paths skip that removal for
HERO_COMMAND. Detached first-strike expenditure must happen even for uncertain
Luck and remain branch-local. Conditional stochastic penalty correlation is
Phase2 AI breadth, not permission to fabricate a guaranteed roll. Use separate
Gambler fixtures and append-only side-state serialization. No activation yet;
the root owns the final lifecycle decision and implementation partitions.

Root lifecycle decision: expire only the uniquely identified Gambler penalty
when battleBeginsActivation is true, including Second Wind, in authoritative
BattleInfo and detached AI. Do not broaden legacy STACK_GETS_TURN expiry for
unrelated bonuses. Timed per-unit LUCK-2 uses the existing bonus/SetStackEffect
wire and follows controller changes. Shared side gambler/round expenditure,
setup, append-only NEW_HORIZONS_GAMBLER and registration are staged. Runtime
processor, three AI files and a separate new native fixture have exclusive
workers. Root owns shared helpers/state/config/CMake/docs/build/Git. No
completed coverage or playable delivery is claimed before the focused gates.

Frozen source checkpoint: independent review has no remaining blocking finding.
Pre-consumption Luck outcomes survive detached replay, positive aftermath is
applied once, and valid zero-probability curves are neutral rather than unknown.
The damage cache accounts for the side perk and unit penalty after expenditure
or control changes. Data/inventory checks pass19/19; both-target build49572
is running with12 jobs (`UP086-build.log`). Native execution is pending; do not
count this as completed coverage or playable delivery. Conditional stochastic
penalty correlation, broader reaction/controller matrices, committed-replay
recovery and detached-expiry fixture breadth remain Phase2 findings.

Execution checkpoint: build49572 failed only on fixture probability fields
declared private; repaired build68457 passes both targets. Native52671 passes
15/20, zero skips: the five Gambler gameplay cases retain Advanced Luck+2
despite their intended zero baseline. The tester is repairing fixture setup
without changing rank or production rules. Keep coverage139/310 until the
same focused selection passes. Failed runs are retained in NH_RELEASE_FAILURES.

Final gates: both-target76677 exits0; native39678 passes20/20 with zero skips
in5.324s (`UP086-verified.log`/`.xml`), including six new Gambler cases and14
Luck regressions. Binary SHA-256
`3ef29f6941beefed86678fe8ce02a0d383d3330f45d38eeca490b7f6568ab6da`.
The fixture uses a local ordinary-2 compensation to isolate the+3 bonus while
retaining legal Advanced Luck and Basic Fortune's Favor selection. Production
rank rules are unchanged. Data/inventory19/19 pass; independent review blockers
are repaired. Coverage139→140/310 active,171→170 planned; Luck4/6. Earlier
failed builds/tests remain recorded. Art Not done; no launcher promotion or
graphical acceptance is claimed. Phase2 findings remain listed above.

## UP-085 — Implement Luck Serendipity

Status: Read-only architecture map, 2026-10-01. UP-023 missing Advanced Luck
perk: when no friendly positive Luck trigger occurred in the previous round,
the first friendly attack of the new round receives+2 Luck for that attack.
Map the existing Sylvan Serendipity history, authoritative first-strike
consumption, shared damage forecast and detached AI replay. Do not conflate
perk identities, invent additive coexistence, or activate from description
alone. No runtime edits while UP-084's candidate builds. Root owns the reuse
decision and any narrow design question; worker is read-only. Acceptance:
positive/no-positive previous rounds, first-attack-only behavior, saved/replicated
history, selected/rank gating, AI parity and focused native/data gates.

Map complete: Sylvan's same-named Basic perk is combat-long+1 per stack until
its first positive trigger, not the generic perk's previous-round+2 first-attack
rule. Reuse the shared side-state/round/strike packet lifecycle but retain
distinct flags and round history; combat-long positiveLuckUnits cannot answer
the previous-round question. Detached AI must consume the first-attack window
even for uncertain/no-Luck outcomes, not only guaranteed rolls. The first
executed friendly attack consumes it even when No Luck prevents the bonus;
do not bypass immunity. User question pending: whether round1 receives it or
eligibility starts at round2 after an actual previous round. No activation yet.

## UP-084 — Implement Luck Second Chance

Status: Source/native verified; playable delivery pending, 2026-10-01. UP-023 missing Basic Luck
perk: the first negative Luck trigger against the army each combat is ignored.
Use independent once-per-combat eligibility/expenditure, not Sylvan Nature's
Providence's resetting once-per-round flag. Map replicated/saved side state,
authoritative roll suppression, detached AI expectation and branch expenditure.
Root owns architecture/config/version/docs/CMake/build/Git. Acceptance: actual
first negative trigger suppression, subsequent triggers unchanged across rounds,
side isolation, current-controller ownership, serialization and focused AI/native
evidence. No per-update scan or fabricated extra action. Map complete; root
state/setup/append-only serialization and registration are staged. Runtime and
AI have disjoint files, tester has a new isolated fixture. Data/inventory19/19
pass. Final both-target23927 exits0; native6011 passes14/14, zero skips in3.859s
(`UP084-verified.log`/`.xml`), including six new cases and eight Luck/Providence
guards. Binary SHA-256
`8a34b62c978fa1842b571c9d1e0c5344583d18aa4678e6c5f73f5d61cd553f5f`.
Independent source/fixture review blockers are repaired: safe detached
retaliation target lookup and positive/negative exclusivity. The old Providence
fixtures now satisfy legal Basic Elven Precision before Advanced prerequisites;
failed compile/runs and root's incorrect first prerequisite choice are retained
in NH_RELEASE_FAILURES.md. Coverage138→139/310 active, planned172→171; Luck3/7.
Probabilistic multihit, explicit stochastic-result replay, direct fully absorbed
reaction/controller-change matrices remain Phase2. Purpose-made art Not done;
no launcher promotion or rendered acceptance.

## UP-083 — Implement Luck Lucky Recovery

Status: Read-only next-slice map, 2026-10-01. UP-023 missing Advanced Luck
perk: after positive Luck on a melee attack, surviving attacker creatures
recover HP equal to10% actual damage. Existing Sylvan Luck has the same named
effect; map shared authoritative/AI recovery without conflating independent
perk identities or silently inventing a stacking policy. Map complete: existing
server and detached AI use a shared side-state recovery flag and actual-HP heal.
The user was asked whether both identically named10% perks provide one10%
effect or additive20%. Await that answer before choosing an effective amount.
No activation yet; other unblocked coverage work can continue.
Acceptance: actual HP-loss healing, no resurrection, conditional melee/Luck
eligibility, current-side ownership, AI parity, log feedback and focused gates.

## UP-082 — Implement Luck Lucky Aim

Status: Source/native verified; playable delivery pending, 2026-10-01.
UP-023 missing Basic Luck perk: positive
Lucky ranged attacks ignore 25% of target Creature Defense. Reuse the shared
lucky ranged Defense-ignore payload and damage calculation; normal, negative
Luck, melee and non-creature/non-physical damage must not gain this benefit.
Root owns activation/config/docs/CMake/build/Git; runtime worker owns
CBattleInfoCallback.cpp and tester owns a separate new native fixture.
Acceptance: principal damage path, rank/selection gating, detached AI parity,
both-target compilation and focused native/data evidence. No polling, new
combat counter or save format is needed for this derived attack property.
Final both-target62197 passes; native69961 passes8/8, zero skips in2.487s
(`UP082-final.log`/`.xml`): three Lucky Aim, three Fortune's Favor and two
existing Elven Precision cases. Data/inventory19/19 pass. Source/fixture review
finds no blocker after correcting the fixture geometry and negative-factor
composition; root integrated the failed-run repairs. Phase2 retains executed
shot/reaction and dual-perk combinations plus general fractional-damage rounding.
Artwork Not done; neutral fallback remains. No launcher promotion.

## UP-081 — Implement Luck Perfect Fortune

Status: Read-only next-slice map, 2026-10-01. UP-023 missing Expert Luck
perk: the first eligible army attack each combat triggers positive Luck
automatically. Map authoritative eligibility/roll timing, once-per-combat state
and shared AI expectation without conflating Sylvan Luck's selected Perfect
Moment. Do not activate or implement before the root reviews the map and assigns
exclusive ownership. Map complete: use a distinct side token, shared resolved
creature-strike eligibility and branch-local AI history; do not reuse opt-in
Sylvan Perfect Moment. The user was asked whether No Luck prevents the automatic
guarantee. First-blow/reaction scope must be resolved from canonical normal Luck
eligibility before assigning implementation. Acceptance: registration, authoritative first eligible
attack behavior, state persistence, AI parity and focused native evidence.

## UP-080 — Implement Luck Fortune's Favor

Status: Source/native verified; playable delivery pending, 2026-10-01.
UP-023 missing Basic
Luck perk: positive Lucky Strike damage multipliers increase by +0.25x.
This opens ordinary Luck progression, currently blocked by zero active Basic
perks. Reuse the existing LUCKY_STRIKE_DAMAGE_PERCENTAGE bonus/damage formula
and hero perk lifecycle if they express the rule correctly; do not create a
parallel damage multiplier or new polling. Map live melee/ranged/retaliation,
shared AI and minimum native evidence. Root owns integration/activation/docs/
CMake/build/Git. Veteran is verified and committed as b626171da. Fortune's
Favor derives its bonus through the existing secondary-skill rebuild and
refreshes on accepted perk selection. Both-target56878 passes; native69200
passes4/4, zero skips (1.398s); data/inventory19/19 pass. Independent production
review finds no blocker. Legal offer acceptance, rank loss/reacquisition,
reconstruction deduplication, ordinary/positive/negative damage and detached AI
expected damage are covered. No new save fields or per-update work. Phase2
retains explicit save roundtrips and ranged/retaliation/reaction/Sylvan matrices.
Artwork is Not done, fallback remains neutral; no launcher promotion.

## UP-079 — Implement Armorer Last Stand

Status: In progress; bounded architecture map, 2026-10-01. UP-023 missing
Expert perk: once per combat, the first friendly stack that would be completely
destroyed by a physical creature attack instead survives with one creature at
1 HP and immediately Defends. Map authoritative attack damage, shared health
and casualty handling, side-wide once-per-combat history, detached AI and
replicated/saved state before assigning source ownership. Unlike Veteran, this
rule says physical creature attack, not every physical damage source. Root owns
architecture, activation/version/config/docs/CMake/build/Git. Read-only map
can run while UP-078's frozen source undergoes focused validation; no activation
or completed coverage claim yet.

Map complete. Two consequential choices await user direction: whether surviving
lethal retaliation and immediately Defending ends the stack's own activation,
and whether clones/Phantom Integrity qualify. Preserve the physical-attack
versus physical-damage distinction and actual creature-HP/casualty provenance.
Continue an unblocked Basic Luck foundation while these answers are pending.

## UP-078 — Implement Armorer Veteran

Status: Verified (delivery pending), 2026-10-01. UP-023 missing
Advanced Armorer perk: at the beginning of a stack's activation, restore 15%
of physical creature damage suffered since its previous activation, limited
to surviving creatures. Reuse authoritative damage provenance and activation
events; do not resurrect casualties or restore Phantom Integrity. Share the
history/recovery rule with detached AI, use saved/replicated state where needed,
and preserve Wait versus actual activation semantics. Root owns architecture,
activation/config/version/docs/CMake/build/Git. Workers initially read-only;
no completed coverage or playable claim. Previous cycle was progress: UP-077
committed and pushed as f774b24c3, final 18/18 native and 19/19 data checks.

Architecture checkpoint: reuse existing PHYSICAL_CREATURE damage provenance,
including sources already classified that way (physical Poison, reflection and
Rain of Arrows). Record actual creature HP loss, not absorbed temporary or
Guardian Spirit HP. Veteran says physical creature damage, unlike the narrower
physical creature attack wording in Last Stand/Bastion. Recovery floors 15%,
cannot resurrect, and consumes its interval only at a genuine activation.
JSON unit updates preserve the counter; older wire formats reject nonzero
history. Ordinary saving during combat is already blocked by CBattleQuery;
unsupported binary battle snapshots must reject pending history rather than
silently discard CUnitState. No polling or new packet type. Runtime implemented,
AI and focused fixtures in progress; coverage remains unverified.

Client12894 compiles; data/inventory19/19 pass. Independent Astra source review
requires a repair before completion: Guardian Spirit is absorbed again when
the AI commits a post-absorption strike payload, and incoming damage clamps
omit its buffer. AI worker repairs raw incoming versus actual HP-loss handling;
tester adds preview/commit HP-buffer-history assertions. Preserve this finding
in NH_RELEASE_FAILURES.md; native verification and coverage increase pending.

Final checkpoint: both-target8101 passes; native19447 passes14/14, zero skips,
in4.124s, reports `UP078-focused-buffer.log`/`.xml`. Binary SHA-256
`ef35142a822610a400a5f9dad60f358fb21645a2cb15736ce325a84f0428dca8`.
Data/inventory19/19 pass. Astra review blockers are repaired. Coverage135→136/310
active perks, planned175→174; Armorer5/5→6/4 active/planned. Rank84/93 and
combat identity60/67 counts are unchanged. Focused principal live activation,
survivor-only healing, JSON/wire safety, owner-scoped AI and real Guardian-buffer
preview/replay evidence pass. Failed fixture runs remain preserved. Phase2
retains fully absorbed multistrikes and Guardian reactions/Rain combinations.
Purpose-made icon remains Not done; no GUI acceptance or launcher promotion.

## UP-077 — Implement Armorer Formation Fighting

Status: Verified (delivery pending), 2026-10-01. UP-023
missing Advanced perk: a stack adjacent to at least one friendly stack cannot
be flanked and receives an additional10% physical damage reduction. Share live
and detached battle geometry, actual allegiance and existing physical cap;
include melee/ranged/retaliation, movement/death changes and two-hex footprints.
Root owns activation, docs/builds/Git. Map exact production/test ownership before
edits; no coverage or playable delivery claim yet. Diplomacy remains pending
its authored free-join exception choice, not silently dropped.

Source checkpoint: shared callback protection handles current allegiance,
projected defender footprint and living allies, with no new saved state.
Independent10% reduction uses the existing physical cap; Shroud and Flank
melee/history are suppressed, Combined Arms ranged remains available. Root
repaired review blockers: require the active Advanced perk, explicitly gate the
ranged branch, and exclude detached self aliases by unit ID rather than pointer.
Client build57962 passes (`UP077-client-build.log`); native prerequisite
compile84365 passes (`UP077-native-prerequisite-build.log`). The standalone
fixture was registered only after its actual file existed; subsequent builds
and native evidence are recorded in the final checkpoint below.
Phase2 retains synchronization of other allies' projected movement/death in
multi-blow AI forecasts. No completed coverage or playable promotion yet.

Final checkpoint: both-target74477 passes after fixture repairs. Native61868
passes18/18, zero skips, in4.465s; reports `UP077-focused-final.log`/`.xml`.
Binary SHA-256 `1ea4d9dba78922b514f2763f1a6353c5f87a4f5313abb637a50aee04a013f6e8`.
Data/inventory19/19 pass. Independent source/fixture review has no remaining
blocker. Coverage134→135/310, planned176→175; Armorer5/5 active/planned,
ranks84/93 and combat identities60/67 unchanged. Starter-army isolation and
owner-scoped AI views repair fixture assumptions, not production privacy.
Keep failed runs and the separate Encirclement repeated-hit assertion in
NH_RELEASE_FAILURES.md. Purpose-made art remains Not done; no launcher promotion.
Next unblocked missing perk: Armorer Veteran's surviving-creature physical
damage recovery; map authoritative activation/physical damage history and AI.

## UP-076 — Implement deterministic Diplomacy foundation

Status: In progress; bounded architecture map, 2026-10-01. UP-023 missing
foundational rank/neutral encounter mechanic. Basic/Advanced/Expert eligible
neutral joining thresholds are25/50/75% of the hero's current Army Value,
paid at normal recruitment Gold cost; scripted/explicitly hostile encounters
may remain ineligible. Shared authoritative eligibility/cost must feed AI and
required pre-encounter feedback. Preserve Leadership and army-transfer validation,
no rerolled joining chance or frontend state mutation. Map existing monster
join/offer/query/cost, Army Value and AI encounter paths before assigning safe
ownership. Root owns architecture, activation, docs/CMake/builds/Git. No rank
activation, verified coverage or playable claim yet.

Prior UP-048 map reused rather than repeated. New evidence confirms global
joining percentage deliberately retains the original full-stack Gold price;
per-object HotA percentage is parsed but ignored by existing admission. Authored
COMPLIANT free-joining versus normal paid threshold remains a material design
choice; concise question renewed. Keep rank activation on hold and continue
UP-077 while awaiting direction. Preserve existing Leadership/garrison lifecycle.

## UP-075 — Implement Estates Estate Network and Learning Quick Study

Status: Verified (delivery pending), 2026-10-01. UP-023 missing
Advanced perk coverage. Estate Network grants1 Wood and1 Ore per three owned
towns, rounded down, minimum1 with any owned town, at the start of each week.
Quick Study rerolls the initial level-up offer once before presentation at
every fifth hero level. Reuse authoritative weekly income and saved level-up
choice machinery; do not add polling, UI-side RNG or repeated rerolls on query
re-exposure. Map shared AI paths and minimal native evidence in parallel.
Root owns activation, integration, CMake, docs/builds/Git; workers initially
read-only until disjoint source ownership is assigned. No coverage claim yet.

Mapping approved: Estate Network uses current owned towns and eligible hero
holders (including garrison heroes), exact grants after ordinary income/AI
handicap calculations in NewTurn, including day0→1 but no setup-day daily
income. Existing calendar/replicated resource application is the lifecycle;
no new counter or polling. Worker owns NewTurnProcessor.cpp and existing
economy/Estates-AI fixtures. Quick Study owns CGameHandler.cpp plus isolated
NewHorizonsQuickStudyTest.cpp: reached level is hero.level+1; redraw complete
skill/perk offer with saved RNG/fresh perk seed once after the initial draw,
preserving one primary gain and final query snapshots. Human and AI consume
the same offer; repeated candidates by chance are permitted. Prompt exposure
must not redraw. Mid-query saving is already blocked. Source registration is
being enabled for development, not verified/countable until builds/tests pass.

Production checkpoint: both bounded runtime edits are frozen and independently
reviewed with no blocking finding. Client retry51396 passes; data/inventory19/19
pass. Root's premature CMake registration failure and repair are retained in
NH_RELEASE_FAILURES.md; isolated Quick Study registration is deferred until
the real fixture exists. Economy/AI and query fixtures remain in progress.
No verified coverage increase, commit or playable promotion yet.

Final checkpoint: both-target20329 passes after recorded fixture repairs;
native80431 passes29/29 with zero skips in10.865s. Reports
`UP075-focused-repaired.log`/`.xml`; test binary SHA-256
`93bdab7a969ec6a92b2b6ce6210066f2c9930b1f1a60003941f78ee62c5373fd`.
All four Estate Network server cases, both AI cases and all five Quick Study
query cases pass with prior economy/Mentor regressions. Final data/inventory19/19
pass; independent review has no remaining blocker. Coverage132→134/310 active
perks, planned178→176; Estates2/10 and Learning2/10 open ordinary Expert
progression. Ranks84/93 and spells60/67 unchanged. Preserve the original AI
mixed-offer failure as a fixture lesson, not a repaired production valuation.
Phase2 keeps comparative perk valuation, crash/pending-query recovery and
custom-calendar/script interactions. Commit/push follows; no graphical journey,
new art or immutable launcher promotion. Committed and pushed as7b5c4c21d.
Next highest-priority missing foundation:
deterministic Diplomacy ranks and joining path, with minimum AI/Leadership hooks.

## UP-074 — Implement Learning Academic Study

Status: In progress; read-only map, 2026-10-01. Independent UP-023 Advanced
perk coverage after Mentor's Basic progression path. On the hero's first visit
to each town, grant250 Experience for each Mage Guild level already built.
Use authoritative town visits, existing recipient Learning composition and
persisted per-hero/per-town first-visit provenance, never a periodic map scan.
Map whether existing visit history can be reused and how AI previews/choices
consume the result. No activation or verified coverage increase yet. Root owns
integration, registration, builds and Git; mapper does not edit source or run
builds. Preserve the ongoing Mentor build and frozen source ownership.

Read-only map complete: successful town entry/capture, town portal, Castle Gate
and recruitment reach heroVisitCastle; map-authored replacement scripts can
bypass it. mageGuildLevel supplies built levels0–5. The serialized hero
visitedObjects set can represent town IDs, but ordinary town arrival does not
currently populate it. Existing VISITOR_ADD_HERO also changes player/team
history, so avoid those incidental effects when adding a hero-only marker.
Mark before Learning-adjusted XP to keep level-up reentry idempotent; a zero-guild
visit must have explicitly resolved first-visit semantics. Asked whether visits
before learning Academic Study consume eligibility or whether its first visit
after acquisition qualifies. Old saves cannot reconstruct historic town arrivals.
Do not activate before resolving that timing choice. Minimal tests cover
0/1/3/5 guild levels, rank/perk gates, repeats/other towns, later guild builds,
save/load, marker/query order and ordinary AI selection/award. No extra hero
history field is required if the existing set is reused safely. Destination XP
valuation and authored-script overrides remain separate AI/integration work.

## UP-073 — Implement Learning Mentor

Status: Verified (delivery pending), 2026-10-01. Unblocked UP-023 Basic perk progression while
Historian's primary-XP classification awaits the user. First lower-level allied
hero met each week gains250×the mentor's captured meeting level, composed with
the recipient's ordinary Learning XP rule. Handle field heroExchange and town
visitor/garrison meetings; capture eligibility before the award and record a
replicated per-mentor absolute-week use before granting XP. Level-up queries
must not be hidden beneath a subsequently added exchange dialog. Persist used
weeks and fail closed when an old format cannot retain them. Master Teacher
remains planned; do not grant its second-recipient or500× benefit.
Root owns activation, serialization feature version, CMake, docs/builds/Git.
Runtime worker owns the declared hero/packet/visitor/server paths and isolated
native fixture. Focus actual meeting/weekly eligibility, XP and query ordering,
state roundtrip and ordinary AI exercise; no activation/counting yet.

Frozen source checkpoint: field/town hooks snapshot levels and weekly use,
replicate SetNewHorizonsLearningMentorState (append-only type286) before XP and
put field exchange below any Mentor level-up query. Hero unused defaults remain
readable in older saves; used state and new packet writes reject older formats
under NEW_HORIZONS_LEARNING_MENTOR. Mentor is source-active with neutral icon
fallback (art Not done), not native verified. Content/inventory78/78 pass;
production review has no confirmed blocker. Client build93948 passes. New
server/AI fixtures are frozen and reviewed. Phase2 retains nested town-building XP,
mixed-owner allied meetings and save/load mid-prompt. Merchant Prince remains
planned; its independent best-market selector is source-reviewed and wired.

Both-target repair build81553 passes; focused native52779 passes24/24 with zero
skips in7.070s, covering field/town meetings, XP composition, weekly eligibility,
query ordering, marker persistence/wire guards and real Nullkiller perk choice
and meeting. Reports `UP073-mentor-focused-repaired.log`/`.xml`; binary SHA-256
`513b9d11767748e25f98f8e265fd6a71197caf8ec1c4f7be06991a9945dc92f4`.
Final data/inventory19/19 pass; earlier broader checkpoint78/78 passes.
Coverage131→132 active perks, planned179→178; Learning1/10. Preserve the failed
fixture builds and first25-test run in NH_RELEASE_FAILURES.md. The unrelated
Muster higher-tier fixture prerequisite failure is deferred to Phase2, along
with comparative AI valuation/proactive meeting planning. No graphical run,
purpose-made art or playable launcher promotion. Committed and pushed as
07fe8d95c955d43dd2f9cb714937fce094feb6a0; origin/definitive-mvp matches.

## UP-072 — Implement Nature Elemental Convergence

Status: In progress; read-only architecture map, 2026-10-01. UP-023 missing
Level5 combat identity. Terrain chooses one of the five canonical Elementals
using Experimental Values; summon exact250+5×SP HP with ceil-count and wounded
last creature at a caster-selected legal position. Retain complete native
abilities and remove the summon after battle. Share captured spell coefficients,
placement/HP, serialization and AI forecast. Audit native Summon/Transfigure
reuse before assigning files; no new mapping or creature type may be guessed.
Root owns integration, registrations and builds/Git. No activation or coverage
increase is claimed by this map.

Mapping blocker: canonical terrain rows omit Dirt, Sand/Desert, Swamp and
Wasteland; the engine also forces Sand for coastal arenas. Asked whether to
use Earth for Dirt/Sand/Wasteland and Water for Swamp/coastal battlefields.
Do not silently infer those mappings or activate an incomplete spell. Use the
captured battle terrain rather than the hero's map tile; town/object arenas may
override that terrain. Generic summon infrastructure may progress independently.

## UP-071 — Implement Learning Historian; map Estates Merchant Prince

Status: In progress, 2026-10-01. UP-023 missing Basic perk coverage and ordinary
Learning progression. Historian grants +50% Experience from adventure objects
whose primary reward is Experience, not combat or every source of XP. First
map source classification, reward publication, ordinary Learning composition
and AI forecasts. Independent read-only mapping locates Merchant Prince's
shared Marketplace count/rate API while Steward's resident stacking decision
is pending. Root owns architecture, activation, docs, builds and Git; no edits
by explorers until exact disjoint ownership is assigned. Require authoritative
reward/trade results, eligibility and principal AI/shared forecast evidence.
No new activation, verification or playable delivery is claimed at selection.

Merchant Prince map: CGTownInstance::getMarketEfficiency feeds the existing
IMarket quote shared by UI, authoritative trade validation and Nullkiller.
Outdoor markets are separate and must not inherit the town perk. Asked whether
visiting/garrison holders both count, whether +2 applies once per town or per
holder, and whether all existing rate-based exchanges qualify. Do not infer
those boundaries. AI currently selects the first owned resource-market town;
selecting the best applicable quote is required to exercise the perk reliably.

Historian map: selected reward rows and the object itself have no explicit
primary-XP classification. Learning Stone is pure XP; Treasure Chest has
alternative XP/Gold/artifact rows; Tree of Knowledge grants a level; mixed
Pandora/quest/custom bundles may contain XP secondarily. Asked whether XP
Chest branches and Tree should qualify, with explicit metadata for mixed
bundles. Do not insert a global XP multiplier affecting combat, altar trades,
Sirens, scripts or cheats. Actual reward and displayed components must share
the classification. Basic Mentor's fully specified weekly allied-meeting
trigger is being mapped as an independent progression path while this waits.

## UP-070 — Implement Estates Tax Collector

Status: Verified (delivery pending), 2026-10-01. Independent UP-023 missing Basic perk, formerly
blocking ordinary Estates progression. Gain 50 Gold per day per owned town,
capped at 500 Gold per day from this perk. Audit existing daily hero income and
AI forecasts before editing; reuse the daily event, not a polling scan or a new
mirrored treasury. Respect active perk/rank and saved rules. A read-only Luna
map establishes exact runtime/test ownership outside lib/spells and the
Spellcraft fixtures. Root owns activation, documentation, builds and Git.
Require owned-town count/cap, absent/planned/rank gating and authoritative
daily-income evidence before counting. No implementation or delivery claimed.

Source checkpoint: dailyIncome adds the capped contribution before the existing
handicap, and authoritative NewTurn payout and Nullkiller BuildAnalyzer consume
that shared result. Independent production/fixture review found no blocker.
getTowns reconstructs its collection from owned objects, so this is not O(1)
end-to-end; it runs on income requests, not a per-frame invariant scan. Native
test build `65937` is running; focused execution and coverage counting remain
pending. Phase 2 retains handicap, reload and hero-ownership-transfer scenarios.

Focused native `86706` passes all twelve economy cases and the Tax Collector AI
case, zero skips, after the test rank-parameter repair. Both-target build
`24828` passes. Overall selection is 35/38 due to separate Grand Formula fixture
failures retained in NH_RELEASE_FAILURES.md. Tax Collector can advance
independently after final integration; no playable promotion is claimed.

Isolated native `25581` passes 13/13, zero skips, in 4.388s; reports
`UP070-tax-collector.log`/`.xml`. The same production/test bytes were used as
the combined run. Tax Collector is native verified; Grand Formula's remaining
fixture repairs do not invalidate this independent payout result.

## UP-069 — Implement Spellcraft Grand Formula and audit Concentration

Status: Grand Formula verified (delivery pending); Concentration blocked on design, 2026-10-01. UP-023 missing-perk coverage. Grand Formula
must scale the Spell Power-derived component of the first accepted Level 4 or
Level 5 hero spell to 150% before other multipliers, retaining the flat base.
Reuse completedHeroSpellLevels rather than add duplicate battle state; creature
casts, rejected actions and ordinary round rollover must not consume/reset it.
Authoritative mechanics and detached AI must share the multiplier for damage
and other numerical consumers. Concentration's exact single-stack targeting
boundary is being audited before choosing an implementation; do not silently
equate selected aims with all affected stacks. Root owns architecture,
activation, docs, builds and Git; independent Luna runtime/test maps are
read-only until exact ownership is assigned. Require focused actual casting,
shared forecast and first-combined-Level-4/5 evidence before activation/counting.
No coverage increase or playable delivery is claimed at selection.

Architecture checkpoint: Grand Formula snapshots the shared first-4-or-5 gate
beside Arcane Focus in BaseMechanics. A generic cast-component percentage
combines 150% Grand Formula with 120% Arcane Focus multiplicatively (180%,
not additive 170%); all Mechanics-backed numerical helpers consume the same
snapshot before accepted-cast publication. No new persisted field is required.
Independent tests own separate new server/AI fixtures. Concentration remains
planned: the user has been asked whether direct single-stack targeting alone
qualifies or a spell affecting exactly one stack can qualify even if it is an
area/global/chain spell. Do not resolve that distinction silently.

Runtime checkpoint: the bounded Grand Formula source is implemented and
independently reviewed without a core-mechanic blocker. Root corrected the
spell-level lookup to the battle callback API before compile (IBattleInfo is
not the spell-level callback). Object probe `89982` passes the changed mechanics
and effect translation units; full build and focused runtime/AI cases remain
pending. Ordinary hero-only descriptions still omit battle-specific modifier
values, a deferred shared presentation limitation. No verification/counting or
playable claim is made from this object compile alone.

Final both-target build `68608` passes; native `45801` passes 38/38, zero skips,
including all six Grand Formula runtime/AI cases and thirteen economy/AI cases.
Reports `UP069-UP070-focused-repaired.log`/`.xml`; failed builds and fixture
repairs are retained in NH_RELEASE_FAILURES.md. Content/inventory78/78 and
independent final review pass. Coverage advances129→131/310 active perks,
Spellcraft3→4 and Estates0→1; ranks/spell identities unchanged. No graphical
acceptance, new artwork or launcher promotion is claimed. Concentration's
targeting question remains unanswered. Steward's mapped daily-income seam is
next; its two-resident stacking question is pending.

## UP-068 — Implement Wisdom Mana Conservation

Status: Verified (delivery pending), 2026-10-01. UP-023 missing Advanced perk; independent
coverage work alongside UP-066's expected-outcome AI. After combat restore
20% of actual Mana spent during that combat, capped at 20, into Normal Spell
Points only; preserve Buffer Spell Points and the current normal maximum.
Do not infer expenditure from initial minus final Mana, since regeneration,
refunds and Buffer grants make that incorrect. First audit existing accepted-cost
accounting before adding state. Root owns architecture, activation, documentation,
builds and Git; the Luna worker must obtain an exact ownership contract before
editing. Require authoritative packet application and focused cost/result tests.
Both-target build `66640` passes. Native `65013` passes all ten Mana Conservation
cases: accepted/rejected/creature costs, successful ward payment, malformed
metadata, floor/cap/current-capacity/Buffer handling, inactive perk/rank gates
and versioned state/packet persistence. The total run is 68/69; its separate
random-form AI failure is retained and under repair. Coverage increases
128→129 active perks (181 planned); Wisdom 7/3→8/2. Retreat/surrender/draw
native scenarios remain Phase 2 findings. No playable promotion is claimed.
Isolated perk run `36603` passes 10/10, zero skips, in 2.823s; reports
`UP068-mana-conservation.log`/`.xml`. Content/inventory checks pass 78/78.

## UP-067 — Implement Spellcraft Arcane Focus

Status: Verified (delivery pending), 2026-09-30. UP-023 missing Basic perk; independent bounded
work while the Polymorph shared-form contract is mapped and UP-065 awaits its
design answer. The first accepted hero spell in combat gains 20% on its Spell
Power-derived numerical component only, not the flat base. Reuse the existing
battle-long completed-hero-spell state; no duplicate counter. Creature casts and
rejected actions must not consume it, and round advancement must not renew it.
Authoritative mechanics and detached AI must share scaling and completion, with
no mutation of live state/RNG during previews. Cover timed and damage principal
paths and audit helper-based numerical consumers rather than certifying damage
alone. Root owns configs, test wiring, docs, builds/Git; runtime owns lib/spells
and its new server fixture; AI tester owns only its new AI fixture. Source
registration is not completion; require successful build and focused execution.

Resumed after recording UP-065's design blocker. The interrupted exploration
made no runtime edits; premature activation/test-file registrations were removed.
Reuse completed hero-cast history and propagate the cast-specific modifier into
direct numerical helpers (including Quicksand and Sorrow), not just damage.

Final both-target build `55273` passes; isolated native `49925` passes 27/27,
zero skips, with actual AI selection/accepted casting, detached first/second
casts, Sorrow after completion publication, rejected/creature casts and Land
Mine count guards. Content/perk 76/76, placement/module/diff checks pass; review
has no remaining blocker. Reports `UP067-arcane-focus-focused-retry.log`/`.xml`.
Coverage advances 127→128 active perks, Spellcraft 2→3; no rank/spell identity
change. Broader interactions and full battle save/load remain Phase 2. Artwork
is Not done and launcher promotion/manual playable acceptance remain pending.

## UP-066 — Implement Chaos Polymorph and battle-local creature forms

Status: In progress; architecture/ownership checkpoint, 2026-09-30.
UP-023 Phase 1 missing combat identity; UP-065 Basic Toxic Spines remains
blocked on the requested design choice, not forgotten or silently rewritten.
Canonical Polymorph is Level 3, 12 Mana, one enemy stack, random same-tier form
from any faction for two rounds. Preserve exact aggregate creature HP through
ceil(HP/new per-creature HP) plus a wounded final creature, and convert surviving
HP back on expiry. Preserve owner, allegiance, current initiative position and
transferable magic; replace creature stats, movement, attacks, abilities and
resistances. Keep the same battle unit ID, original campaign-army species and
casualty provenance. Normalize the form before early battle-result accounting;
never persist the replacement species/count into the hero's permanent army.
Authoritative and detached AI must share effective-form and HP rules, without
original creature-bonus leakage or live RNG during previews. Registration,
required targeting/status feedback, build and focused real cast/reversion/AI
evidence are required before counting this identity. Shapeshifter's two-form
lower-Army-Value selection is a separate modifier, not implied by the base spell.
Root owns shared architecture, registration, docs, builds and Git; the bounded
form-contract explorer is read-only. No implementation or playable delivery
claimed at this initial checkpoint.

Geometry decision resolved by the user: relocate to the nearest legal position
when the replacement footprint cannot fit at the original anchor. Keep all
same-tier forms eligible rather than excluding non-fitting forms. Ownership,
allegiance and current Initiative queue position remain unchanged. The approved
rule is integrated into canonical Polymorph; do not overlap blocked/occupied
hexes. Authoritative and detached relocation must share the same legality rule.

Read-only contract checkpoint: preserve CStack's original typeID/base/baseAmount
for campaign army identity. Effective form belongs in shared CUnitState and must
copy/save with detached state. Filter old CREATURE_ABILITY source-ID bonuses at
the effective unit view, then add the replacement's native bonuses; do not mutate
the original army stack or retain both species' abilities. CHealth's integer
form counts cannot double as original casualties/remains: use an original-species
HP/provenance ledger distinct from current-form count and wounded final creature.
Normalize before BattleResultProcessor snapshots casualties/Necromancy, including
early battle end. Current getKilled()/getUnusableRemains() arithmetic is not a
safe form implementation. No source feature or coverage increase claimed.

Implementation checkpoint: shared health and native/detached bonus views are
assigned to separate Luna workers; root owns deterministic nearest-legal
placement, save-version/wiring and integration. An independent Astra reviewer
is active. JSON unit state must round-trip the form and source-health ledger;
binary battle snapshots currently omit CUnitState and must fail closed rather
than silently discard a form. Full spell activation, expiry/result geometry,
AI spell selection and required status presentation are not yet implemented.

Foundation checkpoint: final both-target Linux build `85599` passes; focused
native retry executes 21/21 with zero skips. Reports:
`UP066-battle-form-focused-retry.log`/`.xml`; test binary SHA-256
`86640d13acb1d17f121c8fe91ccab088ef0c75b70e6b50c72dc591d0b763aba8`.
Checks cover exact HP/temp-pool repartition, original corpse/one-battle
resurrection provenance, expiry, real acquired-CStack JSON/native-bonus views,
nested AI rank eligibility, nearest strict placement, baseline Health and
Shadow Gift guards. Independent source review and module/diff checks pass.
The first compiler/native failures and fixture repairs remain recorded in
NH_RELEASE_FAILURES.md. Combat identities remain 60/67; Polymorph is not
activated by this foundation. Next: full cast/expiry-result geometry, AI spell
selection and status feedback. Active capacity-buff/Time Stop ordering,
projected conditional-bonus interactions and clone/Phantom admission remain
explicit integration work, not silently approved targeting exclusions.
No GUI, launcher promotion, purchaser-asset or user-save mutation occurred.

Next checkpoint: native BattleForm cast effect and original-species result
projection are assigned to separate Luna workers; root owns shared safe
reversion placement and wiring/builds. The reversion helper must leave form,
HP and position unchanged if no original footprint can fit anywhere. The
round-expiry policy in that exceptional case has been asked explicitly rather
than silently extending duration or overlapping stacks. Clone/Phantom profiles
remain a foundation gap, not a permanent canonical targeting exception. Do not
activate/count Polymorph until lifecycle, random-outcome AI and presentation
are wired; detached RNG isolation alone is not expected-outcome valuation.

Cast/result checkpoint is now source/native verified: both-target build `70446`
and fixture-repair rebuild `32737` pass. Native retry `13545` executes 28/28,
zero skips, including uniform captured-category packet application, relocation
with exact HP/identity/Initiative, safe reversion/no-space non-mutation, original
army survivor counts, early-result living/undead casualty identities and gated
reserve reconciliation. Reports `UP066-cast-result-focused-retry.log`/`.xml`;
binary SHA-256 `0bff72dc620bb2d687e2bd5badd1c6ef4ff15f437eab1d2342b3c1f28a32d2c7`.
Source and fixture-repair reviews have no blocker; module/diff checks pass.
Preserve the initial 25/28 fixture failure report and repair explanation in
NH_RELEASE_FAILURES.md. The cast fixture uses real state packets and mocked
mechanics, not complete accepted hero-action/Mana accounting. Spell identity
counts remain 60/67. Next: temporary-profile support, expiry/Dispel/Time Stop
lifecycle, random-outcome AI and client form/status presentation. No GUI,
launcher promotion, user-save mutation or final artwork claim occurred.

Current bounded slice: a Luna worker owns cloned-stack form admission, retained
one-hit destruction and source-ledger-safe death/ghost cleanup, plus the canonical
Time Stop pause of form duration. A separate Luna worker owns event-driven battle
sprite replacement using the effective creature's existing animation by reference;
retain battle unit identity, facing, selection and authoritative relocation.
Root owns integration, focused validation, documentation and Git. Phantom Army's
separate Integrity/offensive-body profile and the no-legal-reversion expiry policy
remain explicit gaps; neither clone support nor sprite refresh enables Polymorph
or increases the combat-spell coverage count. No graphical acceptance is inferred.

Phantom composition decision requested: its copied offensive creature body and
separate smaller Integrity pool are not interchangeable. Ask whether Polymorph
should repartition that copied body while retaining Integrity independently, or
derive the transformed creature count from remaining Integrity. Do not silently
make a new temporary-stack targeting exclusion permanent or reinterpret HP while
that answer is pending. The distinct no-legal-position-at-expiry question also
remains unanswered. Source review additionally caught current-round Initiative
snapshot being paused with duration; the fix clears that snapshot on each round
rollover while pausing only the form lifetime during Time Stop.

Clone/presentation checkpoint verified: final both-target build `57163` passes;
native retry `39543` passes 51/51, zero skips, including unchanged CloneApply
regressions, real legacy-clone creation plus generic form packet application,
clone JSON/recast/reversion/one-hit death, Time Stop duration/Initiative behavior,
source-species results and compact status helpers. Reports
`UP066-clone-presentation-focused-retry.log`/`.xml`; binary SHA-256
`ebd913de4bb8a9f4ff5d7f726876b02910ecf97df6e55180450cbf65869dd164`.
Review and module/diff checks pass. First missing-include probe and crashed
native run, including the no-form detached-bonus fast-path repair, are retained
in NH_RELEASE_FAILURES.md. Sprite refresh is compiled/source-reviewed, not
rendered. Combat identities remain 60/67; no launcher promotion occurred.

Expected-outcome AI is the next unblocked slice: enumerate the same complete
uniform creature pool used by the runtime effect, project each form's HP/native
view and legal relocation without live RNG, and wire the mean into real spell
candidate scoring. Do not score RNGStub's middle draw as the expected outcome.
A bounded read-only Luna mapper establishes the shared API and scoring seam;
root retains architecture and assigns implementation ownership after that audit.

Expected-outcome AI dependency verified, 2026-10-01: authoritative runtime and
detached AI use the same typed complete uniform candidate pool and nearest-legal
landing positions. AI computes a signed mean of actual native offensive profiles,
retaining harmful outcomes and bypassing single RNGStub sample valuation while
preserving accepted Hero Action/Counterspell validation. Build `52390` passes
both targets; native `31943` passes 69/69, zero skips, including mixed-outcome
mean, midpoint distinction, live JSON/RNG preservation and actual selected cast.
Reports `UP066-UP068-focused-repaired.log`/`.xml`. The fixture failures and
repairs are retained in NH_RELEASE_FAILURES.md. Polymorph remains inactive:
Phantom composition and no-legal-original-footprint expiry require decisions,
then lifecycle/activation verification. Combat identities remain 60/67;
no playable promotion or rendered acceptance is claimed.
Phantom composition and exceptional no-space expiry remain unanswered.

## UP-065 — Toxic Spines does not trigger in the user's playable battle

Status: In progress, 2026-09-30. The user reports no Toxic Spines trigger,
not merely missing Poison feedback. Prioritize actual authoritative application
over further missing-feature work. Inspect the selected snapshot's perk data,
saved hero/rank eligibility, Defend/melee/reflection path and Poison packet/state
publication. Obtain the reported hero/stack/action or latest battle evidence;
do not assume an unmet condition explains the report. Reproduce with focused
native execution, fix an evidenced defect, and distinguish source verification
from updated playable delivery. Preserve the user's live game and saves.

Evidence: latest client log identifies Basic Bulwark with Toxic Spines and a
Defending stack. The active perk requires Basic, but reflectionPercent(1) is
zero, and authoritative Poison application sits behind reflectedDamage > 0.
The perk therefore has no trigger at its own acquisition rank. This requires
a design resolution, not merely a status icon. The user is asked whether Toxic
Spines should grant 25% reflection on the first qualifying Basic melee hit or
move to Advanced. Do not silently rewrite the approved reflection-based potency.
Until resolved, preserve Advanced/Expert behavior and record Basic as blocked.

## UP-064 — New Horizons main-menu title art and visible product version

Latest user delivery request, 2026-09-30: build all committed changes through
`574f0571d` locally and select that exact candidate for the ordinary Linux launch
script. Use a separate clean source checkout; preserve unfinished UP-063 edits.
Acceptance requires successful optimized client compilation, matching frozen
engine resources/content, focused validation and verified launcher selection.
Do not launch the host GUI or claim user playtest acceptance from promotion.

Local delivery completed: clean committed source
`41d44ee49a0de4592ebc59e58752ebf5c9428aa4` includes the menu commit and two
bounded delivery bug fixes. Release compilation with twelve jobs passes;
sixteen offline checks and four native query regression cases pass. Final
All for One headless smoke reaches thirty-six player turn starts through day 12
without the startup gate's forbidden errors. Its timeout is intentional (124).
Snapshot `a96183639bbc0dbad56f4e2a48a603baaa1debe62d0dbe40160926c092c946b0`
is promoted; the ordinary `play-new-horizons-linux.sh --verify-only` resolves
that exact frozen client/resources successfully. Source fixes are pushed.
No host GUI/input or user save mutation occurred in this final validation.
Menu visual acceptance remains for the user's manual test. Non-blocking AI
`Stack ammo overuse` diagnostic repetition is recorded for Phase 2, not silently
counted as a warning-free full-game acceptance.

Historical delivery gate finding (repaired below): clean Release build and fifteen focused checks pass, but
the frozen candidate's All for One headless run exited 139 during a day-2 AI
battle. Do not promote it until this crash is understood. A first GDB wrapper
incorrectly launched the executable outside the launcher's runtime asset-link
directory, producing a missing-Complete-data fatal diagnostic.
That diagnostic setup failure does not establish missing purchaser assets.
Debugger retries must preserve the runtime asset root and unset desktop display
variables to prevent error dialogs. Keep both first-run logs and do not conflate
the diagnostic setup failure with the original AI crash.

Status: Implemented (rendered/playable verification pending), 2026-09-30.
User interrupts ordinary coverage work for
these two presentation/delivery tasks; preserve the uncommitted UP-063 slice.

Inventory every main-menu title/splash variant, including Complete, Shadow of
Death and Armageddon's Blade. Replace only the edition subtitle with
`New Horizons`, matching each variant's lettering style, color and treatment;
preserve composition and other artwork. Use the HoMM3 art skill even for drafts.
Keep purchaser files intact and do not commit/distribute extracted backgrounds.
Record provenance and a portable integration strategy rather than silently
shipping original game artwork. Review at native menu resolution.

Audit earlier approximately 0.7 version labels and explain their evidenced
rationale. Establish a persistent product-version policy and one authoritative
version value, separate from the upstream engine version, save schema and Git
revision. Show the product version in native brown/yellow typography at the
main menu's bottom-left corner. Acceptance requires actual runtime bindings,
focused validation and build evidence; source edits are not playable delivery.

Inventory finds eight installed illustrations: Complete and Armageddon's Blade
each supply main, two scenario-selection, and loading art. The user explicitly
accepted using these available references; separate Shadow of Death art is not
a blocker. Eight HoMM3-skill subtitle edits and native 800×600 private compositions
exist. Only bounded generated replacement regions are runtime files; purchaser
archives and every pixel outside those regions remain untouched. Unknown source
payloads require a matching reference instead of a guessed overlay.

Historical evidence: a035100a2 introduced 0.7.0 for the saved planned perk
registry, 9e675d976 introduced 0.8.0 for the Tower roster swap, and fd0f03156
introduced 0.14.0 for reviewed biographies. These were module/content identity
epochs, not completion percentages. The current value remains 0.14.0 in the
new single authoring config; menu and module generator share it. Future tested
feature checkpoints increment minor, fixes increment patch; 1.0 remains an
accepted release boundary. Linux client compilation succeeds, nine focused
offline checks pass, and eight pixel comparisons confirm unchanged artwork
outside the subtitle rectangles. Independent review has no blocking finding.
Review repaired patch resource lookup, source CRC lookup precedence, and null
generated-image fallback; the focused source guards cover these repairs.
Actual menu rendering acceptance remains pending. The first shared-tree build
included preserved UP-063 changes and was not promoted. The separate clean
committed candidate is now delivered as recorded at the start of this entry;
unfinished UP-063 changes remain outside that selected snapshot.

## UP-045 — Implement Command Combined Arms

Status: Implemented; source/native verified, rendered/playable acceptance
pending, 2026-09-30.
UP-023 Phase 1 coverage slice.

Focus Fire grants friendly melee attacks against its designated target half
of its damage bonus. Flank grants friendly ranged attacks against its target
half of its Attack-derived damage component only, not the flat base or any
distinct-side bonuses; ranged attacks never record additional Flank sides. Preserve
fractional half bonuses until final damage rounding, ordinary Order legality,
round expiry, ownership and physical-attack restrictions. Do not grant melee
Focus Fire the shooting-only range/obstacle or Target Caller benefits. Audit
admission for melee-only Focus Fire and ranged-only Flank armies with this perk.
Direct `Unit::isMeleeAttacker` inspection confirms that ordinary shooters
already meet Flank's existing admission predicate; preserve and test that path
rather than claiming a new admission fix there.
Share exact runtime damage with previews/hypothetical AI and add the minimum
Order-selection AI hooks, legal perk progression, content registration and
focused build/native evidence. Record broad interaction and rendered/playable
verification for Phase 2; no launcher promotion.

Checkpoint: both Linux targets build (3217; final test-only rebuild 11676).
Five runtime/actual-AI cases and 37 direct Command/Focus Fire guards pass, zero
skips; content/perk/inventory passes 74/74 and mirror/diff checks pass. Exact
fractional damage, frozen cohorts, target/physical guards, legacy isolation,
authoritative submission and ranged side history are exercised. Binary SHA-256
`9100b7e059bbe7822bc1b8df362b444a95e660f672ea40864ce35dc65bac2a5d`.
Independent review has no blocking finding. Both AI fixtures explicitly isolate
other Order coefficients with legal Magic Arrow competition; all-Order ranking
and inherited Flank reachability/remaining-activation valuation remain Phase 2.
Registry coverage advances to 119/310 perks, Command 4/6 active/planned;
combat identities and ranks are unchanged. Neutral fallback is not bespoke art.
First failures and succeeding retry reports remain recorded, not overwritten.

Source delivery: commit `25bd4b08219fd9ff25cbf541a4b1c7f32bd164c1` is
pushed; local and remote branch identities match. Worktree is clean at this
source checkpoint. This is not launcher promotion or Windows package evidence.

## UP-047 — Commanding Presence recipient scope and implementation

Status: Verified (source/native; playable delivery pending), 2026-10-02.
Superseded implementation tracking: see UP-142 for canonical integration,
focused validation and pushed commit401f80384451e0522ff8df8f035901863c03025a.
The user's latest answer reconfirms the effective-benefit endpoint: negative
Morale returns when that recipient's Order benefit is spent or broken, rather
than waiting for round end. Charge consumption, Protect break/exhaustion and
Second Wind completion have focused native coverage. This repeated answer does
not require a new gameplay change or imply new playable delivery.

Implement the Advanced Command perk: friendly stacks currently affected by an
Order treat negative Morale as zero for its duration. Existing shared morale
calculation supports a zero floor; canonical Order states and detached AI do
not yet supply this perk. Include authoritative activation, UI-visible morale,
detached forecast and minimum Order valuation, registration and focused tests.
The floor applies only to covered recipients (such as Protect's pair or Second
Wind's selected stack, versus eligible troops for army-wide Orders), never an
unconditional whole-army aura. The former pending scope/lifetime questions are
resolved; do not reopen them solely because this historical entry was stale.

## UP-048 — Deterministic Diplomacy foundation

Status: Planned; runtime, AI/UI and independent policy maps complete;
map-authored free-join clarification pending, 2026-09-30.
UP-023 Phase 1 foundational coverage slice; no activation claimed.

Audit and implement the canonical neutral-joining rule: Basic/Advanced/Expert
thresholds of 25/50/75% of the hero's current Army Value, normal recruitment
Gold, and explicit hostile/scripted exclusions. Preserve authoritative
validation, map intent, legacy rules, and Leadership-safe admission. Preserve
the existing accepted-join/garrison lifecycle until its remainder semantics
are explicitly redesigned; do not silently introduce a partial-neutral
persistence rule. Share deterministic willingness/cost/threshold
forecast with encounter feedback and minimum adventure-AI use; do not consume
RNG during inspection. Include registration, ordinary progression, focused
native/build evidence and deferred integration findings. Negotiator, Common
Cause and Grand Diplomat can use the same threshold foundation if their exact
paths are clear; other Diplomacy perks remain separate missing requirements.
Do not invent eligibility, overflow or map-authored joining semantics if the
existing source and canonical design leave a material conflict unresolved.

Read-only evidence: `CGCreature::takenAction` still uses legacy disposition,
perceived strength and randomized initial aggression. Raw `getArmyStrength()`
is the existing creature-AI-value sum closest to canonical Army Value.
`getPerkState()` already exposes captured rank activation for old-save gating.
`HOSTILE` and `SAVAGE` seed disposition, not an explicit joining prohibition;
an explicit eligibility flag can avoid repurposing them. Script-controlled
visits already bypass ordinary decisions. `COMPLIANT` supports authored free
joins, so the user is asked whether these remain exceptions or also use the
new paid threshold. No rank/perk is activated pending that decision.

The shared pure forecast should serve visit feedback, permitted popup details
and `AIGateway::showBlockingDialog`. AI must check Gold and legal usable
admission. Existing joining percentages and full-stack pricing need an explicit
implementation audit. `tryJoiningArmy` schedules neutral removal after accepted
joining and provides a garrison for remaining troops; current tests transfer
the remainder before closing, not preservation after dismissal. This is a
separate lifecycle finding, not permission to invent a new gameplay rule.

## UP-049 — Implement Wisdom Mysticism daily Normal-Mana recovery

Status: Implemented; source/native verified, rendered/playable acceptance
pending, 2026-09-30.
UP-023 Phase 1 coverage slice.

At each day start, Mysticism restores the greater of 5 or 10% of normal
Maximum Spell Points. Restore only missing Normal Spell Points, leaving Buffer
unchanged. Reuse the existing daily authoritative recovery and shared forecast,
not an update/render scan. Gate by the hero's captured active perk, preserving
legacy and planned snapshots. Require registration, ordinary selection/help,
focused native daily-path and arithmetic checks, build and independent review.
Track rendered/playable acceptance and broader interactions separately.

Checkpoint: Mysticism now raises existing daily regeneration to at least
`max(5, floor(normalMaximum / 10))`, without adding a second refill. The shared
getter and authoritative daily `SET_NORMAL` preserve Buffer and capacity caps;
Mage Guild rest and stronger regeneration retain precedence. Captured active
selection and current Wisdom rank gate the effect; no new saved field, packet,
scan or scheduler. Generic AI acquisition and daily application use existing
paths; strategic acquisition ranking remains deferred.

Linux client build 55027 and final test build 92352 pass. All six Mysticism
cases plus 30 direct capacity/pool guards pass together (36/36, zero skips),
including real NewTurn packet application, Wizard perk-offer selection,
selection/save-load, planned snapshot, rank loss, floor/cap and Buffer checks.
Binary SHA-256 `0b565de19b837c0f2a3bc476c59009f61c99f570ba15c507d3737df7912be080`.
Offline content/perk/inventory passes 74/74; module and diff checks pass.
Independent review has no blocking finding. Initial fixture failures remain
recorded. Coverage becomes 120/310 active perks, 190 planned, Wisdom 2/8
active/planned; ranks and combat identities are unchanged. Bespoke art is
Not done; neutral fallback is not artwork. No launcher promotion.

Source delivery: commit `c03505830` is pushed to `origin/definitive-mvp`.
The validated working-tree source is recorded separately from playable delivery;
no Windows package or promoted Linux snapshot containing this perk is claimed.

## UP-050 — Implement Wisdom Prepared Caster

Status: Implemented; source/native verified, rendered/playable acceptance
pending, 2026-09-30. UP-023 Phase 1 slice.

The first hero spell in each combat costs 2 Mana less after Wisdom's percentage
discount, minimum 1. Use `CBattleInfoCallback::battleGetSpellCost`, preserving
ordinary spell variants and later battlefield modifiers. Adventure costs stay
unchanged. `CGameInfoCallback::getSpellCost` already routes active combat to
this callback, including ordinary spellbook previews; do not create a duplicate
client cost formula.

Existing per-round `castSpellsCount` and StartAction `usedSpellsHistory` cannot
represent the first accepted combat-lifetime hero cast. Track its completion
at `BattleSpellCast`, excluding creature casts and rejected requests, retaining
accepted resisted/countered casts. Preserve state across rounds and save/load,
copy/update it in hypothetical AI, and expose a shared read-only cost predicate.
Do not consume the discount merely by opening a preview or evaluating AI.
Root owns the exact generic state/API contract and serialization integration
before workers edit distinct runtime/AI files. Require registration, ordinary
progression/help, focused principal native/build and detached-cost evidence.
No rule ambiguity was found. Bespoke art and rendered/playable acceptance remain
separate, explicitly unverified requirements.

Root contract: generic per-side `heroSpellCastCompleted`, read through
`hasCompletedHeroSpellCast`, commits only after accepted hero casts and is
versioned with old-load false and a downsave loss guard. Hypothetical state
copies the marker and receives a generic completed-hero-cast notification
after a target-valid hero projection; live state remains untouched. Existing
StartAction history is deliberately not repurposed. Runtime owns shared state,
cost, acceptance, serialization and its native fixture; AI owns detached state
and its separate fixture; root owns registration, test wiring, builds and Git.

Checkpoint: both Linux targets build (55809; final test-only rebuild 56500).
All ten new runtime/actual-AI cases pass, zero skips. They exercise authoritative
first/later costs across rounds, unchanged Overcharge surcharge, cost floor and
battlefield ordering, rejected/creature exemption, legal Wizard perk selection,
captured planned exclusion, current/old/downsave state, copied/nested/round AI
state and actual evaluator submission without live-state preview mutation.
The 31-case expanded run passes 30/31: the ten new cases plus 20 existing guards;
one unchanged v2 synthetic fixture fails setup on v3-only `selectedPlacement`.
Record that fixture migration for Phase 2; keep its failing report. The new
ten-case rerun exits successfully. Binary SHA-256
`ea8e481c14da2395f288408bece79ae470d0d2ad9534398c57e1bb37f5e815a0`.
Offline content/perk/inventory passes 74/74; mirror/diff checks pass.
Review has no blocking production finding; compile and initial-round fixture
failures are retained in the failure ledger. Coverage is 121/310 active perks,
189 planned, Wisdom 3/7 active/planned. Dedicated Adventure exclusion, broader
interactions and old-save fresh-discount behavior remain Phase 2. Bespoke art
is Not done; no rendered/playable acceptance or launcher promotion is claimed.

Source delivery: `2b5a843d7d10ae68f8e53d40ee962fb27f4f72b9` is committed
and pushed; remote identity is verified and the worktree is clean at that
checkpoint. Full Windows run `36680827103` is queued on this frozen source,
including Combined Arms, Mysticism and Prepared Caster. Dispatch is not
compile/package or Windows graphical evidence; preserve the live handle.

## UP-051 — Implement Wisdom Meditation daily recovery

Status: Implemented; source/native verified and pushed, playable acceptance
pending, 2026-09-30.
UP-023 Phase 1 slice, after Prepared Caster's committed native checkpoint.

Canonical Advanced Meditation: ending the day with at least 25% of maximum
Movement unspent restores an additional 15% of normal Maximum Spell Points.
The day-start mana update is authored before Movement is refreshed:
`NewTurnProcessor::generateNewTurnPack` calls `updateHeroesManaPoints` before
`updateHeroesMovementPoints`, and both inspect the previous day's hero state.
Use the existing `getManaNewTurn`/`SET_NORMAL` recovery path, not polling or a
new day scheduler. `movementPointsLimit()` already selects the current land or
boat layer. Use overflow-safe threshold arithmetic and floor the percentage;
add recovery to ordinary regeneration, cap missing Normal, preserve Buffer and
Mage Guild full-refill precedence. Gate captured active selection/current rank.
First-day and tavern callers are mapped: day zero has no completed day and must
not grant Meditation. The tavern pool currently refreshes Movement before
computing mana; preserve the previous Movement for this check by computing mana
first, and pass completed-day context from `NewTurn` (`pack.day > 1`). On-map
updating can pass the pre-update calendar context explicitly. Do not add a
serialized day marker or infer completion from the already incremented date.
Tavern bonus expiration also precedes ordinary recovery: snapshot the previous
Movement maximum before expiration, then pass it to the shared recovery getter.
Preserve legacy bonus-expiration/recovery ordering; do not add a saved snapshot.
Do not claim a day-end mechanic solely from a pure regeneration getter test.
Require legal Advanced progression, exact threshold/below-threshold checks,
authoritative daily packet evidence, save/selection gating and focused build.
AI heroes use the same passive daily path; strategic Movement reservation can
be deferred explicitly rather than inventing a new mandatory AI behavior.

Checkpoint: client build 35691 links; confirming build exits zero. Test build
88236 passes and native 84667 passes five new cases plus 22 direct capacity
guards, 27/27, zero skips. Binary SHA-256
`280e5b226f1cb9fb651e64ad0fc9067581c25c4c25793729d01d495054c99530`.
Retained reports: `NewHorizonsMeditation-capacity-guards.log`/`.xml`.
Offline 74/74 and mirror/diff checks pass; independent review has no blocker.
Coverage is 122/310 active perks, Wisdom 4/6 active/planned. Neutral fallback
is not bespoke art; rendered/playable acceptance and broad interactions remain
open. No launcher promotion or Windows package evidence for this slice.

Source delivery: `d023766f9beee766a9d4907bbb9f1add17a5dfc0` is pushed;
local and remote identities match, with a clean source checkpoint.

## UP-052 — Implement Wisdom Deep Knowledge bonus-roll chance

Status: Implemented; source/native verified and pushed, playable acceptance
pending, 2026-09-30.
UP-023 Phase 1 slice after Meditation's focused checkpoint.

Canonical Advanced Deep Knowledge adds ten percentage points to Wisdom's
chance of granting +1 Knowledge on level-up. Trace the existing independent
Skill-derived bonus rolls; change only the Wisdom roll's chance for a captured
active selected perk/current rank. Do not change fixed twenty-point class
growth, other Skills' rolls, +1 amount, RNG draw ordering, or legacy rules.
Require ordinary Advanced perk selection, shared probability/help where used,
focused deterministic chance/authoritative growth evidence, and registration.
Reuse existing growth infrastructure; no new saved counter is implied.

Read-only map: `CGHeroInstance::getPrimaryGrowthView` supplies the same
opportunities to `GameRandomizer` and `HeroGrowthWindow`. Increase only its
existing Wisdom row by ten points when the captured active Advanced perk is
selected: Advanced 20→30%, Expert 30→40%. Preserve row order and draw count.
Primary rolls precede the level-up perk query, so a newly chosen perk affects
subsequent rolls, not the already-applied roll. Automatic AI growth uses that
shared path; acquisition preference remains a separate strategic concern.

Checkpoint: client retry 98557 and test build 8638 pass; native retry 96534
passes four new cases plus nine direct growth guards, 13/13, zero skips.
Binary SHA-256 `c9b9cdfd304e9b9db3ef679da3d3d13352a73af892f519d88084d97c3dccac88`.
Reports `NewHorizonsDeepKnowledge-retry1-growth-guards.log`/`.xml` retain
separate first-failure evidence. Review has no remaining blocker; offline
74/74 and mirror/diff checks pass. Registry coverage is 123/310, Wisdom 5/5.
Strategic AI acquisition, broad interactions, bespoke art and rendered/playable
acceptance remain deferred; no launcher promotion.

Source delivery: `a827bbb7b9faa3980a91b381b8da3a86dcdc4bf5` is pushed;
local and remote identities match with a clean source checkpoint. The running
Windows build 36680827103 remains frozen at Prepared Caster `2b5a843d7` and
does not include Meditation or Deep Knowledge. Do not equate it with this
source delivery or restart it solely because newer commits exist.

## UP-053 — Implement Wisdom Arcane Reservoir capacity perk

Status: Implemented; source/native verified and pushed, playable acceptance
pending, 2026-09-30.
UP-023 Phase 1 slice after Deep Knowledge. This Expert perk is distinct from
the Tower building of the same name: it adds 25 Maximum Normal Spell Points,
not Buffer, and does not refill current Mana. Add the flat amount after the
Knowledge/Intelligence calculation in the existing New Horizons `manaLimit`
branch, with overflow-safe saturation and captured active/current rank gating.
All ordinary capacity readouts, restoration and AI capacity estimates share
that method. Perk selection already invalidates capacity reconciliation;
rank loss must use the existing event-driven clamp and preserve Buffer.
Require legal Expert selection, no refill, capacity/rank/save/planned guards
and focused build/native evidence. No additional saved counter or polling.

Checkpoint: client 7727 and test build 86291 pass; native 40452 passes four
new cases plus 27 direct capacity guards, 31/31, zero skips. Binary SHA-256
`4c55d6c999d3a0e64d6982e5403e4f182f5ff6d89f78614a82e2b390e141c3b3`.
Reports are `NewHorizonsArcaneReservoir-capacity-guards.log`/`.xml`.
Offline gates pass 74/74 and mirror/diff checks pass; review has no blocker.
Coverage is 124/310, Wisdom 6/4 active/planned. Overflow saturation is reviewed
but not separately reached within validated fixture limits. No bespoke art,
rendered/playable acceptance, promotion or new Windows package is claimed.

Source delivery: `bccb3bd16d33317db7f5c4a1be64a695a4e09a5b` is pushed;
local and remote branch identities match with a clean source checkpoint.

### 2026-09-30 Windows Prepared Caster checkpoint

Preserved full run `36680827103` now completes successfully on frozen source
`2b5a843d7d10ae68f8e53d40ee962fb27f4f72b9`. Package artifact `11082744152`,
`New-Horizons-Windows-x64-2b5a843d7d10ae68f8e53d40ee962fb27f4f72b9`,
is 750666994 bytes and unexpired at verification. Preflight `11081934464` and
selected-CRT report `11082600293` also exist. This supplies Windows build/package
evidence for Combined Arms, Mysticism and Prepared Caster, not the newer
Meditation, Deep Knowledge or Arcane Reservoir source. No Windows graphical
acceptance, release publication or launcher promotion is inferred.

## UP-054 — Implement Wisdom Arcane Memory accepted scroll learning

Status: Source reviewed and focused native verified; activation blocked on
neutral Adventure acquisition policy, 2026-09-30.
UP-023 Phase 1 candidate after Arcane Reservoir. A genuinely scroll-sourced
accepted cast permanently teaches its spell only if current School acquisition
rules permit it. Do not learn from spellbook/tome sources, failed casts, removed
spells or a merely carried unused scroll. Ordinary scrolls are reusable; the
canonical rule does not consume them. Prefer permanent non-scroll sources over
scrolls, and reusable scrolls over charged artifacts. Capture actual scroll
identity before effects, then use authoritative `ChangeSpells`
and existing `canLearnSpell`. Both combat and ordinary adventure casts need
coverage; preserve external-caster behavior. `CSpell::adventureCast` already
returns a result, but `CGameHandler::castSpell` currently ignores that return
before attempting discharge. The Boolean is not completion evidence: the
mechanics return true for CANCEL and PENDING as well as OK; town-choice queries
call `performCast` later. Map a genuine accepted completion hook before
settling charges/learning, including canceled and deferred selections.
No new saved counter: learned spells already persist. Confirm these event
boundaries with focused native/build evidence, including rejected adventures.

Architecture decision: add a generic successful-adventure-cast notification to
`SpellCastEnvironment` (`lib/spells/ISpellMechanics.h`), with a default no-op
for non-authoritative environments. Notify only in `performCast`'s successful
effects branch after Mana/end-cast processing. `ServerSpellCastEnvironment`
excludes external casters and delegates to the existing shared
`useChargeBasedSpell` handler. That handler can capture true scroll provenance,
discharge only actually charged artifacts, then learn through `ChangeSpells`
when eligible without consuming an ordinary reusable scroll. Remove the
unconditional charge call from `CGameHandler::castSpell`; combat already calls
the same handler after its accepted hero cast. The ordinary `CastAdvSpell`
visitor bypasses `CGameHandler::castSpell`, so completion notification must
cover that path too. Test ordinary success, failed effects, cancellation,
PENDING/valid reply and source priority; no new persisted marker or netpack.

Review checkpoint: the first runtime slice builds successfully (client session
10614); 74 focused offline content tests and module/diff checks pass. This is
not final UP-054 verification. Review found a blocking source-provenance defect:
Town Portal can visit a Guild and learn its spell before completion rescans
sources, substituting a newly acquired book source for the cast's actual source.
Capture a settlement
callback before effects inside `performCast`, after any pending selection has
resolved, and invoke it only on successful completion. Avoid mutable pending
state in the environment and preserve permanent non-scroll source priority.
The runtime worker repaired this before native verification. The frozen
six-file runtime now captures the exact artifact instance and re-resolves it
at successful settlement. The repaired client rebuild (57887) succeeds.
Test retry 28356 succeeds; native 94687 passes 4/6 with zero skips, exposing
the incorrect charge-only assumption for reusable scrolls and a second Haste
fixture rejection. Correct source classification and reusable-scroll
expectations, preserve charges only where authored, and recheck active rank
and learning eligibility. Review/build/native retry evidence is pending;
do not close this item or count it verified. Failure evidence is retained in
`NH_RELEASE_FAILURES.md`.

Acquisition clarification pending: neutral Adventure Spells require no School
rank, but the specification separately describes fixed Guild unlocks. The user
has been asked whether Arcane Memory can permanently learn these spells from
reusable scrolls or applies only to school combat spells. Do not silently
reinterpret that exception. Charge-lifecycle implementation can proceed while
the answer is pending. The canonical artifact section deliberately excludes
the four legacy elemental Tomes from random loot until six-school replacements
are authored. A synthetic matching Tome bonus tests generic permanent-source
priority only; it does not prove a shipped six-school replacement or expose an
unintended remapping bug.

Final provenance repair builds both client/test targets (4257). Native retry
53830 passes all nine feature cases and two direct guards, 11/11, zero skips.
Binary SHA-256: `7efa81f126a237daaf9a48bb0e47382b1de7aa9e26036a8e2de86df7f272b9bc`;
reports: `NewHorizonsArcaneMemory-provenance-retry2-focused.log`/`.xml`.
The exact legacy scroll bonus marker now resolves to matching equipped instance
IDs without changing saves. Ordinary scrolls remain reusable. Review has no
blocking source finding. Keep the production registry planned until the pending
acquisition choice is resolved; positive tests explicitly activate the feature.
Final dormant-registry client/test build 89441 succeeds; native retry 18008
again passes 11/11, zero skips. Final binary SHA-256:
`1928e181a8d676e4e9fcf8a0c5dceff75c7c8c0f194de4d963fb6f1f1d7f7002`.
Reports: `NewHorizonsArcaneMemory-dormant-policy-final-focused.log`/`.xml`.
74/74 offline gates, module mirror and diff checks pass. Final independent
activation review has no blocker. No completed-perk coverage increase or
playable delivery is claimed. Advance an unblocked queue item.

Source checkpoint: `1f8177b97a5bcc81ff0fbe6b6846088c4deee770` is pushed;
local/remote identities match and worktree is clean. Full Windows run
`36691148552` was observed queued on this exact source, not yet successful.
No launcher snapshot or live game profile was changed.

## UP-055 — Implement Wisdom Archmage

Status: Implemented; source/native verified, playable acceptance pending,
2026-09-30.
UP-023 Phase 1 candidate after UP-054. The first accepted Level 4 or Level 5
combat spell in each combat costs 3 additional Mana less after Wisdom's
percentage discount, minimum 1. Lower-level spells, rejected requests and
creature casts must not consume its eligibility. Preserve Prepared Caster
stacking, ordinary battlefield modifiers and separate Overcharge surcharges.
Share the exact cost and completed-cast history with UI and hypothetical AI,
persist combat state with append-only compatibility, and gate by captured
active selection/current Expert rank. Include registration, legal progression,
focused native/build evidence, and recorded Phase 2 interactions. Read-only
mapping may proceed while Arcane Memory's focused test build runs; do not edit
production or change verified coverage during that build.

Map: append generic completed-level history to `SideInBattle`, exposed through
real/proxy/hypothetical battle state. Exact saved levels 4 and 5 share one
Archmage discount; never use the global spell's legacy level or `>=4`.
Authoritative accepted packets and detached accepted-cast callbacks record the
saved level. Extend the shared battle-cost getter after Wisdom/Prepared Caster,
before battlefield modifiers, and append serialization with old-save defaults
and loss-aware down-save protection. Existing runtime/AI fixtures are registered.
Implementation ownership is split: runtime owns generic completed-level state,
serialization, shared cost and actual-cast tests; AI owns detached state/callback
and its focused projection tests. Root owns activation/data, builds and Git.
Use an exact levels 1–5 mask, shared by all consumers, not an Archmage-only flag.
Existing `usedSpellsHistory` is written at cast start, so it cannot substitute
for this accepted-completion history. No activation/verified count is claimed
before the focused gates; preserve all unrelated changes.

Checkpoint: client/test crash-repair build 22317 succeeds; final test-only
build 13005 succeeds. Native 18779 passes 21 runtime/AI cases plus three direct
Time Stop/Pursuit guards, 24/24, zero skips, on binary
`8e2222981acf90654d38166321ece81af245860deaf55a38680af0cc10dece52`.
Reports: `NewHorizonsArchmage-score-retry4-focused.log`/`.xml`.
Legal Expert offer, shared discount/floor, lower-level preservation, accepted
Level 4/5 history, creature/rejected exemption, append-only save compatibility,
nested detached copies and actual evaluator submission pass. A real stale-dead
unit request admission hole is repaired before StartAction; its regression and
living/Time Stop/Pursuit guards pass. Earlier failed/crashed attempts remain in
the failure ledger. Offline gates pass 74/74, module/diff checks pass, independent
review has no blocking finding. Coverage is 125/310 active perks, Wisdom 7/3;
ranks and combat identities unchanged. Broad lifecycle/countering interactions,
full save-world journeys, artwork and playable acceptance remain deferred.
No launcher promotion or GUI run. Next unblocked item: UP-058.

Source delivery: `fffd9b81329e06bda04ec48d2253f5f4a890e0ab` is pushed;
local/remote identities matched with a clean checkpoint. Full Windows run
`36697665400` is queued on that frozen source, not yet a successful package.
The previous full run `36691148552` succeeded on `1f8177b97`; its package
artifact `11087514647` is 750678892 bytes and unexpired. That package includes
the dormant Arcane Memory seam, not Archmage, and neither run establishes
Windows graphical acceptance or Linux launcher promotion.

## UP-056 — Complete canonical Adventure Spell effects

Status: Partial; Summon Boat existing-only clause source/native verified,
2026-09-30. Remaining Adventure Spell effects and required targeting UI are open.
UP-023 Phase 1 functional gaps, not merely Phase 2 hardening. Guild acquisition
is implemented for all five spells; none is yet certified effect-complete.
The source audit finds these remaining canonical clauses:

- Summon Boat existing-only creation policy is now implemented in the
  authoritative effect and AI; adjacent legal target selection/preview remains.
- Water Walk already uses the shared 1.5x step multiplier; end-day land legality
  remains unestablished in the mapped authoritative turn/movement path.
- Town Portal must use the nearest controlled town, never a player-selected
  destination, and exhaust remaining Movement. Current Advanced/Expert effects
  permit selection and subtract fixed legacy Movement instead.
- Fly already uses the shared 1.5x multiplier and ordinary landing rules;
  scenario-protected barrier enforcement remains unestablished.
- Dimension Door requires a visible legal tile within eight tiles, protected
  barrier enforcement, and exhausted Movement. Existing effects use a legacy
  rectangle, lack a mapped visibility/barrier guard, and subtract fixed Movement.

Share legality/result policy with client targeting and AI; no frontend-only
fix or polling. Root must inspect the existing deterministic nearest-town
distance/tie-break rule rather than infer that the specification demands a new
expensive route scan. Protected-barrier metadata and occupied-nearest-town
semantics need evidence or clarification before inventing behavior. The forced
Advanced Town Portal query in UP-054 is generic completion compatibility
coverage, not canonical New Horizons nearest-town/movement acceptance.
2026-09-30 checkpoint: shared caster-aware policy blocks creation under captured
New Horizons Adventure rules, forces existing-boat retrieval and rejects no-boat
casts before the adventure packet, Mana payment or daily completion. Legacy
Expert creation remains unchanged. Actual Nullkiller path generation cannot
forecast creation but can summon a known available boat. Client build 54426 and
test build 61522 pass; native 83331 passes 13/13, zero skips (five new cases,
eight direct Adventure registration/state/AI guards). Binary SHA-256
`a674e4a67a73b5cf18357ddbf4b1fafedad87fa8cc43df01eff666b69b5bc79b`;
reports `UP056-summon-boat-existing-only-initial-focused.log`/`.xml`.
All 77 offline checks and module/diff gates pass; independent review finds no
blocker. Deferred: occupied/multiple boats and nearest ties, direct packet/
completion observer assertions, broader interactions and rendered/playable
acceptance. Required adjacent-target selection/preview remains Phase 1 work,
not deferred polish. No GUI/profile/launcher promotion. Other Adventure design
ambiguities remain unresolved; identity/rank/perk coverage does not increase.

Town Portal policy map complete: existing squared planar distance and strict
first-entry tie-break are deterministic; no route scan is required by the
specification. Preserve occupied-nearest cancellation, without silently choosing
a farther free town. Effect and AI currently enumerate different candidate pools
and independently resolve distance, so share the policy/resolver instead.
Keep canonical gating in saved `isAdventureSpell` rules, not global mastery JSON;
Reinforcements uses the same base effect and must remain unchanged. The client
only renders the requested generic picker, so eliminating the canonical query
requires no new client-owned destination logic. AI must also predict zero
remaining Movement. The user is asked whether controlled means owner-only or
team towns, and whether any positive Movement permits casting instead of the
legacy 200/300 minimum. Do not silently choose those semantics. Archmage UP-055
is the next unblocked implementation while answers remain pending.

## UP-057 — Implement Chaos Hand of Fate

Status: Implemented; focused source/native verified, playable delivery pending,
2026-09-30.
Both Linux targets build (90769 final incremental gate). Native 54761 passes
17/17, zero skips: six Hand of Fate runtime cases, accepted/read-only AI cast,
eight current Holy Wrath cases and two existing AI guards. Binary SHA-256
`3ac2c0c602cb277c228164144ff86b2d448257b45cac526294c72cccdd7c09fd`;
reports `UP057-hand-of-fate-isolated-ai-retry5-focused.log`/`.xml`.
All 77 offline checks, module check and independent principal-path review pass.
Coverage is 59/67 combat identities, Chaos 5/11. See the failure ledger for
preserved initial failures and Phase 2 findings. Bespoke art remains Not done;
no GUI/profile/snapshot promotion occurred.
UP-023 Phase 1 missing combat identity. Canonical detailed roster controls over
the abbreviated table: primary damage is `70 + 2.5 * SP`, with ordinary saved
School/Spellcraft scaling on the SP term. After the primary hit, use actual HP
lost, not attempted damage or overkill. Choose one other surviving stack
uniformly, with friendly and enemy stacks equally eligible, and inflict half
that actual loss. Do not filter the random choice by resistance, immunity or
tactical value; the primary target is excluded. With no other surviving stack,
there is no secondary hit. Respect ordinary target/casting legality and share
expected collateral valuation with detached AI without consuming live RNG or
state during inspection. Register the spell, expose existing casting/preview/log
hooks, preserve legacy saved-roster isolation and validate principal actual/AI
paths. No bespoke art or completed effect is claimed by a placeholder binding.
The shared mapping is complete. The existing
damage script returns actual HP-clamped loss and supplies the post-hit pool;
detached AI needs expected collateral value rather than one RNG-stub recipient.
The user approved applying the secondary recipient's own magical defenses to
half the primary actual loss. This does not influence selection or permit a
reroll. The asynchronous answer received on 2026-09-30 explicitly confirms
"Apply the recipient's own magical defenses"; no change to the implemented
behavior is required. The clarification is integrated into the detailed canonical section
and its abbreviated table; Pending Changes records the integration. UP-058 and
UP-059 admission corrections are source/native verified; this missing combat
identity now has focused runtime and actual AI evidence.

Windows full run `36710097476` succeeds on frozen Hand of Fate source
`8473b53e169067315fbd5f637182f76ccb6d28e1`. Package artifact `11096561868`,
`New-Horizons-Windows-x64-8473b53e169067315fbd5f637182f76ccb6d28e1`,
is unexpired (750709876 bytes). It excludes subsequent Summon Boat and
Misfortune changes and does not establish Windows graphical acceptance.

## UP-060 — Implement Chaos Fate Dealer

Status: Planned; sampling-policy clarification requested, 2026-09-30.
UP-023 Phase 1 slice after Hand of Fate. Advanced Chaos draws two random spill
targets; if exactly one is hostile, use it, otherwise randomly choose a draw.
Clarify whether draws are independent with replacement and whether “legal”
retains Hand of Fate's defense-unfiltered pool before implementing a materially
different selection distribution. Require captured active-perk/rank admission,
runtime selection, matching read-only AI expectation, normal perk progression,
registration, focused native/build evidence and recorded deferred interactions.
Root owns registration/docs/builds; read-only policy worker owns the bounded map.
No bespoke art, production activation or playable completion claimed.
The user is asked whether the two draws permit duplicates (as Blinkmaster
explicitly does) or must name different stacks when available. These produce
different hostile-selection probabilities; do not silently choose one.
Read-only map settles the pool: reuse Hand of Fate's other living on-field
non-turret stacks, including protected stacks; defenses apply only after final
selection. “Legal” does not override the detailed no-defense-filter rule.
Blinkmaster code's with-replacement policy is precedent, not explicit canonical
evidence for Fate Dealer's sampling distribution.
Continue UP-056's unambiguous existing-boat-only correction meanwhile.

## UP-061 — Complete Chaos Misfortune and Misfortune Weaver

Status: Unambiguous probability foundation implemented and source/native
verified; innate-resistance scope and playable acceptance pending, 2026-09-30.
UP-023 Phase 1 foundational probability-debuff gap. Current Misfortune is legacy
-1/-2 Luck with single-stack targeting; canonical requires positive Luck cannot
trigger, duration `min(4, 2 + floor(SP / 80))`, favorable random creature-effect
probabilities multiplied by `max(25%, 75% - 0.25% * SP)`, and deterministic
abilities unchanged. Basic Chaos Misfortune Weaver reduces that multiplier by
ten percentage points, retaining the 25% floor. Introduce a shared timed
representation and explicit creature-chance consumers with matching AI hooks;
do not globally reduce unrelated RNG, hero effects, negative Luck or deterministic
abilities. Preserve captured legacy rules, status expiry/Dispel and ordinary
registration/progression. Root owns API/ownership partition and final gates.
Require focused authoritative casts/chance/Luck/expiry and detached/actual-AI
evidence; record unverified interaction classes for Phase 2. Weaver is active
and principal-path verified; full effect-complete/playable delivery is not claimed.
Runtime and AI workers own distinct files. The shared basis-point helper and
timed Luck-cap representation are implemented; Death Blow, attack-triggered
spells, destruction/transmutation and Death Stare are explicit consumers.
Hero-owned machine bonuses and harmful Fear remain unchanged. Whether innate
creature Magic Resistance is also a favorable probability is awaiting the
user's scope decision; mixed hero/aura resistance must not be blanket-reduced.
Canonical Misfortune's missing subtraction symbol is repaired from its own
20/100/200-SP examples, without changing the intended formula.

Checkpoint: both Linux targets build; final rebuild 84281 succeeds. Native
42389 passes 25/25, zero skips (18 new cases plus seven direct guards), binary
`01f92c0564da87a2d21e2a471f692f2f95c6af4ce86df7370dbddcba9589629e`.
Reports `UP061-misfortune-expiry-retry2-focused.log`/`.xml`. Actual casts,
Weaver floor/scaling, Death Stare, legal Dispel/round expiry, negative Luck,
v2 isolation, shared state serialization/downsave, spell help and legal AI
submission pass; forecasts leave live RNG/Mana/HP untouched. All 77 offline
checks and module/diff gates pass; independent review has no remaining blocker.
Failure ledger retains compile/fixture errors and the fixed permanent-marker
production defect. Coverage increases to 126/310 active perks, 184 planned,
Chaos 2/8; identities 59/67 and ranks 84/93 are unchanged. Phase 2 includes
full proc-family AI valuation, direct fractional seeded roll and new-marker
Sylvan/Perfect Moment execution, custom-specialty and full world-save journeys.
Dedicated art remains Not done; no GUI/profile/snapshot promotion.

Source delivery: `63431ceb3cc0e216f9aff9785445e522fab7cddf` is committed and
pushed; remote identity matches and the source checkpoint is clean. Full
Windows run `36719626047` is in progress on that frozen source, including the
later Summon Boat clause and this Misfortune foundation. Preserve the live run;
dispatch does not establish compile/package or graphical acceptance.

## UP-063 — Implement Shield of Chaos and Paradox Shield

Status: Verified (delivery pending), 2026-09-30.
The preceding answer-only turn verified an already-recorded Hand of Fate
decision; it did not increase implementation coverage. Resume the next unblocked
UP-023 Chaos identity rather than wait on Berserk's pending Morale decision.
Shield of Chaos targets one friendly or enemy stack for two rounds, applies
-10 Morale and -10 Luck, and independently reduces physical and magical damage
by min(80%, 50% + 0.15% × Spell Power). Preserve fractional precision and the
saved School/Spellcraft scaling of the Spell Power term. It is damage reduction,
not magic immunity or resistance to non-damaging effects. Expert Paradox Shield
adds ten percentage points to both reductions without changing the penalties.
Audit the interaction with the canonical global physical reduction cap before
claiming the perk. Reuse timed effects, authoritative mutation, saved-roster
admission and detached AI; do not create polling or bypass casting validation.
Acceptance: registered spell/perk and principal real casting/damage paths,
friendly/enemy targeting, two-round lifetime, defenses distinct from spell
immunity, fractional coefficients/caps, meaningful read-only AI valuation,
focused native tests, successful builds and independent correctness review.
Record broader integration findings for Phase 2 and bespoke art as Not done
until an authored asset exists. Source verification is not playable delivery.

User clarification: retain the existing 80% total physical cap. Paradox's ten
points are added after the spell's own base cap; magical protection can reach
90% under its ordinary 95% total cap. This is integrated into the canonical
section and Pending Changes history. Runtime and signed AI source edits are
reviewed without a blocking finding; builds/native verification remain pending.
All 78 offline checks pass after the activation inventory correction. Deferred
AI exposure/recast forecasting findings are recorded in the functional matrix.

Final continuation checkpoint: both Linux targets build (`41010`); isolated
native `61362` passes 13/13, zero skips, including accepted friendly/enemy AI
casts, live-state/RNG preservation, fractional damage and caps, refresh/expiry,
Dispel and bonus serialization. Reports `UP063-shield-final-retry3-focused.log`
and `.xml`; 76 focused content/perk checks and module/diff gates pass.
Final independent Astra review finds no blocker. Coverage advances to 60/67
combat identities and 127/310 active perks. Existing launcher selection remains
the clean committed menu/delivery snapshot; this slice is not promoted and no
rendered acceptance is claimed. Next missing Chaos identity: Polymorph; preserve
original army species/casualty accounting while implementing its battle-local
same-tier form, exact aggregate HP, two-round reversion and detached AI.

## UP-062 — Complete canonical Berserk and Frenzied Curse

Status: Partial; targeting foundation source/native verified, 2026-09-30.

The preceding answer-only turn confirmed an already-recorded Hand of Fate
decision and made no implementation progress. Current source is revalidated
clean at `c66a4f6ab`; Windows run `36719626047` is confirmed live and preserved.
Two Luna workers now own disjoint shared-callback/test and BattleAI/test files;
root owns authoritative tie selection, activation regression tests and integration.
This checkpoint corrects melee-only shooters, equal-cost target enumeration,
server-only random tie selection, empty-target safety and exact AI forced movement.
It does not resolve the pending negative-Morale/one-activation lifecycle decision,
activate Frenzied Curse, or certify all-blocked approach behavior. Completion
evidence is recorded below after build and focused execution, not inferred from edits.

Checkpoint: v3 shared candidates force melee, use path cost and retain uniform
target ties; the server alone draws the actual target and supplies the defender's
side on forced WALK. Empty sets are safe; legal-target filters prevent rejected
invincible/hostile Sanctified primaries. Legacy shooters and singleton first-nearest
melee are retained. Detached AI movement/no-action and signed tied expectation
work, and the legal AI cast is accepted without forecast mutation of RNG/Mana/HP.
Both Linux targets build; final build `27932` and native `9314` pass 21/21,
zero skips (nine callback, two activation, four AI and six profile cases).
Binary `83356a9a474e1300cbe78c66616e4dd004ef9fcab7305d44310b813f8e1bdee3`;
reports `UP062-berserk-foundation-final-focused.log`/`.xml`. All 77 offline gates,
module and diff checks pass; independent review has no remaining blocker.
The failure ledger retains all compile/fixture failures and debugger attribution.
Counts are unchanged. Full Berserk/Frenzied completion still needs the pending
Morale decision, one-activation expiry and perk implementation. All-blocked
approach remains uncertified; broader tied-branch/forced-walk forecast progression
is Phase 2. No GUI, launcher profile or playable snapshot promotion.

Source delivery: `8c462143286f910e91eea0849afe9d83d4eb4209` is committed and
pushed; remote identity matches. Full Windows run `36719626047` is confirmed
still compiling its frozen `63431ceb3` source and does not contain this Berserk
checkpoint. Preserve that live run; queue a newer build after it terminates.
Native verification is not Windows or graphical acceptance.
UP-023 missing Chaos base-mechanic slice. Canonical Berserk affects one enemy's
next activation, forces melee even for shooters, selects by actual movement
cost regardless of allegiance, randomizes equal-distance ties and approaches
the nearest reachable target when an attack is out of range. Basic Frenzied
Curse grants +2 Speed for that forced activation. Preserve legacy v1/v2 rules,
authoritative action validation and detached/read-only AI forecasting.

Current profile tests establish targeting only. Generic UNTIL_OWN_ATTACK
lifetime persists after WALK/NO_ACTION; the shooter branch shoots and ranks by
raw hex distance; ties use deterministic first-element order. STACK_ACTIVATION
expiry infrastructure already exists. Perk has no live runtime consumer and
remains planned. Required principal evidence includes forced shooter melee,
path-cost/tie selection, movement-only expiry and perk speed restoration.
Ask whether a negative-Morale skipped turn consumes Berserk or leaves it for
the next usable activation; do not silently resolve that material lifecycle
question. All-paths-blocked fallback also needs a bounded policy audit; do not
claim complete Berserk from correcting only its target shape. No implementation,
activation or playable evidence is claimed by this map.
Minimum AI gap: shared forced WALK/NO_ACTION currently loses its exact target
and destination in PotentialTargets and falls into ordinary tactical movement.
No explicit projected next-activation Berserk value is present. Keep shared
forced-action candidates deterministic/read-only for inspection, choose tied
runtime targets authoritatively, and value friendly as well as hostile harm.
The current empty-target helper indexing is also a crash-risk guard to repair
with the bounded path work. Nullkiller uses BattleAI; no parallel adventure-AI
forced-action implementation is needed.

## UP-058 — Repair canonical combat-spell School assignments

Status: Implemented; focused source/native verified, playable delivery pending,
2026-09-30.
UP-023 Phase 1 data/functional correctness, not a numerical balance change.
The functional matrix already lists Implosion as Sorcery and Earthquake as
Nature, but current `config/newHorizonsMagic.json` still assigns both to Havoc.
Correct fresh saved profiles, mirrored module and relevant acquisition/School
consumers/tests after the frozen Archmage gate. Preserve prior snapshots rather
than silently reinterpret already saved rules. Audit the adjacent recorded
roster corrections without treating an absent Counterspell row or a note as
proof of every spell's effect. Archmage's present fixture intentionally tests
the current saved Level 4; it does not establish correct Implosion School.
No data edit or verified repair is claimed yet.

Final checkpoint supersedes the initial audit state: fresh Implosion is Sorcery
and Earthquake is Nature; generated module matches. Both Linux targets build
(74940), final test-only rebuild 76420 succeeds, and focused native 76202 passes
4/4, zero skips. Binary
`d492ad73bae4a628efb7f91dfdf49f18328722339a55bbebbbcff61d6b23f37f`;
reports `NewHorizonsCanonicalSchools-retry1-focused.log`/`.xml`.
Actual hero School-rank/acquisition policy uses the corrected fresh data;
captured old Havoc classifications survive world save/load and BattleStart
serialization; existing shared classification cast and updated Archmage AI
submission pass. Offline gates pass 75/75, mirror/diff checks pass, independent
review has no blocker. The Ice Bolt cast in the round-trip helper also retains
Speed and Initiative in current profiles. Counterspell/Master Chain Lightning
ordinary acquisition findings are separately UP-059, not fixed by this slice.
Spell/perk/rank counts remain unchanged; Implosion percentage/pull and full
Earthquake mechanics are not certified. No GUI/profile/snapshot promotion.

## UP-059 — Exclude noncanonical and specialty-only Guild spells

Status: Implemented; source/native verified, playable delivery pending, 2026-09-30.
Adjacent UP-058 audit: Counterspell is absent from the detailed canonical
roster but remains active in the fresh magic configuration. Master Chain
Lightning is Solmyr's specialty, not an ordinary Guild spell; its definition's
zero gain chance does not exclude it from fixed-school generation, which
deliberately ignores weights. `CGameState::initTowns` currently admits ordinary
combat definitions from the active saved roster without a specialty-only gate.
Repair fresh ordinary acquisition using explicit saved eligibility, not spell
weights or a global definition change that silently changes old saves. Preserve
Solmyr's legitimate inscribed specialty and its casting, and distinguish
noncanonical Counterspell from independently specified countering mechanics.
Require focused Guild/teacher/acquisition evidence and retained saved-profile
behavior. Shared optional saved `ordinaryAcquisition` now separates learning
and generated offers from casting; absent markers preserve historical eligibility.
Fresh Master Chain Lightning disables ordinary acquisition while retaining
Solmyr's inscription. Fresh Counterspell is inactive, with historical execution
fixtures explicitly retaining their captured roster. Guild authored/random pools,
hero learning, House of Wisdom generation and authoritative purchases use the
policy. Random reward default pools also exclude ordinary-ineligible spells;
explicit named references retain their prior roster/limiter/casting semantics.
Adventure acquisition remains unchanged. Final client/test build 73711 succeeds,
native 27381 passes 42/42, zero skips, on
`e5a3ed12075a54ed827d1acb60c84b2b647263528ff33fc90eb17592f068f14e`;
reports `UP059-acquisition-final-focused.log`/`.xml`. Solmyr known casting,
actual Guild grants and constrained fresh/historical generation, House stock
and purchase guards, random/default/named reward selection, schema admission
and retained historical Counterspell AI paths pass. Content gates pass 76/76;
module/diff checks pass; independent review has no remaining blocker.
Failed compile/fixture runs are retained in the release failure ledger.
Coverage counts remain unchanged. Broader world-save/teacher/scroll interaction
journeys and rendered/playable acceptance remain Phase 2/delivery work.
No GUI, snapshot or launcher-profile promotion.

## UP-046 — Elemental Rebirth foundational effects

Status: Planned; read-only map complete, HP-basis clarification pending,
2026-09-30. UP-023 Phase 1 coverage candidate; no effect activation claimed.

Implement the Conflux rank effects: destroyed non-summoned allied stacks create
temporary random Elite Elementals at their position with exact aggregate HP
at 25/40/50%. Reborn units cannot recursively trigger the base effect. Include
physical attacks and spell injury paths, legality/footprint, temporary casualty
provenance, exact wounded-final-creature HP, authoritative packets, detached AI
projection and summon/result feedback. Existing class assignment/metadata is
not runtime coverage: all three rank effects and ten perks remain planned.

Reuse pre/post damage reaction seams and existing temporary-summon helpers,
not original same-stack REBIRTH. Capture the source position and HP basis before
damage; the user is asked whether the basis is the original battle-start stack
or remaining creatures immediately before the fatal hit. Do not choose this
material rule silently. Later perk work requires serialized origin/original-HP
and once-per-combat state, and terrain candidate sets still need clarification.
While the question is unanswered, continue another unblocked Phase 1 item.

## UP-044 — Implement Command's attribute-specific efficiency perks

Status: Implemented (rendered/playable verification pending), 2026-09-30;
UP-023 Phase 1 coverage slice.

Implement Aggressive Commander, Defensive Commander and Veteran Commander.
Attack-derived Order
components gain +20 percentage points of Command Efficiency from Aggressive;
Defense-derived components gain +20 points from Defensive. Flat bases remain
unchanged; Veteran adds +25 efficiency points to Leadership-derived terms.
Rank efficiency still applies, and none of these increases Leadership
capacity. Share exact per-component math between authoritative Order snapshots
and AI evaluation; preserve Warcasting and legacy saved rules. Activate the
canonical perk entries and ordinary progression, retain existing generic perk
UI hooks, and require focused source/native/build and AI evidence. Record
broader interactions and rendered/playable acceptance for Phase 2. No launcher
promotion. Runtime and AI workers own distinct files; root owns registration,
validation, documentation and Git integration.

Source/native checkpoint: both Linux targets build; all 11 focused runtime,
progression and actual-AI cases pass, zero skips. Content/perk/inventory passes
74/74; mirror and diff checks pass. Independent review has no blocking finding.
Existing Command Order guards also pass 13/13 with zero skips.
Coverage advances to 118/310 active perks, Command 3/7 active/planned; combat
identity coverage remains 58/67. Test binary SHA-256 is
`e228836aac3189c35ed63b803c2facd57ec22b5c006161537054ee860a13a2a3`.
AI cases isolate each Order's coefficient consumer while retaining a legal
Magic Arrow competitor; all-canonical-Order tactical ranking and AI Warcasting
interactions remain Phase 2. Runtime Warcasting and binary snapshot checks pass.
The synthetic old-rules/new-active-registry Focus Fire edge remains deferred.
Bespoke art is Not done; neutral fallback is not final art. No launcher promotion.

Source delivery: `fcecc23d3d72ac6c67fd354bf8b2bfcb26234a5d` is committed
and pushed; remote identity verified and worktree clean at this checkpoint.
Full Windows run `36672365779` succeeds on frozen source
`dc50b5353ceb86d8800eac9e162c69ad324ed4d6`, containing that source.
Downloadable package artifact `11081176965` is available (750,646,843 bytes).
This is Windows build/package evidence, not graphical acceptance or Linux
launcher promotion. Later Combined Arms, Mysticism and Prepared Caster changes
are not included in that frozen package.

## UP-043 — Implement Chaos Confusion and Confounder

Status: Planned; two design answers pending, 2026-09-30. UP-023 Phase 1 slice.

Implement the canonical Level-1, 5-Mana enemy-stack spell: its next activation
becomes random Attack, Defend or Wander. Attack chooses an enemy of that
creature, never an ally, and uses ordinary attack/movement legality. Wander
uses legal movement, without deliberately engaging an enemy. Confounder
prevents consecutive identical resolved behaviors on that target. Require
authoritative forced activation, serialized pending/history state, shared
legal-choice geometry, detached AI expectations without live RNG, status/
combat feedback, registration and focused build/native evidence.

Read-only runtime mapping is complete. Reuse BattleFlowProcessor's automatic
action path and normal action validation, not direct state mutation. The
Berserk helper is only a reference: it targets allies and nearest creatures,
unlike Confusion. CUnitState's JSON save/load and UnitChanges are the state
propagation seam; hypothetical AI copies that state. Preserve genuine
activation-start effects through makeAutomaticAction. Two user questions are
pending: impossible behaviors/Confounder's sole-legal-result fallback, and
whether a Morale/Berserk-consumed activation also consumes pending Confusion.
Do not silently invent these gameplay rules. Other unblocked missing coverage
can proceed; this is not a blocker for the entire Phase 1 goal.

## UP-042 — Implement Chaos Blink and Blinkmaster

Status: Implemented (rendered/playable verification pending), 2026-09-30;
UP-023 Phase 1 coverage slice.

Implement Level-1/4-Mana Blink on any legal friendly or enemy creature stack:
uniform random legal relocation within `min(4, 2 + floor(SP / 100))` radius,
excluding the origin and accommodating the whole footprint. Ignore intervening
terrain, obstacles, walls and Zones of Control; this is not voluntary movement
and must not grant activation, retaliation, Initiative or movement-trigger
benefits. Reject an empty destination set before Mana or Hero Action. School
proficiency strengthens the SP-derived part, never adds a mass cast.
Blinkmaster generates two random legal destinations and automatically uses
the farther one, with deterministic hex-order ties. Reuse shared geometry for
pre-cost validation, radius/legal-destination preview, authoritative execution
and bounded detached AI evaluation without consuming live RNG. Require real
AI submission, focused native/build evidence, acquisition/registration and
feedback. Full save/load, broad status/obstacle interactions and rendered/
playable acceptance remain Phase 2. Do not promote the normal launcher.

Source/native checkpoint: both Linux targets link; the isolated Blink filter
passes 12/12 and focused immunity/Entangle guards pass 24/24, zero skips.
Evidence covers whole-footprint geometry, capped School-scaled radius, exact
endpoint weights, legitimate Blinkmaster progression, pre-cost empty-ring
rejection, friendly/hostile resistance and Mirror handling, and actual AI
submission with live position/health/Mana/RNG immutability. Content/perk/
inventory checks pass 74/74; UI source, mirror and diff guards pass.
Independent review has no remaining blocker. Coverage is 58/67 combat
identities, Chaos 4/11, perks 115/310. Art is Provisional. Failed fixtures
and corrections are retained in NH_RELEASE_FAILURES.md. Broader save/status/
obstacle interactions, tactical AI quality and rendered/playable acceptance
remain Phase 2; no launcher promotion.

Source delivery: commit `d6f976a1b` is pushed; full Windows preview run
`36670136812` is live on that source. No compile/package success is claimed
for Blink yet; the preceding successful Hydra artifact does not contain Blink.

## UP-041 — Implement Hydra's Vitality and capacity-safe creature health

Status: Implemented (rendered/playable verification pending), 2026-09-30;
UP-023 Phase 1 coverage slice.

Implement the canonical Nature Level-4, 16-Mana, three-round enchantment:
maximum creature HP increases by `min(50%, 25% + 0.15% × SP)` and each
surviving creature regenerates 10% of enhanced maximum HP at genuine activation
start. School rank strengthens only SP; no mass variant. Increasing capacity
must not immediately heal any creature, change living count, restore casualties
or create a Guardian Spirit-style shield. Actual current health, damage,
ordinary healing and restoration must retain coherent creature counts while
enhanced capacity is unfilled. Expiry/Dispel clamps excess body HP without
resurrection. Use compact serialized health cohorts rather than one entry per
creature or a per-frame army scan. Share principal lifecycle with hypothetical
AI; expose useful target preview/status and combat feedback. Require focused
principal/native and minimum health-integrity guards plus a successful build.
Record broad interaction/save/reward and rendered/playable checks for Phase 2;
no implicit launcher promotion. Root owns rounding clarification and integration.

Source/native checkpoint: both Linux client/test targets link. The isolated
Hydra filter passes 8/8 and existing health/Regeneration/Cure guards pass
16/16, zero skips, on refreshed identical binaries/resources. Coverage rises
to 57/67 combat identities and Nature 9/11; active perks remain 114/310.
Principal evidence includes raw wide-tail targeting, no instant HP/count gain,
genuine activation healing, ordinary healing without resurrection, exact
temporary-resurrection cleanup, recast/expiry clamping, saved-v2 and overflow
pre-cost rejection, actual AI submission, detached/live immutability and real
activation parity. Independent review has no remaining blocking finding.
Failed runs and fixture repairs are retained in NH_RELEASE_FAILURES.md.
Full combat save/load and status interactions, reach-aware Order valuation,
two-packet expiry presentation, rendered/playable acceptance and art approval
remain Phase 2. No normal profile or launcher snapshot was changed.

Source delivery: committed and pushed as `75c8aea71`; full Windows preview
run `36665665686` succeeds on that source, including client compile and
packaging. Downloadable artifact `11076608841` is named
`New-Horizons-Windows-x64-75c8aea71b8c4be48d561d727a897ee88d62c9fb`.
This is a Windows compile/package pass, not Windows graphical acceptance or
Linux playable promotion.

## UP-040 — Implement Verdant Prison and Verdant Warden

Status: Implemented (rendered/playable verification pending), 2026-09-29;
UP-023 Phase 1 coverage slice.

Implement the canonical Nature Level-3, 12-Mana enemy-targeted prison using
actual temporary Dendroid Guard stacks on legal empty hexes bordering the
target's occupied footprint. Divide the shared `180 + 3 × SP` pool evenly
across created stacks, retaining exact whole HP and wounded final creatures.
School rank strengthens only SP; Verdant Warden increases the whole pool by
25%. Preserve ordinary Dendroid abilities, Initiative, collision and temporary
summon provenance; escape does not remove the summons. No abstract root or
permanent troop/resource creation. Use shared effect geometry for legal ring,
HP/count preview, authoritative execution and AI; reject empty/stale rings
before Mana or Hero Action. Require registration, combat feedback, focused
runtime/AI tests and build evidence. Record rendered/playable, full save/reload,
reward and broad status interactions as separate Phase 2 work; no implicit
launcher promotion.

Source/native checkpoint: both Linux client/test targets link. The isolated
active-profile Verdant filter passes 11/11, zero skips, including full/partial
and double-wide rings, exact wounded-creature HP, legitimate Warden progression
and 229-HP rounding, pre-cost empty-ring/v2/full-resistance rejection, reflected
friendly placement, spawn/state JSON UPDATE, persistence after target movement,
and actual AI selection/submission with per-hex forecast/resolution parity.
Summon Trolls shared-path guard passes 10/10; content/inventory passes 55/55.
Independent review has no remaining production blocker. Failures and fixture
repairs are retained in the release-failure ledger. Coverage is 56/67 combat
identities, Nature 8/11, and 114/310 active perks. Spell art remains Provisional,
Warden art Not done. Full combat save/load, rewards/status interactions, AI
tactical quality and rendered/playable acceptance remain Phase 2; no launcher
promotion. Next missing Nature identity: Hydra's Vitality.

## UP-039 — Implement Summon Trolls and Beastcaller

Status: Implemented (rendered/playable verification pending), 2026-09-29;
UP-023 Phase 1 coverage slice.

Implement the canonical Nature Level-2, 9-Mana spell: summon existing Trolls
on a legal empty hex chosen by the caster, with aggregate HP `100 + 2.5 × SP`.
Convert to `ceil(pool / Troll HP)` creatures and wound the final creature so
initial HP equals the pool, without rounding-generated HP. Preserve intrinsic
abilities/regeneration and ordinary Initiative entry. Temporary summons vanish
after combat and cannot create permanent troops or strategic resources.
Beastcaller increases the pool by 25%; School rank strengthens only the Spell
Power component. Preview legal placement, footprint and resulting HP/count
before spending Mana or a Hero Action. Reuse shared aggregate-HP/placement and
summon state where safe, with authoritative validation, AI use, combat feedback,
registration and focused native/build evidence. Track broad save/load, reward,
interaction and rendered/playable checks separately for Phase 2, without
silently claiming those paths complete or promoting the normal launcher.

Source/native checkpoint: both Linux client/test targets link; the isolated
active-profile `NewHorizonsSummonTrolls*` filter passes 10/10, zero skips.
It covers exact count/HP preview and resolution, School rank, Beastcaller,
flat/percentage health artifacts, occupied-hex and saved-v2 pre-cost rejection,
independent recasts, spawn/state JSON and authoritative UPDATE replay, and
actual AI destination submission with detached forecast/resolution parity.
The shared new-unit AI bonus-inheritance repair also passes the two existing
Phantom Army/Transfigure Matter guards. Content and perk inventory pass 54/54;
UI source guard, module mirror and diff checks pass. Independent review has
no remaining blocker. Coverage is 55/67 combat identities, Nature 7/11, and
113/310 active perks. Original Provisional spell art is bound; Beastcaller
perk art remains Not done. Full mid-combat binary save/reload, broader reward
and effect interactions, tactical placement quality, rendered/playable
acceptance and launcher promotion remain separate Phase 2 work. Next missing
Nature identity: Verdant Prison, with Verdant Warden.

## UP-038 — Implement Nature Vengeful Vines

Status: Implemented (rendered/playable verification pending), 2026-09-29;
UP-023 Phase 1 coverage slice.

Implement the canonical Level-1, 5-Mana oriented six-hex winding attack.
The caster selects an origin and one of six orientations, with affected-hex
preview and rotation controls before committing. Hit intersected enemies
once per stack for `20 + 1.1 × SP` Nature damage, then apply −2 movement
Speed for two rounds without changing Initiative. School rank scales only
the Spell Power damage term, never grants a mass variant. Author the clean
hex template as requested by the specification; use shared geometry for
authoritative validation, client preview and AI enumeration. Preserve Mana,
Hero Action, target legality, resistance and saved-rule boundaries. Require
focused native/build evidence; rendered/playable and broad interactions stay
separate Phase 2 work. Do not promote the normal launcher implicitly.

Source/native checkpoint: both Linux client/test targets link. The isolated
active-profile geometry/runtime/AI filter passes 13/13, zero skips, including
rank damage, movement-only Speed penalty, duration/Echoed Duration, malformed
and stale pre-cost rejection, resistance/immunity, double-wide deduplication,
friendly exclusion and actual AI forecast/submission/resolution parity.
Content passes 51/51, perk inventory 2/2, UI source guard and module mirror
pass; purpose-made Provisional art hashes/dimensions/runtime copies match.
Independent review's preview mismatch and native fixture/rule findings are
repaired and recorded in the failure ledger. Coverage is 54/67 combat
identities, Nature 6/11, perks unchanged at 112/310. Full save/load, Dispel,
combined movement statuses, hypnosis ownership, wider AI horizons, rendered
keyboard/visual review and playable delivery remain separate Phase 2 work.
Next missing Nature identity: Summon Trolls.

## UP-037 — Implement Nature Entangle and Rootcaller

Status: Implemented (verification pending), 2026-09-29; UP-023 Phase 1 coverage slice.

Implement the canonical Level-1, 4-Mana single-enemy-ground-stack root.
Voluntary movement becomes unavailable without changing Initiative or
preventing adjacent attacks, retaliation, shooting, Wait, Defend, or
nonmovement abilities. Base duration is `min(2, 1 + floor(SP / 100))`;
School rank strengthens only the SP term, and Rootcaller adds one round
up to three. Actual displacement and teleportation remove the root; mere
activation, attacks and absent binding creatures do not. Preserve normal
casting legality, saved-v3 boundaries and source-specific effect lifecycle.
Provide AI choice/projection, status and combat feedback, registration,
focused native tests and build evidence. Rendered/playable acceptance and
unverified cross-system interactions remain separate Phase 2 work.

Source/native checkpoint: both Linux targets link; the isolated active-profile
`NewHorizonsEntangle*` filter passes 17/17, zero skips, exit 0. It includes
actual AI selection/submission, duration/rank, Rootcaller plus Echoed Duration,
preserved nonmovement actions, teleport/displacement, refresh/expiry and
pre-cost legacy rejection that leaves Haste castable. Content passes 50/50,
perk inventory 2/2, status wiring 4/4, module mirror and diff checks pass.
Independent review's two blockers were repaired. Coverage is 53/67 combat
identities and 112/310 active perks, Nature 5/11. Original Provisional art is
bound; Rootcaller perk art is Not done. Combined classic Bind lifecycle,
full save/load/Dispel, wider AI horizons, rendered/playable acceptance and
launcher promotion remain open. Next missing Nature identity: Vengeful Vines.

## UP-036 — Implement Light Crusade! and Crusader

Status: Implemented (verification pending), 2026-09-29; UP-023 Phase 1 coverage slice.

Implement the canonical Level-5, 24-Mana entire-friendly-army empowerment:
Attack/Defense `min(6, 3 + floor(SP / 75))`, flat Initiative
`min(3, 1 + floor(SP / 100))`, independent multiplicative Magical Damage
Reduction `min(25%, 12% + 0.065% × SP)`, and negative-Morale floor zero.
Duration is three rounds, four with Crusader. School rank strengthens only
the Spell Power-derived components; fixed bases and caps stay unchanged.
Preserve fractional magical reduction, Speed/Initiative separation, recast
refresh rather than stacking, saved-v3 roster boundaries, and ordinary
action/Mana restrictions. Provide authoritative execution, BattleAI use,
active status/help, registration, focused tests and build evidence. Record
unverified cross-system and rendered/playable checks for Phase 2 separately.

Source/native checkpoint: both Linux client/test targets link; the isolated
active-profile Crusade filter passes 19/19 with zero skips, including actual
AI choice/submission/casting, recast/expiry, fractional reduction, current
bonus serialization, and Echoed Duration with and without Crusader. The
49-case content suite, two perk-inventory checks, two UI wiring checks,
module mirror and diff check pass. Independent review has no remaining
blocking finding. Coverage advances to 52/67 combat-spell identities and
111/310 active perks; Light identity coverage is 11/11. Appropriate original
Prayer assets are referenced, not copied; Crusader's bespoke perk art is Not
done. Full combat save/reload, Dispel, generic duration artifacts, hypnosis
and wider AI forecasts remain Phase 2 work. Rendered/playable acceptance
remains open; no launcher snapshot is promoted by this source checkpoint.

## UP-035 — Implement Light Purify and Purifier

Status: Implemented (verification pending), 2026-09-29.

Implement the canonical Level-4, 15-Mana radius-2 area cleanse with selected
negative effects per friendly stack, capped at one below 120 Spell Power and
two at 120 or above. Physical Poison is a selectable base effect; Purifier
adds an automatic physical-affliction removal outside that cap. Preserve
positive effects and Orders, reject invalid or empty selections before
spending resources, and provide UI, AI, serialization and original
Provisional art.

Source/native checkpoint: both Linux targets link and all 10 focused
active-profile server/helper/AI cases pass with zero skips. The 48-case
content suite, module mirror, picker routing guard and diff check pass.
Independent review's detached-state Poison finding was corrected. Coverage
is 51/67 combat-spell identities and 110/310 active perks; Light is 10/11.
Purpose-made Provisional art was generated with the HoMM3 art workflow.
Rendered/playable acceptance, full save/load and other physical afflictions
remain open. Phase 2 must align hypnosis ownership: server eligibility uses
current ownership while UI/AI additionally check original side. UP-023
remains open; the next missing Light identity is Crusade!.

## UP-034 — Implement Light Divine Retribution and Retributionist

Status: Implemented (verification pending), 2026-09-29.

Implement the canonical Level-4, 16-Mana, one-friendly-stack Divine
Retribution. For two rounds, a damaging enemy creature attacker becomes
Judged; at the end of that round it takes Holy damage equal to the lesser of
30% of damage dealt and `25 + 1.25 × Spell Power`, at most once per attacker
per round. Melee and ranged creature attacks qualify; spells do not. The
School rank strengthens only the Spell Power term. Retributionist grants +20%
reactive damage to the spell's final capped result. Provide authoritative
saved-state/lifecycle, clear status and combat log, AI use, original Provisional
art, and focused native evidence.
Interpret "damage dealt" as the sum of actual HP loss after mitigation from
qualifying creature-attack packets by each attacker against each protected
effect in a round. Resolve pending Judgments before the protected spell's
round-end decrement.
Record broader multi-packet and shield/overkill interactions for Phase 2.
Both Linux targets link; 14/14 isolated active-profile server/AI cases pass
with zero skips. The 47-case content suite, module mirror, and diff checks
pass. The independent review's blocking recast finding was fixed and covered.
Purpose-made Provisional 44/32/30 spell art is bound; the Retributionist perk
still uses a neutral fallback and needs its own art. In-game rendering,
playable delivery, full save/reload, Dispel, unusual physical packets, and AI
valuation under mixed threats remain unverified. Do not mark this Resolved
until the delivered game has the intended behavior and presentation.

## UP-033 — Implement Light Heavenly Gale and Aegis

Status: Implemented (verification pending), 2026-09-29.

Implement the canonical Level-3, 13-Mana, entire-friendly-army Heavenly Gale:
for two rounds, physical ranged projectile damage (including physical siege
shots) is reduced by `min(80%, 50% + 0.15% × Spell Power)`. Preserve the
specified fractional percentages, School-rank potency of the Spell Power
term, and exclusion of melee, spell damage, magical beams, area explosions,
and non-projectile magic. Activate Aegis's +20% Spell Power-derived
protection component for both Heavenly Gale and Holy Armor. Provide saved
effect state, clear status/feedback, AI casting and valuation, purpose-made
Provisional art, and focused native evidence. Record broader classification,
cross-system, rendered, and playable gaps separately.

Source/native checkpoint: Heavenly Gale's saved-v3 two-round mass marker,
fractional physical-projectile mitigation, Aegis scaling for both it and Holy
Armor, stack status, BattleAI choice/valuation, and purpose-made Provisional
icons are implemented. Both Linux targets link. The isolated active-profile
server/AI filter passes 15/15 with zero skips; curated content passes 46/46
and the module mirror matches. Rendered/playable acceptance remains open.
Defer exhaustive magical-beam and area-shot classification, AI valuation under
combined physical-damage caps, AI mass projection logging, Dispel and
save/load round trips, and live AI submission to Phase 2.

## UP-032 — Implement Light Guardian Spirit

Status: Implemented (verification pending), 2026-09-29.

Implement the canonical Level-2, 8-Mana, single-friendly-stack Guardian Spirit:
a separate pool of `50 + 2 × Spell Power` temporary HP absorbs physical
creature damage from melee, shots, retaliations, and physical creature
abilities before actual stack HP, but spell damage bypasses it. The effect
expires after two rounds or when the pool is exhausted. Apply the Healer and
Guardian Light-perk modifiers to their specified components. Provide
authoritative/save behavior, active status and combat feedback, BattleAI
use/valuation, purpose-made provisional artwork, and focused native evidence.
Keep rendered/playable acceptance separate and record Phase 2 interactions.

Source/native checkpoint: the saved-v3 spell, separate serialized pool,
physical-creature damage provenance, two-round expiry/exhaustion, combat
feedback, active status, Healer/Guardian modifiers, BattleAI casting path, and
purpose-made Provisional icons are implemented. Linux `vcmiclient` and
`vcmitest` link. The private active-profile Guardian/Healer filter passes 7/7
with zero skips; curated content passes 45/45 and the module mirror matches.
Rendered/playable acceptance remains open. Defer AI physical-attack exchange
forecasting, scripted nonmagical ability classification, full combat
save/reload, Dispel, and broader interactions to Phase 2. Next missing Light
identity: Heavenly Gale.

## UP-031 — Implement Light Sanctuary

Status: Implemented (verification pending), 2026-09-29.

Implement the canonical Level-1, 5-Mana Sanctuary spell for one friendly stack.
While Sanctified, the stack cannot be deliberately selected for an enemy
creature attack or hostile single-target spell, but area, global, and indirect
effects still work. Moving, attacking, or using an offensive active ability
ends the effect immediately; Wait and Defend preserve it. Give the effect
authoritative lifecycle/save behavior, visible status and combat feedback,
BattleAI targeting/use, a purpose-made provisional icon, and focused native
evidence. Do not count registration or source alone as playable acceptance.
The interpretation of expiration after a later Wait/Defend activation has
been asked of the user; until clarified, preserve protection through those
passive actions and keep the lifecycle easy to adjust. Update the functional
coverage matrix and record any Phase 2 interaction gaps before resolving.

Source/native checkpoint: saved-v3 Light registration, authoritative direct-
target rejection and pre-action break, active-status UI, BattleAI targeting/use,
and purpose-made Provisional 44/32/30 artwork are implemented. Linux `vcmitest`
and `vcmiclient` link; 7/7 server and 2/2 AI focused cases pass in an isolated
active New Horizons profile with zero skips. Curated content tests pass 44/44,
and the generated module mirror matches. Independent source review found no
remaining blocking defect after the hostile-spell flag and owner checks were
fixed. Native-resolution rendering, playable delivery, and the Wait/Defend
expiration clarification remain open; do not mark this resolved on source/native
evidence alone. Phase 2 interaction gaps are recorded in the coverage matrix.

This is a task register, not a replacement for the canonical Markdown or Pending
Changes. Existing ordinary backlog remains in the completion audit and other
registers; it is not cancelled by this new queue.

## UP-029 — Commit the accumulated work and clear the worktree

Status: Resolved on 2026-09-28.

Stop new feature edits, let the already-running native build finish safely,
identify generated artifacts versus source and user-owned work, then commit
all meaningful uncommitted changes in truthful, coherent checkpoints. Do not
discard, reset, or silently hide user data. Acceptance: committed source and
documents, focused validation status recorded, and `git status --short` empty
apart from explicitly disclosed ignored local outputs. Pushing is a separate
delivery step after local commits are reviewed.

Delivery: `4fec9c75a` (policy/design/ledgers), `f81d0aab4` (provisional art),
`124c78c7d` (tooling), and `18dea9a1a` (Phase 1 source/config/tests) were
committed and pushed to `origin/definitive-mvp`. `vcmitest` and `vcmiclient`
link; Storm's authoritative 4/4 and AI 2/2 focused cases pass under the curated
New Horizons profile. The Storm and Adventure Guild client source guards and
the generated-module check pass. No playable rendering or full integration
claim follows from these gates. `git status --short` was empty after delivery;
local `output/` previews and Python caches remain preserved but ignored.

## UP-030 — Activate Shadow Magic's Malediction perk

Status: Implemented with focused native evidence; rendered/playable verification
pending, 2026-09-29.

Implement the canonical Basic perk: Curse and Sorrow each last one additional
round. New Horizons v3 Curse must use its authored fixed three-round duration;
v1/v2 Curse must retain legacy duration behavior. Keep Sorrow's Morale-strength
formula and the unresolved lower-bound wording separate from this duration
change. Register the perk, provide a distinct provisional icon made through
the Heroes III art workflow, make AI projections and contextual help reflect
the effect, and verify authoritative casts and refreshes under an active New
Horizons profile. Acceptance is source, module-mirror, Linux build, focused
native behavior and active-perk art-guard evidence. Rendered/playable
acceptance remains separate.

Checkpoint: saved-v3 Curse and Sorrow now use three rounds ordinarily and four
with Malediction; recasting replaces and refreshes the timed bonus. V1/v2
effects retain legacy durations even when the perk is selected. The Linux
`vcmitest` and `vcmiclient` targets link; focused active-profile authoritative
tests pass 8/8 and projected-AI valuation tests pass 5/5, both with zero skips.
The 17-case perk-data contract and curated-module mirror pass. A purpose-made
provisional hourglass icon has a named binding, four distinct 44×44 states,
source master and prompt; its targeted checks pass. The global active-perk art
guard still fails on 21 previously documented unrelated neutral-icon gaps.
No rendered/playable or full AI cast-choice claim is made. AI same-round
exchange overlap and equal-strength refresh valuation are Phase 2 findings.

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

### UP-028 — Persist the Heroes III UI construction standard

Status: Resolved in source; future visual work must apply it.

The user supplied a reusable UI-design prompt emphasizing continuous
materials, restrained ornament, dense hierarchy, tactile controls, consistent
grids, authentic assets, outside-in panel construction, and explicit review
for pasted cutouts. Persisted it as `docs/NH_HOMM3_UI_STYLE_GUIDE.md` and linked
that guide from `AGENTS.md` so future UI tasks read it before implementation.
The guide also requires comparison at native resolution against relevant
original Heroes III dialogs and clarifies that painted period-appropriate
shading is allowed while modern-style gradients are not. This records a work
standard, not a claim that every current UI screen already meets it.

### UP-027 — School ranks strengthen spells as well as unlock acquisition

Status: In progress; several native slices verified, but complete spell coverage
and playable validation remain pending. Assigned 2026-09-27. The user clarified that Basic, Advanced,
and Expert ranks of each of the six Magic School Skills should provide
progressively stronger versions of spells from that school, not merely unlock
learning higher-level spells. Preserve the already-approved rule that a
legitimately inscribed spell is castable without the School rank; this request
changes the effect of a cast, not whether the cast is permitted.

Audit the canonical spell formulas and existing rank consumers before choosing
the scaling contract. Define what improves for direct damage, healing,
protection, debuffs, summons, duration, and special/non-numeric spells without
silently adding multipliers to incompatible mechanics. State how multi-school
spells, perk-granted Mass variants, and specialty spells interact. Integrate the
approved rule in canonical Markdown, catalogue descriptions, authoritative
cast/damage/status paths, AI forecasts, tooltips/logs, and focused tests. Keep
numerical balance provisional but make the rule intelligible and coherent.

User clarification: start modestly with a Heroes V-like model for damaging
spells—School rank strengthens the coefficient multiplying Spell Power, not
just a flat base-damage term. Expert School rank must never automatically grant
Mass versions; Mass variants remain explicitly perk-granted. Use considered,
effect-appropriate scaling for non-damage spells rather than forcing the damage
formula onto them. This first systemic pass need not hand-author every spell's
unique rank behavior before establishing the common rule.

Initial provisional damage ladder: no rank / Basic / Advanced / Expert scale
only the Spell Power coefficient by 100% / 115% / 130% / 145%. Save the new
rule in magic-rules version 3; old v1/v2 saves retain 100%. Multi-school spells
take the highest School rank once; neutral Adventure Spells are excluded.
Numeric non-damage effects may share the coefficient rule where appropriate;
discrete effects need authored variants or an explicit exception.

2026-09-28 checkpoint: the shared school-rank rule has been integrated into
the canonical Markdown and its source hash synchronized with the perk registry.
The new-game magic snapshot and module mirror now select v3 with the four
provisional factors. A New Horizons spell overlay suppresses all 23 active
core creature spells whose inherited Expert range was Mass; the focused
data test passes. This is source/data evidence only, not runtime, target-build,
or playable verification. Initial non-damage rank scaling covers Cure's
Spell Power-derived healing and Transfigure Matter's summoned-HP term;
other schools' non-damage spells still need authored effects, and UP-027
remains open.

Non-damage audit, 2026-09-28: Transfigure Matter is the first additional
low-risk authored case: scale only its `2 × Spell Power` summoned-HP term,
leaving fixed/obstacle HP, Matter Shaper, and placement unchanged. Phantom
Army now scales only its Spell Power-derived integrity with Sorcery rank;
the fixed base, cap, and Illusionist order are preserved. Fractional ranked
basis points survive until the final Health floor; a review-found Basic/SP 1
case now checks the exact 20,172 Integrity result from 100,000 source Health.
The Phantom test translation unit compiles, including rank values,
preview/cast parity, v1/v2 fallback, and tooltip assertions; native execution
remains pending. Bless,
Spell Lock, and Time Stop have authored Spell Power-derived durations but
need their matching runtime/preview paths checked before rank adjustment.
Nature's Quicksand, Shadow's inherited status spells, and Chaos's legacy
Misfortune currently expose old rank behavior, not the new authored contract;
Havoc's authored live spells are covered by direct damage. Do not count those
legacy tier values as completion of this queue item. Transfigure's source now
uses a saved-rules, caster-specific coefficient through a separate Lua binding
that preserves the existing two-argument scaling API; focused source tests
cover four v3 ranks, v1/v2 fallback, preview/cast parity, and Matter Shaper.

2026-09-29 Phase 1 native checkpoint: Shadow's Sorrow is corrected from its
erroneous Chaos-school roster assignment to the canonical Level-1 Shadow
identity. The saved-v3 effect is one hostile stack, three rounds,
Morale penalty `min(3, 1 + floor(SP × School coefficient / 70))`, with no
implicit Mass variant. The source's “not below 10” sentence conflicts with
the global −10..+10 Morale range; clarification is pending. The Linux native
target links; 7/7 authoritative and 3/3 projected-AI cases execute under an
isolated curated profile, with no skips. Source/AI review found no blocker.
Saved v1/v2 retain their legacy Chaos/Mass behavior; full AI action choice,
save/load, and playable acceptance remain open.
The Sorrow vertical slice exposed a scale hazard: `CGHeroInstance` retains a
legacy Spell Power divisor of 10 under New Horizons primary growth, but the
canonical Sorrow thresholds refer to the raw hero SP rating (0–69, 70–139,
140+). Its v3 formula must use that raw rating. Audit other authored
rating-based spell formulas individually; do not globally remove the divisor
from inherited effects without save/version review.

2026-09-29 Quicksand continuation: the saved-v3 patch-count formula is in
source, with a shared caster/battle coefficient path and a real Lua obstacle
application test. Both Linux targets link; 31/31 adjacent active-profile
Obstacle and Magic-v2-rule tests pass, including Nature-rank threshold and
v1/v2 legacy-count cases. Independent review found no blocking defect.
At that checkpoint Quicksand was not complete: v3 still used random NO_TARGET
placement, whereas the canonical
spell requires sequential caster-selected legal hexes, count/undo/confirm
feedback, authoritative exact-target validation, and AI placement. V1/v2 must
retain their configured legacy counts. Mire Shaper remains planned, and the
canonical text does not yet settle whether its +1 patch can exceed the usual
five-patch cap. Native graphical/playable evidence is still absent.

2026-09-29 Quicksand exact-placement checkpoint: saved-v3 new games now
require the caster to select the exact ordered patch count on legal empty
ground. Client count/undo/confirm controls, authoritative no-spend rejection,
the Lua effect, concealed obstacle flags and `StartAction` presentation,
BattleAI placement, and an append-only protocol gate are in source. Older
v1/v2 and markerless-v3 saved battles keep random placement. Both Linux
targets link; the focused native filter passes 9/9, the magic-data gate 12/12,
and both repeated-placement UI source guards pass. This resolves the missing
Phase 1 selected-placement path, not UP-027 as a whole or playable UI
acceptance. Deferred: hidden enemy-obstacle collisions, obstacle-packet
confidentiality, trigger/lifecycle integration, native-resolution readability,
and Mire Shaper's unsettled extra-patch cap.

2026-09-29 Holy Armor continuation: Level-2 Light protection now uses the saved
School-rank coefficient on its Spell Power term while keeping its fixed 30%
base. The spell, independent magical-reduction runtime, focused AI choice,
and provisional art binding link in the Linux client; 25/25 active-profile
native and 39/39 focused Python cases pass. This advances the protection
category but does not close UP-027: other non-damage spells and full playable
coverage remain. Holy Armor's lifecycle/save integration and Fire Shield's
separate reduction path are deferred to Phase 2, not assumed verified.

Independent overlay review found three additional inherited-Heroes-III shape
or side-effect leaks (Berserk area targeting, Dispel obstacle removal, and
Chain Lightning rank-dependent chain length). New-game overlay corrections and
focused assertions are in the worktree. The review also found a save-compatibility
gap: unlike the versioned coefficient, global spell-content overlays affect
older v1/v2 saves. Do not call this slice complete or playable until the
overlays are guarded or that compatibility is deliberately resolved and native
behavior is verified.

Validation checkpoint: the v3 magic/perk module mirrors exactly match their
canonical JSON inputs; 34 focused Python schema/perk tests pass, as does the
Expert targeting data test. A native source review found and corrected the
v3 Warcasting gate, stale spellbook damage estimate, v1/v2 test-fixture
assumptions, arithmetic divisor bound, Cure test expectation, and an AI test
that assumed zero Overcharge. Touched production and test translation units
compile using existing Ninja commands. The full native test binary was not
rebuilt or run, and the broader generated-module check still fails on an
unrelated already-dirty creature-categories settings mirror (the v3 magic and
perk mirrors match exactly). At that checkpoint validation was source-only; a subsequent
safe filtered-manifest Linux build linked `bin/libvcmi.so` successfully with
the v3 magic and Transfigure runtime. The focused Transfigure test object
compiled, but no current `vcmitest` binary could be linked: the full test
target stopped in `NewHorizonsDemonicGatingTest.cpp` on obsolete
`STACKS_DEFENSE`, `battle::Unit::movedThisRound`, and default
`SideInBattle` assumptions. Those stale fixture calls, plus Unique Building
Training and Hero Command AI test compile gaps, have now been repaired and
their translation units compiled. The full suite still has not linked or run;
the user prefers faster feature-to-playtest cycles over pursuing each unrelated
fixture failure now. Therefore native execution, target-client build, and
playable verification still remain pending. The user
has been asked whether v1/v2 saves should retain old Expert targeting or
receive the new no-Mass correction; do not infer an answer.

2026-09-28 native v3 follow-up: the curated module mirror now passes the full
generator `--check`, including the previously stale creature-category section.
The current Linux `vcmi`, `vcmiclient`, and `vcmitest` targets link after
repairing stale test APIs. Bless now uses raw Spell Power in its v3
`min(4, 2 + floor(coefficient × SP / 80))` duration term, adds Benediction
after the ordinary cap, keeps explicit overrides and v1/v2 enchantment logic,
and remains single-target at Expert. In an isolated TEST profile with
`new-horizons` active, all six Bless runtime tests and the AI hypothetical-vs-
authoritative forecast test pass (7/7). Independent Astra review caught and
cleared the divisor error before this result. This validates one Light spell,
not every non-damage rank effect; the global v1/v2 spell-overlay compatibility
gap and graphical/playable verification remain open.

2026-09-28 saved-profile trace: the new `core:*` spell patches in the curated
module are merged into shared `CSpell` objects at content load, before a v1/v2
or v3 saved magic-rules profile is considered. Consequently old New Horizons
saves can inherit v3-only Expert single-target ranges, Berserk/Dispel targeting
and effects, fixed Chain Lightning chain length, and Bless/Curse mastery
changes. This is a concrete compatibility defect, not merely an untested
possibility. Keep it open until saved-rule-aware cast, UI, and AI resolution is
verified against v1/v2 and v3 side by side; do not promote a new gameplay
snapshot as save-compatible based only on the coefficient's version gate.

2026-09-28 Expert-range compatibility slice: removed the 23 new global
`range: "0"` spell patches and made their Expert single-target targeting a
saved-v3 battle-mechanics decision. Expert effect mastery remains Expert;
explicit perk-granted Mass remains available. The current Linux `vcmitest`
target linked, a focused isolated New Horizons profile passed four native
helper/Bless/Temporal Field cases, and the offline content check passed.
Independent Astra review found no blocker in this narrow slice. Existing Cure
and Slow special cases still cap old-profile ranges, and the separate global
Berserk, Dispel, Chain Lightning, Bless/Curse, and Ice Bolt effect leaks remain
open. Do not describe the entire v1/v2 spell-overlay problem as resolved.

2026-09-28 Berserk saved-profile slice: removed its global content patch and
resolved single-creature targeting through the saved-v3 battle mechanics. Old
v1/v2 profiles retain core area targeting and effect; v3 remains single-target,
without making Expert a Mass spell or changing explicit Mass effects. The
current native `vcmitest` target links; six focused tests pass (including
authoritative old-profile area casts, v3 single-target casts, and friendly-
target rejection without spending mana). The focused content suite passes
33/33. This is native/source verification, not playable delivery. Dispel,
Chain Lightning, Bless/Curse, and Ice Bolt global-effect compatibility leaks
remain open, as do other School-rank spell effects.

2026-09-28 Chain Lightning saved-profile slice: removed the global fixed-five
patch and chose the effective chain count from the saved battle rules through
shared spell mechanics/Lua targeting. The native `vcmitest` target links;
three focused tests pass. V1/v2 previews use `{4,4,5,5}` targets by mastery
and an authoritative base cast hits four; v3 previews and base cast use five.
The focused content suite passes 33/33. No playable snapshot was promoted.
Independent review then found that v3 Base/Basic spellbook help still used the
inherited four-target description; a v3-only five-target description and
v1/v2/v3 regression assertions were added. The incremental native target
linked and all three Chain profile cases passed again with the description
checks. This slice
does not claim the canonical jump-damage percentages or Conductor perk are
implemented. At this checkpoint, Dispel, Bless/Curse, and Ice Bolt global-effect
compatibility leaks remained open, along with other non-damage School-rank
effects.

2026-09-28 Dispel saved-profile slice: removed its global smart-targeting and
Expert effect override. Saved v3 mechanics now permit either allied or enemy
single-stack targets and use the full status-removal effect without inherited
Expert obstacle removal; v1/v2 retain core smart/Expert effect behavior. The
current native `vcmitest` target links and seven focused tests pass, including
six v1/v2/v3 profile cases and the existing Selective Dispel no-default-Mass
guard. The focused content suite passes 33/33. This is not a playable
 promotion. Bless/Curse and Ice Bolt global-effect leaks remain open, as does
 broader non-damage School-rank coverage.

2026-09-28 Bless/Curse saved-profile repair: the v3 natural-endpoint values
are selected during timed-effect conversion from the saved battle magic rules,
not by changing shared core spell data. V1/v2 retain the original Expert
Bless +1 and Curse -1 damage-endpoint modifiers; v3 uses zero while retaining
Expert effect mastery and single-stack ordinary targeting. The Linux
`vcmitest` target linked, all 11 focused Bless profile cases passed with New
Horizons active, the v3 AI hypothetical-versus-authoritative Bless case passed,
and the content guard passed. Independent source review found no blocker. The
global Ice Bolt speed-effect leak and broader School-rank spell coverage remain
open; no gameplay snapshot was promoted from this source/native result.

2026-09-28 Ice Bolt saved-profile repair: its inherited -2 movement-range
effect is now gated at spell-effect evaluation by the saved battle magic
profile. V1/v2 retain the prior effect; v3 Ice Bolt changes neither movement
range nor Initiative and deals only its authored damage. The gate covers cast
legality, authoritative application, affected-target queries, and hypothetical
AI previews. The Linux `vcmitest` target linked, the focused content guard
passed, and three native v1/v2/v3 cast-plus-preview cases passed after test
fixtures were corrected to use valid v1 rules and detached preview targets.
Independent review found no source blocker. Edge-case applicability tests,
save/load round-trip, remaining School-rank spell effects, and playable
delivery remain open; this is not a promoted snapshot.

The first broad `NewHorizonsDirectDamageMechanicsTest` run exposed three red
Conductor/Annihilator cases. Their fixtures skipped the existing prerequisite
perks; production tier validation was correct. The fixtures now select active
Basic Stormcaller before Advanced Conductor, and both before Expert
Annihilator. After correction, the full 36-case direct-damage mechanics suite
passed under an isolated New Horizons profile. This does not complete those
perks' wider gameplay acceptance or the School-rank roster.

2026-09-28 current overlay audit: the curated spell-content directory now has
only one `core:*` root patch, Ice Bolt. The prior Expert-Mass, Berserk, Dispel,
Chain Lightning, Bless, and Curse patches are absent; their v3 changes are
instead selected by saved battle magic rules. Ice Bolt's remaining shared
content patch is wrapped by the saved-profile effect adapter, and focused
v1/v2/v3 cast/preview tests already pass. This narrows the original global
overlay concern but does not close save/load compatibility: a real old-profile
round-trip test against installed v3 content is being added, and the 23
Expert-range identities still lack a table-driven cast-path sweep. No playable
snapshot is implied.

2026-09-28 saved-profile round-trip checkpoint: a real world save/load plus
BattleStart packet test now retains exact v1, v2, or v3 rules against the
currently installed v3 content. It checks Berserk/Dispel target mechanics,
Chain Lightning's affected target identities, and an authoritative Ice Bolt
cast (damage, Mana, legacy movement slow, v3 non-slow). A fixture-only issue
where BattleStart revived original army stacks was corrected in the test;
no production change was needed. The Linux `vcmitest` target links and 54/54
focused and adjacent profile tests pass with no skips. Independent Astra
test review found no blocker. This is not a resumed mid-combat save test,
Berserk/Dispel effects were not cast in this round-trip case, and the 23
Expert-range identities still lack a table-driven cast-path sweep. No
playable snapshot is implied.

2026-09-28 Focus Magic rank slice: the authored Arcane Breach penetration
formula now applies the saved Sorcery School coefficient only to its
Spell Power-derived term before Warcasting and final flooring; the fixed
10% base, 20% cap, three-mark limit, and duration are unchanged. V1/v2
profiles retain 100%. Canonical text, all four static spell descriptions,
and hero-context help state the rule and show the current ordinary per-mark
value without implying battle-only Warcasting has already applied. The Linux
`vcmitest` target links and 12/12 focused authoritative tests pass with zero
skips under an isolated New Horizons preset. Independent Astra source review
found no blocker after the help correction. Rank-sensitive detached BattleAI
forecast proof, rendered/playable help, and broader spell-rank coverage remain
open.

2026-09-28 Focus Magic AI parity follow-up: the detached ranged-attack
forecast now has a rank-sensitive regression using the authoritative cast
test's uncapped 1015/1021-basis-point mark values. Against Defense 2000,
the second shot projects strictly more damage for the Expert value while
the first-shot baseline is equal; projected marks retain their captured
values, and forecast/exchange tracking leaves live battle state unchanged.
The Linux `vcmitest` target links, `AttackResourceProjectionTest.*` passes
8/8 with zero skips under New Horizons, and independent Astra review found
no blocker after test-strengthening. Rank-to-value capture and AI consumption
are proven in separate native paths, not in one end-to-end AI spell-choice
journey. Rendered/playable help and the wider spell-rank roster remain open.

2026-09-28 Expert-range cast-mechanics follow-up: a saved v1/v2/v3 world and
BattleStart round-trip now checks the range, Mass classification, target type,
and effect mastery of all 23 inherited core creature-spell identities, with
Cure, Slow, and Dispel exceptions explicit. The Linux `vcmitest` target links;
the isolated New Horizons profile passes 45/45 focused tests with zero skips.
The broader adjacent run passes 70/71; the one independently reproducible
failure is Cure's selected removal of physical Poison from a full-health
stack. Keep that gameplay defect open under UP-023; it is not evidence against
the table-only range test. Source review and playable validation remain open.

2026-09-28 post-Cure integrated rerun: after the authoritative Cure fix and
its survivor-healability refinement, the same isolated New Horizons profile
passes the expanded adjacent spell/Cure selection 74/74 with zero skips;
the formerly failing physical-only Poison Cure case and the added combined
Poison case pass. The focused v1/v2/v3 range/profile selection passes 45/45
again with zero skips against the stable current `vcmitest` binary. Source
review found no blocker in the range table or final Cure validation. The
earlier 70/71 line above is historical failure evidence, not current status.

2026-09-28 Time Stop rank-radius slice: saved-v3 Sorcery rank and eligible
Warcasting now scale only the Spell Power-derived radius threshold before
flooring. The fixed radius 1, ordinary cap 2, Chronomancer cap 3, and stasis
lifetime are unchanged. One shared Lua radius path feeds selected targets,
hex overlay, and AI affected-stack valuation. Hero-context help and static
descriptions explain the ranked threshold; v2 saved rules retain 100%, while
v1 does not gain a spell excluded by its roster. The Linux `vcmitest` target
links. In an isolated New Horizons TEST profile, the focused changed-behavior
selection passes 11/11 and all Time Stop-named tests pass 15/15, including
authoritative cast/preview parity, rank and Warcasting boundaries, v2 fallback,
Chronomancer geometry, AI geometry, and existing lifecycle behavior. An
independent Astra source review found no production blocker. Broader adjacent
CTest still reports unrelated old fixture failures; rendered/playable evidence,
other non-damage School effects, commit, and delivery remain open.

2026-09-29 Slow rank/tempo slice (source and focused native checkpoint):
saved-v3 Slow now derives its Initiative-only penalty from the
canonical fixed 20% base plus the Sorcery-ranked Spell Power term, capped at
50%. Temporal Field still takes 60% of the final ordinary magnitude. Its
ordinary hero duration is the authored two rounds, with Temporalist and
existing duration extensions applied separately; v1/v2 retain their prior
configured magnitude and duration. Hero-context help reports the current
ordinary value, and the same timed-effect path serves AI previews and casts.
The Linux `vcmitest` and `vcmiclient` targets link. An active-profile focused
rank, cap, duration, Mass, old-profile and hero-help filter passed 19/19 with
zero skips. The broad name filter also exposed four pre-existing unrelated
fixture failures (two old Ice Bolt
rules fields and two AI perk-tier setup errors); these belong to Phase 2.
Rendered/playable verification and other non-damage spell effects remain open.

Acceptance: all six School Skills have meaningful rank-dependent spell effects
on applicable spells; casting access remains independent of School rank for
legitimately inscribed spells; acquisition gates remain intact; AI and player
feedback match authoritative results; data, native, target-build, and playable
evidence are tracked separately. The coefficient ladder is authored provisionally;
the non-damage exception matrix remains to be completed.

### UP-026 — Repair and promote Markdown as the sole canonical design source

Status: Resolved (design/source migration); assigned 2026-09-27. The committed
Markdown, source registry, and audit are the authority handoff. A new target
package is a separate playable-delivery gate, not a design-migration blocker.
The user converted the current `New Horizons.docx` to
`/home/icaro/Downloads/New Horizons.md` and explicitly chose the repaired
Markdown as the sole canonical design specification. The repaired repository
copy is `docs/design-sources/New Horizons.md`; it intentionally differs from
the original export because table defects and approved later decisions were
reconciled.

Audit the conversion item by item against the DOCX, especially split/paginated
tables, headings, formulas, and omitted material. Preserve design intent; do
not silently treat conversion artifacts as new rules. Integrate the approved
Toxic Spines and Immovable trigger clarifications. Keep the original DOCX as a
historical source, not a competing active authority. Update all repository
authority references, tests and generators to use the repaired Markdown; retire
the relevant Pending Changes entry only after canonical integration is proven.

Acceptance: a source-to-Markdown fidelity audit records omissions and repairs;
the Markdown has parseable tables and complete rule text; the two Bulwark
clarifications are present; source-derived tests pass; no active instruction
continues to call the DOCX canonical; independent review confirms the authority
switch. Do not ship its embedded illustration as game art.

2026-09-27 source checkpoint: the DOCX-to-Markdown audit and repair record is
`NH_MARKDOWN_CANONICAL_MIGRATION.md`. The repaired Markdown has 136 uniform-width
tables, all 31 perk pools/310 entries, restored non-perk spell/rule tables and
School-rank acquisition-only wording consistent with inscribed-spell casting.
The registry and curated module point to its SHA-256; all 16 source-derived perk
and table tests pass. The first independent review found conversion blockers;
those were repaired. A final Astra cell-text review found one stray Shield of
Chaos resistance-scope word, now corrected. The scoped migration commit contains
the repaired source, registry identity, audit, and source-derived tests.

### UP-025 — Split dialog owner indicators and unclipped layout

Status: Revised Linux build promoted for user playtest (rendered aesthetic
acceptance pending);
assigned 2026-09-27. User mock:
`https://i.imgur.com/j1G5Qzi.png` (438 × 612).

2026-09-28 user priority: deliver a Linux playable snapshot containing this
garrison/hero split UI, selectable through `play-new-horizons-linux.sh`.
Build the client and matching library from the UI-containing source, freeze
and verify the snapshot, then promote it only after appropriate headless
validation. Record the exact snapshot identity and tell the user how to launch
it. Source checks alone do not satisfy this request.

2026-09-28 delivery: built a clean detached checkout of committed source
`8c4ad7e5f253b5596f12e5743fb931909fb7139d` (which includes split-UI commit
`3865be695`) as a Release Linux `vcmiclient` and matching `libvcmi.so`.
All three split/garrison source guards passed in that checkout. Froze snapshot
`e1d6a5aec6fe0e154d0323bd464b7646ca5f0936c85390daa88e6e280716abaf`;
its SHA256 inventory passed. An isolated `--headless --disable-video` All for
One smoke loaded the map and observed 46 AI turn starts in 35 seconds without
the smoke suite's forbidden errors. Promoted the same snapshot; default
`play-new-horizons-linux.sh --verify-only` resolves it successfully. This is
playable delivery, not rendered confirmation of the owner markers or actual
split-dialog interaction; user playtest remains the acceptance gate.

2026-09-28 user playtest feedback: screenshot
`https://i.imgur.com/O0tdnvq.png` shows the "Split Troglodytes" dialog.
The user explicitly confirmed that transfers work both garrison-to-garrison
and hero-to-garrison; the defect is **aesthetic, not owner routing**. They
called out the pasted-on gold line and the overall appearance of a collage of
cutouts rather than a coherent Heroes III dialog ("MS Paint"). Compare the
rendered screenshot with their earlier mock `https://i.imgur.com/j1G5Qzi.png`
and their clearer target `https://i.imgur.com/8nKTXds.jpeg`: one continuous
leather surface, ornate outer border, and individually recessed native-looking
portrait/crest, slider, and amount wells, without full-width gold seams.
Rework the frame, panel transitions, owner emblems, slider, amount fields, and
footer as one native-looking leather/red/gold composition; remove stray
divider lines and excessive blank space. Preserve working transfer behavior.
Rebuild, inspect an actual render, and obtain playable/user confirmation before
marking the visual defect resolved.

2026-09-28 source revision: removed the repeated decorated `GPUCRDIV` center
strips that produced the full-width gold seams. The revised split background
uses the continuous native `DiBoxBck` leather, retains the original ornate
outer frame and creature art, and gives the owner markers, slider, and amount
fields individual recessed wells. Fallback owner labels fit above fixed
controls without shifting their backgrounds. The focused split/garrison source
guard passes; both changed client C++ translation units compile in the main
worktree, and the complete `vcmiclient` target builds in the isolated clean
Linux UI checkout with only these UI changes applied. This is **not yet** a
rendered visual acceptance or a promoted playable update; the existing
launcher snapshot remains unchanged.

The first unpromoted candidate snapshot `51fd276eb69c29a2ade1c021fddfaf22f3a05f84f23d593bfcd7692b3109bd3a`
passed build/freeze but failed an isolated All for One runtime smoke: repeated
"Hero spell unavailable under authoritative target validation" messages
occurred during AI turns, with schema warnings as well. This candidate is
retained only for diagnosis and must not be promoted; the previously selected
snapshot remained active at that point. The visual source change has not been blamed for
unrelated spell/AI errors, and no screenshot of the revised dialog exists yet.

2026-09-28 follow-up: an independent Astra review found owner-well height and
control spacing risks; both were corrected. The revised Linux client built
successfully, then an isolated 35-second All for One smoke observed 46 AI turn
starts and no server problems, crashes, or unavailable-spell messages. The two
`mageGuildGeneration` schema warnings also occurred with the former promoted
snapshot and are not attributed to this UI change. Froze and promoted immutable
snapshot `3edad4fb06c63d59128fa1546ed4b8ad94a5831f81a3a3d5cd075aef568b7caf`;
`play-new-horizons-linux.sh --verify-only` resolves it. The user's already
running process was not touched. The new dialog is now playable for review,
but an actual rendered split-dialog image and user aesthetic acceptance are
still pending, so UP-025 remains open.

2026-09-28 target-image refinement: the user supplied
`https://i.imgur.com/8nKTXds.jpeg` as the cohesive Heroes III reference.
The current source now mounts the two creature images in narrow beveled frames,
and gives the actual owner emblems, slider, amount fields, and native buttons
individual recessed wells on one leather field. The short amount wells leave a
leather gap above the buttons; repeated full-width gold dividers are absent.
The client/library build and focused split source guards pass, and independent
Astra source review found no geometry or callback blocker. That review still
flags a possible leather-texture join and double-framed button look, both of
which require an actual rendered split-dialog screenshot. This revised UI has
**not** been frozen or promoted; the prior snapshot remains the playable one.

2026-09-28 private rendered checkpoint: the current unpromoted combined-source
client was frozen as candidate
`344129b2c0a7aa3ce8591fce4d0c2a0d91cc2b34bea28f3dd2dd59bb78150fae`
and launched on an owned private Xvfb display with purchaser assets and a fresh
profile. Its actual `Split Imps` dialog was captured at
`/tmp/nh-split-dialog.YzRRHW/split-dialog-actual.png` on the installed
Arrogance scenario, without touching the host desktop or user saves. The
capture shows the pasted full-width gold center dividers are gone; creature
art, two hero-owner portraits, slider, amounts and buttons are visible on a
single leather field at game scale. A narrow texture transition below the
creature art and native buttons within larger wells merit user aesthetic review.
The candidate is **not promoted** and the screenshot is not user acceptance;
the prior selected snapshot remains the playable default.

2026-09-28 combined-source smoke after the schema repair: a fresh private
headless `All for One` run reached 12 turn starts without the prior category or
magic schema warnings, but the client exited with signal 11 while the AI was
finishing tan's day-four turn. A second fresh-profile run reached 24 turn
starts in the 25-second bound without a crash, yet emitted an authoritative
`Leadership limit exceeded` server problem during an AI battle. These are
distinct observations, not proof that the visual change caused either issue.
They block promotion of this combined-source candidate; the previously
selected playable snapshot remained unchanged at this checkpoint. Preserve both private logs at
`/tmp/nh-schema-smoke.D8MyWU` and `/tmp/nh-schema-smoke-repeat.2BBvhT` for
diagnosis. The split-dialog render itself remains a provisional visual check.

2026-09-28 visual-only playable delivery: applied the same two UI source files
(SHA-256 `b86afb477e8a7ccaac5ee47881732ca4d990f759ec3ddc03bb1c26e2b706f176`
and `a1a7afe652fbad24ddfd845afcab9c8043aa7e6130f0e67ca8d91e58404d1204`)
to the detached committed `8c4ad7e5` source line, leaving the unrelated dirty
mechanics out. The incremental Linux `vcmiclient` build and all three split/
garrison source guards passed. Froze snapshot
`107947d37280117049ec8573081cf226fb9dee4e958729c9fb02ec7f4ab696b3`;
a fresh-profile, headless `All for One` run reached 49 turn starts in 35
seconds, exited only on the bounded timeout, and logged no server problem or
crash. Promoted that exact snapshot; `play-new-horizons-linux.sh --verify-only`
resolves it. This delivers the UI refinement for user review but does not
assert user aesthetic acceptance or deliver unrelated in-progress mechanics.

2026-09-28 schema-warning follow-up (validation-only; no UI or gameplay source
change): the private profile log at
`/tmp/nh-split-dialog.YzRRHW/profile/cache/vcmi/VCMI_Client_log.txt` records
the category warning at lines 521–530 and again under merged settings at
11986–11999. `newHorizonsCreatureCategories.json` used string `pattern`, which
this engine's `JsonValidator` reports as `Not implemented entry in schema` and
then rejects; the existing `CreatureCategoryRules` runtime parser already
requires exactly one non-edge colon for each growth-line member. The same log's
magic warning at lines 35068–35090 and 35246–35257 came from a core-scoped
`gameSettings.magic.newHorizons` object whose children remain New Horizons
scoped: `required` under `not` treats absent `factionWeights` as satisfied for
the core object, so the schema rejects otherwise valid v2/v3 rules. Removed
only the unsupported category pattern and the v2/v3 schema `not`/`required`
combination; `newHorizonsMagic::validateRules` continues to reject simultaneous
fixed Mage Guild generation and faction weights. Added mixed-scope named and
`gameSettings` wrapper regressions plus a malformed growth-member case proving
runtime rejection. With dirty worktree atop `8c4ad7e5f253b5596f12e5743fb931909fb7139d`,
`build/new-horizons-linux/bin/vcmitest` passed 30/30 focused category schema,
category runtime, v2/v3 named/wrapped schema, and Mage Guild runtime tests.
The isolated XDG profile was `/tmp/nh-schema-validation.evGjfS`; the native
test run did not launch a game or verify a post-fix client log. No candidate was
frozen or promoted for this schema-only follow-up.

The current split/transfer dialog places ownership wording behind the creature
art, so it is clipped and hard to read. Follow the mock's visual direction:
identify the hero side with its portrait and the garrison side with its banner
or crest, beneath the corresponding creature art. The user explicitly said the
extra wording is unnecessary if the visual identification works. Keep both
amounts, slider, confirmation and cancel controls usable, preserve the Heroes
III leather/red/gold presentation, and handle hero-to-hero or other army
pairings without misidentifying either side. Do not change authoritative
transfer behavior as a layout workaround.

Acceptance: focused source/UI checks plus rendered inspection show both owner
markers visible, correctly aligned, and unobscured at the actual game scale;
left/right amounts and controls remain legible and functional. Record exact
candidate build and playable confirmation separately.

2026-09-27 source checkpoint: built-in hero portraits and player crests now
identify the two sides beneath the creature panels. Names appear only when a
marker is unavailable or two distinct armies share the same marker; long names
are width-bounded with full text on hover/right-click. The installed 298×337
`GPUCRDIV` art is recomposed at runtime into a player-colored 298×440 dialog
with its original title, side rails and footer. The lowest button ends at y391,
above the y403 footer. No extracted original art is committed. The split and
garrison routing source guards and `git diff --check` pass; independent Astra
source review found no remaining blocking issue. C++ target build and actual
rendered/input acceptance are still pending.

### UP-024 — Universal Blacksmith inventory and Stronghold Ballista Yard

Status: Implemented (rendered/playable verification pending); assigned
2026-09-27. Canonical Markdown integration, source implementation, focused
native verification, and commit/push are complete. The in-game shop and weekly
effect still require a playable acceptance check.

Every town Blacksmith must sell every ordinarily purchasable War Machine. Towns
retain economic identity through price rather than exclusive inventory: a
machine historically associated with that town is cheaper there, while the
other machines remain available at their ordinary configured prices.
Do not expose the siege Catapult as ordinary shop inventory unless the canonical
War Machines rules explicitly make it purchasable. Put the price table in data,
not UI conditionals or repeated hardcoded faction branches; numerical price
tuning is provisional under the fun-first contract.

Stronghold's Ballista Yard retains its canonical visiting effect: the visiting
hero gains +20 Siege until the end of the current week; revisiting refreshes but
does not stack it. Its Ballista sale must coexist coherently with the universal
Blacksmith inventory rather than creating a duplicate item or charging the hero
twice. Human UI, AI purchasing/valuation, authoritative affordability and
inventory, save/load duration, descriptions and logs must agree.

Acceptance: the canonical Markdown records the universal-inventory and price-identity
rule; all nine towns expose the same ordinary War Machine set with the correct
data-driven faction prices; Stronghold Ballista Yard grants exactly the saved
weekly +20 Siege effect; focused authoritative/UI/AI/save tests and an exact
target build pass. Playable and rendered shop acceptance remain separate.

2026-09-28 Phase 1 source/native checkpoint: saved capability ruleset v4 defines
the three ordinary machines and all nine faction price identities. Town offers
deduplicate Blacksmith/Yard stock, server purchase and client/Nullkiller use the
same quoted price, and the Yard's weekly +20 Siege refreshes without stacking.
Both Linux `vcmitest` and `vcmiclient` link; the active-profile combined focused
filter passes 17/17 across this and the Regeneration slice, including the
authoritative shop/refresh case. Client geometry and AI source guards pass.
Independent review's building-under-visitor and UI saved-rules-gate findings
were repaired. This is not rendered/playable shop acceptance; keep UP-024 open
for that evidence and record broader AI spending/week-boundary interactions for
Phase 2.

Source checkpoint `e6545354a` was pushed to `origin/definitive-mvp` on
2026-09-28; the worktree was clean afterward. This is source delivery, not
playable snapshot promotion.

### UP-023 — Complete all missing Skills, perks, and spells before further art

Status: In progress; reprioritized by the user on 2026-09-27 ahead of the
Fortress faction-completion lane and nonessential artwork.

Finish functional gameplay breadth for every canonical Skill, every rank effect,
all ten perks per Skill, and every canonical spell. Work in dependency-safe
vertical slices, but do not substitute catalogue activation, descriptions,
borrowed icons, or isolated formulas for working mechanics. Each slice requires
authoritative execution, legal acquisition/progression, Battle/adventure AI as
applicable, save/network compatibility, UI/status/log feedback, focused tests,
independent review and target-build evidence. Remove or disable legacy spell
acquisition routes that contradict the canonical roster. Purpose-made provisional
art remains required when an active surface cannot function without it, but
polish and final-art replacement follow functional completion.

Acceptance: a requirements matrix accounts for every canonical Skill rank,
perk and spell with implementation and evidence status; no entry remains merely
planned or inert; AI can use and respond to every relevant mechanic; target
builds and focused native tests pass; unresolved rendered/final-art acceptance
is tracked separately and does not conceal gameplay gaps.

2026-09-28 Phase 1 coverage direction: use the canonical Markdown Version 1.0
specification and the coverage matrix as the implementation ledger. Missing
features outrank exhaustive revalidation of working features. Apply focused
build/mechanic checks and record non-blocking interactions for Phase 2; move
through independent missing items with separate worker file ownership.
For Storm of Daggers specifically, inspect existing spell-effect animations
before choosing a multi-target presentation. Reuse one only if it reads
clearly as the intended dagger storm; otherwise create a new purpose-made
animation (including provisional art via the HoMM3 art workflow). Do not
ship an unrelated effect merely to avoid animation work.

2026-09-28 Holy Wrath source checkpoint: the missing Level-3 Light spell has
an active roster and registered single-enemy definition, saved-v3 School-rank
Spell Power scaling, an Inferno-origin/Undead damage bonus applied before the
ordinary per-source damage cap, and an original purpose-made provisional
icon bound to its book/scroll and battle roles. The separate scenario-bonus
image remains an unrelated placeholder. The canonical source clarifies the
classification and cap order. Python content checks pass 34/34 and the module
mirror check passes. The Linux native target built; 10/10 focused authoritative
cases and 1/1 actual BattleEvaluator choice/forecast/cast case passed, and root
re-ran all 11 together with zero skips and exit 0. Independent review found
the cap defect and confirmed its source repair. Save roundtrip, in-game
rendering, and playable delivery are not yet claimed; under Phase 1 these
non-blocking checks no longer hold up the next missing feature. This does not
close UP-023 or Bulwark's Deep Bulwark gap.

2026-09-28 Adventure Spell acquisition checkpoint: the shared Guild I–V
town-owned purchase path now covers Summon Boat, Water Walk, Town Portal, Fly,
and Dimension Door. The server validates owner/turn, built Guild tier,
eligibility, duplicate state and affordability before charging; persistent
town unlocks teach current/later visiting heroes. Client Mage Guild controls
and Nullkiller purchase requests use that command. The Linux `vcmitest` and
`vcmiclient` targets link; 6/6 focused server/AI cases and 1/1 packet
round-trip pass in an isolated New Horizons profile, and the client source
guard passes. Independent Astra review found no blocking authority or
serialization issue. Rendered purchase/playable delivery and each spell's
effect-completeness audit remain open; this advances ordinary acquisition
coverage, not all of UP-023.

Durable matrix: `docs/NH_FUNCTIONAL_COMPLETION_MATRIX.md`. Update it whenever a
slice changes catalogue, implementation or evidence status; do not infer
completion from an `active` marker.

2026-09-28 Nature Regeneration checkpoint: the Level-1 spell and Basic
Herbalist perk now have authoritative wound marking/healing, saved fixed-point
state, client status feedback, purpose-made Provisional art and a bounded
BattleAI projection. Independent review caught casualty-mark transfer and
repeated AI forecast healing; both were corrected. The final active-profile
focused filter passes 17/17 combined cases and both Linux targets link.
Regeneration advances spell coverage to 34/67 and perk activation to 96/310;
it does not close UP-023. Rendered/playable status and broader dispel/save
interaction checks remain separate.

2026-09-28 Nature Poison source checkpoint: the separate
`new-horizons:poison` hero spell now has a saved-v3 Nature Level-2 roster row,
7-Mana cost, legal single-enemy targeting, authoritative physical-Poison state,
three escalating activation ticks, Cure/Dispel distinction, BattleAI valuation,
and purpose-made Provisional icon. The original `core:poison` creature ability
is not reclassified or replaced. Both Linux `vcmitest` and `vcmiclient` link;
offline content checks
pass 47/47. A fresh isolated TEST preset with New Horizons active passes the
eight focused authoritative/AI Poison cases with zero skips; the saved-v2
roster exclusion and adjacent Magic Arrow AI regression each pass 1/1. The
source count is now 35/67 combat-spell identities, not 35 verified spell
mechanics. Hero-source kill credit and broad interactions remain deferred.

2026-09-28/29 Spellcraft checkpoint: Basic efficiency now has a saved-v3
110% factor and a live authoritative/forecast/UI path, composed exactly with
School rank. The Basic rank is active; Advanced/Expert formulas are covered but
their registry status remains planned until prerequisite Spellcraft perks make
normal advancement possible. Linux client/test targets link, the active-mod
focused filters pass 15/15 and 32/32, and offline data checks pass 64/64.
Independent review's Focus Magic mismatch was repaired. Old-v3 Summon/Sacrifice
semantics and representative Lua Spellcraft execution remain Phase 2 checks;
rendered/playable delivery is still pending. UP-023 remains open.

2026-09-29 Spellcraft progression checkpoint: Basic Spell Penetration is
registered active and uses the shared spell-damage path to ignore 20% of a
hostile target's Magical Damage Reduction. Its selected perk state opens normal
Advanced Spellcraft progression; the already-implemented 120% Advanced rank is
registered active. The purpose-made four-state icon is Provisional. The Linux
client/test targets link, 4/4 focused native cast/prediction/progression/rank cases
and 17/17 perk-data cases pass, and the generated-module check passes.
Independent review found no Phase 1 blocker. The global active-perk art check
still fails on 21 earlier active perks without named icons; Spell Penetration
itself passes that check's source/runtime assertions. Cross-perk penetration
stacking and rendered/playable acceptance remain deferred. Expert Spellcraft
still needs an Advanced perk. This does not close UP-023.

2026-09-29 Empower Spell checkpoint: the Advanced Spellcraft perk uses the
post-Wisdom Mana cost threshold of 12 before separate battlefield surcharges
or discounts. Its 25% multiplier affects Spell Power-derived components in
the shared direct-damage, custom spell, generic non-damage, and timed-duration
paths; fixed bases and flat duration bonuses remain outside it. Selecting the
perk opens normal Expert Spellcraft progression, and the existing 130% rank
effect is now registered active. No new saved field was added; older v3
duration behavior remains gated. The purpose-made four-state art is
Provisional. Both Linux targets link; the final focused and adjacent spell
filter passes 69/69 native cases, 17/17 registry cases, 2/2 UI-inventory
cases, and the generated-module check pass. Independent review caught and saw
repairs for a Regeneration integer-overflow risk, old-v3 duration drift, a
tooltip typo, and Spell Lock saturation arithmetic.
The global active-perk art check still reports the same 21 older unmapped
perks; Empower itself passes its source/runtime checks. Five Warcasting tests
in a wider run throw at the pre-existing strict perk-tier guard because their
fixtures select Advanced perks without a Basic prerequisite; record that
test-fixture issue for Phase 2, not as Empower execution evidence. Mass Slow
variant and wider Lua interactions remain unverified. This does not close
UP-023 or establish playable delivery.

2026-09-29 Shroud Backstab checkpoint: the first Basic Shroud perk is active.
The selected perk adds +15 percentage points only to the existing rear-facing
physical melee flanking damage path; Basic and Expert rear attacks now gain
+40% and +75% total. No new saved combat state is required, and the shared
damage estimator feeds server resolution and AI candidate forecasts. The Linux
test and client targets link; 5/5 isolated active-profile Shroud tests pass with
zero skips. The perk/UI-inventory data checks pass 19/19, module generation is
in sync, and independent review found no blocking mechanic defect. The
purpose-made four-state icon is Provisional; in-game rendering and save/AI
interaction matrices remain unverified. Nine Shroud perks and the much larger
UP-023 list remain open.

2026-09-29 Hex of Pain checkpoint: the Level-2 Shadow spell is registered and
castable, with a three-round attack/retaliation trigger that applies captured
Spell-Power damage plus 10% of actual inflicted damage without recursive
attacks. The AI forecasts the reactive injury in attack and spell valuations.
The Linux client and test targets link; 6/6 focused active-profile authoritative
and AI tests pass, as do 36/36 content checks. Purpose-made 44/32/30-pixel art
is source-bound but Provisional. Native rendering and playable delivery remain
unverified. Painweaver's specified bonus to the Hex Spell-Power component is
still missing and remains an open UP-023 perk interaction, not a completed perk.
Phase 2 should check Hex versus Lucky Recovery: the current AI projection
resolves Hex before recovery, while authority resolves recovery first.
UP-023 remains open; the next missing Shadow identity is Frailty.

2026-09-29 Frailty checkpoint: the Level-2 Shadow spell replaces ordinary
core Weakness acquisition in new saved-v3 games while older saved rosters
retain Weakness. Each cast removes a percentage of intrinsic Creature Defense
for the battle; recasts accumulate to 60%, ordinary Dispel clears the bonus,
and selected Withering Touch adds five percentage points per cast without
raising the cap. The AI values projected allied physical-damage gains, and
the stack status shows accumulated strength without a round countdown.
Purpose-made spell and four-state perk art are source-bound but Provisional.
Both Linux targets link; 6/6 authoritative and 1/1 AI focused active-profile
tests pass, along with 37/37 content and 3/3 status-source checks. Native
rendering, saved-battle continuation, real AI selection, and playable delivery
remain unverified. Independent review found no blocking mechanic defect;
the two deferred copy/asset-inventory mismatches it found were corrected.
UP-023 remains open; the next missing Shadow identity is Plague.

2026-09-29 Plague checkpoint: the detailed canonical Shadow table makes it
Level 3 / 11 Mana; the older summary roster now agrees. The registered spell
has a saved three-round status, one end-of-turn tick/spread per infected stack
per battle round, WAIT exclusion, deterministic adjacent selection, and
caster-friendly fire. It affects nonliving creature types unless an actual
magical immunity applies. The battle status shows its icon and duration, and
the AI has a read-only first-spread valuation/selection hook. Both Linux targets
link; 6/6 authoritative plus 1/1 AI focused active-profile tests pass, as do
37/37 content checks. Purpose-made spell art is source-bound but Provisional;
Plaguebearer art exists but is deliberately unbound. Independent re-review
found no remaining blocking defect after fixing status expiry, extra-activation
ticks, and independent magical-damage reduction. Spell Penetration/Annihilator
on delayed ticks and wider propagation-chain AI forecast are Phase 2 findings.
Plaguebearer remains a distinct open perk: the canonical text grants one spread
beyond the "normal limit" without defining that base limit. A user choice is
pending; do not infer the perk's rule from base Plague. Native rendering,
saved-battle continuation, and playable delivery need separate evidence.
UP-023 remains open; the next missing Shadow identity is Soul Chain.

2026-09-29 Soul Chain checkpoint: the Level-3 Shadow spell is registered at
12 Mana with an ordered primary plus zero to two distinct secondary enemies.
The two-round, Dispel-removable links echo a saved percentage of actual
secondary damage onto the primary as nonrecursive Shadow damage. Saved
Shadow School/Spellcraft scaling affects only the Spell-Power term; the active
Soul Binder perk adds 15 percentage points after the 40% base cap. The
client has an explicit confirm/undo target selector and secondary/primary
status readback; purpose-made spell/perk art is source-bound but Provisional.
Both Linux targets link. Active-profile authoritative tests pass 5/5 and AI
cast-choice passes 1/1, all without skips; module sync and 38/38 content
checks pass. Source review found no blocking defect. Native rendering,
playable delivery, whole-battle save continuation, and broader interaction
validation remain separate; Phase 2 findings are recorded in the functional
completion matrix (active-chain attack forecasting, Spell Lock, primary
Dispel, and combat-log order). UP-023 remains open; the next missing Shadow
identity is Shadow Gift. Plaguebearer remains separately unresolved.

2026-09-29 Shadow Gift source/native checkpoint: the Level-3 Shadow spell and
Dark Gift perk are registered and implemented with an explicit 10/20/30%
choice, server-validated real HP sacrifice and battle-long maximum-HP cap
loss, a three-round per-victim Shadow spell-damage packet, a compact choice
modal, stack-status cues, and an AI cast-choice path. Both Linux targets link.
The active-profile focused filter passes 8/8 without skips (including cap,
healing, serialization, authoritative attack, AI tier choice and conservative
Phantom-integrity pricing); module mirror and 39/39 content checks pass.
Count as Phase 1 implementation coverage, not rendered or playable delivery.
The icon remains Provisional; native rendering and broader cross-system
interactions are recorded in the functional completion matrix. The prior
Soul Chain commit `176f63845` is pushed to `origin/definitive-mvp`.
Next missing Shadow identity: Vampirism. UP-023 remains open.

2026-09-29 Vampirism source checkpoint: the Level-4 Shadow spell and Advanced
Night Feeder perk have registered 15-Mana/three-round rules, authoritative
attack-and-retaliation lifesteal from actual damage, heal-only packets that
cannot restore casualties, an AI projection/cast-valuation path, stack status
feedback, and purpose-made Provisional spell/perk icons. The saved-v3 School
coefficient affects only the raw Spell Power term; Night Feeder adds 15 points
after the ordinary 50% cap. The Linux native `vcmitest` target links and all
15 focused Vampirism runtime/AI cases pass in an active New Horizons profile
with zero skips. The Linux `vcmiclient` target also links. The 57 focused
content/perk-data checks, three UI source checks, module-mirror check, and diff
check pass. Independent review found no blocking issue. Do not treat
source/native evidence as playable delivery.
Phase 2 findings: ordinary AI attack-choice valuation can undervalue healing,
and expiry, overkill, legacy live-cast rejection, and status save/load
continuation need broader deterministic checks. After this slice the next
missing Shadow identity is Re-animate. UP-023 remains open.

2026-09-29 Re-animate source/native checkpoint: the Level-4 Shadow spell and
Expert Reanimator perk now have saved-v3 registration, 16-Mana cost, a
species-neutral temporary-resurrection path, usable-remains/Disintegrate and
shield-aware target checks, casualty-only Reanimator scaling, AI target/cast
projection, combat logs, a generic Temporary stack indicator, and purpose-made
Provisional spell/perk art. Legacy `core:animateDead` remains classified but
inactive in new v3 snapshots; old saves retain their own roster. Both Linux
targets link. In the active New Horizons profile, 11/11 focused authoritative
and AI cases pass with zero skips; 58/58 content/perk-data checks, the 5/5 UI
source guard, module-mirror check, and diff check pass. Independent Astra
review found no production crash/corruption blocker. A discovered target-
legality discrepancy for Disintegrated casualties and temporary shield HP was
fixed before acceptance. Phase 2: verify full battle-result accounting with
an army-backed stack, interactions with other one-battle restorations,
Spell Lock/Dispel, and live save/load continuation. Native-resolution UI,
playable delivery, and final-art approval remain open. At that checkpoint the
next missing Shadow identity was Soul Reaper. UP-023 remains open.

2026-09-29 Soul Reaper source/native checkpoint: the Level-5 Shadow finisher
is active in saved v3 at 21 Mana. Its target-specific damage is 60 + 1.4 ×
Spell Power + 40% of missing aggregate HP; Shadow School/Spellcraft rank scales
only the Spell Power term. A post-mitigation hit leaving at most 10% of effective
maximum HP executes the surviving creatures, while ordinary remains and
Rebirth still apply. Authoritative cast, detached preview, AI evaluation,
and an explicit execution log line are wired. Saved v1/v2 snapshots cannot
cast it even if a new row is synthetically present. Linux `vcmitest` and
`vcmiclient` build; the active-profile Soul Reaper filter passes 9/9
server/AI cases with zero skips, curated-content tests 42/42, and the module
mirror check passes. Purpose-made Provisional 44/32/30 icons are bound. The
independent Astra review's lethal-damage regression, v2 gate and log-test
findings were fixed before acceptance. Phase 2 retains partial-resistance AI
valuation, broader status/save interactions, scenario-icon consumer sizing,
and native/rendered/playable validation. UP-023 remains open.

2026-09-29 Doom source/native checkpoint: the last detailed-roster Shadow
identity is registered and executable as a saved-v3 Level-5, 25-Mana,
single-enemy malediction. Its capped percentage penalty affects outgoing and
retaliation damage once, Initiative, and battlefield movement for three rounds;
Morale falls by three and Defense is unchanged. Shadow School and Spellcraft
scale only the Spell Power term. Recast refresh, expiry, friendly/multitarget
rejection, pre-v3 cast rejection, AI projection/resistance valuation, combat
logs, stack-status UI, and purpose-made Provisional art have focused source or
native evidence. Both Linux `vcmitest` and `vcmiclient` targets link; 8/8
active-profile server/AI cases pass with zero skips, the Doom status guard
passes 3/3, the content suite passes 43/43, and the module mirror is current.
The reviewer found no blocking production issue. Phase 2 retains Dispel and
save/load round trips, mixed Initiative/movement/Fortune effects, full AI cast
selection and combined exchange-score resistance valuation, plus rendered and
playable acceptance. The next missing detailed-roster combat spell is Light's
Sanctuary; UP-023 remains open.

User ordering clarification (2026-09-27): after the active Spell Lock and full
Archery slices, complete Bulwark of the Mire as the next full Skill slice before
War Machines or Command. Partial Mireborn source is not completion.

2026-09-27 Bulwark Basic checkpoint: Mireborn, Thick Hide, and Bog Ambush now
have authoritative physical-damage/reaction hooks, detached-state BattleAI
forecasts, Defend valuation, and status-panel feedback in source. The remaining
seven perks are still planned; do not call the Skill complete. Focused source,
data, and syntax checks pass. Exact-head Windows run `36360403677` at
`40628d29d92ab0d47282321fd411f5d079f38844` succeeded and published preview
artifact `10945274902`. Native Bulwark test execution, rendered status-panel
behavior, and playable confirmation remain pending.

2026-09-27 design clarifications for the remaining Bulwark perks: Toxic Spines
triggers once per Defending Bulwark stack per round; Immovable applies its first
physical-hit reduction only while that stack is Defending. These user choices
are integrated into the repaired canonical Markdown and recorded in the
migration audit. Toxic Spines additionally has an approved reflection-based
three-activation physical Poison potency and nonstacking stronger-refresh rule;
it must not reuse legacy magical Poison. Deep Bulwark must not be counted complete merely because a
generic immunity helper exists: verify an actual nonmagical forced-displacement
path and AI response before activation.

2026-09-27 Poison application decision: an equal or stronger physical Poison
application replaces the existing potency and restarts all three ticks; a
weaker application is ignored. This applies across different Bulwark sources
and does not create simultaneous Poison instances.

2026-09-27 advanced-slice review hold: runtime and AI source for Vengeful Mire,
Shared Cover, Mire Grip, Swamp Renewal, Immovable, and Toxic Spines is present
but not activated. Independent Astra review found blocking seams: automatic
creature activations bypass the new start-of-turn effects; projected Cure cannot
remove physical Poison; AI Mire Grip expiry/collateral triggering diverges;
Swamp Renewal AI values dead-creature HP and its runtime log/test disagree; and
Poison AI valuation uses raw HP on a different score scale. Repair these before
data activation or a build claim. Deep Bulwark still lacks an actual nonmagical
forced-displacement path. Native tests and performance-bound Defend evaluation
are pending.

2026-09-28 current-source re-audit: physical Poison's Cure handling and
Swamp Renewal's survivor-HP AI clamp are now present, but the advanced perks
remain planned. `makeAutomaticAction` still bypasses the Poison/Mire Grip/
Swamp Renewal start-of-activation hook; Toxic Spines AI values future Poison
on a mismatched scale; Mire Grip AI omits collateral damage; Shared Cover and
Vengeful Mire status hints omit their perk adjustments; Deep Bulwark has no
nonmagical forced-displacement path. An isolated runtime/test repair for the
shared automatic-activation gap is in progress. Do not activate all seven
based on this partial source work.

2026-09-28 automatic-activation source checkpoint: automatic creature actions
now enter the same authoritative start-of-activation hook as ordinary turns,
covering physical Poison ticks, Mire Grip expiry, and Swamp Renewal. A lethal
Poison tick stops the automatic action. Focused regression cases cover all
three effects, including the full rendered renewal log line and lethal Poison;
both changed C++ translation units passed syntax checks and an independent
Astra source review found no blocking issue. Native execution and a matching
target build are still pending, so the advanced perks remain planned and the
other reviewed Bulwark gaps above remain open.

2026-09-28 native activation follow-up: the full current Linux client/library/
test targets link. An isolated TEST profile with New Horizons active passes
eight focused native regressions for ordinary/automatic physical Poison,
lethal automatic Poison action suppression, serialized status clearing on
death, ordinary/automatic Swamp Renewal (including the complete rendered log
line), and ordinary/automatic Mire Grip expiry. The lethal death-packet state
was a real production defect and is now resaved after status clearing; the
other initial failures were fixture observation/tier-progression errors.
Independent Astra review found no blocking issue in the final source. The
seven advanced Bulwark perks remain planned; this is only their shared
activation prerequisite, not the complete Skill or a playable promotion.

2026-09-28 Mire Grip AI parity checkpoint: a bounded two-file projection/test
revision compiles, but its two new focused native cases pass 0/2. In the first
case the trigger is detected, then the projected attacker dies before the slow
is applied; the collateral-only test still fails its trigger assertion despite
positive forecast damage and visible Bulwark ownership. The attacker-side AI
callback correctly conceals the opposing hero, so the direct projection tests
use the owner-visible view; this does not prove omniscient attacker AI behavior.
An independent diagnosis is in progress. Do not activate Mire Grip or describe
the seven advanced perks as complete while these cases remain red.

2026-09-28 Mire Grip AI repair follow-up: the initial failures exposed two
invalid fixtures (retaliation blocked on the defender; Defending set before
`beginCombat()` reset it) and a real hypothetical expiry mismatch. The AI
forecast/exchange now use the authoritative `ONE_BATTLE` Bulwark source and
marker, while `HypotheticBattle` expires both only at a real creature
activation after Poison and before Renewal. The per-victim trigger also
requires an ordinary creature attacker. The incremental native `vcmitest`
build succeeded, and all three focused cases pass in an isolated TEST profile.
They cover direct and collateral triggering, same-activation suppression,
retention through rejected actions, ordinary Orders, round rollover and hero
spell continuation, Second Wind expiry, reapplication and live-state
immutability. Independent Astra source review found no blocker. This repairs
one AI seam only; hidden opposing perks remain hidden to attacker-side AI,
other advanced Bulwark gaps remain, and none of the seven perks was activated.

2026-09-28 Toxic Spines AI valuation follow-up: the detached forecast now
converts the positive residual physical-Poison tick damage through
`calculateDamageReduce`, matching the AI-value scale already used for immediate
reflection rather than adding raw HP damage to the score. The focused native
Toxic Spines case linked and passed 1/1 in an isolated New Horizons TEST
profile after its defender-owner view was corrected; it asserts converted
score, state/tick and live-state immutability. This removes one AI blocker but
does not activate Toxic Spines or resolve the remaining status/Deep Bulwark
gaps.

2026-09-28 Defend-status parity slice: the client tooltip now computes Shared
Cover's effective reduction only with an adjacent same-side ordinary
Defending creature and displays the capped adjustment; Vengeful Mire appears
only in melee reflection. The private-hero visibility guard remains. The
current `vcmiclient` target built successfully (97/97), nine focused UI source
checks pass, and the scoped diff is clean. This is build/source evidence, not
a graphical-playable check or activation of the seven advanced perks. Deep
Bulwark and other runtime/AI work remain open.

2026-09-28 six-perk source activation checkpoint: Toxic Spines, Swamp Renewal,
Mire Grip, Shared Cover, Immovable, and Vengeful Mire are active in the
production perk registry and embedded module. Deep Bulwark remains planned:
there is no implemented nonmagical forced-displacement producer for it to
counter. The isolated New Horizons test profile passes 11/11 focused runtime
cases and 8/8 focused BattleAI cases; both fixtures use production perk status
instead of overriding it. An independent Astra source review found no blocking
activation issue. The broader Bulwark regression passes 53/53 after seven
older fixture corrections. Toxic Spines still needs persistent client
physical-Poison status feedback, and actual rendered/playable validation,
target-package build, commit, and push remain pending. Do not call the full
Skill complete or claim the current play script includes this source.

2026-09-28 physical-Poison client feedback checkpoint: the stack status panel
now reads the serialized physical-Poison state, shows remaining activations
and the authoritative next tick, and refreshes on application, ticks, Cure,
and expiry. Time Stop and Spell Lock retain status priority; hidden overflow
is disclosed. The Linux client and focused native UI test link and pass,
the Python status guard passes 11/11, and independent Astra source review
found no blocker. The Poison icon reuses the classic SpellInt frame; it is
not purpose-made Toxic Spines perk art. Native-resolution rendering,
playable delivery, and Deep Bulwark remain open.

2026-09-28 Cure/physical-Poison integration defect: an isolated native case
reproduces server rejection when a full-health stack has only Toxic Spines'
serialized physical Poison and the hero explicitly selects Poison for Cure.
New Horizons preflight and target selection recognize the affliction, but
legacy effect applicability sees no bonus or wound and rejects the cast before
the existing server-side poison-clear packet can run. The authoritative Cure
path now accepts a validated explicit affliction without requiring legacy
bonus applicability. Selector-free healing requires an injured surviving
creature, not merely casualties below the stack's original total Health.
The Linux `vcmitest` target links and all 24 focused Cure cases pass with
zero skips under an isolated New Horizons profile, including physical-only
and combined Poison, invalid selector no-spend, casualty no-op rejection, and
Spell Lock rejection. This is source/native evidence, not a playable claim.

### UP-022 — Complete the Fortress faction implementation

Status: Open; paused at a preserved uncommitted Fortress-growth checkpoint when
the user reprioritized complete Skill/perk/spell implementation on 2026-09-27.
Resume after UP-023 unless a Fortress mechanic is a direct dependency of that
functional completion lane.

Finish the Fortress faction against the complete canonical Markdown scope rather
than treating one visible subsystem as faction completion. Audit and implement
Fortress heroes/classes/specialties and biographies, creatures and faction
data, town buildings and prerequisites, the faction Skill and every one of its
perks, interactions with global Skills/spells/Orders/Leadership, Battle and
adventure AI, UI/log/status presentation, provisional HoMM3-style artwork, and
all Fortress-specific acquisition/progression rules. Reconcile every canonical
Fortress requirement with source, tests, target builds and playable evidence;
record genuine design ambiguities instead of silently inventing rules.

Acceptance: the completion audit and sprint register contain a granular
Fortress requirement matrix with authoritative evidence for every item; all
implemented entries have focused authoritative and AI coverage, generated
content is synchronized, active assets satisfy the art/provenance guards, an
independent review is clear, an exact pushed commit builds on the target route,
and playable/in-game acceptance remains explicitly separate where still needed.

### UP-021 — Fix Shift stack split/combine crash and Leadership-aware combining

Status: Reopened by playable last-stack transfer defect on 2026-09-27. The
original crash repair is playable-confirmed and the empty-slot/split-label
follow-up is Windows-build verified, but transferring the complete final hero
stack into a garrison can still reach the server with no legal positive split
amount and emit `No creatures to split` as a server problem. Exact-head
dependency/source preflight run 36332113616 passed for commit `be8cb13a5`;
full compile/package run 36333365693 succeeded and uploaded artifact
`10938170495` (617,643,648 bytes). The user confirmed that the original split
crash no longer occurs in that playable build. The empty-slot and split-label
follow-up now also has exact-head Windows compile/package evidence: run
`36341858040` succeeded at `70117e251a5fcf5f2163adbfb8be94626a57b56a`
and uploaded artifact `10940446726` (621,090,196 bytes). Rendered labels and the
new partial empty-slot behavior still require playable acceptance.

2026-09-27 crash evidence: the user supplied
`VCMI_client.exe_crashinfo.dmp` (SHA-256
`8b7527f3e2970ffebb43e1ba580314dc0bd41ba1f6abeae140b22365c69205ee`),
created by exact Windows artifact `6948b1aa56df3358febe86cd48017552ca1fe735`.
The dump records an unhandled MSVC `std::runtime_error` on the main thread.
Binary metadata and the throw-site strings identify
`WindowBase::close()` and its "Only top interface can be closed" guard. The
reproduced control flow is concrete: `CSplitWindow::apply()` invokes the split
callback; an over-capacity Leadership check pushes its explanatory info dialog;
then `CSplitWindow::apply()` attempts to close the split window even though it
is no longer the top window. This confirms that positive Leadership overflow
can trigger the reported crash. The uploaded client log begins with the user's
subsequent run, thirty seconds after the dump, so it is not treated as the
crashing session's event log.

Shift-splitting a creature stack in order to combine it into a hero's army can
crash the game, possibly when the resulting stack would exceed the receiving
hero's per-slot Leadership capacity. Reproduce from the newest relevant log/save
when available, trace both client split/merge request construction and
authoritative server validation, and fix the crash without bypassing server
authority or weakening Leadership limits.

As a quality-of-life rule, a combine operation must transfer as many creatures
as legally fit in the destination stack under the receiving hero's current
Leadership capacity. If the source contains more, combine only the legal amount
and leave the remainder in its source slot; if none fit, leave both stacks
unchanged and provide a precise explanation. Never delete creatures, create an
illegal transient army, overflow counts, or depend on the UI prediction for
validity. Apply the same authoritative behavior to every ordinary stack-combine
route that shares this operation, including AI use where applicable.

Acceptance: focused tests cover exact-fit, partial-fit, zero-fit, empty-slot
split/transfer, Shift split-dialog confirmation, same-army and cross-army hero
exchange, no-Leadership-limit/legacy rulesets, last-stack constraints, invalid or
stale requests, state/network/save identity where applicable, and no mutation
on rejected actions. Client UI previews and explanations agree with the server;
independent review and an exact target build pass before playable promotion.

2026-09-27 playable follow-up: dragging a whole garrison stack into an empty
hero slot still requested an exact full-stack swap, so an over-capacity stack
was rejected instead of filling the empty slot to the receiving hero's current
Leadership capacity. Repair both the client fast path and authoritative empty-
slot swap path so the legal maximum moves and the remainder stays in the
garrison. The split dialog must also label its left and right armies explicitly,
using `Hero: <name>` and `Garrison: <name>` (with accurate equivalents for other
army pairings), so the player can tell which count belongs to which side.

2026-09-27 source follow-up: the client now permits an over-capacity whole-stack
move into an empty hero slot as a server-authored partial-transfer intent. The
server calculates the receiving hero's current per-slot capacity, moves exactly
that many creatures through the normal validated `RebalanceStacks` path, and
leaves the remainder in the source garrison. Missing armies and two-empty-slot
requests reject safely. Focused server regressions establish a legal visiting-
hero exchange, use the UI's destination-first orientation, check conservation
and response status, and cover the stale two-empty request. The split dialog now
retains and renders explicit left/right owner labels. Its source guard and the
existing callback-lifecycle guard pass, and an independent Astra source review
found no remaining logic blocker after two test-fixture corrections. Native,
exact-head Windows, rendered-label/localization, and playable verification are
still pending; the old promoted package does not contain this follow-up.

2026-09-27 source result: `CSplitWindow` now snapshots its callback and amounts,
closes first, and invokes the callback afterward, eliminating the dump-confirmed
top-window exception. Ordinary combines send explicit merge intent and the
authoritative server transfers the largest legal count, leaving excess and any
required last source creature in place. Numeric split requests remain exact;
the client normalizes legitimate reverse rebalancing into a positive request,
while the server rejects malformed negative/stale counts and accepts a true
zero-delta no-op without mutation. Focused server tests cover zero/partial/exact
fit, cross-hero last-stack retention, bulk partial merge, malformed/stale numeric
requests, over-cap rejection and legacy no-cap behavior. Two source guards cover
the confirmed window lifecycle and client routing. An independent Astra review
found and caused repairs for empty-slot exchange, ordinary last-stack routing,
reverse rebalance, and two test compilation defects; its final re-review found
no blocking source issue. Exact-head dependency/source preflight run 36332113616
passed; full compile/package run 36333365693 succeeded with playable package
artifact `10938170495`. Native/GUI and
playable evidence are still required before this item is Playable-accepted.

2026-09-27 playable last-stack follow-up: when the player tries to transfer the
complete last stack from a hero into a garrison, the runtime logs `No creatures
to split` and presents it as `Server encountered a problem`. Preserve the rule
that a hero may not be left without creatures. If the source stack contains more
than one creature, transfer the greatest legal amount and retain one creature
with the hero. If it contains exactly one, perform no mutation and show a normal,
precise gameplay explanation instead of issuing a zero-count split or surfacing
an exception/system-error message. Apply the same result to drag/drop, combine,
and split-dialog routes that share the transfer operation, with the server still
authoritative. Add focused regressions for one-creature zero-fit, multi-creature
last-stack partial transfer, stale requests, conservation and absence of an
exception/error response; obtain independent review, an exact target build and
playable confirmation before resolving this follow-up.

2026-09-27 source checkpoint: ordinary empty-slot last-stack moves now send a
whole-stack intent, allowing the authoritative server to reserve one final hero
creature and clamp the transfer to the receiving hero's current Leadership
capacity. Exact-one no-ops show the localized last-army explanation without a
zero-count split request; same-creature combines and Shift numeric splits keep
their distinct paths. Focused server cases cover exact-one rejection, all-but-
one garrison transfer, capacity-clamped transfer retaining multiple source
creatures, conservation, and stale source rejection. Garrison/hero exchange and
split lifecycle source guards pass. Independent Astra review cleared the server
logic and prompted correction of the final client routing gap. Native tests,
target build, and playable confirmation remain pending.

### UP-020 — Maintain a durable implementation sprint register

Status: Implemented as a living process; ongoing until New Horizons completion,
assigned 2026-09-27.

Maintain `docs/NH_IMPLEMENTATION_SPRINTS.md` as the durable answer to what is in
progress, what comes next, what remains, which dependencies apply, and which
evidence is still missing. Update it whenever work is selected, materially
changes state, is blocked, is committed, or gains native/playable/visual
evidence. Keep source implementation, native verification, playable delivery
and user acceptance distinct. The canonical Markdown remains gameplay authority;
the sprint register schedules work and must not invent or override design rules.
Build failures remain in `docs/NH_RELEASE_FAILURES.md` with their prevention
evidence. Acceptance is that a fresh agent can resume the real next task from
repository documents without relying on chat context.

### UP-019 — Activate Shield Master and integrate its perk art

Status: Windows build/package verified; focused native and playable verification
pending, assigned 2026-09-27.

2026-09-27 target-build checkpoint: exact workflow run `36322531152` completed
successfully at full head `6948b1aa56df3358febe86cd48017552ca1fe735`.
The Windows x64 client compiled, packaged and uploaded artifact
`New-Horizons-Windows-x64-6948b1aa56df3358febe86cd48017552ca1fe735`
(`10933193980`, 614,831,501 bytes). This closes the source-level Windows build
gate for Shield Master but not the focused gameplay tests, playable promotion,
or in-game Protect/interception and artwork acceptance.

2026-09-27 source checkpoint: Shield Master is active and Protect captures a
public one-or-two interception allowance when the Order is issued, so the
authoritative server, clients and opposing-side Battle AI share the same saved
snapshot without exposing a concealed hero. An exact 0..2 consumed count and
allowance serialize together; old boolean state normalizes to ordinary one-use
Protect, invalid shapes reject, and downsaving rejects even an unspent two-use
allowance. Authoritative three-strike coverage expects two redirected/reduced
hits and a third Ward hit; focused sources also cover ordinary one-use behavior,
ranged non-consumption, death/separation, round reset, packets, legacy saves and
AI replay/nonmutation. The Protect log and visible status report used/remaining
interceptions. Purpose-made provisional art retains its exact prompt, 1254x1254
master, 44x44/32x32 reductions, four runtime states, provenance and hashes. The
140 New Horizons Python tests, module check, JSON/CSV parsing, 73-icon active-art
guard, privacy scan and whitespace checks pass. An independent Astra review
found and prompted correction of two AI projection regressions and opposing-hero
visibility, then cleared the revised source. Native compilation/tests, playable
delivery and in-game visual approval remain pending.

Implement the canonical Basic Armorer perk end to end: Protect! may intercept
the first two qualifying melee attacks against its Ward each round instead of
only the first. Track and serialize the exact number of interceptions consumed,
with safe compatibility for older one-use saved battle state. The authoritative
server path, client-visible Order state, forecasts and Battle AI hypothetical
replay must share the same saved-snapshot-aware interception limit and must not
mutate the live battle while evaluating choices.

Acceptance: focused native tests establish two redirects/reductions and a third
attack reaching the Ward for a holder, ordinary one-use behavior for a
non-holder, no ranged consumption, broken/dead/separated pair behavior, exact
round reset, packet/save compatibility and AI replay parity/nonmutation. Update
the Protect combat log/status wording for the second interception. Activate the
catalog entry, regenerate/check the module and bind purpose-made four-state
HoMM3-style provisional art with retained source prompt, provenance and runtime
hashes. Playable delivery and in-game visual review remain separate gates.

### UP-018 — Activate Countercharge and integrate its perk art

Status: Source implemented; native and playable verification pending, assigned
2026-09-27.

2026-09-27 source checkpoint: Countercharge is active with its Basic Armorer
gate. Authoritative Brace damage and Battle AI valuation share one resolver that
adds 25 percentage points to Brace's pre-emptive multiplier and caps the perk's
result at 100%. The modifier is confined to Brace's marked pre-emptive hit;
ordinary attacks, retaliation and Bulwark's independent pre-emptive reaction are
unchanged. Focused sources cover the increase, cap, non-holder, actual server
reaction, separation from Bulwark/retaliation, a real Charge-versus-Brace AI
decision reversal, and a deep-copied active Brace Order carrying a genuine
Warcasting snapshot. Purpose-made provisional art retains the exact generation
prompt, 1254x1254 master, 44x44/32x32 reductions, four distinct runtime states,
descriptor and hashes. The 140 New Horizons Python tests, module regeneration,
JSON/CSV parsing, the 72-icon active-perk provenance/uniqueness guard and
whitespace checks pass. Independent Astra review found no material runtime,
compile/API or art blocker after its two evidence gaps were corrected. Native
compilation/tests, playable delivery and in-game visual approval remain pending.
Exact Windows preview CI run `36318766320` completed successfully at pushed head
`102220f8d54986ad6533b50c3f313d8bbc063fce`, including client compilation,
packaging and artifact upload; this is build evidence, not gameplay acceptance.

Implement the canonical Basic Armorer perk end to end. Countercharge increases
only the pre-emptive attack granted by Brace! by +25 percentage points of normal
damage, capped at 100%. It must not alter Bulwark or any ordinary, retaliatory,
or other pre-emptive attack. Authoritative combat resolution, displayed damage
forecasts and Battle AI valuation must share the same saved-snapshot-aware
calculation and must not mutate live state during hypothetical evaluation.

Acceptance: focused native tests establish the +25-point increase, the 100% cap,
unchanged behavior for heroes without the perk and no spillover to Bulwark or
other attacks; verify authoritative/AI forecast parity and save/load identity;
activate the existing catalog entry, regenerate/check the content module and
bind purpose-made four-state HoMM3-style provisional art with retained source
prompt, provenance and runtime hashes. Playable delivery and in-game visual
review remain separate gates.

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
five findings were corrected. Exact Windows preview CI run `36315781168` built,
packaged and uploaded head `2663c1b500e86208a15c1ca7d44fd9feeae51946`
successfully. Focused native test execution, playable delivery and in-game visual
approval remain pending.

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

Replace the canonical Markdown guild-generation rule and implement it: each faction
has two equal preferred schools. Levels I/II contain one spell from each preferred
school plus 3/2 spells from distinct non-preferred schools respectively. Levels
III/IV/V contain exactly one spell from each preferred school. Totals 5/4/2/2/2.
Select non-preferred schools uniformly without replacement, then eligible spells
uniformly within each school/level; no faction spell weights or duplicates.
If a required school has no eligible spell at that level, leave that slot empty;
never substitute a spell from another school.
Update New Horizons.md directly, not only Pending Changes. Preserve roster/map
eligibility, determinism, and non-NH gameplay. Verify rules and generation with
focused tests; distinguish source completion from playable delivery.

### UP-013 — Complete missing Mage Guild levels and artwork

Status: Implemented and delivered; visual verification pending.

2026-09-27 reconciliation: the retained evidence below proves the complete
supplied-art integration, focused native validation, seven-day headless smoke,
commit/push and promotion through the normal launcher at `42860ed29`. The five
offline asset/integration checks still pass against the current tree. No missing
source, export, binding, prerequisite or playable-delivery task remains under
this entry. It stays open only for an authorized rendered review and the user's
visual acceptance; do not regenerate or replace the supplied artwork merely to
make progress on that separate gate.

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

Status: Source implemented; native and playable verification pending.

2026-09-27 source-completeness reconciliation: a fresh canonical/runtime audit
found no remaining justified source change within UP-003. Spell Buffer resolves
either kind of outstanding Metamagic grant, including Grand's continuation,
before round cleanup; New Horizons Fire Wall passes its three-round base through
the shared Echoed Duration hook. Direct regressions cover Grand-expiry Buffer,
Fire Wall world-save duration/expiry, and isolated Battle AI obstacle ageing
without live-state mutation. Pending Changes is empty and the detailed canonical
DOCX rules match the active ten-perk pool. The focused native cases still require
target-platform execution, and playable/rendered acceptance remains separate.

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

2026-09-28 unrelated fresh-profile `All for One` smoke of the current
unpromoted combined-source build reached 24 turn starts in 25 seconds but
logged one authoritative Leadership-limit rejection during an AI battle:
the receiving hero could command at most 12 creatures at 60 Leadership each
with 760 Leadership. Its diagnostic log is at
`/tmp/nh-schema-smoke-repeat.2BBvhT/stdout.log`. This is a new reproducible
AI symptom, not a replay of the user's missing 45,829 ms turn save. A separate
fresh run exited with signal 11 after 12 turn starts; that cause remains
unattributed. Do not promote this combined-source build on these smokes.

Read-only 2026-09-28 trace: the AI accepted Cuthbert's wandering Halfling
`Followers` offer by answering BlockingDialog query 256 with `1`; the server
then emitted the 12-creature Leadership-cap complaint and opened a garrison
dialog. This was a QueryReply, not an AI-issued stack transfer. The current
`tryJoiningArmy` source plans a partial transfer, so the exact failing count
remains unexplained by the log. A focused accepted-`CGCreature` regression is
being added to the existing Leadership admission fixture before changing
authoritative behavior. The signal-11 run has no stack trace/core and no
Leadership complaint; the two symptoms have no demonstrated connection.

Focused accepted-offer tests now show the partial-join planner itself
conserves creatures: with no free place, the hero takes none and leaves two
Halflings; with one free place, the hero takes exactly one and leaves one.
The latter test also found a separate follow-up anomaly: a manual garrison
swap of that last remaining creature returned `PackageApplied=false` without
a captured Leadership complaint, whereas swapping a two-creature remainder
worked. Keep that last-creature/dialog-query path open for isolated diagnosis;
do not infer a fix to the AI-smoke rejection or signal-11 crash from the
partial-join evidence alone. The latest isolated native accepted-offer suite
passes 2/2 after narrowing its scope to the joining decision and source-object
conservation. No production code was changed for this trace; the separate
last-creature swap, AI-smoke rejection, and signal-11 crash remain open.

2026-09-27 blocker recheck: a read-only search across the available VCMI profile
save trees still finds no save newer than the September 21 `And One For All`
autosaves in the normal New Horizons profile. None is the reported match whose
logs contained 8,766 ms and 45,829 ms Nullkiller turns plus a Leadership-limit
rejection. The exact scenario therefore remains unavailable for faithful replay;
the unrelated saves were not launched or attributed to this regression. Continue
with other unblocked priority/canonical work until a matching save appears.

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
