# New Horizons provisional rule review

## Four-perk batch — principal native validation passed

Magnate records the most recent owned-at-entry town visit in the previous
absolute week. At week start it snapshots a seven-day town award; losing the
town pauses payment, and same-owner reacquisition resumes the original clock.
Losing the granting hero does not cancel the town award. No fallback is invented
when the most recently visited town has been lost. Amounts aggregate before the
ordinary income handicap. Review unusual calendar lengths and the current-vs-
next-day income tooltip boundary in Phase2.

Academic Study consumes each hero's first town arrival even before perk
acquisition or before a Guild exists; later construction cannot create a repeat
reward. Ownership is not an authored restriction. The hero-only visitor marker
precedes XP and does not alter player/team or building-visit history. Mentor's
existing meeting snapshot is retained. Review composed level-up/building/Scholar
queries in Phase2.

Elemental Memory captures the destroyed stack's positive net ordinary Morale and
Luck independently, then adds only the missing contribution after newborn
positive inheritance. Newborn-specific negative effects and elemental Morale
immunity remain effective. Ordinary one-round bonus expiry and Time Stop duration
handling are retained; detached copies eagerly snapshot their own receipt.
Review uncommon aura/controller and paused-duration interactions in Phase2.

Veteran Cohesion uses battle-start maximum aggregate HP and a strict below-half
threshold after actual HP loss. Its once-combat personal receipt survives healing
and restoration; ordinary immunity and caps still govern its +2 Morale. Time Stop
or fully absorbed damage cannot earn it. Review temporary HP, polymorph and
controller transitions in Phase2. Sources are the shared Discipline/unit-state
and Rebirth paths, town/hero visitor helpers, NewTurnProcessor and existing
netpack serialization. These four implementations are source-reviewed, not yet
accepted at native85299:36/36 principal cases pass after linked90928, zero
failures/errors/disabled/skips. Shared68621 passes33/33 on the same pair.
These interpretations remain reviewable; broader interactions above are Phase2.

## Prepared private candidates — not accepted implementation coverage

Royal Standard: capture only the original recipients of an actually selected
Divine Mandate Order follow-up. Its negative-Morale floor lasts through that
Order's scheduled round expiry, even when a Charge is spent, Protect is broken
or Second Wind's activation finishes. Current hostile control suspends the
floor; friendly control restores it within the original lifetime. This differs
from Commanding Presence's explicitly settled benefit-consumption lifetime.
Review Second Wind and future Divine Discipline extensions in Phase2. The
shared morale callback and captured Order recipients implement the private
candidate; eight cases are authored and source review is clear, not executed.

Deep Flank: interpret 'currently attacked from at least two distinct melee
sides' as present friendly melee-capable contact geometry, not historical hit
counts. Union the existing directional footprint masks; repeated contacts on
one direction do not add sides, while a double-wide footprint can contact two
distinct sides. Apply half the rank's base Shroud flanking damage bonus only
to the qualifying physical ranged attack, with fractional precision preserved;
do not halve unrelated Backstab or Ambusher bonuses. Existing Formation Fighting
protection remains. Shared damage/callback and Lua context implement the private
candidate. Eight cases are authored and source review is clear, not executed.
Review incapacitated contacts, walls/terrain and wider double-wide geometry in
Phase2; this is not a completed AI-choice or rendered acceptance claim.

Historian: classify the shipped Chest XP choice and Tree's XP reward explicitly.
Preserve Tree's existing whole next-level threshold delta, not remaining XP to
the next level. Only New Horizons level-derived rewards gain the ordinary
Learning calculation and Historian's additive50%; legacy Tree grants/previews
and AI remain unchanged. Grant, preview and AI share the same gate. Saved
unclassified rewards are not silently migrated. Seven cases are authored and
repaired v2 source review is clear; actual native gates remain pending. Review
unusual mixed reward components and saved classification migration in Phase2.


## Swift Rebirth — normal birth-round activation

