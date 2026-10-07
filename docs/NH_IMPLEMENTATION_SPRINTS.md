# New Horizons implementation sprints

## Current checkpoint — 2026-10-07, initiative origin feedback

Phase1: UP272 adds required initiative-bar distinction for implemented extra
activations, not new scheduling rules or gameplay state. Root integrates the
default post-apply event through CPlayerInterface, saved/current-unit/round
readback and only the first queue entry; worker/tester ownership is separate.
Combined rebuild50608 passes with12 jobs after a retained label visibility API
failure. Four pure origin/reset/continuation cases pass4/4 in0.300s, zero skips;
source/module guards and independent review pass. Executed UI dispatch/locking
and native rendered acceptance remain Phase2. Coverage identities unchanged:
228/310 perks,82 planned,31/31 Skills,93/93 ranks,61/67 combat spells,8/8 Orders.
Full Field Workshop repair remains the next functional candidate pending its
destroyed-target scope decision; do not implement a machine-only substitute.
Windows37577480623 now succeeds on UP268's c338c671f; later UI is excluded.
Normal Linux snapshot and user-owned Cabir work remain preserved.

## Current checkpoint — 2026-10-07, required combat UI coverage

Phase1 continues. UP269's listed/current spell-cost stages and explicit follow-
up base are source/native verified (client/test builds,7/7 in2.472s); source
commit949cde69e is pushed. UP270 detailed real/effective Morale is implemented
(client build,6/6 shared cases in3.631s); commit6c73ed1e7 is pushed. UP271's
detailed target-neutral Luck/overrides/Sylvan feedback is implemented (client
build,7/7 focused cases in0.917s). Native checks establish shared producers,
not rendered widget execution. One extra Wild Chance fixture fails the earlier-
tier prerequisite before effect assertions; retain it for Phase2 repair/rerun.
No gameplay/state/art or mechanic identities change:228/310 perks,82 planned,
61/67 combat identities,31/31 Skills,93/93 ranks and8/8 Orders. Required UI
coverage increases. Normal Linux snapshot remains unchanged, and live Windows
37577480623 compiles older UP268. Next Phase1 work must follow the priority
queue and actual unimplemented canonical paths, not reimplement these accepted
consumers or treat all item-specific design holds as a whole-project blocker.

## Current checkpoint — 2026-10-06, magic handoff / Cabir correction

Perfect Rhythm source is committed/pushed as be78e0758416cabdffd537253fd9250e92a74393
with required author/committer identity. Full Windows run37565586139 is queued
on that exact source, dispatched once after prior37557751116 completed SUCCESS.
No Windows result or Linux promotion is inferred from the new dispatch.

Accepted Perfect Rhythm checkpoint supersedes the pending notes below: all
three builds pass, principal7/7 and activated7/7 native cases pass, adjacent11/11
pass, zero skips (2.065s/2.045s/2.259s). Three focused registry tests/module drift
pass and independent source/fixture review has no blocker. Registry active,
coverage228/310 (157/220 generic,71/90 faction),82 planned; Warcasting7/10.
No new persisted state or polling. Phase2 retains AI choice quality, rendered
UI and wider control/extra-action combinations; no playable promotion. Next
coverage slice must come from an actual ready item or a newly answered hold,
not repeating the now-inapplicable same-Expert-slot composition question.

Perfect Rhythm is the next implementation slice: the old Master Synthesis
composition hold is inapplicable because valid progression permits one Expert
perk per Skill. Shared candidate-action history/bonus helpers are source-frozen
and independently reviewed without a blocker; client build14693 passes. Focused
live/detached fixtures remain in progress, registry planned until acceptance.
No new serialized state, polling or completed-perk credit. Private validation
profile: testing/perfect-rhythm-20261006.5B6wPT1I under the Linux build root.
Both fixture files are frozen, with five live/detached cases and two pure state
cases; independent final review has no blocker. Test build37210 is confirmed
live with12 jobs. Log: build-test.log under that profile. Re-poll this exact
session before native execution or another build; current binary is stale for
these seven cases. Source remains planned/uncommitted pending native acceptance.
Separately, the stale specification hash in the perk registry is repaired and
module metadata regenerated; its previously failing identity test now passes.

