# New Horizons frontend handoff (W2)

## Delivery pipeline checkpoint

Read NH_DELIVERY_PIPELINE.md, NH_AGENT_START.md, updated NH_WORKER_PLAN.md and
design cross-links. Existing full frontend goal is retained, not restarted.
Current release-candidate repair is the real All-toggle click defect below;
future hero-growth/mastery/tier breadth must not delay that bounded fix/retest.
Keep future feature source separate from immutable candidate bytes and report
actual Windows/Linux and GUI limits. Build alone integrates/publishes; no fifth
worker is activated and no frontend staging/commits are authorized. Arranged next
wake: Build's incremental compile/refreeze, then Content's same-path click retest.

## Actual95 All-tab click defect — local fix READY

Content's real95 GUI displayed six schools/headers and observed spell-AI Implosion
(7525 damage, mana84), but clicking All twice left the Primal/Bloodlust page.
Evidence: `testing/magic-gui95/11-All-click-stays-Primal.png` versus initial All.
This is a real frontend failure, not accepted six-school interaction.

Root cause confirmed in existing widget code: CToggleButton::clickReleased first
calls hover(false)/hover(true), THEN tests PRESSED. Our explicit setHoverable(true)
let CButton::hover replace PRESSED with HIGHLIGHTED before that check, so the
selection callback never executed. CButton defaults hoverable=false but still
registers HOVER/SHOW_POPUP; tooltips do not require hover highlighting.

Mutable `client/windows/CSpellWindow.cpp` now removes that All-toggle setting and
sets allowDeselection=false instead. CToggle's own doSelect still supplies the
selected highlight. This is local usage repair, no broad widget/rule/art change;
immutable95 remains untouched. Diff check exit0; SHA256
`f1f9e8c5856821798614e1f386a9fa3ba3619d99fa2baf77f90a9652c9d465d2`.
Immediate READY sent to Build/Content. Next: Build incremental compile/refreeze,
then actual Primal->All click, repeated All, school cycling/page/cast retest by
Content. No fixed/accepted GUI claim until that regression journey passes.

## 95a7001e3 immutable candidate; reward feedback remains authority-owned

Build released registered-source HOLD after an immutable906-file Linux95 copy
and reports113/24 native green. Content has the sole quiet10-minute GUI lease;
no frontend compiler/GUI or candidate changes. Source is at95a7001e3. Independently
read `build/new-horizons-windows-cross/sdl-main-feature-build.exit`:0, matching
Build's first feature Windows client/install success. The explicitly assigned
EntryPoint.cpp fix was exactly `#if __MINGW32__ && !defined(VCMI_SDL3)` around the
legacy `#undef main`: preserve SDL3 wrapper's SDL_main symbol, retain SDL2 behavior.
Build integrated it; Frontend made no commits. No Windows gameplay claim.

Coordinated actual reward-feedback path with Runtime: CQuestLog already passes
its game callback to quest text/components; CComponent displays the supplied
SecondarySkill ID/rank. Runtime confirmed NO new frontend API or conversion:
authored decoder, authoritative skill changes, limiter checks, reward/limiter
components and quest replacements resolve the actual skill in lib/server. Their
existing SEC_SKILL/MetaString output must be correct even for null-hero quest
previews. Do not add a second frontend remapping or alter immutable95. Runtime
will test/repair that path. Hero-family read/choice APIs remain unintegrated;
await real contracts, not fictional controls. Next: actual Tester UI defects or
new Runtime view APIs, with full growth/mastery/hero/tier scope still outstanding.

## Windows feature compilation — registered source HOLD

Build reports native113/24 gates green and is starting the first actual Windows
feature-client compile. Preserve all registered client source/headers/art during
this hold; no frontend compiler or GUI launch. Independent new files/docs are
allowed, but no real hero growth/leadership/mastery/category read-choice API exists
yet. Runtime's pure PrimaryProfile parser/math is not an integrated public view;
do not wire invented values or claim growth from that helper. Reward/limiter gaps
remain documented, so native green is not full six-school acceptance. Await Build's
actual platform result and integrated Tester gates; full redesign scope persists.