Advance the reborn stack's one normal activation after the acting stack's
current activation, preserving any already-earned immediate Morale first.
Simultaneous spawn IDs order ascending. WAIT delays the same normal activation;
it does not create a second one. Birth-round extra activations are excluded,
while genuine continuations remain legal. Frozen/Time Stop forfeiture spends
the normal slot. Later rounds return to ordinary scheduling. Reasoning: the
authored immediate turn is normal initiative promotion, not an extra-action
generator. Shared callback/Swift lifecycle, server flow and detached AI consume
the same typed receipt. Ten principal native cases pass after linked82853, including
incapacitation during an accepted action and nested detached replacement.
Review lazy child materialization before first access and approximate projected
mid-exchange rebirth valuation in Phase2; do not claim exhaustive AI forecasting.

## Prospector — eligible resources and capture timing

The first visit to a mine already owned by this hero's player grants Wood/Ore+2
or one of Mercury/Sulfur/Crystal/Gems+1. Gold is neither common nor rare and
does not pay or consume the weekly use. Capturing a mine is not an owned-at-entry
visit; Land Surveyor retains its separate capture reward. Each hero has an
independent absolute-week receipt published before resources are granted.
Reasoning: use the authored common/rare distinction and avoid consuming a
reward on an ineligible resource. The trigger is CGMine::onHeroVisit; tooltip
and receipt serialization are shared. Nine principal and five minimum AI cases
pass after linked82853. Review custom resource classification, multiple-goal AI
receipt forecasting and capture-followed-by-visit
interaction in Phase2. This interpretation does not amend the canonical text.

## Merchant Prince — resident scope and virtual Marketplaces

An owned visiting or garrison hero qualifies while linked to this town. Two
holders grant +2 virtual Marketplaces once, not +4. Existing supported exchange
modes consuming Marketplace efficiency benefit, retaining their ordinary caps;
fixed transfers and unsupported modes do not change. A real Marketplace remains
required. No kingdom-wide count is mutated. Reasoning: the text grants one town
modifier, not a kingdom-wide or per-holder count. Implementation is
CGTownInstance::getMarketEfficiency; eight principal and three Resource Broker
native cases pass after linked77224. Review future independent holder stacking
or new exchange modes if authored. These scope choices are provisional.

## Steward — resident contribution and day boundary

Provisionally both owned, reciprocally linked visiting and garrison heroes
qualify; each distinct selected holder contributes250 Gold, two contribute500.
Unlike Merchant Prince's town-single modifier, Steward describes a hero's
individual end-day condition. Sample residence at the existing authoritative
day transition and apply the town's ordinary handicap once to combined income;
do not introduce a separate persistent end-turn receipt or treasury grant.
Implementation candidate: CGTownInstance::dailyIncome consumed by
NewTurnProcessor, existing town income label and passive right-click breakdown.
Nine transition/handicap/ownership native cases pass after linked82853.
Revisit captures or residence changes between individual player
turns, asynchronous play and any explicitly authored future town-wide cap.
The choice is provisional and does not amend the canonical wording.

## First Blood and Slayer — independent extra increments

Provisionally each perk adds one extra ordinary Bloodrage increment to its
qualifying destruction. The first Elite/Champion death therefore grants three
increments when both apply, not four multiplicatively or two redundantly.
Both holders observe the same first qualifying death before its shared combat
receipt is spent. A capped grant still spends First Blood; resurrection never
restores it. Slayer uses the saved Core/Elite/Champion category, not numeric tier.
Existing summoned/clone exclusions and Bloodrage caps remain unchanged.
This interpretation remains reviewable; it does not amend the canonical design.

## Eagle Eye retained combat participants

The canonical wording says after combat, not only after victory. Provisionally
grant selected Eagle Eye to participants whose heroes remain available:ordinary
winners and retained retreat/surrender heroes. Deleted defeated heroes gain
nothing. Draw retention follows the existing hero-retreat setting; troopless
winners follow the existing automatic retreat. Introduce no new survival policy.
Capture the highest eligible
Level1–3 enemy HERO_SPELL before battle cleanup, keeping earliest-cast ties,
then use existing learning receipts before map removal/tavern preservation.
Creature casts do not enter that history. Saved roster, school eligibility,
already-known exclusion and selected current-v3 rules remain authoritative.
The unselected/legacy bonus path remains unchanged. This scope is reviewable,
not a claim that every retention/save interaction is certified. All11 principal
cases pass after linked11731, including actual winner/retreat/surrender, creature
history exclusion and defeated hero removal. Broader retained draw/troopless
winner, tavern rerecruitment and save restoration remain Phase2.

