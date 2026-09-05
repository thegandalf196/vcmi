# New Horizons frontend handoff (W2)

Status: two-file implementation authorized and applied; compile and runtime
verification pending. Original proposal below is retained as the scope record;
implementation details and coordination updates follow.
Inspected source: `a9b6d945e`; initial `git status --short` was empty.
Scope: this separate New Horizons fork only, not Reconstruction.

Read before planning: `AGENTS.md`, `docs/NEW_HORIZONS_MVP.md`, and upstream
`docs/developers/{Coding_Guidelines,Code_Structure,Networking,Serialization}.md`.
The Networking document's single-player TCP statement is historical: actual
source already has an internal connection. The MVP contract takes precedence.

## Exact proposed W2 source files

1. `client/CServerHandler.cpp`
   - Make local single-player startup choose `ServerThreadRunner` regardless of
     persisted `server.useProcess`. Cover NONE (new scenario/tutorial/campaign
     setup), SINGLE, CAMPAIGN and TUTORIAL load modes, not just SINGLE.
   - Preserve the multiplayer implementation as unreachable legacy machinery;
     do not rewrite server lifetime or remove process-runner classes here.
   - Remove the single-player debug start/load escape through
     `session.donotstartserver`; retain normal request/validation flow.
2. `client/mainmenu/CMainMenu.cpp`
   - Do not construct menu buttons for parsed `start multi` / `load multi`
     commands; this also removes their registered keyboard shortcuts. Keep the
     existing positions/art/resources of remaining buttons, rather than
     redesigning the menu or editing owned-by-W3 JSON.
   - Guard `openLobby` before resetting state against guest/remote, MULTI and
     hotseat requests. This is an unsupported-entry policy, not removal of
     networking facilities or a source-modification restriction.
   - For local single-player, `CSimpleJoinScreen` must start locally even with
     stale `session.donotstartserver`; do not expose editable address/port or a
     second connect action in that path. Keep progress, Cancel, and existing
     connection/failure callbacks. Preserve legacy multiplayer dialog code.

No header/API change proposed. No `client/lobby/` edits proposed for this first
patch: scenario/campaign selection, save filters, random-map setup, difficulty,
options and start validation remain usable as-is. No `ServerRunner*`, server,
lib, build, configuration, launcher or global-lobby source edits by W2.
This document is the specifically requested documentation exception to W2's
source ownership. Coordinate before enlarging the file list.

## Actual start/load trace

- `CMainMenu.cpp::genCommand`: `start single` calls
  `openLobby(newGame, true, {}, NONE, false)`; `load single` calls
  `openLobby(loadGame, true, {}, SINGLE, false)`. Campaign/tutorial loads use
  CAMPAIGN/TUTORIAL respectively.
- `openLobby` calls `resetStateForLobby` with NEW_GAME or LOAD_GAME and LOCAL,
  sets load/hotseat/battle flags, then constructs `CSimpleJoinScreen`.
- `CSimpleJoinScreen` normally calls `startConnection()` for a host. Empty
  address calls `CServerHandler::startLocalServerAndConnect(false)`.
  Currently `session.donotstartserver` instead exposes remote address entry.
- `startLocalServerAndConnect` currently honors `server.useProcess` on desktop.
  It supplies last difficulty in a fresh StartInfo, then calls
  `runner.start(loadMode == MULTI, connectToLobby, si)` and `connectToServer`.
- `connectToServer` selects the runner when `isServerLocal()` (runner != null).
  Hostname/port arguments alone do not imply a socket in this branch.
- `ServerThreadRunner::start` creates `CVCMIServer`, starts `runServer`, calls
  `prepare(false, false)` for single-player and waits for readiness.
  `CVCMIServer::startAcceptingIncomingConnections(false)` creates a network
  server wrapper but does not call its `start(port)` listener operation.
- `ServerThreadRunner::connect`, with lobbyMode false, calls
  `INetworkHandler::createInternalConnection`. `NetworkHandler` constructs
  `InternalConnection`, hands it to `receiveInternalConnection`, then posts
  the client connection-established callback to the existing event context.
- `CLobbyScreen::startScenario` calls `validateGameStart`, then `sendStartGame`:
  LobbyPrepareStartGame and LobbyStartGame still pass through the connection.
  `startGameplay` dispatches NEW_GAME/CAMPAIGN to client new-game setup and
  LOAD_GAME to `client->loadGame(gameState)`; frontend must not deserialize or
  mutate authoritative gameplay directly as a substitute.
- `openCampaignLobby` also uses `CSimpleJoinScreen`, with campaign state queued
  for sending. Tutorial uses ordinary new-game lobby plus
  `startMapAfterConnection`. Preserve these routes and campaign continuation.
- `debugStartTest(filename, save)` uses NEW_GAME/LOAD_GAME setup but currently
  has its own `donotstartserver` branch; include it in transport-policy review.

## Runtime interface agreement requested from W1

Keep existing `IServerRunner` signatures:

```cpp
void start(bool listenForConnections, bool connectToLobby,
           std::shared_ptr<StartInfo> startingInfo);
void connect(INetworkHandler & network, INetworkClientListener & listener);
void shutdown();
void wait();
int exitCode();
```

W2 single-player contract: construct a thread runner; call
`start(false, false, startingInfo)` (the existing loadMode predicate evaluates
false for all supported single-player entries); then call `connect` through
CServerHandler. No process or TCP fallback on internal-start failure. No new
transport, direct game-state channel, or serialization version change.

W1 owns readiness exception propagation, partial-start cleanup and lifetime
inside `ServerRunner*`/simulation. Please ensure start either reports readiness
or a catchable failure, never an unresolved readiness wait. Agree the exception
behavior before adding frontend error recovery; W2 should reuse the existing
error/cancel UI rather than guess a new asynchronous runner API.

Preserve lifecycle: `sendClientDisconnecting` sends LobbyClientDisconnected
with shutdownServer for local sessions; cancellation sets CONNECTION_CANCELLED
and requests runner shutdown; `waitForServerShutdown` handles joining/reset.
Do not bypass these by directly destroying a running simulation. W1/W5 should
review cancellation-before-connection and failure-before-ready independently.

## Curated UI and content boundary

Retain New/Load single-player, original campaigns and tutorial, save/reload,
scenario setup, settings, credits, high scores and exit. Do not delete art,
translations, manifests, dependency loaders or resources labeled `vcmi`/mod:
these are engine infrastructure, not automatically optional content.

No optional-mod installation/selection command was found in the inspected main
menu command dispatcher. Hiding multiplayer here is not sufficient to implement
the complete curated-content policy. W3/integrator must own the allowed content
inventory, mainmenu/campaign configuration, persisted optional-mod handling,
and launcher/package entry policy. Preserve dependency incompatibility errors;
do not silently activate missing mods to load a map/save or hide errors.
Do not blacklist arbitrary map filenames/extensions as a substitute for that
inventory. Battle-only and extra-rule UI policy should be agreed with W3 before
removal; this initial proposal preserves them rather than risking original
scenario/campaign play. Global-lobby initialization, external launch arguments
and entry points outside these owned files need separate owner review; W2's
menu guard alone is not an application-wide no-network proof.

## Validation and coordination

Before implementation, agree this file boundary and runner failure behavior
with W1; coordinate content/UI decisions with W3 and save continuity with W4.
W5 negative cases: persisted useProcess=true; donotstartserver=true; new, load,
campaign and tutorial modes; alternate multiplayer commands/shortcuts; cancel
while connecting; failed prepare; repeated start/quit/reload. Verify callbacks,
packet validation and presentation ordering remain intact.

No assigned build path was supplied to W2, so no build root was created or
build attempted. Use only the integrator/W6-assigned existing build for later
compile checks. No GUI/game launch, package installation, commit or push was
performed. Source inspection cannot establish playable acceptance or absence
of runtime sockets/children. The full MVP play journey requires a separately
authorized bounded run and independent process/socket observation.

## Authorized implementation update

Only `client/CServerHandler.cpp` and `client/mainmenu/CMainMenu.cpp` were edited
as product source. Persisted process selection is now restricted to MULTI;
debug start/load always starts locally. Main menu skips multiplayer button
construction (including shortcuts), and openLobby rejects remote/guest/MULTI/
hotseat arguments before state mutation.

The single-player CSimpleJoinScreen branch reuses built-in `loadbar` artwork
and the existing Cancel button. It constructs no address/port fields, Connect
button or connection/server title; ignores donotstartserver; immediately starts
local setup; and retains the class identity expected by lobby callbacks. This
is a transient loading surface, not a host/join choice. Normal scenario/options
and save-selection screens, Begin/Load buttons and gameplay progress are
unchanged. Existing MUDIALOG artwork has address-related content, so it is not
used for single-player. The nullable title is checked on cancellation.

Cancellation can race the posted internal-connection callback. The callback
now checks cancellation under the interface mutex before its CONNECTING assert,
closes the abandoned connection and joins through waitForServerShutdown. Queued
lobby packets are ignored after cancellation; a cancelled established session
no longer surfaces an unexpected-disconnection dialog.

### Runtime contract response

Read Runtime's updated readiness/lifetime contract during implementation.
CServerHandler catches failed start, resets the safely destructible runner,
restores NONE and rethrows; it never connects or falls back after failure.
The shared menu helper catches std::exception outside progress-window
construction and reports the existing localized unable-start-map/reason dialog
with the original diagnostic. Thus a constructor-time failure cannot push a
progress window above its error dialog. Campaign setup uses the same helper.
Unknown exceptions continue to propagate, matching Runtime's contract. Debug
startup failures also propagate rather than waiting for an unscheduled callback.

Runtime retains ownership of startup promise propagation, safe destructor/
shutdown/wait and synchronous preparation. Frontend still releases the GUI
mutex when joining through the existing helper. Neither change establishes
concurrent start/reset safety; rapid cancel/re-enter and repeated session tests
remain required.

