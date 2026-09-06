# New Horizons runtime handoff

## Current redesign checkpoint — resumed 2026-09-06

Active ownership is **lib/server/AI/native tests**, per `NH_WORKER_PLAN.md` and
`NEW_HORIZONS_DESIGN.md`; historical W1 sections below are evidence, not current
file boundaries. Build alone compiles/integrates. No Runtime UI/CMake/packaging
edits or commits. Full redesign remains the goal after the first command increment;
architecture experiments are closed. Command native milestone is `54213f042`;
activation/schema repair is `66ddb01bd`. Command/six-school foundation `95a7001e3`
has Linux native and Windows client/install evidence, not full school-family or
Windows gameplay acceptance. Its immutable GUI candidate must remain unchanged.

Read and adopted `NH_DELIVERY_PIPELINE.md` and `NH_AGENT_START.md`, retaining the
existing full-scope goal. Fix declared candidate defects first; keep unrelated
primary/mastery breadth outside its release lane. Build remains sole integrator.

### Latest executable checkpoint

- Actual 14-proof RED captured and XML independently read:
  `magic-reward-red-commands-native-resume.xml` **13 PASS / Hat FAIL, EXIT1**;
  `magic-reward-red-magic-native.xml` **4 schema PASS / 10 mechanics FAIL, EXIT1**.
  Earlier proof API errors were corrected without changing assertions.
- Bounded production fixes compiled successfully. Actual
  `magic-reward-green-baseline.xml`: **128 total, 126 PASS / 2 skips, EXIT0**;
  curated XML: **39 total, 37 PASS / 1 skip / 1 filter-context FAIL, EXIT1**.
  Runtime independently read both. Nine formerly failing behaviors and all four
  schemas pass. Remaining exception was a proof-origin error: core cannot depend
  on NH school IDs. Test-only fix now uses each school's actual owning scope,
  asserts exact identifier resolution and core→NH denial, retaining every expected
  membership set. No production dependency bypass. Final rerun now GREEN:
  `magic-filters-final-baseline.*` **128 = 126 PASS / 2 skips, EXIT0**;
  `magic-filters-final-curated.*` **39 = 38 PASS / 1 skip, EXIT0**. Runtime
  independently inspected XML and exit files. Build now holds registered sources
  for reviewed commit, incremental Windows/Linux identity builds and new freeze.
- Production repairs canonicalize authored secondary
  IDs/variables in JsonKeyExtractor; use saved spell levels and new/original school
  union; resolve server skill changes and reward IDs BEFORE rank arithmetic;
  resolve limiter checks, reward/limiter components and quest text, including
  no-selected-hero quest components using its existing game callback. The LEVEL
  factor now counts known spells. Eight owned files, no global entity mutation,
  getter aliases, frontend API changes or player-validation bypass.
- GUI95 exposed unsupported `patternProperties` (78 unknown scoped keys). Build
  repaired mutable schema with supported typed `additionalProperties`; all four
  named-schema tests now PASS in both native profiles, exercising full/empty/real
  settings and malformed nested spell/faction/version data.
  No generic validation suppression and no mutation of immutable95.
- `NewHorizonsMagicFixtureExportTest` actually PASSES: ordinary full book
  **69 original / 59 combat spells**, map-authored rank3/2/1/1 converted through
  actual curated initialization, no rule overrides, parser/gzip exact readback.
  `testing/magic-native/cache/vcmi/testMaps/NHMagicFullBookRanks.h3m` is 666 bytes.
  School membership counts are 12/11/16/18/7/10 (overlap intentional). Content was
  notified for independent header/hash and later GUI audit. Independent fixture
  audit now reported PASS; no broad school GUI pass yet.

- First six-school build actually passed **691/691, EXIT0**. Baseline
  `magic-first-baseline.*`: 103 tests, 101 passes, one expected skip, one RED.
  Curated `magic-first-curated.*`: 8 tests, 7 passes, one RED. Runtime inspected
  both failure logs. Real six-school rank/cost/server cast, starting conversion,
  legacy-world exclusion, full game and BattleStart saved rules all passed.