## Lucky Recovery composition and attack-local Avatar admission

Generic and Sylvan Lucky Recovery each recover10% of actual non-overkill melee
damage on positive Luck, healing only survivors. If both independent perks are
selected, provisionally add their authored fractions and round down once:
20% total, not two independently rounded ticks. Neither effect resurrects a
dead attacker or applies to ranged/record-only forecasts. Review composition
and delayed casualty interactions in Phase2. Focused live/detached cases are
source/native accepted within the30-case gate after linked71404, zero skips.

Avatar of Rage tests the attack's captured effective Bloodrage against that
side's captured maximum. Blood Scent's existing attack-local increase may meet
that threshold for this attack only, without changing stored Rage. Its25%
intrinsic Creature Defense ignore adds through existing physical damage
channels and their cap; it never converts Hero Primary Attributes into
Creature Attack/Defense. Expert perk cardinality does not permit simultaneously
selecting Endless Bloodshed; extended-cap threshold controls are therefore
pure captured-rule fixtures, not illegally selected hero builds.

Veiled Movement follows the existing current-controller Ghost Walk capability
and suppresses only explicitly movement-triggered Overwatch reactions. Unlike
Night Prowler's separate crossing requirement, its wording does not require
actually crossing another creature. Ordinary shooting is unchanged.
The current-controller fixture preserves the legacy enemy selector's original-
target-side semantics. It proves perk ownership, not correct current-controller
hostility; that existing allegiance interaction remains a Phase2 finding.

## Frozen normal-activation timing

The supplied Conflux rebalance requires a Frozen stack's next normal Creature
Activation to be forfeited, followed immediately by thaw. The freezing attack
and a subsequent Shatter attack never permit retaliation, including after
Frozen is removed by that Shatter. Cleansing before the normal slot permits
normal action; nothing restores an already forfeited activation.

Provisional interpretation: Morale, Second Wind and other extra activations
cannot move, attack or use abilities while Frozen, but do not consume its
normal-slot lifetime or thaw it. Preserve the recipient's successful-application
round stamp after every removal, so cleansing or Shatter cannot enable another
successful freeze that round. The required20% trigger belongs to a resolved
stack melee attack/retaliation, not individual creatures; its roll is distinct
from whether the surviving recipient remains eligible for application.
Review bonus-slot scheduling and multi-strike attacks explicitly during focused
acceptance; do not substitute existing Stone Gaze/Blind activation semantics.
Status:source/native accepted in47/47 focused cases after linked6035; rendered
verification remains pending and is not inferred from native success.

## Reality Warp mixed-pair resistance and confirmation

Status:source/native accepted in73/73 principal cases after linked6035;
rendered verification remains separate.

The canonical total exchange does not specify how a mixed friendly/enemy cast
handles Resistance or Magic Mirror. Selected hostile endpoints, determined by
their current controller, receive the existing cached Resistance resolution;
friendly endpoints do not resist. If any selected hostile endpoint resists,
neither endpoint exchanges effects. A reciprocal exchange is not redirected
onto a third stack by the single-target Magic Mirror path. Recipient eligibility
for each captured effect remains deterministic and does not roll Resistance.
This preserves the exchange's indivisibility without making hostile casting
ignore defenses. Revisit two hostile Reality Breaker targets, Twist of Fate,
Magic Mirror and Counterspell composition during Phase2.

The human interface selects two stacks and opens one centered, scrollable
complete move/stay preview. Only Confirm casts; changed captured state requires
fresh review. This adds no separate activation ability. AI initially values
the next reachable attack horizon using actual detached before/after states;
long-horizon regeneration and delayed statuses deserve a second look.
Implementation: BattleSpellMechanics, RealityWarpEffect, the shared collector,
BattleActionsController and BattleAI. No rendered acceptance is implied.

## Fate Dealer spill candidate draws

Status: provisional implementation; focused native22/22 passes after linked46720.

