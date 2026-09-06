# New Horizons Linux build handoff

## Current checkpoint: six-school native gate passed; reviewed integration next

Actual first six-school build `magic-first-build-20260906T204536Z` exited 0.
Its baseline 103 and curated 8 exposed the predicted accepted-command bonus expiry
and excessive-NH legacy-header failures. Runtime's scoped fixes and preservation
controls rebuilt successfully (`magic-fixes-build-20260906T212026Z`, exit 0), then
passed 109 baseline / 20 curated cases apart from their documented skips.

Source review additionally caught the old-Tome AI affinity mismatch. Actual four
Tome tests in each profile were RED: legacy unknown/known scores 0/20000, curated
20000/20000. The school factor's caller subtracts it from one, so the defect was
maximal valuation in the new profile, not zero valuation. The two-condition fix
unions saved and original affinity and counts genuinely known school spells;
no level-factor or global spell-definition changes were made. Both 4/4 reruns
passed. Final assembled gates `magic-final-baseline.*` and
`magic-final-curated.*` are **113 cases: 112 passed/one expected export skip**, and
**24 cases: 23 passed/one context skip**, respectively, both exit 0. The required-NH
negative test exercised one baseline configuration; do not claim both missing
and disabled statuses were independently recorded. Native evidence includes real
installed Havoc/Implosion AI selection, legal server casting/cost/budget, skill
conversion, old-world exclusions, game/BattleStart persistence and turn controls.
Six-school graphical acceptance and the remaining command GUI checks are pending.

Local Windows progress is now execution-backed: shared PlutoVG fixed SDL_ttf
without removing SVG support; `shared-plutovg-20260906T211122Z` dependency install
exited 0. Cross configuration exposed oneTBB metadata naming a nonexistent `tbb`
alongside real `libtbb12.dll.a`. A consumer-only metadata adjustment, without
changing cached binaries, produced generate-with-build-never exit 0 and
`configure-tbb-fixed.exit` 0. No Windows client compilation or execution is claimed.

Windows82 notice repair `593e40b7f84b982e4e2ccf6833fc304b2a17b205` was committed
and pushed separately. Independent inspection expanded omissions to dav1d,
PlutoVG and Brotli. The original immutable 111081420-byte Conan cache was recovered
with its original SHA256, exact parent identities and six byte-identical runtime
DLLs; its full static requirements identify the three exact source revisions.
The closure is 27 dependencies. Exact recipe source recovery exited 0; the overlay
preserves all 111782 original source entries and adds 590 entries for those three
leaf sources, plus FFmpeg's full LGPL notice. Twenty-six Python packaging tests
passed. Actual local repack exited 0 under `windows82-local-repacked-593e40b7f`:
ZIP SHA256 `5c41caa19ed75df8d1f572fea575d5027ceb61e58376cfc1aaaa308fe5792644`.
All original protected payload bytes and the original compiled fork source archive
are unchanged; packaging execution is explicitly local. Independent final archive
acceptance subsequently passed at notice/source-repair scope: 763 ZIP entries,
725 protected hashes, 26 PE files, 683 resources, exact original source entries,
529 newly recovered upstream source files, all 27 dependency identities and
committed packaging source blobs were checked (`windows-audit-repack593`). The
draft remains unpublished; this is not a new-feature Windows executable or a
Windows GUI pass. The extra packaging source is an exact committed root snapshot; compiled
sources remain the separate original full source companion.

Priority checkpoint: freeze the bounded 113/24 native foundation and start the
actual local Windows feature client compile before expanding native test scope.
The exact invocation is `tools/ci/build_mingw_client.sh build`; capture its log,
exit and resulting path under `build/new-horizons-windows-cross`. Registered
sources remain held during this serialized build; no GUI lease is active.
After its first build checkpoint, resume the Linux committed-identity rebuild,
immutable candidate and short Tester lease.

New independent source review found map-authored legacy-school secondary rewards
and limiters can still grant/check obsolete IDs in a six-school world, with
possible misleading feedback. Four reward proofs and two feedback proofs are
unregistered and unexecuted; they are required follow-up, not a claimed accepted
six-school journey. A separate source-only test targets the pre-existing
SPELLS_OF_LEVEL AI known-weight inversion. Do not silently count these tests as
green or defer the requested first Windows feature compile indefinitely.
Primary-profile primitives also remain unregistered source-only future work,
not part of this native result. Full new spell effects, growth/secondary attributes,
masteries, tiers and final Linux/Windows packages remain open. Older checkpoints
below are historical context, not superseding readiness claims.

## Repaired command GUI gate and six-school source assembly

Repair `66ddb01bd98ecd2c0e748b7bebb26f46ec7d55ad` was committed and pushed.
`commands-preview-54213f042-repair-66ddb01bd` preserves both 542 binaries and all
prior payload bytes except the launcher/schema, with explicit base/repair hashes.
Tester verified the hashes and exercised seven human rounds, all five commands,
Bloodlust/shared budget, cancel, expiry, persistent Doctrine and movement; real
bookless AI issued Aggressive and continued army actions. Three supervised normal
process exits were exactly 0, with full-process prebattle and post-retreat reloads.
No defect was observed in that slice. New-battle reset and the strong-spell AI
journey remain pending, not implied passes. A second ten-minute quiet lease was
given at 20:32:37Z for these remaining checks; no compiler/native/cross execution
until Tester releases it.