- Both fixes and added controls are now actually GREEN: build EXIT0,
  `magic-fixes-baseline.*` **109 total / 108 passes / one expected skip, EXIT0**;
  `magic-fixes-curated.*` **20 total / 19 passes / one context skip, EXIT0**.
  Runtime independently inspected both XML files. Real installed Havoc AI choice,
  exact server cost, turn controls and legacy-header/world/new-game continuation
  all pass. Registered production is briefly held for Build's coherent milestone
  review, commit-identity rebuild and immutable copy. No Runtime builds or commits.
- The latter requires a separate private native `config/vcmi/testModSettings.json`
  preset including `core`, `vcmi`, `vcmi-test`, `new-horizons`. Keep baseline profile
  unchanged; school tests explicitly skip when its required registry is absent.
- Both formerly predicted REDs are now actual: successful Charge expired a
  preexisting STACK_GETS_TURN bonus (speed 10→5); actual ActiveModsInSaveList threw
  ModIncompatibility for the legacy header. Assertions remain intact.
- Fix 1 appends HERO_COMMAND to BattleUnitTurnReason, uses it only for successful
  command reactivation, and exempts it alongside existing UNIT_SPELLCAST from
  turn-bound bonus expiry. Legacy HERO_SPELLCAST/normal-turn behavior is unchanged.
- Fix 2 permits only an EXCESSIVE exact curated NH module in the save loader,
  documenting its non-replacing/save-scoped content invariant. The global mod
  verifier is untouched; required missing/disabled NH and other excess/missing
  dependencies still reject. Added safety controls pass. Required NH rejection
  was exercised in ONE baseline installed-state configuration: the latest native
  XML now records and asserts **DISABLED** against installed inventory. NH-absent
  NOT_INSTALLED is not a separately executed configuration; do not claim both.
  VERSION_MISMATCH alone is not an ordinary-save blocker in ActiveModsInSaveList
  (its caller ignores that status).
- Tester reports repaired activation works after real save/quit/restart/load, all
  three Orders, shared Bloodlust budget, Doctrine switch/persistence, seven rounds
  of bookless Blue AI choosing Aggressive. New-battle NONE and spell-AI journey are
  still pending. The first failed 542 profile genuinely omitted NH from its active
  preset; its save is legacy, not something to reinterpret. Build's launcher fix
  explicitly activates the curated module. Preserve those independent artifacts.

### Six-school foundation WIP (no compile or gameplay acceptance yet)

`lib/spells/NewHorizonsMagic.{h,cpp}` validates saved `magic.newHorizons` settings:
versions 1/1, ordered six scoped schools, all common hero-spell memberships,
optional per-spell level/cost[4], faction major/minor and optional positive weights
(default 3/1), six schoolSkills and legacy skillReplacements. Canonical
`config/newHorizonsMagic.json` is the **unwrapped** object; Build wraps it in generated
module settings. Invalid/unregistered data fails closed, not an inert spell list.

Public game APIs: `getMagicRules`, `getActiveSpellSchools`, `getSpellSchools(SpellID)`,
`getSpellLevel(SpellID)`. Battle counterparts: `battleGetActiveSpellSchools`,
`battleGetSpellSchools`, `battleGetSpellLevel`. Hero adds `getMagicRules`,
`getSpellSchools(const spells::Spell *)`, `getSpellLevel(const spells::Spell *)`;
existing best-school/rank and cost getters now use that snapshot. Frontend wired
those actual APIs, not hardcoded fictional IDs.

CGameState and BattleInfo carry separately serialized magic snapshots; proxies
and CGameInfoCallback delegate to the owning snapshot (not generic MapInfoCallback:
EditorCallback deliberately has no gameState and keeps its safe legacy default). NEW_HORIZONS_MAGIC is appended
before enum aliases with monotonic assertions. SpellSchool gains feature-gated
scoped-string serialization with legacy numeric reads; missing scoped identities
throw rather than falling back to an unrelated module.

