# New Horizons Pending Changes

New Horizons.md is the sole canonical design specification. This document
contains only temporary amendments awaiting integration into its appropriate
sections; it is not a second permanent specification.

For each amendment record its user-approved decision, affected canonical
section, unresolved questions, and integration evidence. Remove an amendment
only after integration is verified, or an explicit decision supersedes it.
Implementation status belongs in the completion audit, not here.

The completed legacy Overrides transition is retained as history in
[NH_OVERRIDE_MIGRATION.md](NH_OVERRIDE_MIGRATION.md). Do not copy its retired
entries here and thereby recreate a permanent override layer.

## Awaiting integration

None.

## Integrated history

### Hand of Fate secondary mitigation — 2026-09-30 (integrated)

User-approved decision: after selecting the secondary recipient uniformly from
the surviving friendly/enemy pool, apply that recipient's own magical defenses
to the hit whose base is half the primary target's actual HP loss. Defenses do
not affect selection and must not cause a reroll. This clarification is integrated
into the detailed Chaos / Hand of Fate section of New Horizons.md.
Runtime implementation and delivery remain tracked in the priority queue.

### School-rank spell potency — 2026-09-27 (integrated)

Basic, Advanced, and Expert rank in each of the six Magic Schools must
progressively strengthen applicable spells of that school, in addition to
gating ordinary acquisition of higher spell levels. A legitimately inscribed
spell remains castable without the rank. Begin with a modest, coherent
Heroes V-like damage rule: improve the coefficient that multiplies Spell Power,
not merely flat base damage. Expert rank does not automatically grant Mass
versions; those remain perk-granted. For non-damage spells, choose meaningful
effect-appropriate rank improvements, with explicit exceptions instead of a
blind numerical multiplier. The initial authored coefficient ladder (provisional
balance) is: no School rank 100%, Basic 115%, Advanced 130%, Expert 145% of
the spell's Spell Power coefficient. Apply it before existing integer rounding;
preserve flat base terms, caps, costs, target shape, mitigation, and specialty
rules. For a multi-school spell, use the highest applicable rank once, never
stack the schools. Adventure Spells remain neutral and unscaled. Saved magic
rules version 3 carries the ladder; v1/v2 saves retain 100% so an ongoing game
does not silently change its formulas. Numeric healing, temporary HP, and
restoration may follow the same coefficient principle where the formula has an
actual Spell Power term. Discrete/binary spells need authored rank variants or
an explicit exception. The shared rule is now in the canonical Markdown Magic
Skills section; implementation and validation of specific spell effects remain
tracked in UP-027.

The five amendments approved before 2026-09-27 were integrated into the
canonical DOCX: Spell Lock duration stacking, Arcane Acquisition target
semantics, generic Faction-Skill combat statuses, consume-on-use Metamagic and
its accompanying perks, and ordinary Mage / Arch Mage melee penalties. The
edited document passed ZIP integrity and a complete 191-page LibreOffice render;
the affected pages were visually inspected without clipping or overlap.

### Bulwark of the Mire perk rules — 2026-09-27 (integrated)

Affected canonical section: Fortress faction Skill, Bulwark of the Mire perk
table. User-approved changes integrated into the repaired canonical
`New Horizons.md`:

- Toxic Spines: “the first melee attacker each round” is tracked separately
  for **each Defending Bulwark stack**, not once per hero army. That attacker
  must suffer Bulwark reflection before receiving physical Poison. Its base
  damage is `max(1, floor(actual reflected HP damage / 4))`; on the victim's
  next three real activations it deals base, `floor(1.5 × base)`, then
  `2 × base` physical damage. A new application with equal or higher base
  replaces the old potency and restarts three ticks; a weaker application is
  ignored. Poison does not stack. Cure removes it; ordinary Dispel does not.
- Immovable: its first-physical-creature-hit 25% final-damage reduction applies
  **only while the particular Bulwark stack is Defending**. Track the first
  qualifying hit separately per stack per round.

The repaired Markdown contains both clarified rows, checked against the perk
registry with no unapproved cell differences. The original DOCX remains an
archival conversion reference. No design choice remains open for these rules.