Outside both immutable candidates, Build has authored the next family:
`config/newHorizons{Magic,Schools,Skills}.json`, magic schema/default setting,
generated inline module v0.2.0 data and CMake equality/registration updates.
There are six real school definitions and six Basic/Advanced/Expert school skills
with the 72 original rank/size images supplied by Frontend. The saved mapping
covers exactly 69 existing common hero spells, excluding Titan's Bolt and creature
abilities. It includes explicit provisional faction conflicts, dual Shadow/Chaos
Blind, optional tier/cost changes, and new-game skill replacements. See the curated
module README for non-final choices and the still-unimplemented spell roster.
`tools/tests/test_new_horizons_content.py` passed six offline tests with thirteen
negative controls (`magic-content-offline.log/.exit`, exit 0). These checks are
not native loading, six-school casting, AI or rendered acceptance. Runtime's
school serialization, save-only compatibility and native tests remain in progress;
Frontend's callback-driven spellbook is source-ready. No newer-family C++ has been
compiled or attributed to the repaired 542 candidate. Eligibility/Clone tests are
now registered for the next native batch, not retrospectively counted among 95.

Runtime corrected an integration concern: although mod verification records a
version mismatch, the ordinary save-list caller ignores that status; do not infer
a load block from the comparator alone. An excessive active NH mod in a legacy
save **does** throw and needs a narrowly scoped save compatibility proof/fix.

Next compiler lane after the remaining GUI lease: repair the existing MinGW shared
PlutoVG dependency route (preserve its old install evidence), or compile the Linux
six-school batch once Runtime declares it ready; never run both concurrently.
Windows delivery, the full spell/mastery/growth/tier scope and final packages remain
open.

## Command activation repair after actual GUI failure

Command milestone `54213f0425500208fe259a6255914f05ad71d663` was reviewed,
committed and pushed through the existing SSH origin. Its committed-identity
rebuild exited 0; `commands-54213f042-native.log/.xml/.exit` records 95 cases,
94 passes and one expected opt-in skip, exit 0. This is not full redesign acceptance.

Immutable local diagnostic candidate `commands-preview-54213f042` contains copied
config/scripts/curated modules, launcher, `BUILD-IDENTITY.json` and `SHA256SUMS`.
Client SHA256 `ddae434a0c83b8aeb2cc0ec02ffab2132b6264e2be58a487f747c3b9af99172a`;
library `51bbf0465d769d92d297da701126b5541177564cc5f1f9da086fefea88e45016`.
Tester verified all hashes, used a fresh guarded private profile, reached a real
hero-versus-hero battle, and found the ordinary spellbook instead of the command
chooser. Actual preset/log evidence proves **new-horizons was mounted but inactive**:
fresh default preset contained only vcmi/core. The failed-run save has legacy rules
and must not be relabeled or reused as the new-rules retest. Its starting bonuses
were actually Random, not Gold; Tester corrected the earlier click-count inference.
No commands/spells were exercised. Normal quit returned exactly 0; the GUI lease
was explicitly released. Failed profile, logs and images remain private evidence.

Build's repair writes an atomic fixed managed mod preset after acquiring the lock:
vcmi/core/new-horizons for complete curated resources, vcmi/core for legacy previews.
Other settings and saves remain untouched; verify-only remains read-only. A shell
stub regression first failed (exit 1), then passed. An independently compiled,
non-GUI bootstrap probe linked to the unchanged frozen library uses the **ordinary**
preset, not the test preset: old launcher exits 2 for missing activation; corrected
launcher initializes all five command rules. The actual native schema validator
also exposed the core-scope required-field exemption: empty legacy rules matched
both oneOf alternatives. Minimum property counts now distinguish full rules and
validate required nested shapes. Old schema probe exits 4; corrected named-schema
checks accept core empty/full, reject a missing coefficient, and exit 0. Evidence:
`activation-native-launcher-red.*`, `activation-native-schema-red.*`,
`activation-native-final-green.*` under the Linux build root. The probe's initial
inline-schema overload attempt crashed on local references; the corrected probe
uses the same named-schema path as production. No runtime fix is claimed for that
separate diagnostic API behavior.

Next: commit only launcher/test/schema/handoff repair, freeze a **new** candidate
with unchanged 542 binaries and explicitly separate repair identity, then obtain
fresh Tester activation/command/AI/save gates. Do not compile or attribute the
shared in-progress six-school C++ to this repair. Runtime/Frontend own the saved
school APIs/UI; Build owns canonical school registration and complete existing
spell mapping/schema, followed by the rest of the full design and local Windows
cross-dependency/package repair. Windows publication remains blocked; no cloud
rebuild loop or corrected-package claim has been made.

## Post-reboot local integration resumed

The user returned and lifted the pause. Build again owns the sole local compiler,
review/staging/commit lane; no cloud workflows or API retries are needed. Current
base is `98bd74f52` plus preserved shared command/UI/art changes, not a clean
feature candidate. Repository privacy/default-branch changes were user actions;
origin SSH is the available integration route.

