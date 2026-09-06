# New Horizons — durable worker plan

## Authority and use

This is the durable work plan referenced by each worker's `/goal` objective.
The user explicitly requested formal worker Goal mode after this plan was written.
Activation is session-specific: only the latest harness-injected Goal contract
supplies active status and the matching goal ID. This document alone never
activates Goal mode or authorizes goal-status tools. Preserve existing safety
limits; report any safety/provider pause rather than claiming uninterrupted work.

Read [NEW_HORIZONS_DESIGN.md](NEW_HORIZONS_DESIGN.md) for the full product scope
and [NEW_HORIZONS_MVP.md](NEW_HORIZONS_MVP.md) for the compatibility foundation.
This plan supersedes historical W1–W6 ownership in old handoff entries, not their
evidence. The four roles below are the active workers. Dispatcher coordinates;
Build alone integrates. Keep existing handoffs rather than duplicate report trees.

## Product objective and sequence

Deliver the user's New Horizons redesign as working, AI-supported gameplay:
Orders/Doctrines, six magic schools, deterministic primary growth, secondary
attributes, masteries, redesigned hero UI, and creature tiers. Fun first; tune
numerical balance later. Correctness, usability, save integrity and AI are required.
The Orders/Doctrines checkpoint below is the first increment, NOT full completion.

1. Finish and independently test the integrated combat-command increment.
2. Six-school registry, actual spells/effects, AI and spellbook integration.
3. Data-driven growth/scaled formulas, secondary attributes and save identity.
4. Masteries, hero UI, remaining commands/spells and creature categorization.

Keep unresolved design choices visible in the design contract. Do not silently
invent settled faction-school tables or delete creatures for a leadership cap.
Keep the existing authoritative in-process VCMI execution architecture; its
performance experiment is closed. No architectural rewrite milestone.

## Runtime — rules, AI and persistence

**Owned source:** lib/, server/, AI/, native test implementation. No frontend,
art, CMake or packaging edits. Coordinate shared interfaces before changing them.
**Durable evidence:** [NH_RUNTIME_HANDOFF.md](NH_RUNTIME_HANDOFF.md).

**Current objective:** make Charge, Hold the Line, Advance, Aggressive and Defensive
execute through validated authoritative commands for humans and AI. One hero
action per round is shared with spells; Orders spend no mana, expire as declared,
and do not consume a creature action. Doctrines persist until changed. Rules and
coefficients are explicit, tunable and versioned; old saves retain old semantics.

**Next checkpoint at restart:** fix actual HeroCommandTest.cpp compilation errors
in `build/new-horizons-linux/commands-build-fix2.log` (incomplete PlayerState,
TeamState, TavernHeroesPool and bonus serialization types). Send Build the minimal
fix; Build owns the shared compiler invocation. This is a dated starting point,
not a claim that later fixes have not landed—consult the latest handoff.

**Acceptance:** compiled tests prove legal/illegal commands, action-budget exclusion
both directions with spells, real damage/movement changes and round expiry,
Doctrine replacement/persistence, legacy/version checks and round-trip state.
AI evaluates commands alongside spells rather than always choosing a fixed Order.
Independent normal-input human/AI gameplay must exercise the resulting behavior.

## Frontend — usable controls and original artwork

**Owned source:** client/, clientsdl adapters, assets/new-horizons/, and
Mods/new-horizons/Images/. No runtime/AI rules or non-Image content registration.
**Durable evidence:** [NH_FRONTEND_HANDOFF.md](NH_FRONTEND_HANDOFF.md).

**Current objective:** deliver discoverable, usable hero actions with accurate
availability, cancellation, active Order/Doctrine feedback and truthful tooltips.
Use the existing spellbook framework; author original editable assets and runtime
outputs with provenance. Do not claim provisional artwork is finished illustration.

**Next checkpoint:** review the current BattleHeroActionWindow and battle feedback
against Runtime's final API, then send Build source/art readiness for a frozen
candidate. Preserve the Dispatcher-added gui/Shortcut.h include.

