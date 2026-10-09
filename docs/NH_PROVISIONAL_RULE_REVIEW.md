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

Status: provisional interpretation; implementation in progress, not active coverage.

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
BattleActionProcessor; evidence remains pending focused tests and AI/UI consumers.