Runtime supplied concrete serialization headers in `HeroCommandTest.cpp`, retaining
full old/current game-state roundtrips and all assertions. At 2026-09-06 18:49:10Z,
started `cmake --build build/new-horizons-linux --target vcmiclient vcmitest
--parallel 2`; log `commands-resume-20260906T184910Z.log`, completion status will
be in the adjacent `.exit` file. Tester confirmed no GUI lease or competing build.
That build exited **0**. The first real command run exited 1 (17/19 passed):
named settings lacked test mod scope; full-state persistence failed. The baseline
also exited 1 (63 passed, one opt-in export skip, three garrison failures).

Build found the production persistence cause: `HERO_COMMANDS` was appended after
`MINIMAL = RELEASE_170`, implicitly setting CURRENT to old value 894. Runtime moved
it before the release aliases and added a monotonicity assertion; no test weakened.
The corrected dependent rebuild `commands-resume-20260906T185734Z.log/.exit`
exited **0**. Combined `commands-version-fixed.log/.xml/.exit` reports **86 passed,
one expected skip, one failure out of 88**: only the strong-offensive-spell AI case
still chooses a command instead. All 19 command/persistence/settings cases and all
66 baseline regressions now pass, plus the bookless AI command/authority case.
The failed fixture attempted power 1000 despite the core cap of 99: Magic Arrow
did not dominate the command value for 100 Angels. Runtime replaced that assumption
with an Implosion fixture asserting actual power 99, legal casting and substantial
nonlethal damage; production AI and its spell-selection assertion were unchanged.

Build `commands-resume-20260906T191510Z.log/.exit` exited **0**, including the
chooser/font and custom-school tab layout changes and four new persistence tests.
`commands-integration-resume.log/.xml/.exit` then exited **0**: **91 passes and one
expected export skip across 92 tests**. Both actual BattleEvaluator choice/server
validation cases passed; full BattleStart replica continuation and recipient rules
passed. This is a native gate, not GUI acceptance or the full redesign.

Final recipient-help text and the two authored hero-versus-hero exporters compiled
successfully (`commands-resume-20260906T192403Z.log/.exit`). Actual exporter run
`commands-fixture-export.log/.xml/.exit` passed 2/2, including parser, real-init,
CRC/EOF and byte equality assertions. Copies and independently audited hashes are
under `testing/commands-assets/Maps` and `testing/commands-fixture-manifest.json`;
external Data/Mp3 are readonly input links, never shipped.

A further rejection regression was proved RED: `commands-rejection-red.log/.xml`
shows rejected Advance reactivated the stack (3 activations versus 2), expiring a
STACK_GETS_TURN bonus (speed 10 became 5). Runtime's minimal BattleProcessor fix
skips post-action flow for rejected HERO_COMMAND only; failed unit/spell recovery
is deliberately preserved because their UI deactivates before submission.
`commands-rejection-green-build-20260906T193528Z.log/.exit` exited **0** and the
combined `commands-rejection-green.log/.xml/.exit` exited **0**: **94 passes, one
expected skip, 95 cases**, including the unchanged formerly-red assertion and both
real fixture exports. No generic failed-action recovery rewrite was made.

Proceed to reviewed native milestone integration, commit-identified rebuild and
immutable candidate freeze. Tester graphical acceptance remains pending. Six
schools/effects, growth, masteries/hero UI and tiers remain full-scope work, not
completed by this first native command gate.

Build corrected `Mods/new-horizons/mod.json` filesystem path to `/Images`:
`CFilesystemGenerator` concatenates the mod prefix without inserting a slash.
The prior `Images` value addressed `MODS/NEW-HORIZONSImages`, not the art directory.
Native resource/startup checks and rendered acceptance remain required.

Also fixed managed launcher curation to mount only `vcmi` plus the complete
`new-horizons` module for new candidates; old resource snapshots remain supported.
Incomplete curated payloads fail closed. Synthetic launcher tests exited 0 in
`commands-launcher-resume.log/.exit`, including legacy/new launches, omission
rejections, unwanted-mod exclusion and unchanged lock/profile safeguards.

Named module settings cannot read an unmounted core file through their own scoped
filesystem. `tools/update-new-horizons-module.py` now generates inline mod settings
from canonical `config/newHorizonsCombat.json`; `--check` passed. Root CMake checks
JSON equality and tracks both inputs. Actual CMake positive and altered-rules
negative checks passed using ignored `commands-module-check.cmake`. These are
registration safeguards, not rendered or gameplay acceptance.

Next: read the completed build exit, run focused HeroCommand and prior regressions
in private XDG directories, incorporate Frontend's bounded feedback fix, then freeze
binary/content/source hashes for the sole Tester. Only afterward resume the existing
MinGW SDL_ttf failure. The architectural experiment remains closed.

