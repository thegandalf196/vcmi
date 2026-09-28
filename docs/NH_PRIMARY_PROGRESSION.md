# Versioned primary-attribute progression

The accepted replacement table is in the canonical
[New Horizons.md](design-sources/New%20Horizons.md). The legacy 18-point
proposal and its disposition are documented in
[NH_OVERRIDE_MIGRATION.md](NH_OVERRIDE_MIGRATION.md). The canonical
`config/newHorizonsHeroes.json` now contains all 18 approved profiles with
explicit progression version 3. The generated curated module
embeds the same data. This changes newly initialized games, not profiles already
captured in existing saves. Local playable-snapshot promotion remains a separate
validation step.

## Saved profile contract

Each class profile may carry `progressionVersion` alongside its `starting` and
`growth` arrays, in Attack / Defense / Spell Power / Knowledge order.

- Missing version or version 1 preserves historical behavior: positive growth
  entries total 10, and the base at level L is `growth * (L + 4)`. The stored
  starting vector remains available but does not change that historical formula.
- Version 2 requires a starting total of 100 and positive growth entries totaling
  18. Its base is `starting + (L - 1) * growth`.
- Version 3 requires a starting total of 100, positive growth entries totaling
  20, and `starting = 5 * growth` for every attribute. Its deterministic base is
  therefore `growth * (L + 4)`. Independently, the configured `extraGrowth`
  entries grant +1 Attack from Offense or Archery, +1 Defense from Armorer,
  +1 Spell Power from Spellcraft, or +1 Knowledge from Wisdom at
  10%/20%/30% for Basic/Advanced/Expert rank. These bonuses do not alter the
  fixed class vector or the captured progression profile.
- Unsupported versions and malformed/nonintegral ratings are rejected. Arithmetic
  uses 64-bit intermediates; the hero rules' existing primary cap still applies
  when ratings are installed on a hero.

The discriminator lives inside the JSON profile already captured in each hero's
saved rules. It adds no independent mutable state or per-update polling. Resolving
a new installed profile must not rewrite an older hero's captured profile. Hero
class identifiers remain stable: Tower `core:alchemist` is displayed as Battle
Mage; Stronghold `core:battlemage` is displayed as Shaman; Solmyr remains a Wizard.

## Historical version-2 integration coverage

The version-2 Knight fixture passed native checks for real map initialization
and Knowledge-derived mana, authored map experience, serialized randomizer growth,
and authoritative level-up gains. A mixed-version world also passed full binary
save/load and campaign crossover checks with a version-2 Knight and an unversioned
legacy Cleric retaining their respective profiles. Existing version-1 fixtures
remain separate and unchanged.

An additional installed-data fixture covers all 18 classes at authored levels
1, 2 and 20 without hero-rule or primary-rating overrides. Its level-1 case also
exercises authoritative level-ups for all 18 classes, followed by full binary
reload. Solmyr is explicitly selected as the Wizard representative. Mana checks
account for genuine Intelligence perks instead of assuming every hero lacks one.
These native checks do not establish rendered UI acceptance.

Activation verification: the selected native growth, compatibility, capability,
AI and spell-mechanics run passed 345 tests across 56 suites, with one opt-in
capability-only export intentionally skipped. All 12 Python hero-data checks and
the generated-module consistency check passed. The opt-in ordinary Knight
experience-quest export also passed with its new starting ratings and mana.
The committed `dcb01a936` build was frozen as snapshot
`4f65c4825321d87c46ad18b2e1fedc3f3e0bdc05a68d1f0e54a75d896dc9f446`.
That exact package completed 75 AI turns in a bounded 45-second headless
`All for One` check, reaching the start of day 26. A fresh private profile used
configured seed 1284510375, dummy media drivers, no autosaves, a 4 GiB memory
limit and a 200% CPU quota. Maximum completed turn time was 3733 milliseconds;
mean time was about 516 milliseconds. No checked crash, command rejection,
Leadership-limit or unsupported-rules error appeared. The planned timeout
stopped the active turn, and no launcher/client child remained afterward.

That historical package was promoted for the ordinary Linux launcher and passed its
non-launching path verification. This is a bounded new-game/AI smoke check,
not evidence that the current version-3 profiles were built, tested, or promoted.

## Remaining activation checks

Verify version 3 with the integrated native regression set, a frozen candidate's headless
new-game/AI flow, and displayed starts/growth before making a broad acceptance
claim. In particular, retain old captured snapshots and their version-1 behavior.
Complete legacy test contexts explicitly replace installed settings, preventing
the new discriminator from being merged into deliberately unversioned fixtures.
Primitive arithmetic and schema tests alone do not establish playability.