Generate two independent uniform legal spill candidates with replacement,
consistent with Shapeshifter. If exactly one is hostile to the caster's current
ownership, choose it; otherwise choose fairly between the draws, including
duplicates. Preserve the existing half-primary-actual-HP-loss amount, then apply
the selected recipient's own defenses. Do not reroll an immune or resistant
recipient. Review replacement versus distinct candidates later; the canonical
rule already specifies the hostile preference and random same-side choice.

Production ownership: scripts/spells/damage.lua collateral selection and
AI/BattleAI/SpellTargetsEvaluator.cpp expectation. With H hostile and F friendly
candidates and N=H+F, each hostile has probability(H+2F)/N² and each friendly
F/N²; without the perk each is1/N. Focused evidence must include duplicate and
same-side draws, controlled ownership, recipient defenses without reroll, exact
weighted AI expectation without live RNG, and paid AI with Orders competing.
Accepted evidence: runtime17/17 in5.471s and AI5/5 in1.888s, zero skips,
failures or errors. Receipt: build/nh-fate-dealer-native.oy8R/receipt.md. Runtime
and AI explicitly compare current combat controller against caster ownership;
ordinary ownerMatches retains its existing initial-side semantics. Review wider
control/casualty interactions in Phase2 and replacement versus distinct draws
in a later gameplay review. Source/native acceptance is not rendered delivery.

## Polymorph footprint restoration and Phantom body

Status: provisional implementation; principal25/25 and foundations17/17 pass.

Final exact-pair native evidence: linked64681, principal24.210s and
foundations1.831s, zero failures/errors/skips. Receipt:
build/nh-polymorph-native.WSrQen7z/receipt.md. Paid registered AI casting with
Orders and active Shapeshifter passes. Runtime, AI, status and protocol guards
are accepted; older preparatory notes below preserve the selection rationale.
No binary form snapshot, bespoke artwork or rendered delivery claim.

Use the approved nearest-legal-position policy for the original footprint on
expiry or Dispel. If no legal original footprint exists anywhere, retain the
current form, HP and position and retry safe restoration rather than overlap,
kill or heal creatures. The resulting delayed restoration is an exceptional
duration rule requiring a second look. Its Pending Changes amendment is now
integrated into canonical Polymorph; status must expose the exception rather
than silently present it as ordinary expiry.

For Phantom Army, preserve the copied offensive body's aggregate creature HP
when transforming; retain its separate current/initial Integrity, ordinary
expiry and Integrity damage behavior. Converting offensive count from Integrity
would silently alter Phantom Army's existing model. Review whether Phantom
forms should intentionally use a different policy. Candidate production seams:
CUnitState, battle/BattleForm and spells/effects/BattleForm. No native proof yet.

Read-only architecture review identifies activation prerequisites: preserve the
logical form marker while restoration is pending; use fresh accessibility in
deterministic unit-ID order after round hooks; validate converted Phantom counts
without confusing body HP with Integrity; clear form provenance before lethal
Integrity resets health; refresh client creature forms after Dispel; and use
separate damage caches for distinct form outcomes. Retain the existing explicit
binary-snapshot rejection until a full form-state save contract is implemented.
These are required implementation work, not accepted coverage.

Shapeshifter uses two independent uniform same-tier draws with replacement;
compare whole transformed-stack Army Value using the exact HP-converted count,
not a single creature's value. Resolve ties by canonical creature order. This
interpretation and Phantom body policy are integrated into canonical wording
under the user's provisional-decision authorization. Review whole-stack value
versus per-creature value and repeated-draw policy later. Runtime and weighted
detached forecasts must agree; no native proof yet.

## Reality Warp transferred-effect beneficiaries

Status: provisional interpretation; next-slice preparation, not activated.

Focus Magic's beneficiary follows the receiving stack's controlling side;
Arcane Breach's beneficiary is the side opposing its new recipient. Preserve
original caster attribution, captured strength/perk parameters and remaining
duration. Keep unknown legacy hostility provenance rather than inventing a
caster. This makes transferred effects function in their new location without
recasting them at the Warp caster's power. Review controlled-recipient ownership
changes after transfer. Confusion pending state travels with its magical effect,
but previous resolved-behavior history stays with the recipient. Orders,
transformations and typed non-transferable effects stay excluded. Candidate
production seam: NewHorizonsRealityWarp's shared validated reciprocal plan and
atomic packet application. No native proof yet.