Local cross-build diagnosis (no cross compilation yet): `install.log` ends at
SDL_ttf with unresolved `__imp_plutovg_*` references from static PlutoSVG. The pinned
PlutoVG recipe only adds `PLUTOVG_BUILD_STATIC` for MSVC, while its Windows header
also requires it for MinGW static consumers. The owned MinGW profile now selects
PlutoVG's supported shared build, retaining SVG/font capability rather than
removing it. This proposed repair is **not verified by a dependency build yet**;
run it only after the Linux candidate/Tester compiler lease permits.

## User-requested reboot pause — resume mod integration after return

User says the worker allowance has been reset, but explicitly requests waiting
for a computer restart. No further implementation/build/GUI until user returns.
Dirty feature/artwork changes are preserved, not committed as a tested milestone.

Packaging repair `98bd74f52` is pushed; Windows notice-only repack of original
compiled run `34005089136` was dispatched as `34050542538`. Check its actual
result after restart; do not infer success or restart a full compile unnecessarily.

Dispatcher resumed Orders/Doctrine integration, added HeroCommandTest.cpp and its
fixture to test/CMakeLists.txt, fixed missing JsonNode forward declaration in
IGameInfoCallback.h and missing gui/Shortcut.h include in BattleHeroActionWindow.cpp.
The subsequent real build compiled the new runtime/AI/client work but failed while
instantiating HeroCommandTest.cpp serialization: incomplete bonus IUpdater and
related types. Full log `build/new-horizons-linux/commands-build-fix2.log`; first
errors, not just trailing template diagnostics, determine the next fixes. No local
cmake/ninja/Conan build remained running at the pause. Next: finish test includes/
compile errors, rebuild vcmiclient+vcmitest, execute focused HeroCommand tests;
then review ruleset activation/assets and perform Tester-owned normal-input UI/AI
journey. No graphical claim for the new command system yet.

This chat's saved Pi session is the historical Dispatcher session ending
`01a0406f-8484-719c-bd35-92bfb7346dbc`. tmux processes do not survive a reboot;
resume that saved conversation first, then restore NewHorizons workers by their
saved sessions rather than creating replacement histories.

## Dispatcher takeover — exact md4c export-source repair

The build worker exhausted its provider allowance while this repair was dirty.
Dispatcher reviewed the existing two-file fix and takes scoped integration for
this checkpoint; unrelated Orders/Doctrine/AI/artwork and MinGW changes remain
untouched. Do not infer worker progress from their open panes while quota-limited.

Failure: Windows run `34040567531` could fetch md4c 0.5.2 upstream source, but
restored Conan cache lacked its exported `honor-vc-runtime` patch. The fix checks
exported-source files against the exact recipe manifest and, if incomplete,
downloads only that same pinned recipe revision into a fresh temporary cache.
It does not replace dependency versions, mutate the binary cache, skip patching,
or bypass corresponding-source/license requirements.

Validation: 10 dependency-notice tests, 6 system-provider tests and 3 PE audit
tests passed. Real Conan proof used exact CI revision
`md4c/0.5.2#3d7106721e458f9f799b87d4d50d02e0`; only the first exported-cache
lookup was redirected to an empty directory to reproduce missing exports. Actual
recipe download, source download, patch application, upstream notice collection
and archive retention then succeeded. Evidence is ignored output under
`build/new-horizons-linux/md4c-export-proof/`. This Linux proof is not a Windows
workflow pass. Next: push the scoped repair and run Windows notice-only repack;
continue the authorized Orders/Doctrines implementation without waiting on cloud CI.

## Selective-autocombat Stage A: policy only, not a UI feature

Added default-true category preferences and a pure `controlsUnit(Unit, Mode)`
predicate. FULL_BATTLE always delegates; towers explicitly retain prior automatic
behavior; SELECTIVE consults the creature/catapult/ballista/tent flag. No skill or
server eligibility checks, client/AI callers, settings or UI wiring were added.
Spells/Tactics defaults remain unchanged. This does not implement user-visible
selective autocombat or its asynchronous spell/manual handoff.

Regression-first: initial build failed on a nonexistent test include, corrected
to existing `CCreatureHandler.h`. Successful retry compiled the unconditional-true
hook. `autocombat-stageA-red.log/xml` then recorded exactly four exclusion failures
and four passing default/cross-category/full-battle/tower controls. Only after that
red result was the predicate authorized. `autocombat-stageA-green-build.log` exits
0; combined `autocombat-stageA-green.log/xml` reports **66 passes and one expected
opt-in export skip**, including all eight policy tests. Lifecycle and launcher
checks also exit 0; no game launched for this internal policy increment.

Separate First Aid Tent characterization adds six cases to the existing real-flow
fixture: wounded target ranks 0–3 (automatic heal versus manual TURN_QUEUE), plus
healthy/no-target ranks 0/1 (forced automatic NO_ACTION). Uses an ordinary injury
packet, real randomizer/seed 1337, and asserts target eligibility and exact action.
Tent/ballista/FireShield/Enchanted tests independently passed 32/32 while policy was
still red (`autocombat-tent-green.log/xml`). Server production rules and SDL
client dispatch remain unchanged; these tests do not establish GUI routing.

## Selective-autocombat prerequisite: ballista server routing

Test-only increment, no product/client/server-rule changes. Existing
`RecordingGameServer` now records `BattleSetActiveStack` and `StartAction` before
application. New `WarMachineControlTest.cpp` follows real battle setup and bounded
ordinary Defend actions, with the existing seed 1337 and no private flow calls.