Casting/learning coverage in source: hero mastery/damage-school bonuses, exact
adventure and battle mana costs, spell-level mechanics and filters, Mage Guild
school-weighted pools and saved-level partitions, Scholar/Eagle Eye limits, AI
spell/scroll/school reward and boat-cost queries. Old elemental tomes and damage
artifacts retain affinity behavior; globals CSpell.schools/level/cost are untouched.
AI's AtLeastOneMagicRule also uses saved schoolSkills and actual known-spell
membership instead of permanently preferring old school IDs.
`test/battleAI/NewHorizonsMagicAITest.cpp` now actually PASSES evaluator/authority
choice, Havoc Expert rank, saved cost and shared budget in the curated 20-test run;
crucially it relies on actual module activation, not a fixture override.

Build's pre-commit source review found a Tome AI affinity regression: the school
factor matches only new schools, not original affinity. Runtime additionally found
that the existing `knownWeight` counts UNKNOWN spells while its caller uses
`1-factor`: the new mismatch therefore MAX-values every original Tome, not zero.
`test/battleAI/NewHorizonsTomeAITest.cpp` now has actual RED→GREEN in both profiles.
Runtime independently inspected XML: four-school RED scores unknown=0/known=20000;
six-school RED scores 20000/20000 for all four tomes. The narrow affinity-union and
SCHOOL-known-counter repair passes all 4+4 proofs. Actual grantability is checked,
not just a score formula. Runtime independently verified final 113 baseline / 24
curated XML results, each with one expected/context skip and no failures.

Foundation source identity is now `95a7001e3`. The first Windows feature client
and install completed: `sdl-main-feature-build.exit` is 0 and
`build/new-horizons-windows-cross/install/VCMI_client.exe` exists (Runtime verified
both). This is build/install evidence, NOT Windows gameplay acceptance. The
Windows-only `VCMIDirs.cpp` repair uses the Boost path's native wide `c_str()`
instead of the unsupported wstring stream constructor; Linux was untouched.
Build completed the committed-identity Linux rerun and immutable GUI copy, then
released mutable production. The reward gaps are not closed by that foundation.

The now-registered reward/feedback/filter/application and LEVEL tests prove the
failures reported above: authored IDs bypassed conversion, quests could reject
migrated ranks, feedback displayed retired schools, and raw reward rank arithmetic
could downgrade a trained school if only the final server callback were remapped.
Spellbinder's Hat also had the analogous LEVEL-known-counter inversion.
Production repairs followed actual RED; their next GREEN run remains pending.

New-game starting old magic skills convert by saved data (duplicate ranks use max,
not addition); offering filters respect map bans and keep NH skills out of legacy
worlds. Six real ranked secondary skills/art/data are Build/Frontend-owned.

Still required: Tome AI proof/repair, broader guild/adventure/reward integration
coverage, dedicated new spell-effect families/AI, and integrated six-school UI
journeys. Positive scoped cast/persistence and legacy-header fixes now have the
actual native evidence above. Growth/scaled primary and derived
attributes, masteries and creature tiers remain later full owned requirements.

Before registering additional common hero spells, preserve the shipped 69-spell
snapshot boundary: current `validateRules` requires coverage of every installed
common spell, and `spellSchools` rejects missing entries. New roster work must
separate new-game completeness from old-snapshot validation and enforce per-world
spell availability (including artifact/AI enumeration), rather than breaking old
six-school saves or leaking new spells into legacy worlds. This is a prerequisite
for that future expansion, not an additional blocker for the current 69-spell
candidate.

During the next registered-source freeze, authored only an independent future
primitive: `lib/entities/hero/NewHorizonsPrimaryProfile.{h,cpp}` and
`test/hero/NewHorizonsPrimaryProfileTest.cpp`. These unregistered files parse
`{starting:[A,D,P,K],growth:[A,D,P,K]}`, require four positive growth increments
summing to ten, and compute deterministic int64 base ratings. Three source-only
proofs cover the level-20 Knight example, class-specific distributions, malformed
data and overflow prevention. This is **not** saved hero-growth activation or a
frontend view/choice API; primary caps, creature-stat isolation, mana, independent
skill rolls and derived attributes remain unimplemented.

### Implemented source, not yet integrated acceptance

