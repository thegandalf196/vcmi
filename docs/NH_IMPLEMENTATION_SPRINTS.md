# New Horizons implementation sprints

## Purpose and authority

This is the durable execution register for completing New Horizons. It answers:

- what is being implemented now;
- what will be implemented next;
- what remains across the whole design;
- which dependency or verification gate prevents an item from being called done;
- which commit, test, build, or playable snapshot proves each completed step.

It does not replace `design-sources/New Horizons.docx`, which remains the sole
canonical design specification. It does not replace `NH_USER_PRIORITY_QUEUE.md`,
whose open user-assigned items take precedence. `NH_COMPLETION_AUDIT.md` remains
the broad requirement inventory; this file turns that inventory into an ordered
working sequence.

## Maintenance contract

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

## Current sprint — Armorer foundation and delivery closure

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
- exact Windows run `36326436603` targets full head
  `9806a27eff4ee4b427c92b270cc7ac5ea45b06bb`; keep this handle until terminal.

Remaining acceptance:

- monitor exact run `36326436603`, inspect its actual terminal result, and run
  the focused `IronDisciplineTest`, `HeroOrderStatePersistenceTest`, and Armorer
  AI cases on the matching native build where the route permits;
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

**State:** Planned; starts after Iron Discipline is committed and its exact-head
build is dispatched.

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

Completing Pavise gives Armorer three implemented Basic choices plus the already
implemented Basic-perk set needed by the strict Skill/perk progression model.

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