`ArtilleryRanks/WarMachineControlTest.BallistaArtilleryControlsAuthoritativeTurnRouting/*`
passes all four ranks: absent Artillery yields authoritative AUTOMATIC_ACTION and
one SHOOT; Basic/Advanced/Expert yield TURN_QUEUE, no automatic machine action,
and the ballista remains active for client input. The live target/can-shoot
preconditions are asserted. No preference grants skill eligibility.

Build log `autocombat-ballista-build.log`: exit 0. Ballista plus existing FireShield
and Enchanted sibling tests: 26/26 passed (`autocombat-ballista-tests.log/xml`).
Combined save/map/garrison baseline: 52 passed, one expected opt-in export skip
(`autocombat-ballista-baseline.log/xml`), exit 0. These native fixtures do not link
SDL client dispatch and do not prove absence of duplicated client commands.
Catapult/tent routing and new selective-autocombat behavior are not covered by this
increment; frontend lifecycle/API implementation remains unapproved at this point.

## Focused synthetic town-fixture export

Added one opt-in existing GoogleTest case, no new framework or product changes:
`NH_EXPORT_TOWN_GARRISON_FIXTURES=1` with filter
`TinyH3MBuilderTest.ExportNeutralTownGarrisonFixtures`. Default runs skip export.
The existing builder writes three fresh SOD maps only after parser and real-init
validation; tests reread actual gzip files through EOF, check zlib/close status,
and compare disk payloads with prevalidated bytes. Seed 0 is a native control,
not a guarantee of the GUI's unspecified-garrison roll.

First enabled-export attempt failed before writing: a post-init exact-four object
count ignored unused-hero registry reservations. Replaced it with authored-object
ID/type/subtype/position/owner checks, keeping exact-four parser assertions.
`gap1-export-build-retry.log` exits 0; `gap1-export-green.log/xml` reports **27/27
passed**, including export. The prior default run reports 26 passes/one opt-in skip.

Build independently decompressed each actual gzip through CRC/EOF, verified
SOD/36x36/one-level/name headers, hashed compressed/raw bytes and copied exactly
three generated fixtures to `testing/gap1-assets/Maps` under the assigned root.
Data/Mp3 there are links to external purchaser inputs; no original Maps are exposed
or changed. Separate diagnostic profile: `testing/gap1-profile`. Unmodified
launcher `--verify-only` exited 0 without creating that profile or launching.

Local `testing/gap1-fixture-manifest.json` records all hashes/provenance. Primary
`NHGap1ExplicitEmptySOD.h3m`: gzip SHA-256
`0293f64bbc68baee87ee9c4a1cbe6474888815aee0ee6147385445ac9d260af6`,
raw SHA-256 `95eddf9f634e89ea89919abbe930aa011f80bcfee2bde4c9bf8ff99b348c273c`.
Other maps: `NHGap1CustomSOD` (17 pikemen) and `NHGap1UnspecifiedSOD`.
All use red Castle (8,10), hero 0 (17,10), neutral target (20,10), blue Castle
(30,30). Sole Tester subsequently verified the primary explicit-empty target:
day-one inspection, pre-capture save/restart/reload, direct capture without battle,
and post-capture save/load preserving ownership and army. PIDs 731666/731818 quit
normally by 19:55:18Z; binary and all three fixture hashes stayed unchanged.
A subsequent bounded run (PID 732152, normal exit 20:01:58Z) passed post-capture
one-turn continuation: popup +1000, gold 20000→21000, two owned towns retained.
The custom fixture's ordinary approach entered a siege with exactly 17 defending
Pikemen. Battle/scenario completion and unspecified GUI control were not exercised;
no claim of those passes. These synthetic fixtures are diagnostic, not shipped original
content; no generated maps/manifests/profiles/assets belong in Git.

## Post-MVP explicit-empty town garrison regression

After the completed ordinary journey in `NH_TESTER_RESULTS.md`, added an
independently reviewed, original-address-corroborated fix for lost explicit-empty
H3M town armies. No Reconstruction implementation was imported.

Regression-first evidence in the assigned root:

- `gap1-red-build-retry.log`: build exit 0 after correcting test private-member
  access. `gap1-red-tests.log/xml`: exit 1, three parser cases passed and all three
  real-init cases (ROE/AB/SOD) failed **only** because explicit-empty neutral towns
  gained two guard stacks; deterministic positive-control seed 0.
- `gap1-green-build.log`: initial compile failure in new persistence tests
  (ambiguous JSON entry point and missing concrete serializer types), not a
  behavioral failure. Runtime corrected test qualification/includes only.
- `gap1-green-build-retry.log`: final client and test links, exit 0.
- `gap1-green-tests.log/xml`: **26/26 passed**, including 12 parameterized parser,
  real-init, JSON-object and binary-object persistence cases, plus the existing
  14 save-path/map/skill-serialization checks.
- `gap1-lifecycle.log`, `gap1-launcher.log`: lifecycle and launcher checks exit 0.