Windows package37557751116 completed SUCCESS on
ce1b5547cf0207575b357f5e1e540de6bc6a2d23,2026-10-07UTC. Root inspected terminal
job status, packaging READY and finalized upload logs. Artifact11457695378 is
1,047,198,549bytes; uploaded artifact-container SHA256 is
`9bdd173632eee2ee0db5325140136d5a35b08c4cee4ce82b2b1aa3bcd342d64b`.
[Download artifact](https://github.com/thegandalf196/vcmi/actions/runs/37557751116/artifacts/11457695378).
The source difference from Last Stand10dc2428c is documentation-only. Thus this
package includes Last Stand, not the private generated walking studies. This is
compile/package/upload evidence, not an independently downloaded package audit,
Windows gameplay acceptance or Linux promotion. No duplicate dispatch needed.

Five-row Spellcraft readiness audit rechecks canonical clauses4433–4442 against
UP132/069/134/133/121. No new ready principal slice is established. Cross-School
multi-school relation, Concentration target-count policy and penetration
composition are now presented as three narrow user choices; awaiting actual
answers, not treating recommended defaults as approval. Extend Spell's terrain/
summon scope and Precise Casting's Time Stop/Earthquake scope remain held.
Accepted-cast conventions may remove older Counterspell questions, but that
cross-reference alone is not a ruling for these two perks. Refreshed planned-row
evidence now covers51 rows; no coverage or runtime change.

The rig-guided eight-pose Cabir art export is frozen privately. Root confirms
eight 72x72 GIF frames at 130ms; raw-cell integrity and pre-composite meaningful
alpha bounds pass. Independent visual review accepts only a provisional human
preview: return-half gait and torso/arm continuity remain incomplete. No runtime
installation, gait acceptance or coverage increase. Exact evidence is in UP265
and the asset register.

Bounded non-perk readiness audit finds no ready principal slice in its inspected
building/artifact/specialty set: Castle Lighthouse UP201 needs departure/duration
scope; Skeleton Transformer UP197 needs conversion rounding scope; Glyphs of
Fear UP200 needs aura geometry/overlap; regeneration artifacts UP207 need
per-item versus aggregate conversion. Existing building producers/minimum AI
paths must not be reimplemented or counted twice. This is not a claim that every
remaining Version1.0 item is blocked. Coverage remains227/310 active perks.
Windows37557751116 has completed compilation and resource staging and is now
confirmed live packaging the client, PE dependency closure and source notices.

Cabir technical producer now supplies a sampled eight-phase constant-length
cycle, evaluated mesh foot-plant checks, actual translated world motion and
local stride closure. Root's independent saved-blend probe and native56 review
support the sampled claims; independent reviewer finds no blocking math issue.
Visual fixed-root drift was corrected before acceptance. Interpolated playback,
whole-sole contact, finished Cabir art and runtime delivery are not established.
This advances the user-priority gait producer, not227/310 perk coverage.

Bounded follow-up audit checks seven previously unrefreshed rows: Defiant,
Veteran Cohesion, Heroic Spirit, Esprit de Corps, Iron Will, Crisis Command and
Seize Initiative. All have recorded principal scope/trigger/lifetime decisions,
not merely Phase2 hardening. Exact holds now replace vague index descriptions;
Esprit de Corps's retired UP152 reference is corrected to UP130. Combined46
planned rows have refreshed evidence; do not repeat their architecture audits
without new rulings. Coverage remains227/310; no new activation/build is claimed.
Windows37557751116 is still confirmed live in client compilation.

Windows notice preflight37556334450 completed SUCCESS on10dc2428c. Full package
37557751116 is confirmed live compiling the Windows client on ce1b5547cf;
the intervening source difference is documentation-only. No duplicate dispatch,
restart, success claim or Linux promotion. Cabir's original articulated
three-pose guide is frozen and validated; one generated contact is rejected and
the focused revision has opposite support but native56 confirms proportion and
camera drift. GenuineRGBA/source hashes and mechanical exports are recorded;
these private studies are not installed/full gait coverage. Next gait producer
needs shared Cabir proportions, not another independent same-camera claim.

Final uncertain-row pass inspects twelve more planned perk rows and all six
inactive base combat identities; exact recorded holds are restated in the hold
index. Combined39 planned perks have refreshed evidence. Existing producers
already cover structural damage, statuses, exact-HP summoning and nearest-legal
Polymorph relocation; rebuilding those does not complete the missing behavior.
No full ready slice is found in these audited sets without resolving material
recorded rules. Coverage stays227/310; do not invent policy or claim the rest of
Version1.0 is blocked from this limited table. Await the narrow presented choices
instead of repeatedly remapping the same seams. Windows preflight37556334450 is
confirmed live in dependency/source-archive validation on10dc2428c.

Last Stand source10dc2428c is pushed and remote-head verified with the required
identity. Prior Windows package37549855253 completed SUCCESS on b9fe600c4.
New notice preflight37556334450 is confirmed live on10dc2428c; do not restart
it on observation timeouts. Functional next-slice audits inspect specific
needs-review queue records in parallel, not assuming those labels mean blocked.
That bounded audit now restates27 exact canonical/queue holds in the planned
index. No new activation, broad tests or speculative partial implementation.
Remaining56 planned entries are not thereby declared blocked. Three small
pending choices can unlock Rapid Response, Mire Shaper and generic Serendipity;
record their actual answers before implementation.

Accepted checkpoint supersedes pending/failure notes below: Last Stand is active,
client/test build23204 passes; principal72648 passes13/13 and activated adjacent
30900 passes22/22, zero skips. Module drift/canonical-data pass and independent
review reports no blocker. Coverage227/310 (156/220 generic,71/90 faction),83
planned; Armorer8/10. Phase2 control/revival/composition remains recorded; no
normal playable promotion. Prepare scoped source commit/push. Cabir guided
study/revision are both rejected and uninstalled; no gait completion credit.

Latest Last Stand gate: client/test retry5034 passes after the defining
NewHorizonsHeroRulesFixture include repair. Native principal89965 runs12 cases,
7 pass and5 fail, zero skips. Keep inactive/coverage unchanged. Bounded fixture
and read-only runtime workers investigate final-state versus accepted-packet
timing, absent retaliation and Veteran descriptor history; do not weaken core
survival/termination assertions. principal.log/XML retain the exact failures.

Last Stand client retry49003 completed successfully. Root integrated stable
primary-first AI hit ordering after independent review; serialized client/test
build11858 is running against that source. Review identified a fixture-only
retaliation blocker (the acting attacker was given BLOCKS_RETALIATION); remove
that grant after the live build finishes, then rebuild before native execution.
Build11858 subsequently failed on a fixture-only typed SpellID source; corrected
that enum conversion and removed the retaliation-blocking grant. Incremental
client/test retry45899 is live. No completed coverage or playable delivery is
claimed from these build steps.

Next-slice evidence: UP159 Rapid Response is genuinely absent, not merely a
planned label. Its accepted activation-end seam is mapped, but immediate enemy
extra-activation precedence is unresolved; root requested that narrow ruling.
Do not infer all remaining Version1.0 work is blocked from hold-index labels.

UP079 implementation is underway with three nonoverlapping runtime, detached-AI
and fixture workers. Shared Armorer lethal cap/Defend builder, side-wide use and
activation-ended state are landing; root registers CMake and performs serialized
focused builds/review. Production remains planned until accepted principal paths
pass. No coverage increase from partial source. Private validation profile:
build/new-horizons-linux/testing/last-stand-20261006.Y5mzBuFn.

Mastery acceptance supersedes the pending-build checkpoint below: both targets
build;4/4 focused cases and16/16 adjacent cases pass with zero skips. Module
drift/canonical data checks pass; independent source review has no blocker.
Coverage226/310 (155/220 generic,71/90 faction),84 planned; Battlecraft8/10.
Source is committed/pushed as b9fe600c4; Windows notice preflight37549759684
passes on that exact revision; full Windows37549855253 is live. Actual AI Defend selection,
controlled/death/revival composition and rendered feedback remain Phase2;
normal launcher delivery is unchanged. Cabir opposite-contact art remains the
active user-priority correction, not an accepted walking animation.

User resolves UP156 machine allocation (first eligible ordinary stack) and UP079
LastStand retaliation ending activation/clone exclusion; both canonical rows are
updated. Mastery runtime/AI/focusedfixtures freeze and source review passes;
client/test rebuild97218 is pending after one qualifiedcallback compile repair.
No completedcoverage credit until native execution. User rejects static/smooth
Cabir preview; cruder56px sixposeRGBA draft is private/provisional, gait/root
alignment still under review. Other new oppositecontact outputs fail alpha.

Cabir direction audit now rules out temporal reversal in the shared renderer.
Original Gremlin/Gargoyle/Magi chronology and Arch Mage palette-alias chronology
are preserved; no equivalent defect is evidenced there. Shared-torso mechanical
alignment reduces jitter but root/independent review still reject the sixpose
draft: opposite planted-leg contact and passing transition must be authored.
UP265 remains Open; no new gait or normal-playable delivery is claimed.
The isolated opposite-contact attempt and its single targeted revision both
repeat the wrong phase and are rejected. Text-only corrective generation is
halted; explicit pose guidance is the next art-production requirement. No failed
draft is installed. Root resumes the design-cleared UP079 Last Stand queue item,
reusing its existing map and checking only current shared-resolution seams.

Latest delivery cycle: paired new-reference standing Cabir preview is isolated
and manually playable with an original5+5-stack map. Combined private glows/books
candidate from02fa7f89b has its own manual launcher,3241-file verified snapshot,
ten importer checks and native864-frame validation. Headless smoke reaches day4;
no graphical acceptance or normal-pointer change is inferred. Cabir contact poses
continue through HoMM3 Art before the ordinary Battlefield Mastery slice. Its
side-round/per-action lifetime architecture is now recorded in UP156; no planned
perk is activated without the machine ruling. Coverage counts remain unchanged.

Explicit user work supersedes the ordinary UP156 candidate: UP263 school casting
glows and UP264 faction tome bookmarks from the supplied v6 ZIP; UP265 Cabir
gait/cruder art, portrait background, selection contour and both-forms shooting;
UP262 residual burgundy robe pixels; UP261 new hero/garrison Leadership report.
These are persisted in the priority queue. Both Cabir portraits/contour are
source-corrected:13 focused Python checks pass, client/fixture builds pass and
dummy-SDL native resource fixture passes1/1, zero skips,2.64s. Optional casting
and guild hooks/importer build and review pass; private873 PNGs remain ignored.
Native book/casting fit and local playable integration remain pending, not Final.
Both-forms shooting is integrated in the canonical design; both source creature
definitions have SHOOTER/8 shots, with three focused config checks passing.
Base shot-art export is installed and nine export checks plus seven config/repair
checks pass. Rebuilt native fixture passes1/1, zero skips,2.67s; independent
source review has no blocker. Normal Linux delivery remains pending. Gait
drafts still repeat poses/are too smooth and are not installed. Do not lose these
user tasks or revert to ordinary perk backlog before their remaining gates.

Phase1 remains active. Linux now selects immutable2af95e81a6 from87c630a2b;
native1/1,2,358-file verification and bounded headless progression pass. UP262
is development-delivered, not full-motion/user-approved. Source evidence and
remaining visual gates stay in the priority queue; do not repeat completed
colour bindings or blocked Gargoyle prompts.

Registry-derived coverage:31/31 Skills,93/93 ranks,225/310 active perks
(154/220 generic,71/90 faction),61/67 combat identities,8/8 Orders. Registration
does not certify every effect, required UI or integration class.

Latest functional checkpoint: UP180 Counterpressure's ordinary accepted damage/debuff
path, independent per-side readiness through the end of the following round,
next accepted hero spell's Spell Power-term snapshot/consumption, and detached
AI parity passes the client/test build and15/15 focused native cases in2.099s,
zero skips/errors, after correcting scripted injury provenance and an illegal
detached-fixture viewpoint. Independent source/delta review has no blocker.
Keep registration
planned/inactive until the outstanding no-op recipient boundary is resolved;
this partial implementation earns no completed-perk identity credit. No playable
promotion; normal Linux remains the previous immutable delivery. Next bounded
principal-path candidate: UP156 Battlefield Mastery's ordinary-stack rank bonus,
subject to its unresolved machine-allocation boundary and inactive registration.

Next implementation-unlocking decisions currently presented: UP072 coastal
terrain mapping (spell plus dependent perks), UP180 Counterpressure's resolved
recipient trigger, UP156 Battlefield Mastery's ineligible-machine consumption.
Reuse existing maps after answers, assign disjoint runtime/data/test ownership,
implement principal paths and minimum AI hooks, then focused validation/commit.
Do not activate a planned entry merely to increase counts. The reusable pending
perk hold index is preparation, not new gameplay coverage or proof that every
Version1.0 category is blocked. Older checkpoints below are historical.

Current priority: UP248's approved Cabir presentation replacement and the
reported Academy roof, ownership-flag and Astronomy Tower connection defects.
The first Cabir standing master and proposed60px preview are shown before
animation expansion; they are not a runtime animation set. HoMM3 Art owns
creative raster revisions; existing mechanics and internal creature IDs remain.

UP245's required Flank side identity/proposed-position readback passes the
client/native build and seven focused cases, zero skips, in2.325s. Independent
review finds no blocker. Source integration/Git and playable delivery remain
separate; rendered fit/localization remain Phase2. No new spell/perk identities.
Windows37437598557 finished successfully on exactbea86a2c3; do not restart it.

Latest checkpoint: UP244's accepted prerequisite is committed/pushed asbea86a2c3.
Exact committed Linux source builds, freezes and passes independent2277-file
verification plus bounded headless AI progression through day7; the normal script
now selects c172340f. Three nonfatal Dispel preview diagnostics stay Phase2, not
silently called clean. Windows37429818459 succeeded on older3eda; full successor
37437598557 is live onbea and must be monitored without duplicate dispatch.
Next selection: bounded principal-path audits of artifacts/specialties, required
hero-development UI, creatures and buildings. The registry-derived audit confirms
the planned-perk holds, including Wisdom Sage's distinct UP074 visit-timing
question; it does not establish that all Version1.0 categories are blocked.
Perfect Rhythm remains inactive while its explicit stacking question is pending.

Current Phase1 checkpoint,2026-10-06: UP244 implements the missing last-three ordinary
Hero-paid Spell/Order history in the existing shared readiness state. Production
and focused fixtures have separate owners; root runs the serialized client/native
build and independent review. Repaired builds pass;30/30 focused native cases
pass in2.319s with zero skips/errors. Perfect Rhythm remains inactive pending its
Master Synthesis ruling; no perk identity credit is earned by this prerequisite.
The repeated UP241 screenshot reopens visual acceptance and is being compared
against baseline/v2 before another art revision. Preserve the current candidate.
Windows37429818459 completed compile/staging/package/upload on the earlier
3eda8ac03 batch; artifact metadata is inspected, not independent Windows play.
Next: commit/push this accepted prerequisite, then another unblocked queue
clause or an answered mechanics ruling. No exhaustive suite or art repetition.

Delivered UP241: source `cadab569a` is committed/pushed, built and promoted as
snapshot `3b7e155aec10506da961d94c6dfce24117bb11700879c903354da078cb23ceac`
after independent2277-file verification and bounded AI smoke through day7.
The existing ammo diagnostic recurs and stays deferred; no user visual approval
is inferred. The next bounded Steward selection confirms its already recorded
two-resident stacking hold (UP070/UP071); the question is presented again, not
silently decided. Next functional work must select another unblocked user-queue
clause or use an actual answer, not repeat that mapped hold. Windows batch
37429818459 is confirmed live at client compilation on the earlier3eda8ac03.

Current UP241 checkpoint,2026-10-06: pinned Provisional Village Hall roof
revision is source-integrated after native/registered-scene review; original
master/native, placement, alias and masks stay unchanged. Eleven focused art
tests and reproducible reduction pass. No gameplay identity count changes
(61/67 combat spells,225/310 perks). Next: source review/commit and exact Linux
candidate delivery, then resume unblocked user-priority implementation items;
do not repeat asset polishing or broad tests in place of missing mechanics.
Full Windows batch37429818459 remains live on3eda8ac03, without this newer art.

Current Gargoyle gate: authored full-colour alternative and reproducible58×64
preview exist under portrait-revisions/v2. It changes creature rendering as
well as background, so user choice is pending before runtime replacement.
Do not silently resolve that scope choice or repeat failed mask prompts.
The bounded Tower-creature/specialty review found implemented principal paths
or recorded holds, not new gameplay coverage; do not generalize it to all126
creature forms. Current playable12/14 portraits and gameplay counts unchanged.

Latest delivery: source `9540b0643` is built and promoted as snapshot
`bad986b13d1b1711a93d901a1749b73568d078291a01bb2644f39c2e64342011`.
Twelve portraits delivered; exact frozen content/map/AI smoke succeeds. Existing
ammo-overuse remains deferred. Obsidian v2/v3 mechanical exports reproduce but
are still rejected art, not new coverage. Next: a different Gargoyle extraction
approach, preserving purchaser-original references outside committed source.

Latest source checkpoint: Titan v3 integrated as portrait12, provisionally
accepted with five small boundary uncertainties deferred. Client/fixture build,
actual scale1–4 consumer (zero skips), three Python checks, exporter and source
review pass. Stone v3 and Obsidian v2/v3 corrections fail material geometry
requirements and remain out of runtime. Next: change Gargoyle correction
strategy rather than repeat the same failed prompts, then deliver the family.
Playable remains10/14; gameplay counts unchanged.

Bounded next-functional selection audit: Adventure effects, artifacts,
town/building mechanics, recruitment and minimum AI hooks did not expose an
unambiguous missing source path. Skeleton Transformer HP conversion still awaits
the recorded pooling/rounding ruling; remaining Adventure restrictions,
Lighthouse/Glyphs scope and artifact regeneration aggregation have explicit
design holds. Recruitment bands/stat cards and universal War Machine shop are
implemented; outstanding rendered evidence is not new source coverage. This
does not prove all V1 items are blocked or authorize changing specified rules.
Continue unblocked user-queue work and surface rulings before those slices.

Source checkpoint: Giant is integrated as portrait11; focused consumer passes
at scales1–4 with zero skips and both Linux targets build. Three Python checks,
runtime export and independent review pass. Titan v2/v3 remain draft only;
v3 violates the requested preserved sky pixel and changes four contour pixels.
Next: correct Titan and rejected Gargoyles, then deliver the remaining family.
Latest promoted Linux candidate remains the ten-portrait source below.

Latest playable checkpoint: source `6e600fc89` is committed, pushed, built and
promoted. The script selects verified snapshot
`bed369d0736cdef3ec6072b7e6ba1e62c859f9e75ca27507dd4ebc0233b927fa` containing
ten portraits. Focused native checks and bounded headless map/AI run pass;
ammo-overuse is still deferred. Next portrait slice: integrate approved Giant,
correct/classify Titan holes, revise rejected Gargoyles. No roof repair claimed.
Older delivery statements below describe their historical checkpoints.

Latest source checkpoint, 2026-10-05: UP239 integrates ten of fourteen large
portraits. Naga (core ID38/frame40) and Naga Queen (ID39/frame41) are registered
through the compositor; Queen uses the provisionally accepted v2 matte
(`aa282c71f59b720ccc2604e81b3bc1527b8e58b7ab60403eee9fb28eb9f64c30`) and
preserves its prior master/mask. Native `nhAcademyBuiltIconRuntimeTest` passes
all ten at scales1–4 with zero skips in `build/new-horizons-linux/Testing/Temporary/LastTest.log`;
client and fixture builds passed in the prior cycle. Four portraits remain
unintegrated: Gargoyle drafts are rejected, Giant is provisional but unregistered,
and Titan remains unapproved pending anatomy review. A mechanical matte check is
not approval. No gameplay identity credit or newer playable portrait promotion:
`e48e04550` remains the two-portrait playable snapshot. UP-241's hall-roof
correction is still open.

Earlier eight-portrait checkpoint: UP239 integrated eight of fourteen large portraits,
adding Genie and corrected Master Genie v2. Root client/native builds with twelve
jobs succeed; actual pixel/alias fixture passes three consecutive scale1–4 runs,
zero skips. Three Python checks, runtime exports, twelve draft reductions and
independent review passed. Naga was accepted but unregistered and Queen needed
correction at that checkpoint; those states are superseded above. No original
colour pixels were shipped.

Latest source checkpoint: UP239 now integrates six of fourteen large portraits,
adding reviewed Mage/Arch Mage geometry through the unchanged compositor.
Root client/native builds with twelve jobs succeed; actual SDL-dummy pixel/alias
fixture passes three consecutive scale1–4 runs, zero skips. Three Python checks,
runtime export validation and independent review pass. Eight portraits remain
unfinished; Genie/Master Genie private comparisons are available but need
luminous-contour/internal-gap review before approval. No gameplay identity credit,
host GUI run or launcher promotion. Existing e48e04550 playable snapshot retained.

Latest source checkpoint, 2026-10-05: UP239 now integrates four of fourteen large
portraits (Gremlins and Golems), all Provisional. Three Python checks and pinned
exports pass; rebuilt native fixture passes ten consecutive scale1–4 runs after
adopting production's async-drain-before-reset contract. Initial intermittent
segfault and unconfirmed cause remain recorded in the failure ledger; no broad
integration suite or host GUI run. Ten portraits remain unfinished; next is native
review of corrected Mage/Arch Mage masks, then runtime registration if accepted.
The launcher remains on validated e48e04550 (two portraits); source validation
is not playable delivery. Perks225/310 and combat identities61/67 are unchanged.

Current checkpoint, 2026-10-05: the committed `a3487aacf` candidate has been
built, checked headlessly and promoted to the existing Linux launcher, including
UP240's reviewed weathered Academy map bodies. Prior snapshots are retained;
user native visual acceptance remains separate from delivery. UP239 is the next
unblocked edit: opaque large creature portraits, not transparent small cutouts.
The corrected Gremlin geometry matte is provisionally accepted; a bounded worker
is implementing the original-pixel-preserving renderer consumer while root
authors the remaining masks through HoMM3 Art. UP241's confusing hall roof is
diagnosed as painted geometry, not duplicate rendering; no roof correction is
yet implemented. No Cabir roster change is authorized by the feasibility question.

Functional coverage remains225/310 perks and61/67 combat-spell identities.
The five Adventure Spell acquisition paths exist, but their effect audit is not
complete. This art slice receives no mechanic-identity credit. A bounded worker
is checking remaining planned items for an unambiguous functional next slice;
already recorded design questions must not be silently answered or re-mapped.

Current user-priority slice, 2026-10-05: UP-235 integrates the supplied Academy
art handoff while preserving current Tower gameplay and externally referenced
original assets. UP-236 repairs the arched Mage Guild hover highlight and the
adventure-spell unlock panel, including popup components accidentally attached
at the main window's origin. These three requested changes precede backlog work.
After reviewed source integration, build a Linux candidate containing every
latest commit and promote the existing launcher pointer; retain the old snapshot.
No graphical or host-input authorization is inferred. Windows run 37348640988
has completed successfully on source `0e645f79b`; it does not contain this new
Academy/UI work. Preserve the completed artifact rather than replacing its identity.

UP235/236 source checkpoint: supplied Academy art/Sand registration and guild
visual repairs pass focused import, art (3), Tower progression (2), existing
guild assets (9), UI guards, independent review and client/native builds.
Production content-loading checks pass 2/2; bounded headless startup and AI turns
work after the four built-icon resource fallbacks remove the Tower schema error.
Native rendered acceptance remains pending. Record static artwork, construction
stages, click/highlight geometry, flags, siege seams and puzzle reveal for visual
playtesting; do not claim a completed visual report from source guards alone.
Phase 1 coverage remains 225/310 perks and 61/67 combat spell identities: this
user-priority art/UI delivery adds no mechanic-identity credit. Next action is
the authorized latest-commit Linux snapshot freeze, smoke check and promotion;
preserve the previous playable snapshot. Do not resume unrelated backlog first.

Delivery checkpoint2026-10-05: Pre-emptive Strike source2ffeaa1297ce5bef225c9eadcd0fb618007f4b36
is committed/pushed with verified author/committer and exact remote hash.
Windows37308848380 is terminal SUCCESS onb8d243076; nonexpired game artifact
11352155062 is802672095bytes. Existing37318395313 started on3ee74704f, so root
dispatches latest full once:37324887768 is confirmed pending on2ffeaa129.
Preserve both handles; no replacement dispatch while pending, no graphical
acceptance or Linux snapshot promotion. Accepted coverage225/310 perks and
61/67 combat identities; next planned Mastery waits its recorded machine ruling.

Phase1 checkpoint2026-10-05: Pre-emptive Strike's independent authoritative
reaction and detached AI path are accepted. Separate per-stack round stamp,
exact50% pre-hit, retained normal retaliation, same-round re-Defend suppression,
next-round eligibility, legal melee and disabled-state rules are implemented.
Both-target67320 and fixture-only4257 pass with12 jobs; focused99767 passes
22/22 in6.291s, zero skips, including seven new cases. Initial24408 passes17/22
with fixture Tactics/adjacent-attack setup failures retained and repaired; do not
call it green. Data/inventory19/19, module drift and independent review pass.
Coverage225/310 perks (154/220 generic), Battlecraft7/10; faction71/90 and combat
61/67 unchanged. Bulwark composition, comparative Defend value and complete
midbattle world saves remain Phase2. No GUI or playable snapshot promotion.
Metamagic/Gating source-consumer audits correct stale labels without count credit.
Next missing candidate UP156 first-action Mastery is mapped; its unanswered
War Machine consumption question has been resurfaced, not silently resolved.

Delivery checkpoint2026-10-05: source3ee74704f6721dc5d7853b592d2ef98babcf9068
is committed/pushed, required author/committer and remote verified. Existing
full37308848380 started, so root dispatches latest full once:37318395313 is
confirmed pending on3ee74704f. Preserve both handles; no replacement dispatch
while pending, no graphical acceptance or Linux snapshot promotion.

Phase1 checkpoint2026-10-05: Perfect Moment now follows the canonical automatic
first eligible primary attack at current Luck+5, rather than a manual declaration.
Shared target-aware Luck excludes only Serendipity's chance-only+1, with no copied
history hotpath or new state. AI no longer offers a weaker opt-out forecast; the
checkbox/local arming UI is removed. Client26695 and native59248 build successfully
with12 jobs. Native22333 passes19/19 in4.540s, zero skips;11 UI source guards and
independent Astra review pass. The wider21000 run passes31/35 in8.997s: four
unrelated fixture/state/downsave guard failures are retained for Phase2, not
called green. Counts remain224/310 perks and61/67 combat identities; this repairs
a registered perk clause rather than activating another identity. No GUI run or
Linux promotion. Next highest-priority clear missing feature: UP157 Pre-emptive
Strike's full independent live/AI path; Bulwark overlap is Phase2 composition.

Phase1 checkpoint2026-10-05: missing no-hero defensive-tower base output is
implemented through saved town rules at Siege0. Client91717 and final both-target
44376 pass; native22240 passes8/8 in2.703s, zero skips, including real automatic
damage and legacy setup, custom77 and all four Engineer controls. Independent
review and module drift pass. Fixture header/lifecycle/override-merge failures
are retained in the failure ledger. No new perk/spell identities; broader v2,
full-save and siege composition checks belong to Phase2. No graphical or Linux
promotion. Narrow Field Workshop destroyed-target, Scholar holder, and
Academic Study/Sage pre-acquisition-visit questions were resurfaced; no answers
are inferred. Next highest-priority full feature: Field Workshop's shared
machine/fortification repair once its scope is resolved. Do not remap its
already-recorded architecture while waiting; other unblocked clauses may proceed.

Windows checkpoint2026-10-05: paid-artifact run37295572917 is terminal SUCCESS
onc675456fe56091137bb22f0ac586349094f27c2b. Nonexpired game artifact11345085085
is802647746bytes. Existing37302451874 on94147b24a has started, so root queued
one full latest build37308848380 onb8d2430765f0a9653f303ea65fb9474af2a49d03;
confirmed pending. That candidate includes canonical growth, Glyphs siege and
machine HP. Preserve both current handles; no duplicate/replacement dispatch.
Package success is not graphical acceptance or Linux snapshot promotion.

Phase1 checkpoint2026-10-05: Glyphs siege20 Defense and all four authored
machine HP values accepted. Native88293 passes4/4 in1.466s, zero skips after
the before gate proved legacy250/1000/75/100 HP. Both-target repaired/final
builds pass; two exact offline guards and independent review pass. Glyphs
area-Morale remains blocked, so do not mark the entire building complete.
Machine battle/save compositions and played sieges remain Phase2; no new
perk/spell identity count or playable promotion. Preserve Windows pending
37302451874 on94147b24a and in-progress37295572917 onc675456fe, rechecked
this cycle; no replacement dispatch. Next: select an unblocked missing
specification clause from the queue rather than remapping unanswered choices.

Phase1 checkpoint2026-10-05:11 actual weekly-growth data mismatches corrected
through existing saved growth lines. Loaded lookup now matches64/64 authored
roster rows, up from53/64, with checked upgraded forms. Both-target83259 passes;
native47814 passes3/3 in1.177s, zero skips, plus exact offline guard/module drift
and Astra review. Rule-object current/historical roundtrips do not certify full
world saves, stocks or recruitment. Those journeys remain Phase2. Perk/spell
counts unchanged. Next selection must use named outstanding decisions rather
than repeatedly mapping their seams; three Rebirth perks now explicitly link
to UP072, and Perfect Rhythm retains UP178's composition question. Further
unexamined specified data/town consumers can be audited for a concrete gap.
No GUI or Linux snapshot promotion. Preserve the two live Windows build handles.

Delivery checkpoint2026-10-05: source94147b24aa181a06faed5e6459fada090b298041
is committed/pushed with verified author/committer and remote. Last-stack full
Windows37289192606 is terminal SUCCESS on1755ee0d4; nonexpired game artifact
11341399297 is802641850bytes. Paid-artifact37295572917 has started onc675456fe.
After confirming no other pending full run, root dispatched latest full once:
37302451874 is confirmed pending on94147b24a, including Cyclops AI and these
Brimstone/Castle changes. Preserve both handles; no duplicate/replacement or
playable acceptance from pending state. Linux snapshot remains unpromoted.

Phase1 checkpoint2026-10-05: Brimstone siege Spell Power and four Castle
role-stat rows accepted. Both-target91972 exits0; native85598 passes5/5
in1.765s, zero skips, plus two exact offline data guards/module drift and
independent Astra review. Actual scoped siege grant/accepted-result cleanup
and loaded creature definitions pass; no new engine state or polling. Counts
remain224/310 perks,61/67 combat identities and126 creature forms. Full native
recruitment/battle journeys, strategic valuation and rendered delivery remain
separate. Next selection: continue bounded unexamined Version1.0 principal-path
audit; do not revisit accepted building/artifact maps or unanswered perk choices.
Death Stare already executes on AI attacks; improved expected-kill valuation is
recorded for Phase2, not treated as a missing action path. Qualitative artifact
source/binding audit found no unblocked rewrite. Windows37295572917 remains
pending behind compiling37289192606; do not replace that pending full run.

Phase1 checkpoint2026-10-05: Cyclops/Cyclops King minimum BattleAI wall-shot
hook accepted. Actual AI-selected gate shots for both forms resolve through
authority; ordinary-shot/no-wall/WAIT and Hero Action controls pass. Both-target
build92551 exits0; native35852 passes6/6 in2.190s, zero skips. No new content
identity count. Broader siege valuation/controller matrix deferred to Phase2.
Next mapped perk: Crown and Altar's automatic second-action bonus. User's
less-clicky decision is canonical and pushed in15ff7c8c3; recipient qualification
shares UP108's unanswered Shared Purpose decision. Do not activate before that
answer or re-explore the documented state/targeting map. Continue another
unblocked Version1.0 item while the question remains pending.

Windows checkpoint2026-10-05: Frenzied37286838037 succeeded onf46e375ee,
nonexpired game artifact11338641211 is802646349bytes. Last-stack37289192606
is in_progress on1755ee0d4; paid-artifact37295572917 is pending on exactsource
c675456fe, dispatched once after the prior pending job started. Preserve both
handles; no duplicate dispatch, new accepted artifact or Linux promotion claim.

Current continuation2026-10-05: previous cycle is progress; sourcec675456fe is
pushed with verified identity/remote and clean worktree. Phase1 coverage audit
now enumerates the six canonical specialty-conversion rows, with actual accepted
slices and blockers rather than a made-up completion fraction. Bounded read-only
workers check previously unexamined Stronghold/Rampart creature clauses and
Castle/Rampart/Necropolis unique-building effects for the next concrete missing
mechanic. Resource-specialty producer retention is audited separately. Do not
re-map known unanswered perk choices or substitute exhaustive testing of accepted
features. No new active perk/spell count from ledger work.

UP023 paid Adventure-artifact slice accepted2026-10-05: final both-target
build79874 exits0; native70394 passes20/20 in6.541s, zero skips. Exact equipped,
unlearned Boots/Wings casts pay20/40 and consume the shared daily opportunity;
removal, genuine cast effects, historical v2 passives and real NK2 current/next-
day routes pass. Seven data checks/module drift and independent review pass.
The failed first native run is retained with both causes and repairs in the
failure ledger. No new perk/spell identity count: two explicit artifact
exceptions now have principal-path evidence. Generic helper layer availability
remains capability-only; NK2 validates the prepared destination day. Deferred:
generic whole-route hypothetical cast budgeting, combined artifacts, rendered
access/audio and strategic valuation. No GUI or Linux snapshot promotion.

Earlier checkpoint: repaired native69581 exits0. First focused execution20 cases has16 pass/4 fail
in6.296s: authentic v2 fixture construction and three real next-day AI routes
need repair. Runtime and fixture owners have non-overlapping follow-up tasks;
preserve logs/assertions. No native acceptance, source commit or promotion yet.

Artifact native build61323 is terminal failed on the AI fixture's missing
TurnInfo include. Minimal include repair is applied without changing assertions;
retry69581 is live. Preserve both logs; no second concurrent build or acceptance
claim. Client35563 and production/fixture review remain passed.

UP023 Adventure-artifact runtime candidate is frozen. Current saved v3 rules
grant exact equipped Boots/Wings sources with20/40 cost and suppress only their
passive artifact bonuses; v1/v2 and genuine spell/OTHER effects retain behavior.
TurnInfo caches raw type lists and filters at presence/value reads. Shared
current-day path admission and movement audio use the same distinction; future
path days remain available. No new state/schema or permanent spell learning.
Client35563 passes297 build steps with12 jobs. Production and five new fixture
reviews have no blocking findings. Seven focused artifact data checks and module
drift pass. Native build61323 is live (UP023-adventure-artifacts-native-build.log);
actual cast/path execution has not yet been run or credited. Preserve this
handle; no second build/GUI/snapshot promotion. Deferred: rendered access/audio,
combined-artifact interactions, strategic value tuning and generic CPathfinder's
hypothetical within-route cast-budget dimension. NK2 already has per-node daily
flags; its two real artifact-route cases must pass before minimum AI acceptance.

Next Phase1 slice: paid Adventure casts supplied by Boots of Levitation and
Angel Wings. Canonical20/40 costs and daily action are explicit; current free
passive movement is a real production gap, not a design ambiguity. Map saved-
rules suppression/availability/cost and all shared consumers before bounded
runtime/test ownership. Preserve legacy worlds, no polling or frontend state
mutation. Artifact framework ledger now enumerates its exact ten rows without
claiming baseline producer existence as acceptance. Coverage counts unchanged.
Bounded parallel audits find the checked Bless/Earthquake/Guardian/Spell Lock/
Time Stop/Poison/Sorrow rank consumers and Tower Mage/Arch Mage penalty/cost
abilities already implemented. This is not full School or126-form certification;
do not invent a patch or remap recorded design blockers. The explicit artifact
gap takes precedence. Runtime and native-fixture maps are read-only until root
partitions all passive-consumer and compatibility seams.

UP021 source1755ee0d405c680d1fde5d771565a20b5d0d0eda is committed/pushed;
required identity and remote hash verified. Full Windows37289192606 is pending
on that exact source, dispatched once behind live Frenzied37286838037. No new
artifact, GUI acceptance or Linux playable promotion is inferred.

Accepted Phase1 principal-path repair: UP021 last-stack transfer. Client39538
and native build88200 pass; native26444 passes13/13 in3.908s, zero skips.
Ordinary/radial routes retain the last creature, transfer available Leadership
capacity and use normal localized modal feedback, without changing numeric
split semantics. Three source guards and independent review pass. No count
increase, GUI or snapshot promotion; rendered/playable delivery remains pending.
Next: select an unblocked missing specification path using existing maps.

Windows delivery: Purifying37280908002 is terminal SUCCESS on71dc35eda6bbe0ac4e07b309aa5ea52c3ec8090b.
Nonexpired game artifact11335635403 is802632735bytes. Frenzied37286838037
is confirmed in_progress onf46e375ee; preserve its live handle without restart.

Current Phase1 work: UP021 reopened last-stack transfer principal acceptance.
Source is implemented but its original native gate remains pending. Bounded
source/test audits identify the smallest server-authoritative exact-one,
all-but-one, receiving-capacity, conservation and stale-request checks; root
executes once, repairing only concrete failures. This is not broad army
integration hardening or graphical acceptance. No GUI/profile/snapshot changes.
Perk224/310, Chaos5/10 and combat61/67 counts remain unchanged.

Frenzied sourcef46e375ee is committed/pushed with verified identity/remote.
Full Windows37286838037 is confirmed pending on that exact source, dispatched
once; Purifying37280908002 remains in_progress. Preserve both handles, not
duplicates or cancellation. No new package, graphical acceptance or Linux
snapshot promotion is inferred. Next is the unresolved Berserk skipped-turn
lifetime; the concise question is resurfaced and no answer is assumed.

Current Phase1 checkpoint: UP062 Frenzied Curse source/native accepted.
Client78683 and final native build64062 pass; native42075 passes30/30 in6.265s,
zero skips. Data/inventory19/19, module drift and independent review pass.
Coverage224/310 perks, generic153/220, Chaos Magic5/10; faction71/90 and combat
identities61/67 unchanged. Action-scoped +2 Speed uses original-caster provenance
and live/AI cleanup without a new saved counter. Broader interactions and existing
stopped-unit valuation remain Phase2; no GUI or snapshot promotion. Next missing
foundation is base Berserk's skipped-activation lifetime, pending the resurfaced
negative-Morale decision. Bounded planned-perk and creature/town/artifact/UI audits
found recorded choices blocking their checked candidates; not a whole-goal
blockage claim. Reuse those maps rather than remapping unanswered choices.

Latest delivery evidence: Heaven37276837622 succeeded on44e4442bc; nonexpired
game artifact11332920803 is802616768bytes and excludes later Purifying code.
Purifying37280908002 remains in_progress on71dc35eda; no artifact claim yet.

Purifying source71dc35eda is committed/pushed with verified identity and remote.
Full Windows37280908002 is pending on that exact source; dispatched once.
Heaven37276837622 remains in_progress. No artifact or playable promotion claim.

Current Phase1 checkpoint: Purifying Mandate source/native accepted. Client15739
and repaired native build30070 pass; native4954 passes43/43 in7.802s, zero skips.
Data/inventory19/19, module drift and independent review pass. Coverage223/310
perks,71/90 faction perks, Divine Mandate6/10. No new persistent state, GUI or
snapshot promotion. Broader interactions and heuristic tuning remain Phase2.
Town Portal's shared runtime/AI map is complete, but implementation remains
blocked by previously asked town-ownership and minimum-Movement choices.
Divine Discipline's lifetime map is complete: shared live/AI recipient carry
must survive round expiry until the next completed genuine activation, without
changing current-round authorization. Same-Order reissue awaits replacement
versus separate nonstacking-instance choice (UP149); focused question asked.
Rapid Embarkation reuses UP103's complete map and remains blocked by the existing
Navigation10%-versus5% choice. No activation or coverage inferred from mapping.

Delivery checkpoint: Mandate source44e4442bc is committed/pushed with required
identity/remote verified. Full Windows37276837622 is confirmed queued on that
exact source, dispatched once. Earlier37273443600 remains pending and
37270206987 in_progress; preserve handles without duplicate dispatch or
cancellation. Package and graphical acceptance are not yet established.

Accepted Phase1 slice2026-10-05: Mandate of Heaven. Both-target25480 exits0;
native55540 passes49/49 in6.848s, zero skips. Existing total counter, real four
pairs/fifth rejection, first-only Reserve, inactive saved selection, detached AI
and direct/enclosing compatibility pass. Data/inventory19/19, module check,
Order/sidebar guards and independent review pass. Coverage222/310 perks,
70/90 faction perks, Divine Mandate5/10. Logs/XML: UP108-heaven*.
Broad combinations, full-battle saves and rendered/playable delivery remain
separate. No GUI or promotion. Next unblocked slice: Purifying Mandate.

Next unblocked map: Purifying Mandate. Capture the selected Divine Mandate Spell
source before consumption; only targets with actually removed negative magical
effects receive one additional physical-affliction removal, after ordinary
Purify/Purifier cleanup. Reuse the existing deterministic Poison, Disease,
Bleeding, then oldest-other selection and authoritative effect/unit packets.
Physical-only cleansing and no-op removals do not trigger the perk. No new state
is required. This map is not implementation or activation evidence.
AI map identifies the existing selected Divine Mandate candidate in
`BattleEvaluator.cpp`, Purify's chosen negative groups and detached cleanup in
`StackWithBonuses.cpp`. The next slice must project the same extra physical
removal and value it, without a client-supplied source flag or extra action
payload. Existing server/AI Purify fixtures provide focused actual-cast,
ordinary-cast, physical-only and Purifier-composition controls. Broader status
matrices remain Phase2 rather than blocking this bounded implementation.

Delivery checkpoint: accepted Knightly source1bd450fa6 is committed/pushed;
required identity and remote hash verified. Full Windows37273443600 confirmed
pending on1bd450fa62d6842c19c1ab59f55ca776bc81de17, preflight_only=false;
Sacred-source37270206987 remains in_progress. Dispatch only once; retain live
handles. No Knightly artifact or Linux snapshot promotion is implied.

Accepted Phase1 checkpoint2026-10-05: Knightly Sequence. Both-target79514 passes;
native77528 passes32/32 in5.541s, zero skips, six new cases. Data/inventory19/19,
module check, numerical Order/sidebar source guards and independent review pass.
Coverage221/310 perks,69/90 faction perks,Divine Mandate4/10. Logs/XML under
UP108-knightly*. Broad combinations, full-battle saves and rendered/playable
delivery remain separate. Next unambiguous slice: Mandate of Heaven, derive one
extra completed-pair capacity with the existing counter and explicit count4 save
compatibility. No GUI, new artwork or Linux promotion. Earlier live-build notes
below are checkpoint history.

Latest validation/delivery2026-10-05: Knightly source/fixtures frozen and reviewed
without blocking findings. Both-target local79514 runs12 jobs, log
UP108-knightly-build.log; data/inventory19/19 and module drift pass. Accepted
coverage remains unchanged until principal gates. Windows37267127209 terminal
SUCCESS on4af518137, nonexpired game artifact11328478994 (802605583 bytes);
Sacred-source37270206987 is now in_progress oncb5cd56de. No Knightly package,
graphical acceptance or Linux promotion is implied. Earlier observations below
are checkpoint history.

Current Phase1 slice2026-10-05: Knightly Sequence, resumed after UP230 recheck.
Runtime, AI and actual-action/packet fixtures have independent owners; root
integrates existing numerical previews, activation and builds. Accepted coverage
remains220/310 perks,68/90 faction perks,Divine Mandate3/10 until focused gates
pass. No graphical automation or playable snapshot promotion. Current Windows
handles revalidated:37267127209 in_progress,37270206987 pending.

Delivery checkpoint: accepted Sacred Command source cb5cd56de is pushed and
remote/identity verified. Full Windows37270206987 is confirmed pending on that
source; earlier full37267127209 is still in progress on4af518137. The older
candidate excludes Sacred Command. Do not cancel or duplicate either run based
on observation timeouts; compilation/package evidence remains distinct from
graphical/playable acceptance.

Accepted checkpoint 2026-10-05: Sacred Command. Client3475 and repaired
both-target44913 pass; native86438 passes26/26 (4.654s), zero skips; focused
data/inventory19/19, module drift and independent review pass. Counts220/310
perks,68/90 faction perks,Divine Mandate3/10. Retain failed45324 and repaired
build/native logs under UP108-sacred*. Broad composition, chooser-cache edge
cases and rendered/playable acceptance stay separate. Next unblocked is
Knightly Sequence; Shared Purpose awaits recipient semantics. Earlier notes
below preserve the implementation/validation checkpoints, not current counts.

Current Phase 1 slice (2026-10-05): Sacred Command. Runtime captures a distinct
Divine-Mandate-paid Order efficiency contribution; independent workers own AI
valuation and focused actual-action/packet fixtures. Root integrates activation,
registration, append-only compatibility and build evidence. Accepted counts
remain 219/310 perks and 67/90 faction perks pending principal validation.
Shared Purpose awaits the user's recipient-semantics choice. The next unblocked
slice is Knightly Sequence: source-qualified -2 Spell cost (after Wisdom,
minimum 1) or a distinct captured +5-point Order efficiency contribution.
Its read-only map is complete; no Knightly activation is claimed. No graphical automation or
playable snapshot promotion is part of this cycle.

Delivery checkpoint2026-10-05: accepted source4af518137 is committed/pushed,
remote hash and required author/committer verified; both new Divine Mandate perks
are included. Earlier full Windows37263037998 is terminal SUCCESS on45f659b7c.
Its nonexpired artifact11326508028 is
New-Horizons-Windows-x64-45f659b7cfc0e307352c7f7393d2e45ed3b2a2f3
(802590171 bytes): it includes Mage Guild corrections, not the two new perks.
New full Windows37267127209 is confirmed in progress on
4af5181377917139d292621ee0a3d92deae9dd04, preflight_only=false. Retain that
specific handle; no duplicate dispatch or playable Linux promotion. Compilation/
packaging does not prove Windows graphical acceptance.

Accepted2026-10-05: Consecrated Casting. Client97140 and repaired both-target
55168 pass; all three new native actual-effect/projection/control cases pass.
Focused accepted run5534 passes21/21 in5.491s, zero skips, plus17 data guards,
module drift and independent review. Initial22-case run18598 passes21/22; its
sole failure is an older casualty-provenance binary battle-copy rejection in
Grand Formula's final deepCopy oracle. Retain both result sets and defer the
whole-battle save/fixture expectation to Phase2; the accepted filter explicitly
excludes only that case. Perks219/310, faction perks67/90, Divine Mandate2/10;
ranks93/93 and combat61/67 unchanged. No GUI/promotion. Next: Sacred Command,
with distinct Order snapshot contribution/version compatibility and actual AI
payload-aware valuation, not a mislabeled Warcasting field.
The following in-progress paragraphs are checkpoint history.

In progress2026-10-05: Consecrated Casting, a second Divine Mandate Basic perk.
Capture the actual selected Divine Mandate Spell source pre-commit and scale only
the SP-derived component by110%, shared by live/detached mechanics. No state or
save-format change, new action, Warcasting alias or fixed-term buff. Separate
production and focused actual-effect fixture writers; root registry/build/Git.
Keep accepted counts218/310 until its principal native/build gates pass.
Reserve source7074e1509 is pushed/remote-verified with required identity.

Accepted2026-10-05: UP108 Chaplain's Reserve. Repaired client/native build25165
passes; native96092 passes22/22 in2.672s, zero skips, including five actual-action
reward cases and both real AI pair directions.17 data guards, generated-module
drift and independent review pass. Perks218/310, faction perks66/90, Divine
Mandate1/10; ranks93/93 and combat61/67 unchanged. Retain the first compile log
and direct-interface/include repairs in the failure ledger. AI Mana-recovery
valuation, wider perk composition and full battle save/resume remain Phase2.
No GUI launch or playable promotion. Next map: Sacred Command and Consecrated
Casting through typed follow-up selection, with shared live/detached component
math. Earlier in-progress paragraphs below are checkpoint history.

In progress2026-10-05: UP108 Chaplain's Reserve supplies a real Basic perk,
restoring3 Normal Spell Points on the first completed pair. Separate runtime,
native-fixture and minimum AI-execution fixture ownership is assigned; no
polling, new usage counter or save-format change is justified. Spell recovery
occurs after payment/effects, preserving Buffer and capacity. Keep counts217/310
until frozen build/native acceptance. Rebirth Chain/Phoenix Spark await their
explicit25%/other-perk interaction choices; Swift/Morale precedence is pending.

Delivery checkpoint: source45f659b7c is committed/pushed with required author
and committer identity. Full Windows run37263037998 is confirmed in progress
on45f659b7cfc0e307352c7f7393d2e45ed3b2a2f3; no artifact or Windows acceptance
is claimed while it runs. This includes the preceding Mage Guild corrections.
The Linux launcher snapshot remains unchanged.
Swift Rebirth's read-only map is complete: shared queue insertion, serializable
pending/used markers, extra-activation admission and detached mirrors are required.
Its conflict with an already-earned Morale activation is asked explicitly before
implementation; no perk activation or precedence is inferred. UP046 retains
the map and remaining acceptance requirements.

Accepted2026-10-05: UP046 Primal Burst, Greater Essence and Elemental Ward.
Repaired both-target build68374 passes; native92485 passes23/23 in6.366s, zero
skips, plus17 data guards/module drift and independent review. Perks217/310,
faction perks65/90, Rebirth3/10; ranks93/93 and combat61/67 unchanged. Retained
failed fixture compiler logs and direct-type/include lessons are in the failure
ledger. Wider Guardian/native-Rebirth survival and representative valuation
accuracy remain Phase2. No GUI or playable promotion; remaining seven Rebirth
perks are not implicitly enabled. Next mapped foundation is Swift Rebirth.
Dispatch the full Windows build after pushing this checkpoint.

In progress2026-10-05: UP046's next slice covers Primal Burst, Greater Essence
and Elemental Ward. Primal Burst supplies the missing real Basic prerequisite
for normal Advanced-perk selection; do not bypass tier requirements or activate
a placeholder. Separate runtime/AI/helper ownership shares captured perk state,
non-spell magical-ability damage reduction, adjacent current-owner targeting
and exact HP arithmetic. Candidate data gates pass17/17; counts stay214/310
until frozen builds and focused legitimate-acquisition/runtime/AI cases pass.
First build64934 failed on a fixture SpellID enum wrapper and is retained in
the failure ledger. Memory's Elemental Morale scope is asked; UP072's terrain
gaps remain separate. No broad suites, GUI launch or playable promotion.
Windows source-only preflight37259200414 succeeds on135725aa2; dispatch a full
build after the next accepted source push so it includes the new checkpoint.

Current2026-10-05: UP046 base ranks source/native accepted. Client8888 and final
test build81405 pass; native64752 passes12/12 in3.755s with zero skips, including
eight new runtime/AI cases and four adjacent controls.17 data checks/module
drift and independent review pass. Rank effects90->93/93; faction ranks24->27/27;
perks remain214/310 and combat61/67. First compile and fixture failures are
retained with their repairs, not discarded. Broader HP/status/death composition,
stochastic/initiative and unknown-opponent AI forecasting remain Phase2. No GUI
or promotion; full combat save/resume remains unsupported. Next: Greater
Essence and Elemental Ward, then the other unblocked missing specified content.

Implementation start2026-10-04: UP046 Elemental Rebirth base-rank implementation follows
pushedb81ee74bf. Runtime owns startup HP capture, pure reaction/spawn helpers,
versioned descriptors and authoritative injury reactions; AI owns detached
physical/spell consumers and focused native fixtures. Root registers files/data,
serializes builds, reviews integration and keeps coverage at90/93 ranks until
principal paths pass. No ten-perk activation, terrain redesign, polling, GUI
launch or playable promotion is included. Full stochastic AI candidate averaging
and full midbattle save/resume remain deferred, not false acceptance claims.
After the base gate, the next bounded coverage slices are Greater Essence
(Advanced40->55%, Expert50->65% Rebirth HP) and Elemental Ward (20% magical
damage reduction on Rebirth outputs). Both are explicit, terrain-independent
canonical perks. Their saved-perk decisions must be shared by authority and
detached AI; each stays planned until its own implementation/build/native gate.
This map does not activate the other eight perks or resolve terrain mapping.

UP108 implementation resumed2026-10-04 from clean pushedaa6ff84c5.
Acceptance: client/native retry79510 passes after correcting a test-only
`MasteryLevel::Type` parameter. Six new Divine Mandate native tests and21
adjacent allowance/projection/provider tests pass, zero skips; independent review
has no blocker. Rank coverage advances87->90/93 and faction ranks21->24/27;
perks remain214/310. All ten Divine Mandate perks remain planned. Wider perk
compositions/full battle save-resume remain Phase2. No playable promotion or GUI
acceptance is inferred. Next foundation: UP046 Elemental Rebirth.
Shared/server runtime, client continuation/status and detached AI/native fixtures
are being implemented in parallel with separate file ownership. The shared
contract reuses the per-side typed allowance ledger, including its completed-
pair counter and payload-aware selection/commitment; no second pending ledger
or forced creature-action lock. Root registers the generic status provider,
owns data activation/build and obtains independent review. Coverage remains
90/93 ranks and214/310 perks after principal native/build gates pass. GUI and
playable promotion remain separate delivery obligations, not inferred authority.

Current user priority UP230 supersedes the following UP108 next-action notes:
finish all26 custom spell families as transparent symbols, remove the separate
Adventure Spells entrance button in favor of the native guild exterior hover/
click region, and restore Arabic guild tier names. All26 original-preserving
symbol masters/30/32/44px exports are created and inspected; all78 runtime PNGs
are integrated, with no omitted family. Two final alpha/hash/native-dimension/
binding-linkage tests, eight spell-binding checks and module drift pass.
Root owns art generation/source
exports and Git/build; isolated worker owns live raster copies and alpha/hash
manifest guard. Hotspot client92271/source guard and nine-faction guild-name
checks9/9 pass. Do not resume Divine Mandate or ordinary coverage before the
source/native acceptance of UP230; those focused gates now pass. Sourcefa9310b51
is committed/pushed/remote-verified; return to UP108. Rendered delivery remains
separate; no GUI/
promotion is authorized by this task.

Current2026-10-04: user resolves UP046 battle-start maximum aggregate HP and
UP108 Metamagic-like round-end/completed-pair follow-ups. Canonical/data source
e6ba582a9 is pushed/remote-verified;17 perk-data checks pass. Foundation maps
now prepare exact existing death/summon/HP and typed-action/UI/AI/save seams,
not terrain-perk redesign or activation. UP229 Movement tooltip source/native
acceptance now passes and source5b87014e9 is committed/pushed/remote-verified:
client43390 and both-target61049/26637; native34473
15/15 in2.498s, zero skips; two source guards,17 data checks/module drift and
independent review. First13/15 fixture failure is retained, setup repaired
without weakening exact assertions. Next implement the unblocked Divine Mandate
rank foundation via typed allowances,
completed-pair counter, Light restriction and shared live/UI/AI admission.
Rebirth's frozen-HP/death/summon/save/AI map is also ready; serialize shared
foundation file ownership. No GUI/promotion or rank/perk count increase yet.
Windows37241527929 is SUCCESS on older90aac5407 with a nonexpired downloadable
artifact (750688325 bytes); it excludes Adela, decisions and Movement UI.

UP228 bounded audit complete: all five old generic Sorcery specialty aliases
are explicitly removed by the active halon.json module patch and replaced with
NH specialties. Preserve the authored replacements; no eligible built-in slice,
production edit, new test or coverage credit. This is an inapplicable candidate,
not a design blocker and not evidence the remaining Phase1 backlog is blocked.

Current checkpoint: Adela/Bless source0c5964b71 is committed/pushed with remote
hash and author/committer verified. Eight native cases and twelve hero-data
checks pass. UP228 next maps old generic Sorcery specialties to Spellcraft,
using112/124/136% efficiency and12/24/36% SP-growth chances; independent
interpretation review agrees. Mapping is not implementation coverage. Windows
37241527929 remains live on90aac5407, now compiling after successful dependency
preflight; it excludes Adela. Earlier live/next-action notes below are history.

UP224 Adela source/native accepted2026-10-04: client38169, both-target99683
and final48936 pass. Native6322 passes8/8 in5.310s, zero skips; twelve hero-data
checks/module drift and independent reviews pass. Commit/push exact-producer
conversion and SP-only duration scaling. Four non-damage aliases converted,
without new spell/rank/perk identity counts. Historical list/save controls remain
meaningful. Broader composition and graphical delivery are Phase2; full Windows
37241527929 is still live on older90aac5407 and excludes this slice.

Current2026-10-04: previous full Windows37237106185 is SUCCESS; new full
37241527929 is live on90aac5407 (Vault and Resurrection specialties included).
Adela/Bless is the next bounded source slice: exact legacy-producer conversion,
20% only on its numericalSP/80duration term, fixed2/cap4 unchanged. Separate
production/test writers; root module/build/integration. Independent interpretation
review agrees this follows the canonical component rule, not a new design choice.
No native or playable credit before those gates; no new identity count.

UP227 source71604c698 is pushed/remote-verified with the required identity;
clean checkpoint. Windows37237106185 still packages older6cc6e9f05, excluding
the Vault and specialty slices. Preserve that exact live build; no duplicate
full dispatch. Next candidate check finds Encircled Doom awaiting UP174's
existing positional-versus-accepted-side/lifetime ruling, Field Instructor
awaiting UP127 cohort semantics and Elemental Conjurer awaiting UP072. These
are real blockers for those slices, not permission to activate partial perks
or evidence that the entire remaining backlog is blocked. Phase1 remains active.

UP227 source/native accepted2026-10-04: Vault of Ashes construction and Fire/
Energy weekly growth now use the standard Horde2 path. Both-target84391 passes;
native97534 passes3/3 in2.695s, zero skips. Five data guards/module drift and
independent review pass. Commit/push this slice. Dedicated art/rendered delivery,
older category snapshots and strategic AI choice remain separate. Avatar is
still awaiting its existing Blood Scent clarification, not an unblocked task.
Phase1 continues with another unblocked missing specification item; no broad
integration suite or GUI promotion is needed for this source checkpoint.

UP224 Resurrection specialty accepted2026-10-04: client51670 and both-target
5985 pass; native49136 passes12/12 in6.477s, zero skips. Alamar/Jeddite component
conversion preserves fixed100 and historical Cure-only producers. Commit/push
this slice; UP226 Avatar of Rage is the next unblocked mapped perk candidate.
Primary Attribute audit found no eligible built-in flat hero-stat specialty;
do not convert creature-limited bonuses or invent an authored hero identity.
Windows37237106185 remains live on foundation6cc6e9f05, excluding this slice.

Cure sourcecb6cc9614 is pushed and remote-verified. UP225 source/native accepted:
both-target5018/14793 pass; native8017 passes9/9 in4.758s, zero skips.
Commit/push this foundation, then convert Alamar/Jeddite Resurrection specialties
with historical Cure-only supported-list guards. No graphical promotion.
UP225 implements the
canonical Resurrection foundation with separate Luna production/native-fixture
owners. Root owns module generation, registration, serialized12-job builds and
Git; source inputs must freeze before builds. Principal shared healing/forecast,
permanent casualty/cap, exclusions, old-row/save and cost/rank checks outrank
broader integration matrices. No new spell identity or specialty alias credit.

UP224 accepted checkpoint2026-10-04: Cure specialty production and three compact
native cases pass. Independent reviews have no blocker; client52539 and twelve
hero-data/module drift checks pass. Serialized12-job both-target3385/69675
succeed; final native20053 passes22/22 in4.011s, zero skips, covering real
Uland/control forecasts, accepted healing, save/legacy guards and adjacent
damage-component controls. First stale-v3 oracle failure and narrow repair are
retained in NH_RELEASE_FAILURES.md. No playable/graphical or whole-family credit.
Commit/push this slice; next implement Resurrection's mapped canonical foundation.

UP223 accepted checkpoint2026-10-04: Lord Haart Estates core150/300/600,
perks/unrelated income untouched. Client39945 and builds16010/47106 pass;
native95834 passes12/12 in4.501s, zero skips. Module drift/12 hero-data pass.
Commit/push this slice. Windows37227083002 completed SUCCESS onaf17030fc;
full37231394673 is live ond2921158e (UP222/UP220 remainder), excludes UP223.
Next bounded missing coverage: Uland Cure specialty's SP component20%, followed
by Alamar/Jeddite Resurrection. Detailed canonical sections control conflicting
summary spell levels; audit Resurrection's Level3 config against detailedLevel5.
Weakness/AnimateDead are inactive legacy IDs (not their active NH replacements)
and Haste is unresolved; do not invent replacement specialties. Primary+5
specialty family also lacks systematic conversion. Broader financial interaction
and Lord Haart daily receipt verification stay Phase2, not a Phase1 retest loop.

2026-10-04 checkpoint: UP222 Archery source/native accepted. Both-target46837
and native35240 pass (12/12, zero skips,6.231s); UP220 remainder29 access
exclusions remain accepted separately. Module drift/20 magic/12 hero-data gates
pass. Commit/push this coherent batch, then implement the mapped Estates
specialty for Lord Haart. Existing Windows37227083002 is still live on older
af17030fc, excluding this batch; no duplicate dispatch or Linux promotion.
Phase2 retains broad modifier/AI interactions and authored legacy profile gaps.

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

UP220 remainder accepted:29 further audited rows excluded only from hero access
and ordinary acquisition,35 total. Build7593 and native55749 pass19/19 in2.067s,
zero skips, covering real stocks/13 starters, known-spell sources, authorized
rejection, actual creature effects and old-save restoration.20 offline magic/
schema and12 hero-data checks pass; module drift/review pass. First fixture
compile failures are retained. Haste and authored replacements remain open;
random Genie selection/broader interactions remain Phase2. No playable delivery.

Current independent slice UP222: Orrin Archery core damage/growth12/24/36,
with unrelated bonuses/perks and melee unchanged. Production is frozen and
independently reviewed without a blocker; focused native fixture is pending.
Shared hero-aware core helper feeds live/forecast/AI callback payloads, exact
saved markers preserve prior supported lists. No coverage credit yet.

Completed bounded slice UP221: Crag Hack/Gundula Offense specialties,
core melee physical damage and Attack-growth chances 12/24/36 rather than
10/20/30. Actual source-stamped contribution must be isolated from unrelated
bonuses/perks; shared damage forecasts and live resolution must agree. Separate
Luna production/test ownership and Astra review. Client80060, repair builds
22982/50115 succeed; final native91027 passes15/15 in7.752s, zero skips.
Real aliases/ranks, forecasts/live hits, source-removal projection, independent
bonuses/perk, initial-XP sampler, save/load, rank removal and older lists pass.
Module drift/twelve hero-data checks pass. Compile/oracle fixture failures are
retained; no graphical/playable delivery. Whole Skill-specialty family remains
partial. Phase2 retains future magical-melee semantics and broader compositions.
UP220's full legacy-row audit is persisted in the queue; next implement Shield/
Air Shield hero-only exclusion with actual starter/creature controls, then the
remaining mapped absent-roster rows. Leave ambiguous Haste unchanged.

Full Windows37227083002 is confirmed live on
af17030fc43b89059ebddca3f708519760fa1187, covering UP219 and UP220's six-row
access slice. Previous Windows37221556231 completed successfully on dbd5c7da1.
No duplicate build or launcher promotion; newer source acceptance is pending.

UP220 bounded access slice source/native accepted: builds78840/50252/25274
succeed and native18192 passes18/18 in2.044s with zero skips. Module drift,
19 offline magic/schema and12 hero-data checks pass. Actual acquisition/start
paths, rejected authorized Hero Spell, actual creature effect and old save
round-trip are covered. Production approved; fixture overlap repaired before
native acceptance. No graphical/playable delivery. Next: remaining legacy rows
including core:shield, Haste clarification and authored obsolete specialties.

Completed bounded slice UP220: separate saved-v3 hero-access permission from world spell
membership for six confirmed noncanonical legacy spells. Stop guild/default
book/hero-source leaks while retaining actual creature casts and effect storage.
Focused native acceptance requires real producers and rejection without spend,
not helper assertions alone. Haste remains unchanged pending clarification;
obsolete hero specialties require authored replacements, not guessed bonuses.
Acceptance above applies only to the named six rows, not the entire roster.

UP219 source/native accepted: builds21618/2116 succeed; native12882 passes
13/13 in6.135s with zero skips. Module drift/twelve hero-data checks pass and
Astra reports no blocker. First native30347 failures are retained; fixture
repairs preserve exact marker identity and canonical perk prerequisites.
No GUI or launcher promotion. Skill-specialty family remains partial.

Completed slice UP219: Armorer specialties for Mephala/Tazar/Neela,
covering both core physical reduction6/12/18 and Defense-growth chance12/24/36.
Reuse saved supported aliases and exact producer markers. Fresh markers must
exist before automatic initial-XP level-ups; adjust the growth view once because
the production sampler already consumes it. Separate Luna owners/Astra review,
root registration/build/Git. Acceptance evidence is above.

Next mapped specialty slices: Crag Hack/Gundula Offense and Orrin Archery
require both12/24/36 core damage contributions and12/24/36 Attack-growth
chances. Scale only their exact Skill contributions, not the aggregated damage
factor or perks. Offense is a source-stamped bonus consumed by Lua; Archery's
core contribution is supplied by the shared combat callback. Lord Haart's
Estates separately requires150/300/600 daily Gold, excluding other generators,
perks and handicap scaling. Orrin/Lord Haart fixtures must explicitly grant the
active Skill because Might starting-skill migration can replace its old slot.
These are mapped omissions, not coverage credit. Queue UP220 records the higher
priority legacy spell admission/starting-grant mismatch and effect boundaries.

UP218 production dbd5c7da1f8d19ef55eb11e8c504c5aace739b9c is pushed and
remote-verified. Local handles are terminal. Full Windows37221556231 is queued
on that source (includes UP217/UP218); preserve it, no duplicate dispatch.
Next bounded coverage slice: Armorer specialties for Mephala, Tazar and Neela.
Core-only20% means reduction5/10/15 becomes6/12/18 and Defense-growth chance
10/20/30 becomes12/24/36, without scaling perks. Reuse exact secondary alias
metadata, saved opt-in and stable markers; trace both legacy alias and active
NH effect identities. Extend the shared combat and level-up/view paths together.
This mapping is not implementation credit. Offense, Archery and Estates are
the remaining live legacy Skill aliases; explicit NH replacements stay intact.

UP218 source/native accepted2026-10-04. Both-target95053 and bounded repair41124
succeed; native33370 passes15/15 in6.804s, zero skips. All three Logistics
specialists, all ranks/both pools, Navigation, unrelated bonuses, reused cache
removal, save/load and exact legacy retention pass with adjacent controls.
Module drift and twelve hero-data checks pass; Astra has no blocker. The first
native failure46075 exposed the legacy-versus-active Skill identity mismatch;
the release-failure ledger retains it. One Skill specialty slice is accepted,
not the whole family. Combined source-modifier runtime coverage and broad
interactions remain Phase2. Windows37215692312 is terminal SUCCESS422f0ce0a;
no GUI or launcher promotion. Next: Armorer for Mephala/Tazar/Neela, scaling
both its core physical reduction and its core Defense-growth chance, not perks.

Current slice UP218 is in production/native implementation: Logistics specialties
for Kyrre, Gunnar and Dessa, both core movement pools and no perk amplification.
Root selects explicit saved supported-Skill rules and exact alias provenance,
with inert stable local markers and shared TurnInfo numerical transformation.
The20% factor applies before ordinary source modifiers, never to the aggregate
or Navigation25. Cached bonus values/prototypes stay untouched; old snapshots
without the optional rule/marker retain their behavior. Separate Luna owners,
Astra review, root registration/build/Git. No acceptance or count from the plan.

UP217 source87ef2600039d94e6a192fb4eb600a854c2e9d278 is pushed and
remote-verified with correct author/committer. Local handles are terminal;
Windows37215692312 remains confirmed in_progress on422f0ce0a, excluding UP217.
Preserve that exact job. The next goal cycle should implement the already-mapped
Logistics specialty slice, not repeat damage-family exploration or broad tests.

UP217 source/native accepted2026-10-04. Both-target9817 and fixture rebuild65610
succeed; native23804 passes11/11 in3.504s, zero skips. Ciele cast/estimate/save,
Deemer level/tier, Luna stored Fire Wall/trigger, legacy and rational bounds pass,
alongside three creature-line controls. Astra final review has no blocker.
Module drift,12 hero-data and8 guild checks pass. First compile12061 exposed
Lua arity, repaired by preserving its original method; first native56236 exposed
a target-Initiative fixture error, repaired with explicit controller evidence.
Failures remain in the ledger. This adds one specialty conversion family, with
spell/rank/perk/artifact counts unchanged. Earlier active-build statements below
are historical; no local process remains live. Windows37215692312 is live on
422f0ce0a (excludes this slice). No GUI or playable promotion. Next: Logistics
specialties for all three producers, both core pools without perk amplification.

Current implementation UP217: fixed damage-spell specialty conversion. The
producer audit identifies nine eligible heroes/eight visible spell effects;
Solmyr's replacement and non-damage specialties are excluded. Production uses
an optional saved version1 rule and stable exact-provenance local markers,
not a global scan or prototype mutation. The15% bonus multiplies only the
Spell Power term as23/20 inside the shared rational expression before flooring.
Live and forecast formulas must agree; Fire Wall is boosted once when stored.
Separate Luna production/native owners and Astra review are active. Root owns
registration/build/Git. No coverage credit or playable delivery from this plan.

Next bounded missing slice after UP217: Logistics Skill specialties for Kyrre,
Gunnar and Dessa. Their exact specialty.secondary aliases survive; active NH
Logistics has no generated specialty-target bonuses. Preserve alias provenance
and opt-in saved rules, then scale only rank core Land/Sea10/20/30 to12/24/36
before TurnInfo aggregation. Do not scale Navigation's independent25%, other
perks, unrelated movement bonuses or non-specialists. Root resolves the scope
from the new Skill identity: both Land and Sea are its core, not merely legacy
Land. Check cached/live movement, rank invalidation and saved/legacy controls.
No implementation/coverage credit yet; shared Hero/rules files stay frozen for
UP217's build until explicitly released.

Delivered source422f0ce0a is pushed/remote-verified with a clean worktree at
that checkpoint. Full Windows37215692312 is confirmed queued on that source,
preflight_only=false; retain the exact handle. Previous37211254873 is terminal
SUCCESS on6b6afc677. No local build/native process remains live, and no GUI or
launcher promotion occurred. The next functional slice is damage-spell specialty
conversion, not repeated coverage of this accepted creature-line family.

Current accepted implementation: UP216 creature-line specialties, canonical5269.
Replace alias-generated legacy percentages with flat +1 Attack/Defense per five
levels (cap6), +1 Speed and +1 Initiative. Explicit optional saved rules separate
new instances from unmarked old saves; event-driven marked bonus refresh avoids
polling and prototype mutation. Luna production/native fixture owners are
separate; root owns existing tooltip wiring, registration, build and integration.
Creation, level thresholds, line/upgrades, legacy/custom controls and saved-state
preservation pass: both-target4780 and fixture rebuild77861 succeed, native85455
passes7/7 in2.928s with zero skips. This adds one native-verified specialty
conversion family; other feature counts remain unchanged. Independent production
review finds no blocker. Prototype-only description surfaces and broader
interactions remain Phase2. Windows37211254873 is now terminal SUCCESS on
6b6afc677, excluding this slice. Earlier live statements below are historical.

Next audited functional slice after UP216 freezes: canonical damage-spell
specialties. Deemer's SPECIAL_SPELL_SCALING still scales the whole adjusted
result by hero level/target tier; Ciele's SPECIFIC_SPELL_DAMAGE50 also scales
the whole base. Canonical5270 instead specifies fixed +15% of the Spell Power
component. Existing BattleSpellCastTest809 proves legacy behavior, not NH
conversion. Preserve Solmyr's explicit replacement. Do not run a parallel
writer over CHeroHandler/CGHeroInstance while UP216 owns those files. Non-damage
and Skill specialty conversions also remain gaps; resource quantities retain
the specified legacy behavior. Primary-specialty inventory remains unproven.

Next bounded UP023 selection: Reactive Weave (UP215) awaits a newly asked
full-versus-half readiness coexistence decision. No activation/coverage credit.
The other checked candidates share existing blockers: SageUP074, recruited-
cohort trainingUP127, EspritUP130, and Veiled Movement's absent reaction producer.
Do not repeat those maps or turn generic move dispatch into inert protection.
This does not establish that every remaining specification item is blocked.
Phase1 remains active; preserve Windows37211254873's confirmed live handle.

Delivered source6b6afc677 is pushed and remote-verified; worktree was clean at
that checkpoint. Windows37207110382 is terminal SUCCESS onb6ef78e1b (Fortress,
parchment binding and Orbs). New full Windows37211254873 is confirmed in_progress on
6b6afc677, including UP214; preflight_only=false. Keep this exact handle; no
duplicate dispatch, GUI or launcher promotion. Earlier live-job statements below
are historical. A bounded read-only selection now seeks one unexamined planned
perk under UP023, excluding all previously mapped clarification blockers.

UP214 source/native accepted2026-10-04. Both-target80140 and bounded fixture
rebuild14491 succeed; native39842 passes6/6 in2.362s, zero skips. Shared live/
explicitly detached resistance caps75 after unchanged artifact/innate and aura
composition. Real equipment, seeded74/75 accepted hostile casts, positive Haste,
independent immunity, legacy76/100 and penetration/Twist controls pass. Module
drift and seven adjacent artifact-data checks pass; Astra final review has no
blocker. Targeted artifact-family coverage5->6 of10, other counts unchanged.
Phase2: untouched-recipient projected aura previews, shared historical-v2
fixture sanitation and broad interactions/rendered feedback. Scroll candidate
still awaits user approval. No graphical launch or playable promotion.
The mapping and build-in-progress paragraphs below are historical; all local
build/test handles named here are now terminal. Windows37207110382 remains live
onb6ef78e1b and does not include UP214; no duplicate dispatch.

UP214 is the next unblocked functional gap. Canonical total Magic Resistance
caps75%, but existing raw/live/AI/UI consumers allow100% and target legality
treats that as immunity. Root selects one shared battle-aware calculation,
optional unit-environment forwarding and projected adjacency; retain additive
artifact/innate values and existing aura composition/rounding. Legacy behavior,
Spell immunity and Misfortune's separately pending policy stay unchanged.
Production and native fixture ownership are separate; root retains integration,
one serialized12-job build and source delivery. No count until focused principal
execution passes. Scroll candidate remains held for user visual approval.

UP214 frozen production review finds no blocking issue: raw bonuses avoid getter
recursion and all 10,201 clamped base/aura combinations preserve legacy results.
Phase2 finding: HypotheticBattle may return an untouched live recipient while
only its aura-bearing neighbor is projected. That recipient still uses live
adjacency; explicitly detached recipients use projected adjacency. The75% cap
holds in both cases. Focused acceptance must not imply untouched-recipient aura
preview parity. Native fixture/build acceptance remains pending.

UP214 fixture is frozen with three principal native cases: real equipment and
Unicorn aura, detached adjacency/bonus changes, accepted seeded74/75 hostile
casts, independent immunity, positive Haste and legacy76/100 controls. Build
session39401 is live (`vcmitest vcmiclient`,12 jobs); production and AI objects
compile, final link/native execution remain pending. Preserve this handle until
terminal observation rather than starting a second local build.

Build39401 and diagnostic32791 terminated with a fixture-only raw-enum variant
error; corrected to typed SpellID. Retry58491 terminated on root's selector
conjunction mistake; use the existing typed hasBonusFrom API for Haste instead.
Lessons/logs are retained in NH_RELEASE_FAILURES.md. Current resumed build80140
is live at12 jobs; the corrected native fixture object compiles successfully,
but final link/execution and all coverage credit remain pending.

Delivered source checkpoint: Fortress34bf2fa1f and Orbsb6ef78e1b are pushed.
Full Windows37207110382 is confirmed live onb6ef78e1b11f269f2ad1992ebdd999ea5e0d02c6;
preflight_only=false explicitly requests compilation. Keep this handle through
terminal observation; no duplicate job or launcher promotion.
UP212 remaining art is enumerated in NH_GUILD_SCROLL_EXPORT_AUDIT.md (26 opaque
source exports, no transparent alternatives). The Heroes III workflow produced
one local scroll-only Holy Wrath candidate; user visual approval must precede
live import/full-family expansion. Shared book/effect/scenario bindings stay
unchanged. Avoid remapping Pursuit March:UP209/193 duplicate UP104's already
mapped cap/zero-recovery questions and add no implementation progress.

UP210 final native acceptance: build59223 and native71275 succeed. All nine
Orb cases plus Fortress construction pass10/10 in4.479s, zero skips. The cap
fixture preserves acting ownership with explicit low Initiative; production
authentication is unchanged. Four real equipment/save/removal/forecast/cast
paths and explicit element/cap/obstacle/wire controls are accepted. Targeted
artifact-family coverage4->5 of10. Eight data checks and module drift pass.
Broad spell/artifact/proxy composition and strategic AI valuation remain Phase2;
no GUI/launcher promotion. This supersedes historical8/9/no-credit statements.

UP213 Fortress Mage Guild v9 replacement is source/build verified: supplied
all-five native DEFs, masks, campaign icons and hall0–4 imported reproducibly;
71 runtime assets across retained packages,46 validated obsolete Fortress v8
files removed with historical archive preserved. Eight asset tests pass;
independent Astra review reports no blocking issue. Both-target build59223 and
combined native71275 pass (10/10, zero skips), including sequential guild costs,
prerequisites and all five loaded Fortress positions/bindings. Other towns and
non-art rules are unchanged. Private decoded first-frame inspection is not
graphical town-scene/playable acceptance; no launcher promotion.

UP212 binding slice is source/build verified: client86675 succeeds, existing
Mage Guild art/data controls pass5/5, and independent Astra review finds no
blocking issue. Reference purchaser TPMAGES.DEF frame0 under standalone NH
icons, preserving original complete83x61 scrolls, full hitboxes and native
small-emblem sizes; oversized aliases fit within54x45. No template pixels or
new dependency shipped. Opaque painted backgrounds/proper transparent scroll
emblems and actual rendered acceptance remain open UP212 work; no final-art or
playable promotion claim. Frozen Orb native controls now pass8/9, with a single
cap-cast fixture rejection under bounded diagnosis; do not credit it yet.

Full Windows37199468684 is terminal SUCCESS, confirmed2026-10-04, on committed
69c18b19e1f08008834df67131701a0e0e26de6a. It covers Conflux/Garden, not the
current uncommitted Orb or Mage Guild fixes. A fresh compiled checkpoint may
be dispatched after those changes pass focused gates and are committed.

UP212 resumption evidence: plain iconScroll images are not complete83x61
parchments; some are opaque RGB paintings with their own dark background.
Adding that square over a blank is not visual acceptance. Inspect native blank
frames and preserve proper role composition, transparency and native hitboxes.
The old worker service handles disappeared at goal continuation; root rechecked
the team (root only) and delegated the bounded asset inventory to Luna
guild_parchment_assets. No new art or original-pixel import is authorized here.
UP210 retry34064 also lost its handle, with no cmake/ninja/compiler process
remaining and no terminal-success log. Root verified stoppage before resuming
the incremental native-only build65339,12 jobs; do not advertise the interrupted
retry as a successful build.

New priority UP212,2026-10-04: Mage Guild new spell emblems are missing from
their parchments. Independent Luna UI/asset diagnosis now takes priority, using
the original rendering and VCMI Extras blank parchment reference. Preserve the
frozen Orb production source and safely finishing focused fixture owner. Do not
start another backlog feature or claim visual acceptance from code-only checks.
No GUI/input authorization is inferred. Root will serialize combined builds.

Current slice UP210 implements the approved actual-element Orb conversion.
Generic metadata and caster/proxy final damage are delegated independently from
real equipment/cast/forecast fixtures. Root owns append-only Bonus and save-format
guards plus registry/data and one12-job build. Ten explicit elemental tag rows
are approved from canonical descriptions; neutral/necrotic/physical spells have
no inferred affinity. Do not credit until production paths and focused native
acceptance pass. Full Windows37199468684 remains live on Conflux69c18b19e.

UP211 committed/pushed69c18b19e1f08008834df67131701a0e0e26de6a. Notice-only
37199469826 succeeds on that head; full Windows37199468684 is in progress on
the same head. Preserve its handle; no duplicate dispatch, compiled-success
claim or local snapshot promotion. Source/native evidence remains separate.

2026-10-04 UP210 ruling received: actual-element tags independent of Schools,
neutral/necrotic untagged. Its design blocker is resolved; elemental Orbs are
next after accepted UP211 delivery, ahead of the Vault map. No Orb coverage
credit until production damage, equipment, forecast and focused evidence exist.

UP211 Conflux recruitment/Garden source/native accepted2026-10-04. Both-target
build7085 and fixture-only retry28194 succeed; native75381 passes3/3 in2.168s,
zero skips, UP211-conflux-focused-retry.log/XML. Independent Core stocks14/10,
Garden18/13 growth, next-week32/23 stocks, actual construction/recruitment,
eight-row save/load, explicit old-seven-row rejection and built AI forecasts pass.
Python13/13, module drift and Astra source review pass. Source delivery follows;
no GUI acceptance or playable promotion. Counts remain214/310 perks and61/67
combat identities. Next unblocked missing item: Vault of Ashes+2 Fire Elemental
growth. Phase2 retains co-located art/layout and preconstruction Sprite/Garden
AI valuation; do not reopen adequate native coverage to polish those now.

Full Windows37194377145 is now terminal SUCCESS on cd416f22e72591f8132dc990dbf4067fb1b329f3,
confirmed2026-10-04. It excludes UP205/UP206 and the current Conflux candidate.
The next compiled checkpoint may be dispatched after the new source is accepted
and committed; no dirty-source or duplicate build is being advertised as delivery.

2026-10-04 current slice UP211: the prior reply confirmed an already implemented
Puppet Master ruling and added no coverage. UP210's independent maps identify
missing element metadata; its tagging-policy question is pending. Conflux growth
audit finds Pixie/Sprite remain a legacy upgrade chain despite explicit separate
Core lines14/10. Root selects existing eight-dwelling support, saved single-member
growth lines and shared Garden growth, with independent data/UI and native/AI
owners. Remove the upgrade path and exercise actual construction/weekly stocks,
not just query-only values. Vault of Ashes remains a separate missing building.
This preceding audit is now superseded by the focused acceptance above; no
graphical acceptance or promotion. Full Windows37194377145 is terminal SUCCESS
on cd416f22e and does not contain UP211.

Resumption correction: deeper queue inspection finds UP208/UP209 repeat the
complete UP103/UP104/UP193 maps and unanswered design choices. Both new maps
are stopped and marked superseded; do not keep cycling through them. Select
UP210 elemental-Orb conversion instead: canonical25% final matching-element
damage, not a legacy School50% modifier. Parallel bounded runtime/data maps
check actual tags, shared damage/AI and fixture surfaces. No activation/count
from mapping. UP207 Mana stacking and Logistics questions remain unresolved.

2026-10-04 next cycle: preceding UP205/UP206 cycle made verified progress and
pushed runtime a8e8c4a55 plus delivery notes8c3d32c83; resumption tree is clean.
Notice-only37196269759 now succeeds on a8e8c4a55. Full37194377145 remains live
on cd416f22e, excluding those features. Preserve its handle. Parallel bounded
Luna maps now cover Rapid Embarkation and Pursuit March, the two remaining
Logistics perks; root retains architecture and waits for consequential rule
boundaries before activation. UP207 stacking clarification remains unanswered.

UP205/UP206 committed/pushed a8e8c4a55b66b1f95e233a6e5f085bc1e70047eb; tracked
tree clean before these delivery notes. Notice-only37196269759 is queued on
that source. Full37194377145 remains in_progress on cd416f22e, excluding this
slice; no duplicate full dispatch or playable promotion. UP207 mana-artifact
map identifies a real per-item-versus-aggregate maximum boundary; clarification
is requested and queued, not silently defaulted. Wizard's Well is outside the
explicit old1/2/3 conversion. Next unblocked candidate: missing Logistics Rapid
Embarkation, mapping the existing shared boarding-cost path and actual AI use.
The Phase1 goal remains active;96 perks and six combat identities remain planned.

UP205/UP206 accepted source/native2026-10-04. Both-target retry68082 succeeds;
native26470 passes6/6 in3.290s, zero skips, UP205-UP206-focused.log/XML. Master
Logistician has actual legal progression/day/boat/pathfinder/Stables/save and
legacy controls. Three Speed artifacts have matching Initiative with explicit
and fallback live creatures, cache-refresh removals and detached AI projection.
Python25/25, module drift and Astra reviews pass. Perks213->214/310, Logistics
7->8/10; ranks87/93, faction perks62/90 and combat61/67 unchanged. Four targeted
artifact-conversion families now have evidence. Future-day AI carry forecasting,
projected creature-form limiter reevaluation, broad composition and graphics
are Phase2. No GUI/playable promotion. Commit/push this coherent checkpoint;
preserve full Windows37194377145, still in_progress on cd416f22e, which excludes
these new features. Next read-only gap map is Mana-regeneration artifacts.

2026-10-04 resumption: the preceding clarification turn verified an already
implemented Puppet Master decision and made no new coverage progress. UP205
native fixture remains delegated and running. Select independent UP206 next:
conditional Initiative bonuses for the three Speed artifacts, with actual
equipment/live-battle and detached-AI evidence. No new coverage credit yet;
root retains serial builds and integration, workers have separate new files.

Full Windows37194377145 is confirmed in_progress on committed
cd416f22e72591f8132dc990dbf4067fb1b329f3, containing UP203/UP204 but not UP205.
It was dispatched once after full37191507353 terminal SUCCESS. Preserve this
handle and do not restart because an observation times out. UP205 client57328
succeeds; selected registration/inventory19/19 now passes after updating the
explicit activation expectation. Source Astra review finds no blocker;
principal native day/boat/Stables/save acceptance is still pending.

2026-10-04 UP205 selected: implement the mapped Master Logistician Expert perk
through NewTurn, keeping ordinary maximum Movement unchanged and retaining the
15% unused carry through Stables. Separate Luna source/fixture ownership;
root owns integration/activation/build/Git. The preceding goal cycle made
concrete progress: UP203 and three UP204 artifact rows are committed/native
verified. The tree is clean at resumption. Notice37194146484 now succeeds on
ef02ff1d72; full Windows37191507353 now succeeds on ebc1d58db. A subsequent
meaningful full checkpoint may include the committed friendly-fire/artifact
slice; do not confuse it with the still-uncommitted UP205 runtime.

UP203/UP204 delivery checkpoint: committed and pushed
ef02ff1d72b9ee9b68ac678644a12b03c4c8cea2; tracked tree clean and0ahead/behind
before these evidence notes. Windows notice-only37194146484 is confirmed live
on that source, not a compiled package. Full37191507353 remains live on its
previous ebc1d58db source; preserve the job rather than duplicate it. Root owns
the next meaningful full checkpoint once this job is terminal. Phase1 goal stays
active; next implementation is the mapped Master Logistician perk, not polishing
the already focused-verified confirmation or artifact framework.

UP203/UP204 accepted source/native2026-10-04: friendly-fire confirmation uses
actual effect recipients (including possible Hand of Fate collateral) and the
native yes/no dialog; three artifact-conversion rows now have78 corrected bonus
records across43 NH overrides with truthful descriptions. Client retry16088 and
both-target64537 pass. Native71900 passes6/6 in1.610s, zero skips, plus focused
Python24/24, module drift and diff checks. Independent Astra reviews find no
blocking source/fixture issue. Initial compiler/fixture failures are retained.
Phase1 continues; perks213/310, ranks87/93, combat61/67 unchanged. Phase2 retains
rendered confirmation/callbacks, broad spell interactions, assembled artifact/
save roundtrips and strategic artifact valuation. No GUI/playable promotion.
Next highest-priority mapped unblocked perk: Master Logistician, using NewTurn
events and preserving its carry through Stables refill. Full Windows37191507353
remains live on ebc1d58db053243a9d201169974adc26853366c6 and excludes this slice.

2026-10-04 next selected slices: UP203 implements the canonical friendly-fire
confirmation using actual effect destinations and the native yes/no dialog;
UP204 supplies the missing NH-only Primary Attribute and flat Movement artifact
conversions. Separate Luna workers own those independent surfaces and focused
fixtures. Root retains CMake/module registration, builds, integration and Git.
Master Logistician is mapped as an unblocked subsequent perk, including the
Stables refill interaction; it is not silently substituted for required UI.
No new coverage credit until compiled principal-path evidence passes.
Full Windows37191507353 is confirmed in_progress on ebc1d58db053243a9d201169974adc26853366c6.
The previous answer turn verified an already-recorded Puppet Master ruling;
it added no implementation coverage. This cycle proceeds with concrete edits.

2026-10-04 post-UP202 selection audit: root revalidated the clean source and
live full Windows37187930978, preserving its handle. Two independent Luna
read-only audits check planned perks/foundations and creature/artifact/specialty/
required-UI gaps for genuinely unblocked next items. Existing unanswered rules
are not silently defaulted; already documented architecture is reused. Root
corrected stale breadth counts from the current canonical tables:37 grouped
unique-building rows and10 artifact-conversion rows, not33/nine. No mechanic
activation or completion credit follows from inventory correction.
Full Windows37187930978 completed SUCCESS on5899674a0. Root dispatched one
new meaningful checkpoint only after that terminal success: full37191507353
is queued on ebc1d58db053243a9d201169974adc26853366c6, incorporating Stables
and Blood Obelisk. Preserve this new handle; no duplicate job or playable
promotion. Notice-only37191098623 already passed on the Blood Obelisk source.

UP202 Blood Obelisk accepted2026-10-04. Client32362 and both-target20101 pass;
native31232 passes4/4 in2.870s, zero skips, UP202-blood-obelisk-final.log/XML.
The actual siege defender gains20 hero Attack and corresponding HeroCommand
coefficient, not raw creature Attack. Shared cancellation/results cleanup,
restart, no-hero isolation, real weekly per-hero/per-physical visits, both damage
subtypes, saved blessing/history, accepted-result consumption and next-week
reuse pass; Stables/Fountain remain green. Data/inventory22/22 and module drift
pass. Independent Astra production review found no blocker; its fixture review
caught a null layout argument before execution, repaired by the tester. Root
corrected compile/baseline assumptions and inspected the final fixture. One
specified town mechanic added; perk/rank/spell counts unchanged. Complete damage
resolution, strategic AI valuation and graphics remain Phase2, as do generic
setup-snapshot producer limitations. Integrate this source checkpoint; preserve
full Windows37187930978 on5899674a0, still compiling and excluding this slice.
Source committed/pushed cd1b1f93c4c99659beaefa75f59b711605375693; notice-only
Windows37191098623 completed SUCCESS on that source. No compiled Windows or
playable delivery claim follows from notice preflight. Preserve the full run.

2026-10-04 UP202 Blood Obelisk implementation is in progress. Generic
defendingHeroBonuses content applies only to the actual siege defender hero;
reserved building-scoped bonus identity supports cancellation/results cleanup
without consuming visiting blessings. Independent runtime and fixture workers
have disjoint ownership. Root has added Fortress content and a focused data
guard; data/perk/inventory20/20 and module drift pass. These checks do not
establish runtime coverage. The previous turn confirmed an already implemented
Puppet Master decision, not a new coverage item. Current full Windows37187930978
remains live on5899674a0, now compiling the Windows client; no replacement
dispatch, GUI run or playable promotion occurred.

UP201 Stables accepted2026-10-04: client56799 and both-target62880 exit0;
native71208 passes2/2 in1.894s, zero skips, UP201-stables-focused.log/XML.
Both resident slots, shared exact Movement/refill, save, expiry/nonstacking,
midday isolation and slow/fast army parity pass, plus adjacent Fountain. Data/
inventory21/21, module drift and Astra production review pass. Root inspected
the focused fixture. One specified town mechanic added, no perk/rank/spell
count changes. Integrate this source checkpoint while UP202 Blood Obelisk is
read-only mapped. Source supports legitimate allied residents; explicit allied
scenario coverage, inconsistent-reference hardening and strategic AI valuation
remain Phase2. No graphical run or playable promotion is claimed. Preserve
the existing full Windows37187930978 on5899674a0; it excludes Stables.

2026-10-04 UP201 Stables production is frozen and Astra-reviewed with no
blocking finding. Day-start after NewTurn expiry grants visiting/garrison
Castle residents a saved ONE_DAY land-Movement20 PERCENT_TO_BASE town bonus,
then refills the beneficiary from the shared current-day maximum. Legitimate
allied residents qualify; nonresidents and legacy movement are unchanged.
The NH override clears the old flat400/week visiting reward and alias.
Data/inventory21/21, module drift and diff checks pass. Client56799 is building
with12 jobs; the isolated fixture remains unregistered until build terminal.
No coverage credit or playable promotion yet. Phase2 retains defensive checks
for inconsistent town-resident references and broader strategic AI valuation.
Existing full Windows37187930978 remains live on5899674a0, excluding this
dirty Stables slice; no replacement or duplicate full build is dispatched.
Stables is now committed/pushed761ba562be91ca43488f6ff388d400e192943f16;
notice37188732374 completed SUCCESS on that exact source. Full37187930978
is confirmed in_progress; preserve it. UP202 Blood Obelisk map is complete:
the weekly melee/ranged physical blessing fits existing rewards, while siege
Attack20 needs a precise defending-hero-only hook and HeroCommand propagation
inspection, not a blanket creature Attack20 bonus. No design blocker found;
this is the next unblocked implementation slice, not new coverage yet.

UP201 Fountain native acceptance: final both-target23674 passes; native12287
passes1/1 in1.136s, zero skips, UP201-fountain-final.log/XML. Actual construction,
visits, recipient isolation, independent hero/building weekly history, saved
bonuses/visitors, accepted-result cleanup and next-week regrant pass. Two fixture
setup assumptions were repaired without changing production behavior. Data/
inventory20/20 and module drift pass; Astra production review finds no blocker.
Root inspected the passing native fixture; separate independent fixture audit
remains Phase2 (the reviewer returned its production assessment only).
Add one specified town mechanic, not a perk or
spell. Full battle/retreat/replay, strategic AI routing and graphics remain
Phase2. Integrate this source checkpoint, then continue mapped Stables; do not
claim that accepted-result cleanup proves a full battle or playable promotion.
Fountain is committed/pushed12fc078e844ed269a71c53d33d653a107287c4e1;
notice37187847868 is confirmed live on that exact source. Preserve its handle
and dispatch the next full Windows build after this preflight, once only.

2026-10-04 UP201 Fountain of Fortune is the next unblocked building slice.
The NH patch replaces local defending Luck2 with3 and adds a Luck2 ONE_BATTLE
visiting reward using per-hero/per-physical-building history with weekly reset.
No new runtime state, poller or art is needed. Data/inventory20/20, module drift,
Astra source review and client build38823 pass. The isolated real-visit/save/
week/combat-expiry fixture remains pending; no coverage credit or playable
promotion yet. Castle Stables/Lighthouse are mapped real functional gaps,
not tooltip changes; daily grant/refill ordering and town-source embarkation
must be shared by authoritative movement/pathfinding/AI. The Lighthouse source
scope question is asked; Fountain is independent of it and UP200 aura choices.
Full Windows Resource Broker37182637895 is confirmed completed SUCCESS on
a8046ec2fbc204237c4e17da6e335f8863bed8cb. It does not include UP198/199/201.
Academy notice37185975539 completed SUCCESS on ce666c92c; it is a source
preflight, not a compiled Academy package. Dispatch the next full build only
after the next coherent source checkpoint, not as a replacement for a timeout.

UP199 is committed and pushedce666c92c1b50ef02654ccc98cba9c11f630f769.
Notice preflight37185975539 was dispatched once and is confirmed in_progress
on that exact source. Existing full Windows Resource Broker37182637895 remains
in_progress on a8046ec2f; it excludes Amplifier/Academy. Retain both handles;
no duplicate or replacement full build was dispatched. UP200 Glyphs of Fear
map is complete; radius/layer and overlap-stacking answers are pending. No
production aura or extra town coverage is inferred from mapping. Phase1 goal
remains active; this design choice blocks that slice, not the full backlog.

UP199 Academy accepted2026-10-04: client77558, baseline19532 and both-target
retry82390 build successfully; native49376 passes10/10 in3.561s, zero skips,
retained as UP199-academy-focused.log/XML. Real visits/preview/grant/history/save
and reward parser/version/cap/Learning guards pass. Adjacent Spell Point reward
tests remain green. Data/inventory21/21, module drift and Astra reviews pass.
One specified town mechanic added, no perk/rank/spell count changes. No playable
promotion. Root integrates this coherent slice before UP200 implementation;
Glyphs of Fear is still read-only mapped, not an implemented area aura.

UP199 baseline19532 completed successfully. Root registered the frozen Academy
fixture and both-target33367 failed on forward-declared Bonus serialization
types in that fixture. The tester owns a direct-header correction; retain
UP199-academy-fixture-build.log. Production/client already builds; native
acceptance is still pending. Do not widen this to an unrelated integration run.

UP198 is committed and pushed90c7d41331bb37586dce062a38dc3b194489d8f3.
Its notice preflight37184744361 completed successfully on that exact source.
Full Windows Resource Broker37182637895 remains live on a8046ec2f and excludes
Amplifier. Retain the existing handle; no competing full build was dispatched.
UP199 runtime and isolated-fixture writers are now active with disjoint files.
The NH Dungeon special4 content uses once-per-hero25% remaining XP and zero
fixed XP; its focused Python guard passes. No source/native coverage increase
or playable promotion is claimed until the actual shared reward and visits pass.
UP199 production is frozen and Astra source-reviewed without a blocker. Client
build77558 is live with12 jobs; retain its handle and frozen headers. New
isolated Academy tests may be written unregistered during compilation; root
alone registers CMake after this build terminates. Data/inventory21/21 pass.
The percentage helper reuses Learning, shared preview/grant and existing
physical-building visitor history. New reward data is append-only versioned,
old reads default zero and populated old writes reject before Reward payload.
Inherited extreme-XP calculateXp multiplication overflow is deferred to Phase2.
Client77558 completed successfully (323 steps). Baseline vcmitest compilation
is started next against the same frozen production bytes; the separate Academy
fixture remains unregistered until its bounded source corrections are frozen.
Do not claim native acceptance or run the stale pre-Academy test binary.
Baseline19532 is confirmed live. The two-case Academy fixture is now frozen
and independently Astra-reviewed without a blocker; register only after the
build ends. Required worker/reviewer tasks are complete, not left running.
The focused filter is NewHorizonsBattleScholarAcademyTest.*. Real town-visit
execution for a computer-owned hero does not claim Nullkiller route/valuation.

2026-10-04 UP198 accepted: final both-target96096 exits0; native4614 passes
19/19 across five focused suites in1.692s with zero skips, retained as
UP198-amplifier-accepted.log/XML. Real visit/save/refresh/day expiry and actual
computer-winner raising pass. Data/inventory20/20, module drift and Astra review
pass. One specified town mechanic added;213/310 perks,87/93 ranks,62/90 faction
perks and61/67 combat identities unchanged. No GUI/playable promotion.
UP199 Academy proportional XP is next; root will integrate the accepted
Amplifier before permitting its runtime/test writers to change the next slice.

2026-10-04 UP198 Necromancy Amplifier is the next unblocked functional building
slice. Its canonical visiting-hero7-day bonus was absent: the core aura was
kingdom-wide and ignored by the NH raising resolver. Production/configuration
are frozen and independently reviewed without a blocker; data guard/module
check pass. Client68479 is running with12 jobs. Preserve it until terminal;
the separate native fixture is being written and remains unregistered. Exact
visit, nonstack/refresh/expiry, actual raising, save and AI evidence are pending.
The generic stored-bonus expiry path is reused, with no new poller or counter.
All existing coverage totals remain unchanged until the principal gates pass.
Client68479 completed successfully (293 build steps). Baseline vcmitest41059
is now live with12 jobs against the changed headers; the new isolated fixture
remains unregistered. Focused Python data/inventory20/20 and module drift pass.
Mindbreaker full Windows37180938926 completed successfully on1d3a80185;
Resource Broker37182637895 is now in_progress on a8046ec2f. Both exclude dirty
UP198. Retain the existing handles; no duplicate full build was dispatched.
Next unblocked building UP199 is mapped: Academy still grants fixed1000 XP
rather than25% remaining-to-next-level. Reuse generic reward/preview/visitor
paths, ordinary floor/Learning conventions and guarded saved reward data.
Implementation waits for UP198 principal acceptance; mapping is not coverage.
UP198 baseline41059 reached its final link and its process is terminal. The
registered fixture build45525 then failed on missing direct CHero and
CSkillHandler includes; retain UP198-amplifier-fixture-build.log. The tester
owns the narrow include fix. Final semantic fixture review found no blocker,
including exact stored1/7-day durations across save/load and actual computer
winner raising. Native acceptance is still pending; no stale test was run.

2026-10-04 continuation: Resource Broker notice preflight37182430857 completed
successfully on d4e0e996a. Full Windows37182637895 was dispatched once and
confirmed queued on a8046ec2fbc204237c4e17da6e335f8863bed8cb, whose only
additional change is this tracking document. Retain that handle; do not replace
the running Mindbreaker37180938926 or claim compiled delivery from a queued run.
The worktree was clean before this record. Phase1 continues with a bounded
audit for the next unblocked missing functional item; existing quota/design
questions remain blockers for their specific entries, not for the whole goal.
The next concrete missing building is UP197 Skeleton Transformer: the legacy
type-only conversion does not implement the authored HP-based output. Runtime
and interaction/test maps are complete; pooled-selection versus per-slot
rounding is awaiting one explicit answer. Existing vector trades can represent
a combined selection, but the window currently emits individual requests.
Output preview and minimum AI conversion hooks are missing. Do not declare the
building complete from a single-stack calculator or a registration flag.
Independent ledger review verifies213/310 perks,87/93 ranks and62/90 faction
perks and the corrected Necromancy/Diplomacy rows. No production code changed
in this audit cycle; no broad test suite or local playable build was run.

UP196 Resource Broker is committed/pushed as
`d4e0e996a711c4d7be8544f0687b0c70c9057518`. Notice preflight `37182430857`
was dispatched once and confirmed queued on that exact source. Retain that
handle before dispatching a full build. Mindbreaker full Windows `37180938926`
remains confirmed in_progress on `1d3a80185`, excluding Resource Broker.
No source/native acceptance is promoted into graphical or playable delivery.

2026-10-04 UP196 Resource Broker source/native accepted. Client retry94429,
baseline vcmitest13751 and both-target fixture retry38283 exit0. Native64173
passes7/7 across two suites in1.373s, zero skips: legal Advanced offer, exact
shared quotes/resources, local residence/direction guards and actual AI callback
request through server validation. Reports UP196-resource-broker-focused.log/XML.
Independent Astra source/fixture reviews find no blocker; data/inventory19/19,
modulecheck and diffcheck pass. Perks212->213/310 (97 planned), Estates5->6/10;
combat61/67 and ranks87/93 unchanged. No new stored state, art, GUI or playable
promotion. Pair-aware AI best-market selection, broader perk composition and
rendered feedback remain Phase2. Earlier UP196 pending/build observations below
are historical and superseded by this acceptance; compile repairs remain in
NH_RELEASE_FAILURES.md.

2026-10-04 bounded remaining-item audit: Learning Master Teacher still awaits
UP164's Mentor prerequisite ruling. Learning Sage is a distinct Expert perk
from Wisdom Sage's extra-guild-spell reveal; its unimplemented first-visit award
also depends on UP074's pre-acquisition visitation policy. Neither planned row
is implemented by ordinary giveSpells. Do not conflate the two Sage identities
or invent historical visit entitlement. Master Logistician likewise remains
planned: the carry arithmetic in "up to15% of unused Movement" needs an explicit
choice before activation. Resource Broker is the unblocked implementation in
progress; these read-only findings do not increase coverage.

UP196 client70173's private-member compilation error is corrected through
getVisitedTown(); client retry94429 exits0. Serialized vcmitest baseline compile
is running against the changed shared headers, before the new isolated fixture
is registered. Retain UP196-resource-broker-test-baseline-build.log. Native
acceptance and coverage increase remain pending; no launcher promotion.

2026-10-04 UP196 Resource Broker production is frozen in IMarket and town
resource-pair effectiveness hooks. The common quote path applies the20% rate
once for Wood/Ore-to-rare trades while an active captured perk holder actually
visits/garrisons the town. Null-hero town trades benefit; remote holders and
other resource directions do not. Existing custom-market virtual dispatch and
integer rounding are preserved. Independent Astra review finds no blocker;
broader perk composition and rendered feedback remain Phase2. Candidate
registry/module/inventory are active for normal-offer verification, not accepted
coverage yet; counts remain212/310. Data/inventory19/19 pass. Client build70173
runs with12 jobs, retaining UP196-resource-broker-client-build.log. Native and
AI fixtures are being written separately and remain unregistered. Preserve the
build handle and launcher snapshot; no GUI/art or playable promotion.

UP194 source/native acceptance is committed and pushed as
`1d3a8018580b1fc3631c77e7c627b20cebfb2f6e`. Windows notice preflight
`37180892273` completed successfully on that exact source. Full Windows
`37180938926` was dispatched once and confirmed queued on the same source;
retain its handle. Earlier full Windows `37177603721` completed successfully
on `e4946162f`, excluding UP194. Neither observation is UP194 compiled-package
or graphical acceptance; the launcher snapshot remains unchanged.
Next missing candidate is UP195/UP129 Legendary Reputation. Its production
forecast/join/state seams are mapped; the monthly quota boundary after refusal
or zero admission awaits the user's answer. Do not replace mercenary-provenance
or other already recorded blockers with speculative gameplay decisions.

2026-10-04 UP194 Forgetfulness and Chaos Mindbreaker are source/native accepted.
Client retry5595 and test retry49144 build; final focused native retry2 passes
24/24 across seven suites in5.855s with zero skips. Data/inventory19/19,
modulecheck and diffcheck pass; canonical SHA remains unchanged. Independent
Astra review finds no blocker. Active perks advance211->212/310 (98 planned),
Chaos Magic3->4/10; combat spell identities61/67 (Chaos7/11) and ranks87/93
are unchanged. Status is Verified (delivery pending), not a GUI or playable
promotion. The creature-window status popup's legacy Forgetfulness text, broad
cross-system interactions and external retaliation-grace behavior remain
Phase2 follow-ups. The successful full Windows job37177603721 ran on
e4946162f and excludes UP194; it is not Windows acceptance for this slice.
See NH_RELEASE_FAILURES.md for the retained historical failure trail.

The dated UP194 candidate/pending entries below are historical pre-acceptance
checkpoints preserved for traceability; they are superseded by the accepted
status above and do not describe current blockers.

2026-10-04 UP194 candidate registration is active for legal-offer verification;
accepted counts remain211/310 until focused native/build gates. Data/inventory
pass19/19. Shared runtime and AI raw-baseline filtering are implemented; review
identifies bounded known native special-attack classification omissions for
correction before final freeze. No playable promotion or graphical testing.

2026-10-04 Forced March notice37175786029 succeeds on e4946162f. Full Windows
37177603721 is dispatched once and confirmed in_progress on that same revision.
It excludes the uncommitted UP194 candidate. Preserve the exact job handle;
successful preflight is not compiled/playable acceptance.

2026-10-04 Windows37174334529 completes successfully on f534f59c4, including
client compile/package. It excludes Forced March. Notice37175786029 is now
confirmed in_progress on e4946162f; retain it before dispatching that revision's
full build. Earlier live/pending statements below are historical observations.

2026-10-04 UP194 implementation assigned after baseline audit. Canonical
Forgetfulness is incomplete beyond shooting. Shared runtime and real-cast
fixture owners implement full base restrictions plus Mindbreaker; root handles
typed marker/version, Lua duration/cost/profile and integration. Astra review
requires unsuppressed evaluated baselines for live/nested projected restoration,
not trait deletion. A separate AI-worker spawn hit the service thread limit;
reuse a Luna owner after freeze. No activation/count/build acceptance yet.

2026-10-04 UP193 maps complete and reconfirm the prior UP104 contract, including
its unresolved recovery cap and zero-recovery daily-expenditure choices. No
production activation. Continue UP194 Mindbreaker: a bounded read-only map of
Forgetfulness and passive offensive creature-ability suppression. Existing
Discipline/Logistics design blockers are not remapped or silently resolved.
Windows37174334529 remains confirmed in_progress on f534f59c4 and notice
37175786029 pending on e4946162f; retain those exact handles.

2026-10-04 next missing feature: UP193 Logistics Pursuit March. Runtime and
focused-test owners map only the post-win recovery/day-state and real battle/AI
seams. Preserve accepted Forced March e4946162f, its independent daily allowance
and unchanged launcher snapshot. Counts remain211/310 until native acceptance.
Windows full37174334529 remains live on f534f59c4; Forced March notice37175786029
is pending on e4946162f. Do not replace either handle on an observation timeout.

2026-10-04 UP192 Forced March source/native accepted and active. Standard
accepted exhaustion grants10% post-transition maximum Movement once daily;
typed day markers precede guard/object combat, and a generic side snapshot
applies-1 Morale only in playable round1. Accepted battle startup consumes
pending fatigue; replay keeps its original snapshot. Client and tests build;
active native91757 passes18/18 in5.867s, zero skips, data/inventory19/19 and
module check pass. Independent Astra production/fixture review finds no blocker.
Coverage210->211/310 perks,99 planned; Logistics6->7/10. Initial failures retained
with narrow corrections; no graphical/playable promotion. Prospective AI burst
forecasting and broader vehicle/guard/control/Morale matrices remain Phase2.
Next missing Logistics candidate: Pursuit March, a win-triggered daily refund,
not a replacement for this perk or a permanent Movement capacity bonus.

2026-10-04 next missing feature selected: UP192 Logistics Forced March. The
existing mastery is not the canonical perk. Runtime and test/AI maps are complete;
bounded hero/movement, battle snapshot and isolated-test owners now implement.
Absolute-day markers plus a generic first-round Morale snapshot avoid polling
and timed-stack-bonus lifecycle mistakes. Serialization version is append-only.
Implement the complete exhaustion burst plus first-round penalty, not a flat
capacity bonus or a button. No count increase before native/registration gates.

2026-10-04 protected-barrier map finds no authorable localized representation
or Fly/DD crossing consumer. Asked tile markers with straight-line DD crossing
versus region boundaries; blocked until marker/geometry is defined. No speculative
rock/guard/quest-gate classification or one-sided UI enforcement. Continue an
independent unblocked Version1.0 combat/perk gap; coverage explorer is read-only.

2026-10-04 UP056 DD ends-Movement warning hook accepted: generic NH-only text ID
and existing statusbar entry/hover/exit lifecycle, no new panel/art/gameplay rule.
Dedicated Adventure text map and generator/CMake parity pass; two focused
translation checks and manual UI wiring/module guards pass. Build1721 succeeds;
native38925 passes13/13 in3.979s, zero skips (UP056-dimension-door-hint-focused.log/XML).
Independent Luna UI/data review finds no blocker. Rendered text/input evidence,
manual-guard CMake wiring and pre-existing stale mastery version fixture remain
recorded, not counted as graphical acceptance. Protected barriers still block
full DD completion. Combat61/67, perks210/310 and ranks87/93 unchanged. No playable
promotion. Next scope: protected-barrier representation/enforcement mapping,
without inventing a map-author rule; Water Walk policy question remains open.

Current accepted UP056 DD subset: visible/legal rounded radius8, successful
full-Movement spend, shared live/UI targeting and planned AI source/cost.
Client retry55650 and combined retry22130 build; native43587 passes6/6 in2.086s,
zero skips (UP056-dimension-door-policy-focused.log/XML). Module/diff gates pass.
Independent Luna runtime/test review plus root integration finds no blocker;
separate Astra reviewer spawn was service-rejected at the thread limit.
Initial scope/header failures remain in NH_RELEASE_FAILURES.md. No full DD,
new identity/perk/rank count or playable promotion. Protected barriers and the
ends-Movement warning remain Phase1; next unblocked clause is that warning.
Water Walk's stranded-hero policy remains unanswered and blocked.
DD checkpoint committed/pushed ae32ac3c4; notice-only preflight37172296610
completed successfully. Hint checkpoint f534f59c4 notice37173593409 also succeeds;
full Windows37174334529 now runs on that exact committed source, excluding
the uncommitted Forced March slice. Neither notice is a compiled playable
package. Next bounded read-only UI map is a localized casting-ends-Movement
hint in existing native targeting/status surfaces. No panel/art or gameplay
change. Source/wiring/native gates and rendered acceptance remain distinct.

UP123 status foundation committed/pushed9d0b11405; no Pandemonium activation.
Next UP056 slice: read-only Water Walk end-day land-legality map across shared
pathing, authoritative movement/turn completion and AI, with a separate focused
test-seam map. An independent Dimension Door map isolates its explicit
range/visibility/movement clauses from unresolved barrier/threshold choices.
Do not infer drowning/forced relocation or other Adventure design
decisions. Summon Boat targeting is committed/pushed26efdd523.
Water Walk map is complete and blocked on stranded-hero policy: existing movement
can leave zero Movement on water; explicit EndTurn bypasses the last-move timer
hint, which also fails to aggregate multiple heroes. A simple turn-end rejection
could soft-lock or loop AI. Asked preventive unsafe-step rejection versus explicit
emergency return; no policy is implemented before the answer. Existing cost/expiry
tests do not prove the day-end rule. Dimension Door's independent map continues.
Dimension Door map complete: minimumMovement is already zero; implement the
unambiguous visible/legal radius8 and successful full-Movement expenditure
clauses through shared live/UI/AI policy. Radius uses the engine's existing
rounded DIST_2D convention, not a new metric. Runtime, AI and tests have bounded
ownership; preserve legacy config. Protected barriers and the canonical UI
casting-ends-Movement warning remain Phase 1 work and block full completion.
Accepted source/native UP056 slice: Summon Boat highlights legal adjacent water
destinations using shared spell legality and native map targeting visuals.
Bounded Luna owners implement shared effect/capability APIs, client targeting,
and isolated tests separately. Exact selected position is honored authoritatively;
only the production (-1,-1,-1) sentinel falls back to the first legal neighbor.
Use native range-mask brightness contrast, not new marker artwork or a forged
ranged-spell class. Preserve legacy and AI fallback; no global polling.
All candidate source is frozen; independent source review finds no blocker and
the narrow UI source-contract guard passes. Combined build7395 fails on a missing
callback include; root adds it and retry39815 builds both targets. Native49715
passes8/8 in2.563s, zero skips (UP056-summon-boat-targeting-focused.log/XML).
Selected/fallback placement, invalid/hidden target rejection, missing boats,
legacy and existing AI planning pass. Required targeting is source/native
verified; rendered/playable acceptance remains pending. Identity totals unchanged.
Do not resolve other Adventure design questions or count a new spell identity.
Focused source/native gates first; rendered/playable evidence remains separate.

UP191 is consolidated with existing UP123: full Pandemonium's repeated-application
count and perk-composition questions remain unanswered. The duplicate selection
is corrected, not counted as new coverage. The unblocked prerequisite is generic
Bonus statusTags/statusIdentity metadata with strict saved representation and
refresh semantics; runtime and isolated fixture have separate Luna owners,
Astra reviews. No count consumer, implicit producer classification or spell/perk
activation is authorized by this foundation. Combat coverage61/67 unchanged.
UP123 foundation client14349 builds successfully. Independent source review
reports no blocker. Corrected combined build24367 passes; focused native gate
passes14/14 in0.917s, zero skips (UP123-status-tags-focused.log/XML), including
four new metadata cases and ten adjacent transfer/control serialization cases.
Original90794 fails on a final GTest fixture; the qualifier is removed, with
both failed and retry logs preserved. No producer or count consumer is activated.
Special marker replacement metadata and
additional wire/refresh/copy edge tests are deferred, not spell acceptance.
UP190 is committed/pushed620b25eec. Its notice preflight37167546781 succeeds;
older full Windows37164498532 succeeds on13d4691f5. Full37168548146 now succeeds
on620b25eec; it excludes the later status foundation and Summon Boat targeting.
Notice-only preflight37169597939 succeeds on9d0b11405. It is not a compiled
package and does not establish acceptance of26efdd523 or the current DD slice.

2026-10-03 UP190 Puppet Master/Lucidity is source/native verified.
Separate action controller from allegiance; preserve physical-side unit packets,
ordinary Morale and reaction relationships. Runtime, client/AI and isolated
native fixtures have bounded Luna owners. Root integrates data/build/review.
Registration/perk/inventory checks pass22/22; module metadata matches. Final
client90585/test72097 builds exit0. Native97155 passes8/8 in2.290s, zero skips;
adjacent Berserk guard71741 passes6/6 in1.986s, zero skips. Combat identities
increase60->61/67, Chaos6->7/11; perks210/310 and ranks87/93 unchanged.
The user subsequently answered the pre-existing Berserk question: successful
Puppet Master removes that spell effect. Canonical rules are updated; the
narrow correction is implemented and verified in the final cases above.
No GUI or playable promotion. Dedicated Time Stop, multi-control/status/reaction
matrices, move-only AI valuation and unused canCastWithoutSkip continuation
cleanup remain Phase2. Full Reality Warp still awaits its beneficiary-side
decision; do not count its accepted prerequisites as the completed spell.
New Hypnotize13d4691f5 notice37163408746 succeeds; full Windows37164498532 is
running on that committed prerequisite, not the dirty Puppet Master slice.

2026-10-03 UP179 Hypnotize ceiling prerequisite accepted: client retry26745
and final focused test build39697 exit0; native5489 passes22/22 in5.958s,
zero skips (UP179-hypnotize-refresh-final.log/XML). Exact cast-time integer
metadata and real duration-only refresh are verified without changing targeting
or action rules. Independent review has no blocker; data/inventory19/19 pass.
Combat spells60/67, perks210/310 and ranks87/93 remain unchanged. Full Reality
Warp is not implemented or promoted. Next live collection/authoritative exchange,
paired UI and AI; beneficiary-side question remains pending. Phase2 retains
detached refresh parity, original-side Hypnotize targeting interactions and
metadata validation by eventual binary-loaded transfer consumers. Prior failed
builds/fixtures are retained in NH_RELEASE_FAILURES.md.

UP179 prerequisites accepted source/native: client8019/test retry45423 exit0;
principal47075 passes9/9 from2 suites in1.201s, zero skips. Log/XML retained.
Binary SHA670d04c6d3c8d4241512402128876163f777510723cfb1bc2a7a97fc0ccfe715.
Reciprocal bundles, independent timers, all three sidecars, exclusions/legality,
detached snapshots, original-owner hostility, current/previous wire, lossy-write
rejection, JSON validation and actual hostile/friendly cast stamping pass.
Independent source review has no blocker; data/inventory19/19, module check
and diffcheck pass. Combat spells60/67 and perks210/310 remain unchanged.
No full Warp acceptance or playable promotion. Next live discovery/authority,
paired UI and AI; resolve pending beneficiary-side clarification before deciding
Focus Magic/Arcane Breach cross-side behavior. Retain prior failures below.

UP179 test retry15193 terminates143 before link after179/320, with no compiler
error in its log. Root confirms no remaining cmake/ninja/compiler processes
before resuming; termination cause is unestablished. Preserve retry log and
reuse objects in retry2, not a second concurrent build or stale test binary.
Previous full Windows37155153392 is now completed success (46b9421b7); matching
Pact notice37157406583 succeeded. Neither proves the uncommitted UP179 slice.

UP179 test94692 exits1: new pure Bonus serialization fixture needs complete
parameter/limiter/propagator/updater headers. Tester corrects owned includes;
root will retry with retained compiled objects and a distinct build log. Client
remains accepted, but native prerequisite acceptance has not run. Failure log
is retained; no production weakening, stale test binary or coverage increase.

UP179 tester freezes six planner/wire cases and three strengthened existing
Steadfast cast/provenance cases. Root test build94692 is live with twelve jobs,
log UP179-prerequisite-test-build.log; production remains frozen. Independent
Astra review finds no blocking source issue. Reflected casts, special refresh
versus duration refresh and eventual live exchange remain Phase2 interaction
checks, not substitutes for completing the spell. Data/inventory19/19 and
generated module check pass. After build run only the named nine-case filter
on the fresh binary and retain log/XML. No accepted spell count increase.

UP179 client8019 exits0. Root source review catches test-only invented BonusType
names and a direct member-variable lambda capture before compiling the fixture;
tester corrects both without changing product behavior. Next fresh vcmitest
build and smallest planner/provenance/real-cast filter; no full spell coverage
or playable promotion follows from this client build.

UP179 prerequisite production sources frozen; root client build8019 is live
with twelve jobs, log UP179-prerequisite-client-build.log. Test author owns
only the new pure planner/wire fixtures and two existing real-cast provenance
assertions. Runtime stamp is source- and actual/base-spell-ID guarded so Warp
cannot attribute transported effects to itself. Planner carries Guardian,
Regeneration and Hydra fractional-regeneration progress; actual creature HP and
capacity baseline remain with their own stack. Independent source review is
running. Do not edit production during this build or claim spell acceptance.

Next slice UP179 Reality Warp: three independent bounded lanes now own
caster-provenance representation, pure reciprocal bundle planning, and actual
recipient/sidecar legality inventory. Root chose original caster ownership,
not target-relative historical hostility or the Warp caster, as the provenance
needed when a magical effect moves across owners. Existing legacy hostility
remains unchanged until transfer; unknown old provenance is not guessed.
Time Stop/Spell Lock endpoints remain illegal under their canonical immunity.
Full spell coverage requires live discovery/application, data, paired UI/AI and
focused native acceptance; prerequisites do not increase the60/67 spell count.
Previous goal cycle is progress: Pact d520113ff pushed,27/27 focused tests pass.

Pact test retry95539 exits0; principal retry85631 passes27/27 from3 suites
in6.764s, zero skips. Original failures remain retained. Accepted coverage
209->210/310,100 planned; Diplomacy6->7/10, ranks87/93 unchanged. Independent
production and fixture review has no blocker. Data/inventory19/19, module
check and diffcheck pass. No rendered acceptance or playable promotion.
Deferred: manual Swap/Bulk intake, subsequent troop return, weekly-perk
interactions and restored modal context. Next missing unambiguous slice is
Reality Warp; remaining Diplomacy perks await recorded design decisions.

Pact test retry87524 exits0. Fresh principal execution11141 runs27 tests:
23 pass, four new encounter fixtures throw the preceding-perk-tier advancement
exception during setup. Original principal log/XML retained. Tester corrects
normal progression by selecting Basic Envoy before Advanced Recruitment Pact;
no assertion weakening or production change. Coverage remains209/310 pending
corrected execution. The user's Tribute quota decision is reconfirmed and its
existing native case passes. Reality Warp read-only mapping completes without
a design ambiguity; bundle/provenance and sidecar architecture precedes source.

Test54732 exits1 on a test-only incomplete StackLocation type in the newly added
accepted-offer fixture. Tester owns the missing defining include and new-warning
brace correction; production/client acceptance remains unchanged. Original log
UP129-pact-test-build.log retained. Retry/native acceptance pending; no coverage
increase and no stale binary run.

Discount-qualified acceptance fixture is frozen, including actual Gold debit,
positive partial admission, closure and rearm on inclusive expiry day. Root
test build54732 is live with twelve jobs; log UP129-pact-test-build.log. Next
run NewHorizonsDiplomacy* on that fresh binary and retain principal log/XML.
Do not edit frozen sources, run the stale binary or restart a live build for an
observation timeout. A Windows status request for37155153392 receives HTTP504;
this is not a terminal job result or authority to restart its build.

Pact client66210 exits0 (UP129-pact-client-build.log): production state, encounter,
admission hook, shared prediction and client compile. Native acceptance pending;
test target waits only for the bounded discounted-acceptance fixture freeze.
No production edits or playable promotion follow from client compile alone.

Independent Astra review reuse now succeeds after execution lanes finish. No
blocking production finding; deferred manual Swap/Bulk admission, subsequent
troop return, Pact with weekly perks and restored modal context remain Phase2.
Tester frozen source initially covers discount-qualified refusal but not actual
discount-qualified acceptance. Root requests one principal acceptance/rearm
fixture, while client-only compilation continues; this is not a broad matrix.

Pact production lanes are frozen after root source review and clean diffcheck.
Client compilation starts with twelve jobs, log UP129-pact-client-build.log;
tester may finish only its isolated test file before the test-target build.
Data/inventory19/19 and generated-module check pass; these are not native Pact
acceptance. A second independent Astra reviewer spawn also hits the service
thread limit. No review success is claimed; retry after tester completion.

Recruitment Pact integration adds server-only accepted-visit context recording
positive neutral-to-hero troop admission from authoritative Rebalance/Bulk/Swap
packets. At visit completion, before deleting the source, the encounter callback
arms the next Pact only when actual intake occurred. Manual transfer closure is
included; accepting and dismissing everything without intake grants nothing.
Root owns CGameHandler.cpp and VisitQueries.cpp/.h. No ongoing-dialog save support
is inferred. Reviewer follow-up initially fails with the service thread limit;
retry after an execution lane finishes, rather than inventing a lower capacity.

2026-10-03 continuation: preceding cycle made concrete progress (weekly perks
committed/pushed46b9421b7, client/test build and21/21 native acceptance). Windows
37155153392 is confirmed in progress on that source, not restarted. Recruitment
Pact is now released with bounded ownership: saved hero/snapshot/version lane,
neutral encounter/shared threshold lane, and isolated focused-test lane. Root
owns registration, integration, builds and Git. Arm after successful neutral
recruitment; use the next neutral contact within seven elapsed game days,
including day trigger+7. Contact resolution retains its discount through the
blocking joining offer, consumes on that response including refusal, or consumes
immediately when no joining offer exists. A successful contact rearms a new Pact.
No per-frame scans or permanent monster discount flags. Accepted209/310 remains
unchanged pending principal execution. Mercenary cohort question remains open.

Next Diplomacy mapping is complete (read-only Luna workers). Recruitment Pact
must preserve the contacted offer's discount through its modal response; consume
on the first contact even if unwilling, not only on a subsequent successful hire.
Root will choose a query-scoped entitlement or atomic modal-resolution approach
before releasing implementation. Legendary Reputation needs an explicit ruling
on already-authored free joins. Mercenary Captain/Loyal Mercenaries require
troop recruitment provenance through split/merge/transfer, not a stack-wide bool.
Design review needed: mixed ordinary/recruited cohorts, casualty attribution and
which completed combats count toward the first-three-combats benefit. Do not
invent exact cohort ownership or activate these four perks from mapping alone.

2026-10-03 weekly Diplomacy accepted: client10506 and test68471 exit0 with
twelve build jobs. UP129-weekly-principal.log/XML establishes21/21 across three
suites, zero failures/skips,5.119s. Test binary SHA256:
cdbbb7cf064f63d3047d441cd6f3bccd00b26c043e67379d027c56eedf841ef0.
Peacemaker protection, expiry, deliberate attack, precedence over Tribute,
full-price Tribute removal, insufficient-Gold quota preservation, ordinary
willing offers and versioned state validation pass. Independent Astra review
has no blocking finding. Accepted perks207->209/310;101 planned;Diplomacy6/10.
Ranks87/93 unchanged. Four missing perks: Mercenary Captain, Loyal Mercenaries,
Recruitment Pact and Legendary Reputation. This is source/native acceptance,
not rendered or playable delivery; no local snapshot promotion. Deferred
guard/cursor/query and live AI integration findings remain recorded below.

2026-10-03 continuation classifies the preceding turn as concrete progress:
Envoy6ef610550 is pushed and weekly production/client compile completed. Test
build68471 remains confirmed live; no restart for an observation timeout.
Fresh Astra reviewer allocation succeeds this continuation. Independent weekly
review finds no blocking defect; the tentative teleport lifetime concern is
withdrawn after tracing the early blockingVisit return. Phase2 findings:
Dimension Door cursor still uses hero-independent guard appearance; subsequent
protected movement, another hero's actual encounter, overlaps and live client/
NK2 path recalculation lack focused integration coverage. Root retains those
findings without broadening every feature into a full certification exercise.
Two Luna workers read-only plan Recruitment Pact/Legendary Reputation and
Mercenary Captain/Loyal Mercenaries. No new production edits during build.

Envoy checkpoint committed/pushed6ef610550. Matching notice37152417973 is live;
full Windows37150731428 remains live on foundationfad71a2fc. No local playable
promotion. Weekly implementation released with nonoverlapping ownership: Runtime
owns three saved hero fields and the atomic typed state packet/version; movement
worker owns CGCreature, hero-aware guardian callback and pathfinding call sites;
root owns the client packet event invalidating human and NK2 path caches. Existing
NewTurn invalidation handles logical week expiry, without global polling or
bonus/stat scans. Tester plans focused actual passage/payment/wire fixtures.
Peacemaker and Tribute remain planned pending source/build/native acceptance.
Matching notice37152417973 subsequently succeeds on6ef610550. Weekly state and
wire fixture sources are frozen; movement/encounter implementation remains live.
Root review moves hero unsupported-write rejection ahead of payload bytes and
repairs a fixture that attempted to write a new packet in an unsupported format:
old-reader reset uses a documented synthetic heroId prefix, while the actual
old packet writer remains rejected. No weekly native acceptance yet.
Root review further requires cached no-guardian fast paths, visitable-coordinate
comparisons, and captured IDs before a visit callback can remove its guardian.
Actual movement Tribute is a required focused fixture. Registry/module and
inventory now activate Peacemaker/Tribute solely for verification; accepted
coverage remains207/310, not209. Future-day path prediction across week expiry,
overlapping/scripted guard combinations, full AI valuation and rendered feedback
are Phase2 unless focused execution exposes a foundational blocker.
Weekly production is frozen; root client build10506 is confirmed live with
twelve jobs, log UP129-weekly-client-build.log. Do not edit production or restart
the build merely for observation timeout. Tester may finish its isolated fixture
file while the client-only target compiles, then freeze before vcmitest build.
Movement suppresses a same-guardian destination revisit if the callback pacifies
or removes the stack. No removed object is read after the callback. Accepted
coverage remains207/310 pending client/test/native outcomes; no weekly commit or
playable promotion yet.
Client10506 subsequently exits0: frozen weekly state, encounter, pathfinding,
AI call sites and client cache event compile. Native weekly acceptance is still
pending; tester completes isolated fixtures, then root rebuilds vcmitest. No
production changes are needed to accommodate test setup or private-method calls.
Tester subsequently freezes six new focused cases: real movement Peacemaker
with funded Tribute precedence, hero-bound protection/week expiry, deliberate
attack, successful movement Tribute, unaffordable combat fallback, ordinary
willing offer, and versioned state (five encounter cases plus one wire case).
Root test build68471 is confirmed live with twelve jobs; preserve the handle/log
UP129-weekly-test-build.log. Next run NewHorizonsDiplomacy* against the fresh
binary, retaining log/XML; do not accept209/310 from registry status alone.
Data/inventory19/19 and diffcheck pass. No production or fixture edits during
this test build. Full Windows37150731428 remains live onfad71a2fc.

Envoy accepted: client69085/test68817 exit0; final principal retry2 passes15/15
in3.282s, zero skips. Binary024782815a9de49a138ebad07e2c7de5cead3f8a54ab4df629b176a94f2a2831.
Data/inventory19/19, module--check and diffcheck pass. Accepted207/310 perks,
103 planned, Diplomacy4/10; ranks87/93 unchanged. Prior independent production
review and root final fixture review establish this checkpoint; a fresh review
could not be allocated. Dedicated art/rendered UI remain unaccepted. Next saved
weekly state and actual movement/pathfinding for Peacemaker, then paid Tribute.

2026-10-03 resumed Envoy verification: retry2776 passes14/15, with hidden-target
setup still revealing its neutral. Hero sight uses library settings rather than
the attempted map override. Tester replaces the override with an authoritative
sight penalty and fog-hide packet, retaining actual hidden-before-query checks.
Focused rebuild68817 is live; no production edits during build. A fresh reviewer
spawn and reuse attempt both hit the service thread limit; prior production
review remains evidence, root rechecks the fixture diff, and no additional
independent review is claimed. Peacemaker/Tribute planning remains read-only.

2026-10-03 continuation: fad71a2fc pushed, clean at start. Matching Windows
notices37150248875 succeeds; prior full37146835406 remains live onaeddb6900.
Runtime narrowly maps saved weekly usage and real pass-through guard semantics
for Peacemaker/Tribute. Independent Envoy implementation owns neutral tooltip
files; tester owns focused fixtures. No additional activation/coverage yet.
Full Windows37146835406 succeeds onaeddb6900. Matching notices37150248875
succeeds forfad71a2fc; full Windows37150731428 is now confirmed live on that
accepted Diplomacy-foundation source. Do not cancel/restart a live job for an
observation timeout. Envoy is registered active for focused verification only;
accepted206/310 remains unchanged until native range/visibility acceptance.
User resolves weekly mechanics: pacification lasts through the current week,
Peacemaker resolves before Tribute, and Tribute consumes only after payment.
Canonical Diplomacy updated; SHA58a3cd1c20a1b47641ff65866b4e4f3cf9ddc3d5767ed742126b9e0442f2290f
is synchronized to registry/module/matrix. Envoy client69085 passes; frozen
fixtures include true hidden-target denial with reduced fixture scouting, then
explicit reveal. Focused test build is running; no weekly production edits until
this Envoy checkpoint is verified and committed.
Envoy test68880 passes. First principal61370 passes10/15 in3.239s; new cases
fail before exercising Envoy due to artwork-anchor/visitable-offset positioning
and a Basic-perk argument supplied as Advanced. Tester owns focused fixture
repairs; original log/XML retained. Production range and selection gates remain
unchanged; accepted count remains206/310.

2026-10-03 UP129 foundation accepted: final client67358/test39859 exit0;
principal retry10/10 passes1.870s, zero skips. Three ranks and Negotiator/Common
Cause/Grand Diplomat use shared deterministic forecasts, normal Gold/count,
authored-free exceptions, explicit saved eligibility and minimum AI admission.
Actual query/payment/transfer dismissal and current/old wire pass. Binary:
94754dc4103f089d4097f2eb032903dbfe9eb9b257a4ab670379487d8077af5e.
Accepted perks206/310,104 planned; ranks87/93,6 planned; Diplomacy3/10;
faction62/90 unchanged. Adjacent7/8 passes2.440s; same-hero exact-fit merge
rejection reproduces in isolation and is an unresolved Phase2 finding, not an
assertion to weaken. Deferred restored/stale queries, full AI/valuation and
rendered/localized feedback; dedicated perk art missing. No playable promotion.
Next Peacemaker within the still-open seven-perk Diplomacy continuation.

2026-10-03 UP129 starts on committed/pushedaeddb6900. Reuse the completed
Diplomacy map and resolved authored-free/surplus-dismissal choices. Runtime
implements the shared captured-profile deterministic forecast and author
eligibility flag; AI consumes exact count/price components with Gold/usable
admission checks; focused fixtures exercise real offers/payment/transfer.
Root registers helper/test CMake entries and owns activation/build/Git.
Ranks and Negotiator/Common Cause/Grand Diplomat are registered active for
focused verification; accepted coverage stays203/310 until native acceptance.
Other Diplomacy perks are separate.
Matching notices37146642103 passes onaeddb6900; full37146835406 is live on
that same source, following completed successful full37142169494.
Initial client95849 exits1: AIGateway dynamic_cast used CGCreature without its
defining include. LogUP129-client-build.log retains the failure. Root adds the
explicit include and repairs refusal-response recomputation to disable joining
after a declined offer; focused refusal regression requested from the tester.
Client retry88847 exits1: HeroPtr's dereference operator returns a pointer,
where the shared forecast requires a reference. Root uses *heroPtr.get(); log
UP129-client-build-retry.log retains the failure. Retry2 is separately logged.
Client retry2 handle11816 exits0. Independent frozen production/fixture review
reports no blocker; vcmitest rebuild is now running with twelve jobs. Data and
inventory gates pass19/19, module--check and diffcheck pass. No native acceptance
or playable promotion yet; accepted coverage remains203/310.
Test15477 exits1 on fixture translator/JSON constructor/binary type-definition
errors; tester owns the narrow repairs. LogUP129-test-build.log is retained.
Production client success is unchanged; focused native acceptance is pending.
Tester repairs concrete translator/bonus/template includes, qualifies the object
JSON overload, and supplies the supported optional resolver argument; current/
old binary and JSON assertions remain intact. Test retry66042 is separately
logged in UP129-test-build-retry.log. No production edits during the retry.
Test retry66042 exits0. Before execution, reviewer catches a fixture-only
populated-object JSON load; tester must use a fresh empty CGCreature and retain
the original neutral for binary assertions. One-file rebuild follows the fix.
Test retry2 handle77176 exits0. First principal56667 passes5/10 in1.766s;
original log/XML retained. Tester used the core Diplomacy ID instead of the
decoded NH skill; separately, runtime excluded real map monsters because their
owner is UNFLAGGABLE, not NEUTRAL. Corrected decoded-ID fixture and production
unowned-owner filter; actual map owner and player-owned exclusion are asserted.
Independent review approves the bounded correction. Client67358 exits0; test
retry3 is separately logged. Accepted coverage remains203/310 pending rerun.

2026-10-03 UP189 accepted source/native: Lord of the Dead captures original
living-Champion presence, consumes12 residual/Elite/Core equivalents before
other conversions, and delivers one exact Bone Dragon via atomic Hero/Ossuary
admission. Both targets build94998/27283. Principal40/40 passes9.199s,
adjacent12/12 passes2.615s, zero skips; normal Expert selection/no override,
actual armies and current/older wire are verified. Binary SHA256:
690acea167f885c0dae1d4111d28705b43e32de4c4e8be577f2f76e1264459cb.
Data/inventory19/19, module/UI guard and independent reviews pass.
Coverage203/310 accepted,107 planned; Necromancy10/10; faction62/90,28 planned.
Broader Champion/form/AI interactions and rendered feedback remain Phase2;
dedicated art is missing. No playable promotion. Next UP129 Diplomacy.
Full Windows37142169494 succeeds onb384196c1; next release candidate will
include8822239c4 and this checkpoint after matching notices.

2026-10-03 UP189 source implementation is frozen on8822239c4: original living
Champion roster capture,12-equivalent residual/Elite/Core depletion before
Dark/Soul, exact Bone Dragon fourth output, atomic Hero/Ossuary admission and
packet-driven feedback. Registry active for focused acceptance only; accepted
coverage stays202/310 and Necromancy9/10. Root client94998 runs12 jobs,
logUP189-client-build.log; native fixtures and Astra review remain in progress.
Data/inventory19/19 and UI source guard pass. No playable promotion.
Client94998 exits0. Independent production and fixture reviews report no
blocker; test27283 is live with12 jobs, logUP189-test-build.log. Production
and fixtures remain frozen through compile/native acceptance. Matching Windows
notices37144633554 succeeds for8822239c4; older full37142169494 remains live.

2026-10-03 UP188 accepted source/native: whole-batch Ossuary town delivery,
Hero Leadership/slot overflow, foreign-town exclusion and atomic nearest-town
failure. Client retry67941 and test retry79662 exit0; principal37/37 passes
8.395s, adjacent12/12 passes2.626s, zero skips. Actual winning-Hero Mana,
normal Advanced selection/no override and guarded destination wire pass.
Binaryca960a648600671a8ede1a8f918409d8de80fd323784169acb8c84ef68d53d8c.
Data/inventory19/19, module/UI guard and independent Astra review pass.
Coverage202/310 active,108 planned; Necromancy9/10; faction61/90,29 planned.
Deferred visiting/garrison Hero variants, rendered popup and broader saved/
concurrent battle/full AI interactions; dedicated art remains missing.
No playable promotion. Next UP189 Lord of the Dead is design-resolved.

2026-10-03 UP188 starts from committed/pushedb384196c1: Ossuary's whole-batch
Hero-capacity fallback to the nearest owned Necropolis, normal upper army,
no partial mutation or farther-town search. Three bounded Luna lanes own
runtime/UI/focused fixtures; root owns version, guards, registration, builds/Git.
No new coverage accepted yet (201/310, Necromancy8/10). UP189's Bone Dragon
species is resolved but category depletion for its first12-Skeleton conversion
is now asked explicitly; do not double-spend Core/Elite contributions. Windows
notices37142047603 passes onb384196c1 and full37142169494 is live on that source.
User subsequently resolves UP189 depletion as Champion/unclassified, then Elite,
then Core. Diplomacy's existing-map questions are also resolved: authored free
joins remain exceptions, accepted-transfer surplus is permanently dismissed on
closure. These canonical decisions unblock future source work, not active ranks
or additional coverage. Keep the source hash/module synchronized.

2026-10-03 UP187 accepted: Death Lord and Grave Knowledge extend captured
casualty eligibility at their specified independent rates, feed category-based
automatic conversions and preserve atomic outputs. Root client13126 and
test86643 pass; test-only retry17335 repairs the faster Vampire's legal action
window without changing production. Final principal32/32 passes6.716s and
adjacent12/12 passes2.607s, zero skips; original11/12 failure is retained.
Production-active/no override, ordinary rank/perk selection, actual army counts,
actual spell provenance and guarded current/older wire cases are verified.
Binary212ea29fb37c2f95a844e452174c6b5db40da917d08d432abf4b57cacd77d07c.
Data/inventory19/19, generated module/UI guard and Astra review pass.
Coverage201/310 active,109 planned; Necromancy8/10; faction60/90,30 planned.
Deferred: broad interactions, full AI play, rendered acceptance and dedicated
art. No playable promotion. Next UP188 Ossuary; UP189 output species awaits
user choice. Full Windows37136224312 succeeds on older e8f2cb4b5.
Subsequent user choice resolves UP189: Bone Dragon is the output. Canonical
row/registry identity are updated; paired UP188/189 implementation is next.

2026-10-03 UP187 implementation: Death Lord/Grave Knowledge runtime, separate
provenance-filtered capture, packet-driven result text and guarded appended wire
fields are frozen. Registry is active for native acceptance, not yet counted as
completed coverage. Data/inventory19/19, module generation and UI guard pass;
independent Astra source review reports no blocker. Root client build13126 runs
12 jobs, logUP187-client-build.log; focused native fixtures remain independent.
Full Windows37136224312 is confirmed live on preceding e8f2cb4b5; preserve it.
No local playable promotion or rendered acceptance is claimed. Next read-only
preparation is Ossuary's owned-town fallback, without displacing this acceptance.
UP188 scope resolved by user: both Leadership limits and unavailable army slots
trigger fallback. Canonical source/hash and registry text are updated, still
planned. Root interpretation uses normal visible town upper-army and atomic
single-nearest fallback. UP189 Lord of the Dead map finds no explicit output
species binding; asked Bone Dragon vs Ghost Dragon. Neither item is activated.

2026-10-03 UP185 accepted: Master of Bones upgrades remaining Skeleton output
only with a currently owned, built appropriate Necropolis upgrade. Configured
upgrade/actual roster checks, atomic form-aware admission and explicit packet/UI
identity exist; base-equivalent conversion labels are retained. Client57879's
concrete/interface mismatch was repaired; retry43912 and test65198 pass. Luna
tester principal26/26 passes5.386s, adjacent9/9 passes1.707s, zero skips.
Production active/no override and ordinary BasicCP->AdvancedSoul->ExpertMaster
selection are recorded for the four town-availability cases. Binary SHA-256:
b5612702c235e3d66403429999fe6838558e13635680337d701ace6e3ba276c9.
Data/inventory19/19, module/result guard and independent Astra review pass.
Coverage199/310 active,111 planned; Necromancy6/10; faction58/90,32 planned.
Deferred: actual construction/capture roster refresh, broader interactions,
full-AI/rendered acceptance and dedicated art. No playable promotion. Next is
the prepared weighted-casualty slice below. Full Windows37136224312 targets
e8f2cb4b5, not this source; notices37137524285 succeeds on12431082e.

2026-10-03 next-slice read-only preparation (after UP185): Death Lord and Grave
Knowledge need separate weighted casualty inputs, not normal-rate additions to
the living Core/Elite counts. The current eligibility snapshot drops Undead and
NON_LIVING species even when usable remains exist; extend provenance-filtered
capture, never grant these pools from the unfiltered legacy casualty fallback.
Original-form accounting, Corpse Preservation's magical-casualty gate and
Disintegrate/unusable-remain exclusions remain authoritative. Current original
Golems/Elementals use NON_LIVING; MECHANICAL is separate. Grave Knowledge's 20%
is a fixed conversion rate; Death Lord is one quarter of the normal rate.
For nonnegative values floor(floor(x)/4) equals floor(x/4), so that algebra is
not a design blocker. Tier contributions must fund Dark/Soul conversions at
their own rate, while remainders stay Skeletons. A versioned special-capture
marker is required to distinguish new filtered pools from old snapshots.
This is mapping, not implementation/activation; no coverage increment.

2026-10-03 UP184 accepted: Soul Harvester raises the explicitly named Core Wight
from complete groups of six Skeletons attributable to eligible Elite casualties.
Independent Core Zombie conversion and global remainders are retained. Atomic
three-output authority and explicit UI/wire counts exist for human/computer
winners without conversion queries. Client95124 and test retry15042 pass;
initial53850's fixture-only `final` failure is recorded, not concealed.
Luna tester principal20/20 passes4.193s, adjacent9/9 passes1.718s, zero skips;
production active/no-override properties present in all five battle cases.
Binary cf6fe68c13be8424f92e519508ddca19e1d6bb5d9f31f072b11fd553e6bc63f8.
Data/inventory19/19, generated module, result guard and Astra review pass.
Coverage198/310 active,112 planned; Necromancy5/10; faction57/90,33 planned.
Deferred: combined fractional carry, broader interactions, full-AI/rendered
acceptance and missing perk artwork. No playable promotion. Next UP185 Master
of Bones; existing full Windows37136224312 targets preceding e8f2cb4b5.

2026-10-03 UP186 verified: Dark Conversion now automatically converts complete
Core-derived groups only, retains global base rounding and all remainder
Skeletons, and admits every output atomically. Human/computer winners share the
same authority path without a conversion query. Client35092/resumed9620 pass;
interrupted70772 is retained. Initial11/12 and retry11/12 were caused by missing
simulated-controller readiness; only fixture setup was repaired. Ready71025
passes. Principal12/12 passes2.383s, adjacent9/9 passes1.778s, zero skips.
Data/inventory19/19, module consistency, UI result guard and independent review
pass. Tester remained pending initialization after transition; root explicitly
cancelled it and executed the focused gates. Final binary SHA-256:
70900e308674b933b1ba3835d5a78085aad55bbc5af83e85fd7f785086c9b5ae.
Registry197/310 active,113 planned unchanged; repaired faithful coverage rather
than a new activation. Broader interactions/full-AI play/rendered acceptance
remain Phase2; no playable promotion. Next UP184 Soul Harvester: approved Wight
output from Elite casualty contribution, with Wight still Core-tier. UP185
Master of Bones is mapped but not implemented. Windows37127577580 succeeds on
previous756d225818; no UP186 Windows package yet.

2026-10-03 UP186 in progress: Soul Harvester's map exposed a prerequisite gap.
Dark Conversion is registered active but still optional/all-tier at runtime;
correct it to the canonical automatic Core-only conversion. Preserve global
base Skeleton rounding; floor the Core contribution only for complete
three-Skeleton conversion groups. One worker owns shared resolver/authority;
another owns focused existing fixtures. Root owns result wording, serialized
builds, integration and Git. No coverage increase or native acceptance yet.
Soul Harvester's output is resolved by the user: retain Wight, still Core-tier;
only its input is Elite casualties. Canonical and registry descriptions agree.
Master of Bones is mapped for next coverage work: currently owned built upgrade
availability plus explicit result output form; it is not implemented.
Previous UP183 source is756d22581875f34ada21409a78232d050beeed63, pushed clean.
Notices37127483096 succeed on that revision; Windows37127577580 remains live
on the same source and must not be replaced by a competing full run.
Latest delivery checkpoint: Windows37127577580 now succeeds on756d225818,
including Corpse Preservation but not the current UP186 correction. Native
build70772 was interrupted during the environment transition; no process
survived and its log ends77/257. Resume9620 uses the same incremental build root,
logUP186-resumed-build.log. Do not execute the earlier test binary.

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