- `HeroCommand` IDs NONE=0, CHARGE=1, HOLD_THE_LINE=2, ADVANCE=3,
  AGGRESSIVE=4, DEFENSIVE=5; `BattleAction::makeHeroCommand(side, command)` uses
  existing validated MakeAction transport. Queries: `battleUsesHeroCommands`,
  `battleCanUseHeroCommand`, `battleGetActiveOrder`, `battleGetActiveDoctrine`.
- Full coefficient JSON is captured at new-game init, serialized per game and
  copied into battle state. Missing old-save rules default to legacy, independent
  of currently installed module defaults. Build owns canonical config, strict
  schema and generated inline module settings/equality checks.
- Commands use StartAction/SetStackEffect/EndAction, existing damage/speed bonus
  mechanics and a dedicated non-spell bonus source. Shared once-per-round budget
  excludes spells in both directions; commands cost no mana/book/creature turn.
- Declared first-slice semantics: recipients are currently living ordinary own
  stacks (not turrets/SIEGE_WEAPON). Orders expire next round. Doctrines persist
  across rounds **within the battle**, switch without stacking; same selection
  and NONE/removal reject without spending. No cross-battle hero preference,
  stationary-history requirement for Hold, or Wait restriction for Aggressive
  is implemented. These limitations are explicit, not claims of full philosophy.
- BattleAI evaluates legal command effects in its existing hypothetical exchange
  scoring alongside legal spell/target pairs, with no fixed default Order. Actual
  situational AI tests pass in the committed command milestone; six-school AI
  behavior remains to be verified under its separate real registry/profile.

### Actual failures, fixes and evidence

`commands-build-fix2.log` failed instantiating complete game-state serialization.
Focused concrete-type includes were added only to `HeroCommandTest.cpp`, preserving
all assertions; Build's resumed client/test build exited 0.

`commands-native-resume.log/xml`: **17/19 pass**, including all nine spell/Order/
Doctrine budget combinations and real damage/movement/expiry/replacement controls.
NamedSettings failed because the synthetic array lacked its required resource mod
scope; fixed with `ModScope::scopeBuiltin()` (no lookup fallback). Full-state
roundtrip failed resolving an identifier. `commands-baseline-resume.log/xml`:
**63 pass, one expected skip, three town binary-compatibility failures**.

Root cause: Runtime incorrectly inserted HERO_COMMANDS after the MINIMAL enum alias,
which made CURRENT=894 and disabled later serializer feature gates. Fixed by moving
HERO_COMMANDS immediately after TOWN_CUSTOM_INITIAL_GARRISON, before aliases, with
an explicit monotonic static_assert. Do not treat pre-fix feature save bytes as a
valid redesigned-rules candidate. Assertions were not weakened.

Actual corrected-version run `commands-version-fixed.log/xml`: 86 passes, one
expected skip, one failed AI fixture. All 19 command tests and all 66 baseline
regressions passed. The AI fixture's Magic Arrow at capped power 99 was not a
sound dominance oracle against 100 Angels. Changed only that fixture to Implosion,
asserting effective power, legal cast, substantial damage relative to melee and
nonlethality; retained actual evaluator choice and authoritative server execution.

Build subsequently reports actual build EXIT0 and `commands-integration-resume.log/
xml/exit`: **91 passes plus one expected export skip, EXIT0**, including both real
AI choices, all four persistence/recipient tests and all prior baselines. Build log:
`commands-resume-20260906T191510Z.log/.exit`. Native green is not GUI acceptance.

### New native proofs and next executable task

- `test/battleAI/HeroCommandAITest.cpp`: actual evaluator chooses a beneficial
  command without a spellbook, or a strong offensive spell despite available
  Orders; each chosen action then goes through the real server validator. Checks
  mana and exhausted shared budget. Both now pass.
- `test/server/battles/HeroCommandPersistenceTest.cpp`: separately authored full
  BattleStart packet roundtrip into independent pre-battle game/army state, then
  actual packet application, round expiry and validated Doctrine switch. Build
  registered/compiled/ran it: original state is checked intact. All four tests
  pass, including war-machine/enemy exclusion, no ordinary recipient availability,
  and the explicit late-arrival limitation: new units gain no retroactive Doctrine
  bonus; switching Doctrine applies to then-living eligible stacks. Clone's existing
  Lua implementation creates a fresh unit, not a copy of command bonuses.
  This is not ordinary mid-battle GUI save support: CGameState excludes active
  battles from normal serialization.

