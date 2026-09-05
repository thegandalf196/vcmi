# New Horizons Linux build handoff

## Combined Runtime / Frontend integration verification

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
