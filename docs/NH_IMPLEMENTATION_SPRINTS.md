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

## Current implementation priority — complete Skills perks and spells

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
errors. Both repairs are pushed through `ddcd57391`; full Windows run
`36350655648` is in progress. No target-build success is claimed yet.

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
