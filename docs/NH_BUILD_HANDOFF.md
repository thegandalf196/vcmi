# New Horizons Linux build handoff

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