`HeroCommandFixtureExportTest.cpp` is now source-ready, not yet executed:
`NH_EXPORT_COMMAND_FIXTURES=1`, filter `BooklessAndSpell/HeroCommandFixtureExportTest.*`.
Exports `NHCommandsBooklessAI.h3m` and `NHCommandsSpellAI.h3m` under the existing
private native cache's `testMaps` only after parser and real-init assertions, then
checks gzip EOF/CRC and byte equality. Red hero 0: A2/D2/P3/K10, book with Haste,
Bloodlust, Magic Arrow. Blue hero 2: A2/D2/P3 or 99/K10, explicitly bookless or book
with Magic Arrow/Implosion. Both: 600 Dendroid Guards, 80 Grand Elves, Ballista,
100 mana, Basic Pathfinding only. Anchors (17,10)/(20,10), towns (8,10)/(30,30).
Select Red human, leave Blue computer, and choose Gold starting bonuses in normal
setup; the H3M permits both player types, while native init explicitly checks Blue
AI. No GUI state injection or existing-save activation.

Exporter subsequently passed: Build reports 94 tests, 93 passes and one expected
skip, with both named assets copied/audited. No GUI acceptance yet.

New independently reproduced rejection defect: `commands-rejection-red.log/xml/exit`
shows a rejected second command reactivated the unit (3 activations instead of 2)
and expired its temporary speed bonus (5 instead of 10). Existing green tests had
not asserted that state invariant. `HeroCommandRejectionTest.cpp` retains both
failing assertions. Runtime fixed `BattleProcessor.cpp` to return before flow
processing for rejected HERO_COMMAND only. Do not indiscriminately gate all failed
actions: existing unit clients deactivate/block on submission and their
`requestRealized` has no failed-MakeAction recovery. Command chooser only closes and
sends, so it needs no synthetic activation. This preserves existing unit/spell
recovery; no frontend mutation or protocol shortcut. Actual
`commands-rejection-green.xml/log/exit` now verifies **95 total, 94 passes, one
expected skip, EXIT0**; Runtime independently inspected the XML and rejection
suite. Build integrated the scoped native milestone as
`54213f0425500208fe259a6255914f05ad71d663`; identity rebuild/candidate copy remains
Build-owned. This is not GUI or full-scope acceptance.

Independent, unregistered next-batch proof files (not in that milestone):
- `HeroCommandEligibilityTest.cpp`: tactics, missing commander and invalid-side
  guards; also preexisting STACK_GETS_TURN bonus BEFORE a successful Charge.
  That positive characterization is expected to fail from source review because
  command reactivation still uses legacy HERO_SPELLCAST expiry. It is not yet an
  executed defect or an additional Tester GUI hold. Preserve legacy spell behavior
  when addressing it; a distinct command reactivation reason is the narrow option.
- `HeroCommandCloneTest.cpp`: actual server HERO_SPELL Clone under an active
  Doctrine, no copied command bonus, then a subsequent Doctrine switch applying
  to both original and clone. Source-only, not yet compiled/executed.

Recovered the original read-only Word document under a PDF name at
an external read-only copy of the original design document; re-extracted all 990 paragraphs
under `/tmp` and read completely. Do not redistribute source document or art.
Future-school compatibility findings: preserve builtin four IDs/global legacy
spell classification; expose saved active school/membership mappings. SpellSchool
currently serializes as StaticIdentifier (numeric), so six-school work must address
stable IDs or feature-gated scoped-name serialization, retaining old numeric reads.
Prose/list Blind school disagreement joins the declared provisional data choices.

Next: Build reruns the rejection proof and full combined suite, then Tester performs
the frozen normal-input human/AI journey with the authored maps. Fix any concrete
failures before first-increment acceptance, preserving old saves. Independent human/AI UI/save journey
is still required before first-increment acceptance. Six schools, growth/scaled
attributes, masteries and tiers remain later owned implementation families, not
completed or blocked by remote API authentication.

## W1 — simulation / runner ownership

