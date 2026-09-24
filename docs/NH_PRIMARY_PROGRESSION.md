# Versioned primary-attribute progression

The accepted replacement table is in
[NEW_HORIZONS_OVERRIDES.md](NEW_HORIZONS_OVERRIDES.md#approved-replacement-primary-attribute-table--2026-09-23).
Its activation is a separate integration step from this profile primitive.
The canonical `config/newHorizonsHeroes.json` still contains the older table
at this checkpoint; supporting a formula does not install the new class values.

## Saved profile contract

Each class profile may carry `progressionVersion` alongside its `starting` and
`growth` arrays, in Attack / Defense / Spell Power / Knowledge order.

- Missing version or version 1 preserves historical behavior: positive growth
  entries total 10, and the base at level L is `growth * (L + 4)`. The stored
  starting vector remains available but does not change that historical formula.
- Version 2 requires a starting total of 100 and positive growth entries totaling
  18. Its base is `starting + (L - 1) * growth`.
- Unsupported versions and malformed/nonintegral ratings are rejected. Arithmetic
  uses 64-bit intermediates; the hero rules' existing primary cap still applies
  when ratings are installed on a hero.

The discriminator lives inside the JSON profile already captured in each hero's
saved rules. It adds no independent mutable state or per-update polling. Resolving
a new installed profile must not rewrite an older hero's captured profile. Hero
class identifiers remain stable: Tower `core:alchemist` is displayed as Battle
Mage; Stronghold `core:battlemage` is displayed as Shaman; Solmyr remains a Wizard.

## Native integration coverage

The version-2 Knight fixture has passed native checks for real map initialization
and Knowledge-derived mana, authored map experience, serialized randomizer growth,
and authoritative level-up gains. A mixed-version world also passed full binary
save/load and campaign crossover checks with a version-2 Knight and an unversioned
legacy Cleric retaining their respective profiles. Existing version-1 fixtures
remain separate and unchanged.

These checks exercise the new formula without activating the canonical table.
They do not establish all-class initialization, AI decisions using the new
canonical ratings, or rendered UI acceptance.

## Remaining activation checks

Install all 18 approved profiles with version 2 together; verify exact values,
new-game generation, level gains, saved-world and campaign continuity, displayed
starts/growth, and AI use of the resulting attributes. In particular, retain old
captured snapshots and their version-1 behavior. Primitive arithmetic and schema
tests alone do not establish that the new table is playable.