### Build owner request and evidence

W6/integrator: please compile the changed CServerHandler.cpp and
mainmenu/CMainMenu.cpp in the active `build/new-horizons-linux` build after
Runtime's changes are included. W2 did not start a competing build.

`git diff --check` on both source files passed. Inline Python source-contract
checks passed for process-selection gating, removal of the debug escape, local
progress branch without address/connect/title controls, multiplayer guard and
button filtering, and cancelled callback/packet guards. Additional source
checks verify failed preparation resets/rethrows before connect and the menu
helper reports errors outside constructor execution. These checks are not C++
compilation, unit execution or graphical acceptance.

### Actual remaining UI/validation limits

- Loading artwork and Cancel placement have not been rendered; installed-asset
  visual verification is still needed. The setup surface is static artwork,
  not a fabricated numerical progress indicator. Existing gameplay loading
  progress remains intact.
- Runner start is synchronous: Cancel cannot be processed during preparation
  itself. It is available once control returns while handshake/setup completes.
- Scenario/options retain battle-only, extra options and random-map controls;
  content/extra-rule curation remains W3/integrator work, not deleted resources.
- Ordinary setup no longer displays the join/address screen. Legacy remote
  dialogs and global-lobby code still exist outside reachable menu entries;
  this is not an application-wide no-network proof.
- Existing unexpected-disconnection and compatibility error diagnostics may
  still use upstream terminology. No new translations or configuration edits
  were made; engine mod/dependency validation was not bypassed.
- No game/GUI launch, package installation, commit or push. Other workers'
  runtime/server/build changes were preserved. Full MVP play and negative
  failure/cancel/reload tests remain pending authorized execution.

## Independent runtime/client teardown review (follow-up)

Inspected the actual pending ServerRunner and CVCMIServer diffs against
NetworkHandler::createInternalConnection, InternalConnection::{close,disconnect},
NetworkServer::receiveInternalConnection and the client callbacks. No Runtime
files were edited.

Concrete findings communicated to Runtime/integrator:

1. `stop()`/Asio stop plus final SHUTDOWN does not call the client's
   onDisconnected. InternalConnection destruction likewise does not emit that
   callback. Our earlier frontend Cancel closed the window immediately and,
   after onConnectionEstablished had already run, had no guaranteed join/reset
   trigger. This is a frontend cleanup defect, not a request for Runtime to
   synthesize network events.
2. Early Cancel also allowed a new setup while the previous readiness callback
   was queued. Checking only CONNECTION_CANCELLED was insufficient once a new
   reset changed the state back to CONNECTING. Runner destruction while holding
   the GUI mutex is not a safe replacement for orderly serialized teardown.
3. A successful synchronous start does not guarantee successful connection
   allocation/posting. The earlier try/catch covered prepare only, leaving a
   live worker if connectToServer threw during progress-window construction.
4. Queued packet callbacks carried an explicit connection identity, but the
   frontend discarded it. After reset that could feed a previous session's
   packet into the new logicConnection or a null connection.

Own-file fixes now applied:

- Local cancellation schedules the existing network timer, even when the
  internal transport never emits a disconnection event. Cancel is disabled and
  the same loading surface stays up until cleanup is complete; no host/join UI.
- A cancelled readiness callback records its connection identity and closes it.
  If the timer happens to arrive first, it reschedules until that already-posted
  internal callback has been consumed. No new setup is exposed in the meantime.
- The timer closes/reset connections and pending tutorial auto-start, joins via
  waitForServerShutdown (releasing GUI mutex), then dismisses the loading surface
  and returns to NONE. It tolerates an already-joined runner. Obsolete retry
  timers outside CONNECTING do not reconnect/assert.
- Cancelled onDisconnected retains identity until timer cleanup. Packet callbacks
  reject mismatched connections. Connection-failed callbacks check cancellation
  under the mutex, before asserting CONNECTING.
- Failure after successful readiness requests shutdown and joins before
  propagating to the existing local-setup error dialog; no fallback or retry.

Runtime's readiness promise ownership, joined preparation exception rethrow,
thread-creation failure cleanup and stopped-before-run semantics appear coherent
with these callers by source inspection. `run()` exceptions still terminate the
worker/process as documented; not reclassified as preparation failures. Raw
stop is cancellation, not graceful gameplay disconnect: keep the ordinary
packet-driven sendClientDisconnecting path for game exit. Runtime must retain
shutdown/wait safety after failed start and must not assume stopping alone has
completed client cleanup.

Build owner: these two frontend files changed again during the combined build;
please rebuild their objects after this follow-up. No competing build was run.
Need independent runtime cases for cancellation before callback, after callback
but before lobby acknowledgement, rapid cancel/re-enter, preparation failure,
connection setup failure, and normal exit/reload. Source reasoning is not a
replacement for these tests or graphical acceptance.