Owns `client/ServerRunner.cpp`, `client/ServerRunner.h`, and `server/` only (plus this coordination note). Initial tree was clean. Read AGENTS, MVP, upstream Coding Guidelines, Networking and Code Structure; Networking's universal-TCP statement is historical and contradicted by current implementation.

### Proven startup trace / W2 interface

`CMainMenu::openLobby` -> `CServerHandler::startLocalServerAndConnect(false)` -> runner `start(loadMode == MULTI, connectToLobby, si)` -> runner `connect`. `ServerThreadRunner` runs `CVCMIServer::prepare` and `run` on `runServer`; non-lobby `connect` uses `createInternalConnection`. `NetworkServer` construction creates no socket; only `start` creates TCP acceptor. Internal connections retain serialized packets, `CVCMIServerPackVisitor`, and `CGameHandler::handleReceivedPack` validation/AI ordering.

**W2 requested change:** ordinary single-player must select `ServerThreadRunner` regardless of saved `server.useProcess`; preserve `start(false, false, si)` and current connection/shutdown flow. No runner API change needed. W1 will not edit `CServerHandler` or menu files.

### W1 proved defect and implemented minimal fix

`CVCMIServer` constructor starts UDP discovery while initial state is LOBBY, before `prepare(false, false)` knows transport intent. Moved discovery startup into the `listenForConnections` branch after successful TCP startup in `server/CVCMIServer.cpp`. No discovery creation for internal-only sessions. Global-lobby login still explicitly calls `startAcceptingIncomingConnections(true)` and retains discovery then. No change to simulation, commands, AI, save/load or threading architecture. No other owner files/notes present at initial inspection.

### W5 focused verification request

Check constructor has no discovery startup; `prepare(false,false)` creates only the socket-free NetworkServer holder; explicit listening alone starts TCP + discovery; internal start/load/restart/shutdown never creates discovery. Independently test stale `useProcess=true` selection after W2 fix. Source checks do not establish playable acceptance.

### Build / authorization

No assigned build root communicated to W1 yet; no new root, package installs, GUI/game launches, commits or pushes performed. W6's concurrent CMakePresets change was inspected and preserved; it proposes `build/new-horizons-linux`. W6/integrator should provide build readiness and focused test target. Runtime/graphical acceptance remains pending separate authorization.

### W1 verification / W2 response

Read `docs/NH_FRONTEND_HANDOFF.md` once it appeared. Agree exact file boundaries and unchanged runner interface; W2's thread-selection and debug escape fixes complement this patch. No W1 edits to runner/header were needed for the discovery fix.

Five inline Python unittest source checks passed: constructor discovery regression (also confirmed HEAD contains the defect), discovery guarded by explicit listening and sequenced after TCP start, socket-free internal holder and discovery-null state transitions, unchanged internal runner connection/simulation loop, and unchanged authoritative packet dispatch. `git diff --check` passed. These are source checks, not compiled or runtime tests; W5 should supply durable independent negative coverage.

Initial failure review found that preparation exceptions terminated the process. The following implementation supersedes that deferred proposal; full game runtime verification remains outstanding.

### W1 readiness/lifetime implementation — Frontend catch contract

`IServerRunner` API is unchanged. `ServerThreadRunner::start` now owns its readiness promise inside the worker. Exceptions from thread naming or `prepare` are captured, the failed thread is joined, the partial server destroyed, and the original exception rethrown synchronously from `start`. Constructor/thread-creation failures also propagate synchronously, without a live worker. Successful return still means preparation is complete, not that the client connection callback has run. No fallback to process/TCP is introduced.

**Frontend action:** catch `std::exception` around local runner startup, reset the runner and report through existing failure UI; do not call `connectToServer` after failure. The runner can safely be reset, shut down or waited after a failed start. Unknown exceptions are also preserved (not converted into arbitrary messages). Do not retry a failed preparation automatically or wait for a connection callback which was never scheduled.

`wait` is safe before startup and on repeated calls. Destruction stops and joins any remaining worker. Starting an already joinable runner is rejected with `std::logic_error`, without replacing its server. Lifecycle calls must remain serialized on the owning client thread; these changes do not promise concurrent start/reset safety. Normal successful-session packet-based disconnect remains unchanged.

