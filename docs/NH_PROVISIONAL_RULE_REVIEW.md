# New Horizons provisional rule review

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

Status: provisional interpretation; prerequisite preparation, not active gameplay.

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