Production scope is exactly H3M loader, town header/implementation and serializer
feature enum. `customInitialGarrison` preserves authored presence independently
of current stacks. It bypasses initial random guards only; owner guard and weekly
rules remain unchanged. Town JSON writes an explicit true key even if empty army
is omitted; old/missing key retains legacy false. Binary feature advances CURRENT
without raising MINIMAL, with false on old reads and no mutation on old writes.

Native object roundtrips do not prove full saved-game or zipped-map integration.
Tester subsequently passed the retained pre-feature MVP save → continue → new
save → normal quit/restart/reload route on `023ffe7da`, preserving the old named
save unchanged; exact identity/limits are in `NH_TESTER_RESULTS.md`. This does not
cover every historical save version. Focused synthetic explicit-empty capture
and pre/post-capture save/load subsequently passed on frozen `9bd41073b`; see
Tester results and fixture provenance above. Subsequent populated GUI battle-entry
control and post-capture turn/income checks passed; see the bounded Tester evidence.
AI/core resources remain enabled; no package installation or Build-owned GUI run.

## Native-test checkpoint after run1 release

Tester explicitly released the client/profile at 18:11:38Z on 2026-09-05;
PID 722537 was absent before configuration. No live binary was overwritten.
Enabled existing `vcmitest` in the assigned root using installed sources:

```sh
cmake --preset new-horizons-linux -DENABLE_TEST=ON \
  -DVCMI_GOOGLETEST_SOURCE_DIR=/usr/src/googletest
cmake --build build/new-horizons-linux --target vcmitest vcmiclient --parallel 2
```

Both commands exited zero; final log includes both executable links.
`test/CMakeLists.txt` now permits a local GoogleTest source path, retaining the
bundled submodule default; no downloads, installations or extra build root.

Native filter (run from build `bin`, with private XDG data/config/cache below
`testing/native`):

```text
SavegamePathTest.*:TinyH3MBuilderTest.*:HeroSecondarySkillsTest.allEightSkillsAreSerializedIntoMap
```

Initial attempt exited 1 during global setup: missing DATA/LCDESC. This was missing
original-data mounting, not a product regression. A build-local `bin/Data` symlink
to purchaser-supplied external Data enabled the existing read-only resource loader;
no original files copied or modified, no profile reuse. Retest **14/14 passed**:
four save-path policy tests, nine synthetic H3M load tests, one map skill
serialization test. These do not prove authoritative savegame reload/seven turns.

`python3 server/tests/test_server_runner.py --build-dir build/new-horizons-linux`
also exited zero: four source checks plus actual-runner/fake-server lifecycle
compilation/execution. Ordinary AI and core/vcmi resources retained. No game launch
by Build. Tester owns same-save reload/continued-play/scenario-outcome acceptance.

Local evidence: `native-configure.log`, `native-build.log`, `native-build.exit`,
`native-tests.log` (initial failure), `native-tests-assets.log`,
`native-tests-assets.exit`, and `native-lifecycle.log`, all below the assigned root.
Earlier reports below are historical, not the current checkpoint status.

## Integrator correction: combined build and focused tests PASS

The failed follow-through below was fixed by exposing the existing read-only
`CServerHandler::isServerLocal()` query to the Cancel UI. No simulation mutation
or new transport path was added. The integrator prematurely pushed checkpoint
`55654be98` before reading that failed build result; it is not a tested candidate.
This correction preserves that failure record rather than relabeling it.

Verified after the header correction:
- `cmake --build --preset new-horizons-linux`: exit 0, 46 build steps ending in
  client relink; log `build/new-horizons-linux/integrator-build.log`.
- `python3 server/tests/test_server_runner.py --build-dir build/new-horizons-linux`:
  exit 0, four source checks and compiled production-runner/fake-server harness.
- `bash tools/tests/new-horizons-launch-test.sh`: exit 0, synthetic stub only.
- `git diff --check`: exit 0.

Rebuilt client SHA-256:
`d364b0314bdf3a38f2b7f659108c8acac27bc733b8e7163659fa18de69085d6b`.
No game launched. Graphical gameplay and actual process/socket acceptance remain
pending explicit bounded execution authorization.

## Latest follow-through: updated Frontend build FAILED

This result supersedes the successful earlier combined build below. After reading
the Frontend cancellation/identity follow-up and `tools/README.new-horizons.md`,
removed only both frontend generated objects and ran:

| Command | Exit / result |
| --- | --- |
| `cmake --build --preset new-horizons-linux` | **1**: CServerHandler.cpp compiled; CMainMenu.cpp failed; no relink |
| `python3 server/tests/test_server_runner.py --build-dir build/new-horizons-linux` | **0**: four source checks plus compiled lifecycle harness passed |
| `bash -n tools/new-horizons-launch.sh tools/tests/new-horizons-launch-test.sh` | **0** |
| `bash tools/tests/new-horizons-launch-test.sh` | **0**: synthetic stub tests passed; no game executed |

Exact compiler failure requiring Frontend owner action:

```text
client/mainmenu/CMainMenu.cpp:827:56: error:
‘bool CServerHandler::isServerLocal() const’ is private within this context
client/CServerHandler.h:141:14: note: declared private here
```