## Mire Shaper additional Bog Ambush patch

Status: provisional implementation; focused native acceptance passed10/10.

Calculate the ordinary School/Spellcraft/Warcasting-scaled patch count with its
five-patch cap, then add the selected perk's one additional patch. The perk thus
permits three to six patches rather than disappearing at high Spell Power.
This preserves the spell's normal cap and the perk's explicit extra patch.
Review whether a future design should impose a global five-patch cap instead.
Implemented shared seam: NewHorizonsMagic::quicksandPatchCount in
lib/spells/NewHorizonsMagic.cpp; client, Lua authority and AI consume that count.
Focused count, paid placement and actual AI-submission fixtures are present.
Final native10/10 passes, zero skips, in2.587s after fixture-only relink74808.
Receipt: build/nh-mire-miracle-native.lBbjTbsn/receipt.md. No rendered claim.

## Miracle Worker casualty restoration

Status: provisional implementation; focused native acceptance passed14/14.

Preserve healing allocated to wounded surviving creatures, then increase the
remaining casualty-restoration HP pool by25%, flooring once. A fully destroyed
eligible stack receives125% of the whole pool, subject to the existing original
count cap. Wound-only healing is unchanged. This follows the perk's "casualties"
wording without multiplying already-rounded creature counts or granting extra
wound healing. Review whether the intended design should instead boost the
entire restoration pool. Implemented seam: scripts/spells/heal.lua amount
calculation used by legality, forecast and execution. Fourteen focused native
fixtures pass14/14, zero skips, in5.580s on the final exact pair, including
paid AI with Orders. Receipt: build/nh-mire-miracle-native.lBbjTbsn/receipt.md.
Broader casualty/capacity compositions remain Phase2; no rendered claim.

The user authorizes reasoned provisional gameplay judgments when rules or
interactions are unclear. Implement and verify the choice, rather than stopping
the implementation loop for every ambiguity. This ledger identifies situations
worth a second look; it does not replace the canonical New Horizons.md.

For each material choice record the specification clause, behavior, rationale,
source paths, focused evidence and review scenarios. Preserve resolved entries
and their eventual disposition. Actual specification amendments belong in
Pending Changes until integrated. Explicit settled user decisions take priority.

## Terrain Rebirth selection and modifier composition

Status: provisional interpretation; focused native acceptance passed25/25.

The authored terrain table names one Elemental per context. Adaptive Element
therefore selects that legal singleton; Perfect Convergence forces the same
primary result. Do not invent secondary thematic types to manufacture a
difference. Review whether future design should give Adaptive a broader pool.

Elemental Attunement applies to both first and Chain appearances because it
describes a reborn Elemental without a generation exclusion. Perfect's "every
Rebirth" changes Chain's default random selection too. Chain keeps its fixed
25% immutable original-HP basis and combat-use restriction; apply the new
appearance's matching20% bonus once after that base calculation.

Production: lib/battle/NewHorizonsElementalRebirth.cpp,
server/CGameHandler.cpp, AI/BattleAI/StackWithBonuses.cpp. Review successive
appearance HP composition, terrain-selection usefulness, and saved-battle
continuation. Focused native results belong in the functional completion matrix.

## First-round Elemental Conjurer Initiative

Status: provisional lifecycle implementation; normal-round native acceptance passed.

Use the existing one-turn spell bonus for +2 Initiative through the summon
round, preserving normal bonus transport and caching. Review Time Stop and
Spell Lock interaction: those systems may freeze generic duration beyond the
literal first battlefield round. Production: scripts/spells/elementalConvergence.lua.
Normal next-round expiration is included in the focused native fixture.

## Overwatch range and voluntary movement

Status: provisional interpretation; principal native acceptance passed29/29.

Use the ordinary unpenalized ranged distance (10 hexes), capped by an explicit
limited shooting range. No-distance-penalty abilities do not make the trigger
radius infinite. Require an outside-to-inside entry, not arbitrary movement
already inside range. This makes "moves into its range" an observable transition
instead of treating every legal ranged target as already inside an infinite range.

