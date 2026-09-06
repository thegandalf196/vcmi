# New Horizons — agent startup and goal prompts

## Before starting work

1. Work in the HeroesIII-Definitive repository, not the historical Reconstruction
   tree. Read AGENTS.md, NEW_HORIZONS_DESIGN.md, NEW_HORIZONS_MVP.md,
   NH_WORKER_PLAN.md and NH_DELIVERY_PIPELINE.md in this docs directory.
2. Inspect `git status --short --branch`, the latest role handoff and actual build/
   test evidence. Old status paragraphs are history, not instructions to redo work.
3. Confirm role ownership with Dispatcher. Do not start a duplicate active owner.
   Resume its saved Pi session when available (`pi --session <saved-session>`).
   tmux does not survive reboot; saved conversations do. No automatic GUI launch.
4. Inspect `/goal status`. Resume an appropriate stopped goal with `/goal resume`;
   edit an existing objective with `/goal edit <objective>` when a change is needed.
   Use the new-goal prompts below only for a session without the intended goal.
   Never repeatedly replace a goal just to reset counters or evade safety limits.
5. Goal activation is only proved by the latest harness contract/status, not by
   this file, a tool being visible, or a sent tmux message. Keep existing safety
   settings. Provider/safety pauses and external waiting must be reported honestly.

Commands below are entered in the worker's Pi editor, not the shell. When delivering
through tmux, use literal send-keys followed by explicit Enter to that worker only;
never inject into the user's Dispatcher chat. Verify the resulting status.

## Runtime goal

```text
/goal Implement and verify all Runtime-owned New Horizons gameplay in docs/NEW_HORIZONS_DESIGN.md under docs/NH_WORKER_PLAN.md and docs/NH_DELIVERY_PIPELINE.md: Orders/Doctrines, six-school spells, deterministic growth/scaled secondary attributes, masteries and creature-tier mechanics, with real AI and versioned save compatibility. Read docs/NH_RUNTIME_HANDOFF.md and actual evidence to select the next unfinished task; do not redo completed checkpoints. Own lib/server/AI/native tests only; coordinate interfaces with Frontend and compilation with Build. Fix release-candidate rule defects before unrelated breadth, then continue full scope. Fun first, balance later; authoritative validation, save integrity and required independent gameplay gates are mandatory. Preserve shared dirt, no UI/CMake edits or commits. Maintain evidence and next action in the handoff. Full owned scope, not a narrow test pass, defines completion.
```

## Frontend goal

```text
/goal Implement and verify all Frontend-owned New Horizons UI/art in docs/NEW_HORIZONS_DESIGN.md under docs/NH_WORKER_PLAN.md and docs/NH_DELIVERY_PIPELINE.md: Orders/Doctrines feedback, selectable six-school spellbook, hero growth/secondary attributes/masteries, redesigned hero screen and creature-tier presentation. Read docs/NH_FRONTEND_HANDOFF.md and current evidence for the next unfinished task. Own client/clientsdl and original editable/generated artwork only. Use real Runtime APIs, never fictional bindings or frontend rule mutation. Fix frozen-candidate control defects first without modifying frozen bytes. Coordinate with Build and sole Content Tester; do not run GUI or commit. Require readable real pixels, normal input, truthful effects and asset provenance before acceptance. Continue the full owned scope beyond the first increment and retain exact evidence/next step.
```

## Build/Integrator goal — includes Windows by default

```text
/goal Locally assemble, test, integrate and deliver the complete New Horizons redesign per docs/NEW_HORIZONS_DESIGN.md, docs/NH_WORKER_PLAN.md and docs/NH_DELIVERY_PIPELINE.md. Read docs/NH_BUILD_HANDOFF.md and docs/NH_WINDOWS_ACCEPTANCE.md and actual outputs before choosing work. Own CMake/config/non-Image curated data/build/package tooling and sole serialized shared builds, reviewed commits/pushes and publication. Keep Linux and Windows green incrementally. Freeze and deliver small coherent playable previews while later feature work continues; do not wait for the whole redesign or let unrelated new features move an existing release target. Preserve exact source/binary/content identity, required DLLs/resources/setup, notices/corresponding sources and independent Tester gates. Keep source ownership and quiet GUI intervals. Use bounded local repair with the working Windows cloud route as a fallback, not endless rebuild loops. Commit/push verified scoped changes with prescribed identity/privacy checks. Confirm actual private GitHub release assets before claiming delivery. Continue all owned full-design integration requirements, not only the first package.
```

## Content/Tester goal

```text
/goal Independently validate the full New Horizons redesign under docs/NEW_HORIZONS_DESIGN.md, docs/NH_WORKER_PLAN.md and docs/NH_DELIVERY_PIPELINE.md. Read docs/NH_COMMAND_ACCEPTANCE.md, docs/NH_CONTENT_ACCEPTANCE.md, docs/NH_TESTER_RESULTS.md and docs/NH_WINDOWS_ACCEPTANCE.md for actual latest evidence. Own independent tests/manifests/reports only, no product source/art edits or commits. Verify each frozen candidate identity and test real human/AI commands, spells/schools, growth/attributes/masteries/UI/tiers and supported save/reload boundaries as implemented; add negative and legacy controls. Only you execute bounded private guarded Xvfb/XTest journeys after Build's candidate/quiet handoff; never host input, original executable, competing GUI or unapproved fallback. Audit package dependencies, source/notices and asset provenance. Send concrete failures to owners for fix/rebuild/retest; preserve passing evidence without accepting stale candidates. Native tests, Wine and Linux GUI are not native Windows gameplay proof. Complete only when all owned full-design acceptance requirements are evidenced.
```

## Optional Windows Packaging goal — only after explicit ownership transfer

Do not start a fifth worker just because this prompt exists. First satisfy the
exact-file handoff in NH_DELIVERY_PIPELINE.md and record it in NH_BUILD_HANDOFF.md.

```text
/goal Prepare and verify Windows packages for the frozen New Horizons incremental candidates and subsequent full-design delivery under docs/NH_DELIVERY_PIPELINE.md. Read the explicit packaging ownership transfer in docs/NH_BUILD_HANDOFF.md and the independent gates in docs/NH_WINDOWS_ACCEPTANCE.md. Edit only the delegated allowlist; without it request assignment and perform read-only review. Consume exact frozen sources/binaries, close runtime DLL/resource/setup and license/corresponding-source requirements, and hand immutable outputs/checksums/evidence to Build and Content. No product rules/UI/CMake edits outside delegation, no competing builds, GUI, staging, commits or publishing. Build retains integration, scheduling and release upload; Content independently accepts packages. Preserve user assets, Git identity and candidate scope; distinguish compilation/package checks from native Windows playability. Continue through the delegated full-design packaging deliverables, not an unaudited ZIP.
```

## Milestone handoff format

Use the existing role handoff, not a parallel report directory:

```text
Checkpoint: <role / milestone / date>
Changed files and source/candidate identity:
Validation: <actual command, exit, evidence path, behavior proved>
Unresolved limits or failing gate:
Next executable action and owner:
If waiting: <arranged wake owner/event; harness-compliant deadline if needed>
```

No goal may declare the entire redesign complete from a successful first-increment
build or narrow test. The user may pause or change priorities; subsequent user and
harness contracts govern. Do not disable safety guards to manufacture continuity.
