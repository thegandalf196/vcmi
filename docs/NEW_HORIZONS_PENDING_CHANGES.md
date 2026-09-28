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

### School-rank spell potency — 2026-09-27

Basic, Advanced, and Expert rank in each of the six Magic Schools must
progressively strengthen applicable spells of that school, in addition to
gating ordinary acquisition of higher spell levels. A legitimately inscribed
spell remains castable without the rank. Begin with a modest, coherent
Heroes V-like damage rule: improve the coefficient that multiplies Spell Power,
not merely flat base damage. Expert rank does not automatically grant Mass
versions; those remain perk-granted. For non-damage spells, choose meaningful
effect-appropriate rank improvements, with explicit exceptions instead of a
blind numerical multiplier. Exact coefficients and the first-pass exception
matrix await a spell-system audit and authored integration into the canonical
Markdown. Track implementation separately in UP-027.

## Integrated history

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