Only accepted ordinary voluntary movement triggers. Flying checks its landing;
Teleport/Blink, forced movement, deployment, gating and return-after-strike do
not. Simultaneous eligible shooters resolve in stable unit-ID order. Review
whether the intended range should instead be a distinct reaction radius, whether
inside-range movement should trigger, and competing-reactor order. Principal
implementation: NewHorizonsBattlecraft, CBattleInfoCallback, CUnitState and
BattleActionProcessor. Principal29/29 native cases pass; occupied-transit AI/UI
forecast parity and advanced reaction effects remain Phase2 review items.

Pass-through movement across an occupied ground hex cannot publish an overlapping
stack position. Reactions therefore occur at the next legal inside-range endpoint;
if transit leaves range before any such endpoint, no shot triggers. Review this
bounded Ghost Walk/Passing Lines exception without introducing illegal state.

Use the existing counter-reaction recursion guard so Counterfire does not answer
an Overwatch reaction. The existing next-attack Battlecraft Wait bonus applies
to and is consumed by that shot. Review these reaction-chain/next-attack semantics
in Phase2; do not duplicate attack-resolution machinery merely for this perk.

## Rapid Embarkation and Navigation

Status: provisional interpretation; principal native acceptance passed29/29.

Rapid Embarkation's explicit "costs only10% of maximum daily Movement" is a
final boarding/disembarking cost, replacing the ordinary cost rather than an
intermediate amount that Navigation halves again. This honors the named fixed
cost without manufacturing a5% figure absent from its wording. Review whether
future design should intentionally allow multiplicative stacking. Shared movement,
authoritative boarding and pathfinder parity pass in the focused29/29 gate;
custom-vehicle composition remains unverified.

Preserve the explicit Lighthouse/free-boarding exception ahead of Rapid
Embarkation: no embarkation penalty remains no penalty, with the existing ordinary
step-cost treatment. The perk must not increase the cost of an already-free action.

## Nature's Wrath conduction and range

Status: provisional interpretation; Nature's Wrath focused acceptance passed16/16.

The authored nearest-unvisited route has no numerical chaining radius. Use the
whole playable battlefield and deterministic unit-ID ties, without changing
generic Chain Lightning. Healthy friends conduct with zero healing; living
immune/invincible stacks conduct but receive no effect. Dead, ghost, turret,
off-board and Time Stopped stacks are not route recipients. Resolve the route
before defenses: a resisted hop still counts and attenuates but does not stop
the current. These choices follow the described living current rather than
turning defenses into random target-selection changes. Review chaining radius,
defended-target continuation and invalid-status exclusions. Preserve the
authored17/19 distinct-recipient caps,93% attenuation and survivor-only healing.

## Pursuit March daily recovery

Status: provisional interpretation; Pursuit March focused acceptance passed13/13.

After a surviving hero wins, including an opponent's retreat or surrender,
restore floor(10% of the current travel-layer daily Movement maximum), capped
at the missing daily Movement. Never reduce already-over-cap Movement. Consume
the once-per-day use only when positive recovery succeeds. The specification
does not define zero-benefit use consumption; preserving it avoids wasting a
reward that cannot restore anything. Review travel-layer changes, victory modes
and whether zero recovery should consume the use. Persist the day through an
authoritative atomic movement update, without per-update polling.

## Pandemonium logical debuff counting

Status: provisional interpretation; principal Pandemonium native acceptance passed25/25.

Count each distinct authored DEBUFF identity once per stack, not every Bonus
component or repeated application. Snapshot all counts before damage resolves.
Pandemonium Master multiplies each contribution by1.25, rather than growing the
multiplier with the count. Physical and magical Poison share one logical Poison
identity. Ongoing spell debuffs may use PERMANENT bonus duration; duration alone
does not make them innate characteristics. Innate/raw-stat sources stay untagged.
Hostile Spell Lock counts; protective friendly Spell Lock does not. Time Stop's
incapacitation and Frenzy's forced zero Defense count as explicit harmful statuses.
Review mixed-effect classification and simultaneous Poison variants. Metadata
must be complete before activation; an unregistered helper is not coverage.