## First six-school build and bounded missing-frame diagnostic

Independently read `magic-first-build-20260906T204536Z.exit`:0. Actual log compiles
CSpellWindow.cpp at519/691 and links client at689/691. Thus saved-school UI source
now has real compiled evidence (not six-school rendered acceptance).
Parsed actual `magic-first-baseline.xml`:103 cases,1 failure; curated XML:8 cases,
1 failure. Named reds are Runtime-owned
`SuccessfulOrderDoesNotExpirePreexistingUnitTurnBonus` and
`LegacyHeaderDoesNotRequireDisablingCuratedModule`. They remain correctness gates;
no frontend bypass or weakened test. Build released source for needed owned fixes.

Read Content's actual repair66 first-journey record in NH_COMMAND_ACCEPTANCE:
chooser/cancel/target-cancel, three Orders, shared spell budget, persistent/switching
Doctrines, numeric labels/footer fitting and bookless-AI command use passed over
seven rounds. Pre/postbattle saves survived restart. Later continuation timed out124;
strong spell-AI/new-battle-NONE GUI checks remain unpassed. No broad completion.

Recurring saved-menu `unavailable frame0:2` logs still lacked a resource name.
Bounded owned diagnostic applied: `client/render/CAnimation.h` exposes immutable
resource name; `client/widgets/Images.cpp` adds that name and group frame count to
its existing failed-setFrame error. No rendering, frame selection or gameplay
behavior changes. `size(group)` inspected: const lookup only,0 if absent.
Diff check exit0. SHA256: header
`05aa2ec512e42c8a1614fd2f5ca47805cee5efdd93b8fe7d0353fce672e1cd25`, cpp
`6ba179fad22a5a12d0e349237f33bb73294f7c644b9c4998938004be02fd89b9`.
Build notified for its next compile; this diagnostic is not yet compiled and does
NOT claim to fix the unidentified missing frame. No compiler/GUI by Frontend.
Next: use actual resource-attributed logs if reproduced, respond to new UI defects,
and continue hero-family wiring when Runtime exposes real development/choice APIs.

## Original six-school skill artwork — READY for Build registration

Build explicitly authorized72 new skill PNGs plus72 editable SVGs. Added to
`assets/new-horizons/generate_icons.py`, `README.md`, owned `svg/` and mod `Images/`:
`NH_<school>Magic_<rank>_<size>.png`, school light/nature/sorcery/havoc/shadow/chaos,
rank basic/advanced/expert, size small/medium/large/scenarioBonus. Exact canvases
32x32/44x44/82x93/58x64 were read from skill schema and CSkill::registerIcons.
One/two/three lit marks express ranks1/2/3, NOT later mastery choices. Reuses our
own original CC0 geometric motifs; no purchaser/concept inputs or extracted pixels.
Build owns the six real skill definitions, gain chances and registration.

`python3 assets/new-horizons/generate_icons.py` exit0. Offline checks verify all72
RGBA dimensions/alpha, matching SVG dimensions and no embedded image/script content;
all256 prior outputs retain SHA256 exactly. Frontend inspected generated contact
pixels for every school/rank/size. Full isolated regeneration exit0: all400 files
byte-identical. Evidence under ignored Linux build root:
`research/skill-art/{before,validation}.json`, `contact.png`, and
`research/skill-art/reproduce-4gjj8tft/reproduction.json`. Total190SVG/190PNG/20JSON.
Content independently audited all400 outputs: full isolated reproduction byte-
identical, all256 previous hashes unchanged, all72 skill variants/sizes/rank markers
checked. Its missing-family and wrong-rank negative controls rejected, then restored
outputs passed. Contact pixels independently reviewed; Tester handoff contains the
record. No actual skill/mastery or graphical acceptance follows from this art PASS.
No compiler, native test or GUI launched by Frontend; frozen542 candidate untouched. Actual
skill progression, cost/rank use, hero/level-up rendering and old-save semantics
still require integrated gates. Next: independent art audit, Runtime/Build compile
readiness and school/command GUI feedback; do not equate assets with masteries.