**Acceptance:** client compiles; rendered controls fit and remain readable;
normal input can choose/cancel commands and reach spells; spent/invalid actions
are disabled without bypassing server validation. Tester verifies actual pixels
and input on the integrated candidate. Static art generation alone is insufficient.
Then continue six-school visuals/UI with real content identifiers, not inert icons.

## Build/Integrator — local assembly, regression gate and delivery

**Owned source:** CMake, config/schema, non-Image curated module data/metadata,
build/dependency/package scripts. Sole owner of serialized shared builds, staging,
reviewed commits and pushes. Preserve all other workers' dirty changes.
**Durable evidence:** [NH_BUILD_HANDOFF.md](NH_BUILD_HANDOFF.md) and
[NH_WINDOWS_ACCEPTANCE.md](NH_WINDOWS_ACCEPTANCE.md).

**Current objective:** assemble/test locally first, integrate coherent working
increments, and deliver auditable Linux/Windows packages without proprietary assets.
**Next checkpoint:** coordinate the Runtime test-compile fix, build vcmiclient and
vcmitest in the existing Linux root, run focused/regression tests, verify curated
rules/art registration and freeze one candidate for Tester. Fix the existing
MinGW SDL_ttf dependency failure afterward in the existing cross-build root; no
repeated cloud rebuilds as a substitute for local debugging.

**Acceptance:** actual successful build/test exits; candidate source identity and
binary hashes; independent Tester result; preserved save compatibility; clean
scoped diff/privacy review before integration. Packages retain required runtime
libraries, attribution, licenses and corresponding sources. Windows cross-compiling
is not native Windows graphical acceptance. Do not publish an unaudited package.

User changed the repository to independent/private with definitive-mvp as default.
SSH origin uses github-gandalf; read access was verified at 98bd74f52. GitHub CLI
API token is invalid; that defers API-only actions, not local work or SSH Git.
Cloud repack 34050542538 failed; diagnose when logs are available, without claiming
its source-collection repair passed Windows. Never force-push or change visibility.

## Content/Tester — independent acceptance

**Owned work:** independent test tools, manifests, provenance review and results;
no product source/art implementation and no commits.
**Durable evidence:** [NH_COMMAND_ACCEPTANCE.md](NH_COMMAND_ACCEPTANCE.md),
[NH_CONTENT_ACCEPTANCE.md](NH_CONTENT_ACCEPTANCE.md), and
[NH_TESTER_RESULTS.md](NH_TESTER_RESULTS.md).

**Current objective:** independently establish that the integrated increment works
for humans and AI and preserves saves; fail concrete defects rather than accept
source coverage or a stale preview.
**Next checkpoint:** prepare fixtures/oracles and audit assets while Build finishes;
then test its frozen candidate through guarded normal-input combat and save/load.

**Acceptance:** reproducible bounded human/AI journeys covering orders, Doctrine
changes, shared spell budget, cancellation/availability, round transitions and
persistence, with identities, concise results and representative screenshots.
Only this worker may run private Xvfb/XTest GUI journeys. No host desktop input,
visible fallback, original executable launch or competing graphical runs. No
physical-display/native-Windows claim from Xvfb or Wine evidence.

## Continuity and reporting

Each worker updates its existing handoff at a material checkpoint with changed
files, exact validation command/exit, evidence path, unresolved defects and one
next executable task. Report defects directly to their owner and Build; tmux is
a wake signal, not the only record. Defer a cross-owner dependency and continue
useful in-scope work rather than broadening ownership or repeating ACKs.

Build coordinates source freezes and shared compiler/test scheduling. Dispatcher
maintains this plan and the design contract; no overlapping staging. A successful
compile is not gameplay acceptance; a first-increment pass is not full redesign
completion. Do not claim workers are executing without checking their real state,
or promise automatic user-chat replies when this turn ends.
