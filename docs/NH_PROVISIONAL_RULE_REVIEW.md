# New Horizons provisional rule review

## Polymorph footprint restoration and Phantom body

Status: provisional interpretation; next-slice preparation, not activated.

Use the approved nearest-legal-position policy for the original footprint on
expiry or Dispel. If no legal original footprint exists anywhere, retain the
current form, HP and position and retry safe restoration rather than overlap,
kill or heal creatures. The resulting delayed restoration is an exceptional
duration rule requiring a second look and a Pending Changes amendment before
activation; it must be visible rather than silently presented as ordinary expiry.

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