## Actual saved-school callback wiring — awaiting Runtime/Build readiness

Runtime supplied exact game/battle classification and level APIs; inspected their
public declarations and actual definitions in `lib/spells/NewHorizonsMagic.cpp`.
CGameInfoCallback delegates game rules, BattleProxy delegates battle rules, and
CGHeroInstance uses battle-or-game saved rules for membership/level/rank/cost.
Runtime moved the game delegation from MapInfoCallback to CGameInfoCallback;
verified CCallback inherits it through CPlayerSpecificInfoCallback. This keeps
map-only editor/mock callbacks on safe legacy defaults instead of calling their
unsupported gameState(). Public signatures and frontend calls are unchanged.
Validation restricts remapped spell levels to1..5, compatible with existing level
text IDs; legacy/special-spell fallbacks remain Runtime-owned. `CSpellWindow.cpp/.h` now calls them:
`getActiveSpellSchools/getSpellSchools/getSpellLevel` in adventure context,
`battleGetActiveSpellSchools/battleGetSpellSchools/battleGetSpellLevel` in battle.
One book-local snapshot feeds sorting, learned counts, page totals, filtering and
level labels/hover. No raw CSpell school/level or global registry reads remain in
the book. Existing hero rank/best-school and cost calls are retained against
Runtime's now-present saved-context implementation. No frontend mechanics invented.

Tabs and keyboard/restored selection use only active visible IDs. New-school
order stays stable when learning spells; stale saved tabs fall back to All with
page0. Inactive legacy strip is covered by an original plain drawn panel with an
All-spells toggle reusing NH_spells_button; six custom glyphs/headers use registry
paths. Legacy four-school snapshots retain original strip/navigation. New-school
turn animation direction follows visible order rather than numeric registry IDs.
School paths/classification are data-driven; no hard-coded faction assignment.
Content independently reviewed the context/navigation and six-school geometry;
local `testing/commands-static/school-context-review.json`. Its wake described
All as48x36, but current source references NH_spells_button: Frontend decoded all
four actual64x64 frames and requested metadata correction. Exact All bounds are
(534+offR,318)..(598+offR,382), inside83x294 panel ending y382. No product change
needed. Content subsequently independently decoded all four64x64 frames, recorded
frame hashes/correct rectangles and corrected its metadata/handoff. No compiled,
rendered, cost/cast or legacy integration claim from this review.

Latest source hashes: cpp
`ceefcb46ae75ac0e3aa974cd03e778a65d26d5389dbce2ea94058c7e8424951d`,
header `9225916c6c86d57b88d97d1ab238c2e5543c132af980231a61e60783eef1bf36`.
Diff check exit0; inspected toggle silent-selection, scaled-image and color APIs.
This is NOT compiled/accepted yet: Runtime reports source WIP, with registration
and native integration still pending. Build must take the agreed shared compile
only after Runtime READY; immutable542 candidate is untouched. No art/config/CMake/rules edits. Content asked for independent source
review; active-six rendering/casts/save compatibility await coherent next freeze.

Actual first-command GUI gate FAILED activation: Tester reports fresh new game,
normal adventure save/reload and field battle opened original book rather than
chooser. BattleWindow correctly branches on authoritative battleUsesHeroCommands;
reported to Build/Runtime, no frontend force-enable or save mutation. Native fixture
overrides did not establish actual module activation. The mutable current.png had
already advanced to quit confirmation when Frontend read it; do not claim that
image independently proves the earlier book screen. Await preserved Tester record.

Next: fix any independent source-review defect, then compile with Runtime READY;
first-command activation repair/GUI retest remains necessary before accepting that
increment. Full growth/attributes/masteries/hero/tier scope remains unfinished.

## After immutable 54213f042 copy — school-context preparation

Build released source freeze after copying immutable candidate54213f042; Content
has the sole20-minute GUI lease. No frontend compiler/game launch or candidate
copy changes. Build reports95-case native gate and identity rebuild EXIT0;
actual command GUI acceptance remains pending, not inferred from those results.