Reported promptly in the build-owner response; no competing product edit made.
The existing executable is **stale relative to these Frontend fixes**, not a final
tested candidate. Its SHA-256 remains
`14265af63977baaaf3230a2b28bc5acc5a7ee78d070554299a207acc685640ca`.

HEAD before/after: `965c5027324ed7c286cd2e43130f0a49d35fbc71`.
Full tracked binary git diff before/after matched byte-for-byte; SHA-256:
`e658ebc1148722b88898d26ecabd3b978a8e8602b4570d075c4bd1fc4c460379`.
Explicit source manifests also matched before/after (including untracked harness
and launcher files). Key exact source SHA-256 values:

```text
3d1360effde44b0f5214bf0d482e4f0371d746fcb6351e1b26e07ab7895db2ab  client/CServerHandler.cpp
ddf4b1db34b37f76783ef4c204779d55f136256b6400d36b480297011450100f  client/mainmenu/CMainMenu.cpp
cf694fb6fcaf4ab86efab1be9d9ae7f4756ea96cb3d69924f2fc019cfd8fcd4e  server/tests/test_server_runner.py
17e746f05ffbea8ea429df528a465a003aed7ff48e5f51d7a793f85987c4876d  tools/new-horizons-launch.sh
9d3ec387cdf57192614be069aba9653d22bc7c5324a79e7f7fd5b6bce5b6789b  tools/tests/new-horizons-launch-test.sh
```

Compiled and executed harness SHA-256:
`8bc55d4558b9d548d299b123777878e500837737bc9d2e1e8c40844ce95dddc8`.
All detailed evidence remains under `build/new-horizons-linux/`:
`final-frontend-build.log`, `final-runner-test.log`, `final-launcher-syntax.log`,
`final-launcher-test.log`, `final-test-results.txt`, `final-artifact-hashes.txt`,
`final-sources-{before,after}.sha256`, `final-working-tree-{before,after}.diff`,
and `final-head-{before,after}.txt`. No GUI/game, install, or commit performed;
shared source dirt preserved. Rebuild after the owner fixes the access violation.

## Earlier combined Runtime / Frontend integration verification

Read the completed `NH_RUNTIME_HANDOFF.md` and `NH_FRONTEND_HANDOFF.md`, then
reconfigured and rebuilt the combined shared tree in the same assigned root.
The incremental build was already current. To explicitly verify compilation of
the final patches, removed only the four generated object files for
`CServerHandler.cpp`, `CMainMenu.cpp`, `ServerRunner.cpp`, and `CVCMIServer.cpp`,
then rebuilt successfully: all four translation units compiled, both static
archives were rebuilt, and `vcmiclient` relinked. No source files were touched.

Executed the authorized non-GUI harness:

```sh
python3 server/tests/test_server_runner.py --build-dir build/new-horizons-linux
```

**PASS:** all four source-contract checks; GCC C++20 harness compilation with
`-Wall -Wextra -Werror`; production runner/fake-server lifecycle execution.
Coverage includes construction/prepare exception preservation, failed-start
cleanup and reuse, duplicate-start rejection, repeated shutdown/wait, 100 early
cancellations with internal connections, and destructor joining. This harness
uses fake collaborators, not real server/Asio or gameplay integration.

Rechecked cache: client ON; dedicated server, launcher and editor OFF. Generated
client link includes `libvcmiservercommon.a` and `libvcmi.so`; standalone server,
launcher and editor targets are absent. Final binary symbols include
`CVCMIServer::run()`, `CVCMIServer::stop()` and `ServerThreadRunner::start(...)`.
No compilation, harness, or linkage-check failures occurred.

Evidence under `build/new-horizons-linux/`:

- `integration-configure.log`, `integration-build.log`
- `integration-recompile.log` (explicit four-file rebuild and final link)
- `integration-runner-test.log`, `nh-server-runner-test`
- `integration-linkage.log`
- `integration-source-before.sha256`, `integration-source-after.sha256`

The before/after diff hashes for all six Runtime/Frontend product files match;
HEAD remained `965c5027324ed7c286cd2e43130f0a49d35fbc71`. Final binary hashes
match those recorded below. Shared dirt was preserved; `git diff --check` passed.
This supersedes the earlier baseline-only verification, but is still a dirty-tree
integration build, not a committed release identity. No install, game/GUI launch,
commit, or package installation was performed. Real-server lifecycle and graphical
acceptance remain unverified.

## Initial baseline result

Configured and built `vcmiclient` successfully using installed system dependencies.
No package installation, dependency downloads, game/GUI launches, installation,
packaging, commits, or pushes were performed by this worker. No product sources
were edited. Only `CMakePresets.json` and this handoff are owned changes.

Read `AGENTS.md`, `docs/NEW_HORIZONS_MVP.md`, and upstream developer
`Building_Linux.md` and `CMake.md` before work.

## Reproduce

From the repository root:

```sh
cmake --preset new-horizons-linux
cmake --build --preset new-horizons-linux
```

The only build root is `build/new-horizons-linux` (git-ignored). The build preset
limits concurrency to two jobs and builds the client target. Its prospective
install prefix is inside that same root, under `install`; installation was not run.
Local evidence:

- `build/new-horizons-linux/configure.log`
- `build/new-horizons-linux/build.log`
- `build/new-horizons-linux/build-verify.log`
- `build/new-horizons-linux/compile_commands.json`
- `build/new-horizons-linux/bin/vcmiclient`
- `build/new-horizons-linux/bin/libvcmi.so`

Configuration and both completed build/verification commands exited zero. The
first compilation invocation hit the tool's 120-second limit; it was resumed in
the same root with a longer limit and completed. No compiler workaround was needed.

## Configuration scope

The new standalone preset leaves upstream presets and Windows configuration
unchanged. It uses GCC, Ninja, Release, C++20, PCH, SDL2, video, the full core
library, LuaJIT, and ordinary Nullkiller2/BattleAI/StupidAI (EmptyAI is upstream
always-on). Dedicated server, launcher, editor, lobby, translations, innoextract,
Discord, experimental MMAI, tests, and ccache are disabled. The shared `vcmi`
facade remains enabled; config copying remains enabled.

There is no original-content-only CMake switch. This is the engine build baseline
for that edition, not proof of runtime content curation. Internal content loading
and engine resources are untouched. Original asset discovery, deployment, curated
configuration and graphical acceptance remain separate owner/integrator work.
No proprietary assets were copied or inspected for this build.

## Installed dependency inventory

Host: Ubuntu 26.04.1 LTS, Linux 7.0.0-30-generic, x86_64.

| Dependency | Installed/selected version |
| --- | --- |
| CMake | 4.2.3 |
| Ninja | 1.13.2 |
| GCC / G++ | 15.2.0 (`15.2.0-16ubuntu1`) |
| pkg-config | 2.5.1 |
| Boost development libraries | 1.90.0 (`1.90.0-6ubuntu1`) |
| SDL2 | 2.32.10 |
| SDL2_image | 2.8.8 |
| SDL2_mixer | 2.8.1 |
| SDL2_ttf | 2.24.0 |
| zlib / minizip | 1.3.1 / 1.3.1 |
| FFmpeg development libraries | 8.0.1-3ubuntu2 |
| avutil / swscale / avformat | 60.8.100 / 9.1.100 / 62.3.100 |
| avcodec / swresample | 62.11.100 / 6.1.100 |
| TBB | 2022.3.0 |
| LuaJIT | pkg-config 2.1.1761786044; package 2.1.0+openresty20251030-1 |
| libsquish | 1.15 |
| Iconv | built into libc (CMake probe passed) |

Inventory used `command -v`, tool version commands, `pkg-config --modversion`,
`dpkg-query`, and CMake discovery. Required selected dependencies are all present;
there are **no missing dependencies blocking this preset**. SDL3's complete set
was not found, and clang was not on PATH; neither is selected. Plain Lua and fmt
had no pkg-config result; LuaJIT is selected and Discord is disabled. This is not
a claim that every optional upstream build is supported by the installed packages.

The dependencies, discord-presence, innoextract and googletest git submodules were
uninitialized. None was required by this successful configuration; no submodule
was fetched. ONNX Runtime and Qt are not required by this preset.

## Internal simulation linkage verified

- Root `CMakeLists.txt` includes `server/` when **client OR server** is enabled,
  while `serverapp/` is conditional on `ENABLE_SERVER` alone.
- `server/CMakeLists.txt` defines the static `vcmiservercommon` target.
- `client/CMakeLists.txt` links `vcmiclientcommon` privately to
  `vcmiservercommon`; `clientapp/CMakeLists.txt` links `vcmiclient` to
  `vcmiclientcommon`.
- Generated `build.ninja` client link rule includes
  `bin/libvcmiservercommon.a` and `bin/libvcmi.so`. It has no standalone
  `vcmiserver`, `vcmilauncher`, or `vcmieditor` target.
- Build completed the final executable link. `nm -C` on that executable finds
  `CVCMIServer::run()` and `ServerThreadRunner::start(...)`.

This establishes compiled internal simulation linkage, **not** runtime absence
of sockets/child processes. That requires separately authorized execution.

## Source identity and limitations

Initial clean shared tree: branch `definitive-mvp`, HEAD
`a9b6d945ee7db2cb6f8d8ab90010cc51bbab2c4a`. Other workers/integrator updated
sources and HEAD while compilation ran. After compilation, an incremental
verification build succeeded at HEAD
`965c5027324ed7c286cd2e43130f0a49d35fbc71`, with other workers' uncommitted
client/server changes still present and preserved. Therefore this is a successful
shared-tree build, not an immutable clean-commit release candidate. Integrator
must rebuild after coherent integration before recording acceptance identity.

SHA-256 immediately after that verification build:

```text
14265af63977baaaf3230a2b28bc5acc5a7ee78d070554299a207acc685640ca  bin/vcmiclient
a61100fc5b01d389031b5b6ddcfb72bab4d3180f98ad6e097f3641daca65e1b6  bin/libvcmi.so
```

`git diff --check` passed. Unit tests were not enabled or run. Neither Windows
buildability nor the installed-asset gameplay acceptance gate was executed.
Preserve this build root for subsequent integration builds; do not create another.