`shutdown` now calls new `CVCMIServer::stop`, which delegates to the existing thread-safe Asio event-loop stop, rather than racing the simulation by writing `state`/destroying discovery from the GUI thread. Cancellation before the loop enters `run` is retained by Asio's stopped state. After the loop exits, `CVCMIServer::run` finalizes SHUTDOWN on the simulation thread, preserving final state and discovery cleanup without a GUI-side state race. `wait` still waits for a currently executing callback to finish; frontend must retain its existing interface-mutex release around joins. A queued connection-established callback after cancellation is a frontend-owned state check, not a reason to change internal transport here. Exceptions during gameplay `run` are outside the preparation promise and remain existing behavior.

### W6 compile coordination

The active build owns compilation; W1 will not start a competing CMake/Ninja build. Please ensure changed `client/ServerRunner.cpp` and `server/CVCMIServer.cpp` are recompiled (and header dependents rebuilt) before integration. Added `server/tests/test_server_runner.py`. Four default source checks passed via `python3 server/tests/test_server_runner.py`; `git diff --check` passed. The build owner should run `python3 server/tests/test_server_runner.py --build-dir build/new-horizons-linux` after/between native compile work. This compiles the actual runner implementation/header against fake collaborators with GCC C++20, warnings-as-errors, then runs with a timeout: construction/prepare exception preservation, cleanup after failure, reuse, duplicate-start rejection, repeated shutdown/wait, 100 early cancellations, internal connection selection, and destructor joining. It writes only one test executable in the existing assigned build root. Build owner subsequently ran the harness: `build/new-horizons-linux/integration-runner-test.log` records all four source checks and production-runner/fake-server lifecycle tests passing. W1 independently read that result; no harness-revealed runtime defect requires a patch. It is not a substitute for real-server/Asio or graphical acceptance.

### To NewHorizons:Frontend — independent cancellation review

Reviewed the current two-file frontend diff against the runner implementation. No overlapping edits made.

**F1 (high): cancel then immediate restart can accept a stale connection or race a join.** `CSimpleJoinScreen::leaveScreen` sets CONNECTION_CANCELLED then immediately `close()` exposes the menu. Before the queued old `onConnectionEstablished` takes the interface mutex, a new menu action can call `resetStateForLobby` and create a new runner, setting CONNECTING again. The old callback now passes the CONNECTING assertion and installs the old connection as the new session. Alternatively, the old callback observes CANCELLED and enters `waitForServerShutdown`, which releases the interface mutex around `serverRunner->wait()`. A new menu action can replace/destroy that same runner while its join is in progress, causing concurrent join/lifetime misuse; the callback may subsequently reset the NEW runner. Idempotent sequential `wait()` is not concurrent-join protection. Keep setup/restart unavailable until cancellation cleanup completes, and/or give callback cleanup stable session identity and runner ownership. Do not rely solely on the global client state check after a new session can start.

**F2 (medium): cancellation after connection-established but before lobby entry need not run cleanup.** Once `onConnectionEstablished` has run, no further connection-established callback is pending. `leaveScreen` stops the simulation loop and closes the window, but internal `stop()` and server destruction do not generate client `onDisconnected`; `InternalConnection` has no disconnecting destructor. Internal success also schedules no retry timer. Therefore neither newly added CANCELLED callback branch is guaranteed to join/reset the cancelled runner or clear the old connection before the menu is usable. Ensure the cancel action itself arranges deterministic cleanup, including the already-established case, rather than relying exclusively on a future connection/disconnection event. This reinforces F1's gate requirement. Existing stop semantics are cancellation, not a transport disconnect notification.

**Other reviewed cases:** preparation occurs synchronously during progress-window construction, so normal GUI Cancel cannot run before `start` reports readiness. A thrown preparation failure has already joined/reset on the runner side; frontend catch/reset/NONE/rethrow followed by `openLocalGameSetup`'s std::exception dialog is compatible. Constructor/thread-creation failures also have no live worker. Sequential shutdown/wait/reset/destructor repetition is safe. No process/TCP fallback was introduced. Unknown non-std exceptions intentionally remain rethrown rather than user-message-converted.