Prepared `client/windows/CSpellWindow.cpp/.h` for the agreed save-scoped contract:
a single `readSchoolContext()` snapshots the existing real registry/classifications.
Sorting, custom-tab learned-spell counts, school page counts and page filtering
now share that book-local view rather than reading CSpell::schools independently.
The reader currently preserves existing semantics; there are NO fictional callback
bindings, new school IDs, global spell writes or claimed school migration. Runtime
can supply the real active IDs/classifications at this one read boundary next.
Caster school rank/best-school selection still uses existing hero mechanics;
explicitly flagged that dependency to Runtime for borders/descriptions/costs.

Static `git diff --check -- client/windows/CSpellWindow.cpp
client/windows/CSpellWindow.h` exit0. Inspection confirms direct global school reads
only inside the reader; inherited registry filtering/order semantics retained.
No compiled/runtime acceptance for this post-copy change yet. SHA256:
cpp `febe7a5551ab5f071a83e2f6880235a2be6140088427cbf2c016232f7809187f`,
header `343c429f5dd2a11894fa28c640081c44f58a0f634c64e191eb1a48816a5d31e3`.
No changes to command chooser/art/CMake/rules. Build notified to defer compiler
until quiet lease ends. Next: wire Runtime's exact callback contract, then gate
legacy/custom tab visibility, keyboard/restored selection and selected borders on
that real saved context; react immediately to candidate Tester defects.

## Current-recipient Doctrine clarification — updated chooser READY

At Tester's concrete request, exposed Runtime's declared first-slice coverage:
BOTH Orders and Doctrines affect only living ordinary own troops present when
issued, excluding war machines. Persistence across rounds does NOT grant effects
to later summons or clones. Such arrivals require switching to the other Doctrine;
reselecting the active Doctrine is invalid. No mechanics/balance changes made.

`client/battle/BattleHeroActionWindow.cpp` now states this in its visible Doctrine
caption, a two-line footer, and detailed command help; Doctrine help explicitly
explains switching and invalid same-Doctrine reselection. Existing percent values,
64px effect labels, action validation and art remain unchanged. Build notified
before freeze; updated cpp SHA256
`8da49071a6058f4a8123e04b73bc109423df464cf6ac31f49d06d1a2df3575db`.
Build reports the preceding combined build EXIT0, including chooser font fix and
school layout; combined92 native cases EXIT0 (91PASS/1 expected skip), including
both AI choices and persistence. These are Build-reported integration results,
not frontend-run tests or graphical acceptance. Final scope-clarification cpp
`8da49071...` still needs Build's next incremental compilation with the GUI exporter.
Build explicitly requests source/art frozen until a Tester defect and will send
the candidate freeze. Rendered/help-fit and command journeys remain unverified. Next executable task remains their concrete integration
feedback, then real school/hero API wiring as recorded below.

## Remaining full-scope gates and cross-owner dependencies

Full goal remains incomplete. Current source/API inspection establishes:

- Commands: bounded fixes READY; Build's next pass includes chooser font correction
  and school layout. Previous native run still had one AI spell-choice failure;
  Runtime is correcting its fixture/oracle. No frozen command GUI acceptance yet.
- Runtime confirmed next-family direction: retain four builtin school IDs and
  register six new IDs; expose save-scoped active IDs AND per-spell classification
  through game/battle callbacks. Do not overwrite global `CSpell::schools`, which
  would reinterpret old saves. Exact public API follows after the first gate;
  no frozen translation units/API edits are requested during command acceptance.
  Frontend must route book filtering/page counts/school borders through that
  classification contract, not merely change visible tabs.
- Schools: registry supplies IDs, scope, names and resource paths. Generic layout,
  ID-based filtering/casting and artwork are ready; need Runtime's game/save-scoped
  active-school list for BOTH battle and adventure books before removing old tabs
  or assigning a fixed six-school navigation order. Installed art is not ruleset
  identity. No faction table invented.
- Hero screen: inspected CHeroWindow; live primary values, manaLimit, morale/luck,
  class, inventory, army and ordinary secondary skills already have real backing.
  Preserve its artifact/army/switcher controls. Runtime must expose the actual
  deterministic growth profile, leadership/siege attributes, mastery eligibility/
  choices and creature categories before those new values/actions can be wired.
  Do not infer masteries from ordinary Expert skill level, creature category from
  legacy numeric tier, or capacity from an invented frontend formula. Read/choice
  API coordination requested directly from Runtime; no cross-owner code edits.
- Art: original command/school assets plus all15 hero motifs have independent
  static provenance/dimension/reproduction PASS. Later hero/control rendering and
  runtime behavior still need integrated Tester evidence; assets alone are not
  completion of any missing gameplay family.

Build/Runtime have explicit wake requests for compiler failures, candidate/Tester
results and next-family APIs. First complete the integrated command gate; then wire
actual school identity and the hero development presentation/choices. No commits,
GUI launches, architecture expansion or rule/CMake edits by Frontend.

## Custom-school layout implementation — ready for Build

Changed only `client/windows/CSpellWindow.cpp` after the command/art freeze.
Existing custom-school book code overlapped80x60 glyphs when more than five
schools were shown in a small book (six in a large book); its truncated hit rows
also disagreed with the selected glyph moved to foreground. Now excess custom
bookmarks use the existing aspect-preserving CAnimImage Rect constructor to fit
inside the same reserved strip, without overlap. Six small-book bookmarks become
68x51; hit areas use the actual rendered image rectangle. At or below the normal
capacity, positions and dimensions remain unchanged. No legacy tabs, spell
classification, costs, targets or save state are changed. Existing authoritative
cast paths and school name/help lookup are retained. This is a real six-school
layout prerequisite, not a completed six-school rules/content migration.

Static validation: `git diff --check -- client/windows/CSpellWindow.cpp` exit0.
Offline geometry checks extracted source constants and covered all24 small/large
count cases (0..10/0..12), verifying bounds, no overlap, positive dimensions and
unchanged full-size layouts for the authored80x60 bookmark contract. Evidence:
ignored `research/spellbook-layout/geometry.json` under the Linux build root.
SHA256 `743808177cc6c69bd5f8a7151c3aa35c9afa09a36b18dedfdbefb40249c4f573`.
Content subsequently independently read the source and CAnimImage Rect constructor
and checked all24 geometry cases: PASS recorded in `NH_COMMAND_ACCEPTANCE.md`,
with local `testing/commands-static/school-layout-independent.json`. This confirms
the geometry review only, not an active registry or rendered hit testing.
Build must compile; Tester must exercise six actual registered schools, mouse and
keyboard selection, headers/pages/search and casts after coherent registry freeze.
No graphical PASS claimed. New hero art independently reproduced all256 outputs
by Content; its evidence is `testing/commands-static/hero-art-audit.json`.

Next: respond to integrated command/AI/GUI defects; then wire stable active-school
navigation when Runtime provides save-scoped school identity. Generic layout no
longer depends on waiting for that API. Hero growth/mastery/tier APIs and screen
remain unfinished; original display glyphs are available but not fake controls.

## Follow-up: font-fit correction and hero-glyph preparation

Tester supplied actual external SMALFONT metrics (offline, not GUI): line height
16px, previous physical-damage line166px versus width163px. Corrected chooser
numeric caption to `Physical taken +/-N%` (full tooltip still states physical
**damage taken**), and expanded Doctrine labels from47px to64px height, y394..458,
before footer y463. This accommodates four bitmap-font lines rather than clipping
three48px lines. Build notified to incrementally rebuild before freeze.
Updated cpp SHA256 `0b85df8fc755d523b8b529ca6a25f5e90e5002b953994a32581e1f5147318e55`;
header unchanged. Actual font/render/input verification remains Tester-owned.

Added 15 original display motifs in two sizes (32/64): four primaries, mana,
leadership, movement, morale, luck, siege, growth, mastery, Core/Elite/Champion.
Files: `assets/new-horizons/generate_icons.py`, `README.md`, 30 new SVGs and 30
new PNGs `NH_hero_<id>_<size>` under owned source/Images directories. No fake
controls, attribute formulas, classifications or mastery choices were added.
They share the original CC0 geometric provenance and provisional-style declaration.

Validation: `python3 assets/new-horizons/generate_icons.py` exit0. Offline Python
checks verified all196 prior outputs SHA-identical, 30 new RGBA dimensions/alpha,
matching SVG dimensions and no embedded image/script/foreignObject elements.
Evidence: ignored `research/hero-art/{before,validation}.json` and `contact.png`
under the Linux build root. Frontend inspected the actual generated contact sheet;
this is art review, not in-game acceptance. Full exports now118 SVG/118 PNG/20 JSON.
Build authorized new art while existing command sources were otherwise frozen.
Additional isolated reproduction exit0: all256 outputs byte-identical using a
copied generator; no product outputs touched. Full hashes and generator identity:
`research/hero-art/reproduce-a6rev_be/reproduction.json` under the same ignored root.

Independent schoolbook audit: current registry offers `getAllObjects`, IDs/scope,
header/bookmark paths; existing casting/search/page code already uses school IDs.
But legacy tabs always remain, custom tabs reorder by learned-spell count, and no
save-scoped active-school API is present. Asked Runtime/Build for actual next-family
IDs and active-school identity for adventure AND battle books. Do not infer game
rules from installed art or fabricate a completed migration. Next: fix any command
compile/Tester defect and integrate stable school navigation once that contract is
available; hero glyphs are preparation, not full hero-screen completion.

## Post-reboot chooser correction — ready for integrated rebuild

Read `NH_WORKER_PLAN.md`; full frontend scope remains commands, six-school book,
hero growth/attributes/masteries/tier presentation and hero-screen redesign.
First-command readiness is not full-scope completion. Sole Build compiles; sole
Content Tester launches graphical journeys. No commits or cross-owner edits.

Changed only `client/battle/BattleHeroActionWindow.cpp/.h` in this checkpoint:

- Corrected Aggressive's tooltip to include **both melee and ranged** damage,
  matching current `config/newHorizonsCombat.json`; Waiting remains allowed.
- Visible effect summaries now read the saved battle rules through existing
  `heroCommands::bonuses`, using the current hero's Attack/Defense. They show
  actual rounded/capped percent bonuses, physical damage-taken penalties and
  base-speed changes rather than duplicating coefficients in the frontend.
  Read-only bonus values are never installed or sent as gameplay mutations.
- Detailed tooltips retain duration, provisional Hold-the-Line scope, shared
  action/no-mana information. Cache numeric descriptions by hero ratings within
  the immutable battle-rules snapshot; authoritative availability still refreshes.
- Avoid calling CLabel::setText on unchanged status: it unconditionally requests
  parent redraw, and this chooser checks status from show(). Button::block already
  protects unchanged state; preserve that existing behavior.
- Preserved Dispatcher-added `gui/Shortcut.h` and existing weak battle ownership,
  click-time validation, cancellation and authoritative request path.

Static check: `git diff --check -- client/battle/BattleHeroActionWindow.cpp
client/battle/BattleHeroActionWindow.h` exit 0 (untracked files also inspected).
Source SHA256: cpp `805704465874d3001524fde843c2b0a441c35e066aa4c0ac0040da78a21547b2`,
header `7d22543e35267d6d6dbc928aae7f9dd5789dc0e1f6e71e2b90fd494ada24e322`.
No compile or graphical PASS claimed for this change; Build's current native lane
must incrementally rebuild it before freeze. Tester must check numeric-label
fitting (especially Aggressive's three effects), penalties and actual commands.
Art unchanged here; earlier padding reproduction evidence is historical until
Tester verifies the current frozen assets. Build corrected its mod mount path.

Next executable task: address any integrated compiler/Tester defect, then audit
existing custom-school navigation/layout against all six registered schools and
coordinate actual IDs with Runtime/Build before wiring further book controls.


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
