# New Horizons independent graphical test results

**Result:** the specified ordinary single-player graphical journey was completed
through genuine scenario defeat across two bounded runs, including save/quit/reload
and continued play. No product defect was found. This is not full-fidelity/audio,
all-campaign, platform-parity or exhaustive original-content acceptance.

## Run 1 — partial gate, normal quit completed

- Candidate: `1a4b1184d31de06b6fa31717fa49f365f822ae25`, client SHA-256
  `d364b0314bdf3a38f2b7f659108c8acac27bc733b8e7163659fa18de69085d6b`.
  Hash unchanged after exit. Later coordination/doc commits did not replace bytes.
- Native Linux 7.0.0-30-generic, x86_64; SDL2/OpenGL, private Xvfb `:191`,
  1280×800 screen. Client PID 722537, approximately 17:53–18:11 UTC on 2026-09-05;
  25-minute supervisor bound. Xvfb had a separate 30-minute bound.
- Purchaser-supplied external Complete `Data`, `Maps`, `Mp3`, linked by the frozen
  launcher; no original executable launched or original content changed/copied.
  Isolated temporary NH profile, retained for reload. Exact local paths and logs:
  `build/new-horizons-linux/testing/run1/` (`profile-path.txt`, console and images).
  No proprietary images, save files or logs are committed.
- Sole Tester used normal XTest mouse/keyboard actions on the private display;
  no host pointer/focus, portal or visible fallback. No gameplay state injection.
  `SDL_AUDIODRIVER=dummy`: **audible output is not verified**.

### Observed journey

| Step | Actual observation |
| --- | --- |
| Menu → new → Single Scenario | Composed original menu, local scenario/options screen, no host/address/connect interaction. |
| Scenario/start | Original **A Warm and Familiar Place**, normal difficulty, red human Ash, green AI, fixed Inferno towns; Begin reached adventure and original introductory event. |
| Hero/movement/resource | Ash inspected (level 1, Bloodlust, 10 mana); plotted/executed multi-step movement with map recentering/fog discovery. Wood pickup showed +8 and stock 20→28. |
| Town/build/recruit | Cinderspire opened. Built Imp Crucible: wood28→23, ore20→15, gold20000→19700. Recruited 15 Imps into town garrison for750, gold18950. |
| AI/seven turns | Seven normal End Turn/confirmation cycles reached Month1 Week2 Day1 and weekly Behemoth message. Day2 income advanced gold18950→19450. The later apparent3000 shortfall was resolved by the original tribute event observed in run2 below. |
| Combat/spell | Reached a visible neutral Familiars stack through normal exploration. Manual combat: Bloodlust targeted Imps, combat log named spell and mana10→5; moved Imps, shot/melee-attacked with Gogs, defended. Battle victory against27 Familiars, +108XP, losses11 Imps/1 Gog. Returned to adventure with4 Imps/6 Gogs. |
| Save | Normal `S` dialog, named save **Autosnh-run1**, explicit success dialog. Local `.vsgm1` size627249 bytes. Saved Week2 Day1, mana5, resources23 wood/16 mercury/15 ore/10 sulfur/10 crystal/10 gems/19450 gold. |
| Quit | Options → Quit to Desktop → confirmation. PID exited; client log shows interface/state/AI cleanup and client stopped. Explicit lease release sent to Build and Runtime before any rebuild/relaunch. |

Useful checkpoints: `02-movement-wood.png`, `03-town-built-recruited.png`,
`04-week-two.png`, `05-bloodlust.png`, `06-combat-victory.png`,
`07-save-success.png`. `current.png` is overwritten during navigation.

### Setup findings, not product defects

1. Launcher correctly rejected a profile inside the purchaser installation's
   ancestor tree. Switched to a separate temporary profile; launcher stayed frozen.
2. Without a window manager, initial fullscreen window was1×1 and black. Normal F4
   switched to windowed1280×720, initially at+639+399. Explicit private-display
   XMoveWindow to0,0 and exact-window XSetInputFocus produced the composed menu.
   This is headless window-system setup, not evidence of a gameplay failure.
3. Before another run, `tools/tests/nh-private-input.py` was hardened to require
   a locally recorded owned-Xvfb PID/start-tick/boot-ID/socket-inode guard, checked
   before connecting and before every action. Missing/stale guard tests reject
   without input; no display fallback. GPL notice retained.

### Runtime evidence and remaining gate

Runtime's independent observer reported3723 samples from17:55:35.569432Z through
exact-PID exit at18:11:35.127819Z, no child or owned INET-positive snapshots;
initial startup before observation is not covered. Local summary is
`testing/run1/runtime-summary.json`. Sampling is not proof against arbitrarily
short-lived sockets/children between samples. Its detailed limitations remain in
that evidence; the historical “network thread” log label alone is not a socket.

Run1 alone did not establish reload/continued play or scenario outcome. Those
remaining journey steps were exercised in run2, after explicit Build permission.

## Run 2 — reload, continued play and scenario defeat

- Build's frozen checkpoint: `4f624a497cf47de2d0370a2d29cc8d3ea89e3b6d`.
  Client SHA-256 unchanged:
  `d364b0314bdf3a38f2b7f659108c8acac27bc733b8e7163659fa18de69085d6b`.
  Shared `libvcmi.so` SHA-256:
  `5389c4902b36143eb6e7edc7d1963e981671a873c9fe66b1d48306a757bfa74c`.
  Build reported version identity refreshed, no intervening gameplay change.
  `testing/run2/before-hashes.txt` and `after-hashes.txt` are identical.
- Same retained NH profile; fresh bounded private Xvfb PID726160 with an exact
  identity guard, display`:191`. Client PID726196 ran approximately18:22:04–18:45:43
  UTC, within its1500-second bound. Existing windowed settings yielded1280×720
  at0,40; private XMoveWindow/focus placed it at0,0. No host interaction.
- Normal Load Game → Single Scenario → **Autosnh-run1** → Load restored Week2Day1,
  Ash XP166,4 Imps/6 Gogs,5/10 mana and the saved resources/gold19450. Screenshot
  `testing/run2/01-reloaded.png` shows the hero snapshot. Position/fog and town
  ownership were visually consistent. Original intro video also composed on startup.
- Two controlled no-spend End Turns yielded live gold19950 then20450; right-click
  resource popup showed income+500. Options → Load Game → confirmation → Single
  Scenario → **Autosave-122** restored Week2Day2, gold19950. Continued from there:
  multi-step movement, external Imp Crucible visit/recruitment (+15 Imps), and
  town construction/recruitment all worked. Built Upgraded Imp Crucible, Birthing
  Pools and Citadel through ordinary dialogs; recruited15 Familiars.
- **Causal income clarification:** the original scenario displayed “The Gods of
  Hell demand Tribute. Payment is mandatory or else torment will be dispensed.”
  with **-3000 gold**. Local screenshot:
  `testing/run2/02-original-tribute-event.png`. This accounts for the apparent
  missing six500 income increments from run1; controlled+500 turns also worked.
  This was original timed-event behavior, **not** a frontend/resource-income bug.
  Both Runtime and Frontend received the evidence; no speculative patch was made.
- Attempted ordinary weekly growth toward the map's500-Familiars objective. AI
  **Olema attacked and captured Cinderspire on Week3Day6**, defeating its15 Imps
  and15 Familiars. Used normal autocombat controls for this later siege (the first
  combat/spell gate was manual). The normal no-town countdown appeared.
- On Week4Day3 Olema reached and attacked Ash. Opened the spellbook and manually
  cast Bloodlust again (mana10→5), then used normal autocombat controls. Ash lost
  all19 Imps/6 Gogs. With the last town and hero lost, the game displayed banishment,
  “You have been eliminated from the game!”, and the original defeat screen.
  This was a **genuine scenario loss**, not a cheat, abandonment shortcut or merely
  a battle result. Screenshots: `testing/run2/03-scenario-defeat.png` and
  `04-defeat-screen.png`.
- Returned to the main menu and confirmed normal Quit. Client log records main-loop
  termination at18:45:42.540 UTC (log prints local15:45); PID absence verified before
  the deadline. No timeout kill or shutdown stall. Released PID/profile to Build
  and Runtime explicitly, then terminated the owned idle Xvfb. No game remains live.

Local run2 evidence: `build/new-horizons-linux/testing/run2/`, including
`client.log`, console log, guard, images and Runtime's separate passive observer
records. Runtime's finalized `testing/run2/runtime-summary.json` records5314 samples
from18:22:54.371481Z through exact-PID exit18:45:42.834709Z, with zero child/owned
INET-positive snapshots and zero observer errors. Gameplay stages were supplied
by the sole Tester; Runtime independently verified process/socket observations.
Initial startup before sampling and transients between0.25-second samples remain
uncovered. Unix/device-event netlink sockets are not single-player INET transport;
this is not an all-socket-free claim.

## Acceptance limits / handoff

- **Completed visually:** menu/local selection/start, hero/multi-step movement,
  resource pickup, town/build/recruit, AI and more than seven turns, manual
  combat/spell, save/normal quit/restart/reload/continued play, autosave load,
  actual scenario defeat, return-to-menu and final normal quit.
- Audio used the dummy driver in both runs: audible music/effects/video sound are
  **unverified**, not passed. Intro and defeat video pixels were observed, not every
  original cinematic. Campaign continuity, victory branch, all maps/factions and
  Windows remain untested. Native tests are Build-owned complementary evidence,
  not substitutes for these graphical observations.
- No product/launcher edits by Tester; only testing helper and this document.
  No proprietary screenshots, saves, maps, logs or profiles staged for Git.
  Candidate lease is released; no new launch without the next frozen announcement.

## Planned gap1 regression — explicitly empty neutral-town capture

**Plan only; not executed.** Runtime owns implementation/native tests. Preserve
both the accepted binaries until Build replaces them and the idle MVP save profile;
use a separate regression profile once Build announces a frozen candidate.

Preflight coordination: Runtime supplies the target scenario identity, town name/
location, and independent evidence that its H3M garrison flag is **explicitly set
with seven empty slots**, not merely an unspecified/default garrison. Target must
be visible/reachable on day1 without intermediate combat or scripted transfers.
Prefer a verified purchaser scenario; none has been identified yet. If Runtime
provides a synthetic map from the existing TinyH3MBuilder, label it focused
integration evidence, not original-scenario acceptance. Agree its private exposure
with Build first; do not alter purchaser Maps, launcher or product configuration.

Normal-input route (private guarded Xvfb/XTest only, maximum15 minutes per run):

1. New Game → Single Scenario → designated map → Begin. Inspect the target through
   normal town information; record neutral ownership and no defending stacks.
2. Save **before capture**, quit normally, and notify Runtime of the PID boundary.
   After a frozen-ready confirmation, relaunch the same regression profile and load
   that save. Verify neutral ownership/empty garrison persisted.
3. Select the hero and execute its ordinary path onto the town entrance. Expect
   immediate ownership transfer/town access **without a battle screen**, attack
   confirmation for defenders, casualties or battle XP. Verify player flag, town
   list, visiting hero and unchanged army. No frontend/state injection.
4. Save after capture; use the normal Load Game route to reload. Check ownership,
   hero/army and buildings persisted. End one turn and inspect expected town income
   (account for declared map events); ensure gameplay continues. Quit normally.
5. Control: an explicitly populated neutral town must retain its specified guards
   and enter ordinary combat on attack. An unspecified garrison remains eligible
   for upstream random initialization, **not guaranteed nonempty**: a single empty
   random result is not a regression. Runtime's paired native tests establish the
   flag/RNG distinction and serialization compatibility; GUI observations alone
   cannot establish those internal semantics.

Keep only a pre-capture/reloaded view and post-capture ownership checkpoint unless
there is a defect. Record source/client/library hashes, scenario provenance, PID
and normal-input steps in local evidence. Notify Runtime before start/load/quit for
passive observation. On unexpected defenders, battle, ownership or reload failure,
send the concrete checkpoint/log and failed step directly to Runtime and Build;
stop/release, await their fix/frozen rebuild, and repeat the same route. No original
execution, package installation, host display interaction or launch is authorized
by this plan itself.

## Gap1 candidate — accepted-save compatibility PASS

Bounded normal-input test on 2026-09-05, approximately19:19–19:30 UTC, using the
preserved MVP profile and guarded private Xvfb only. Frozen checkpoint:
`023ffe7daa447a9613601ffd06401d2920868b00`.

- Client SHA-256:
  `1066015c77c5ba0e7e3b685c20730d234bea4306976913992cc80313b8c0e3a5`.
- `libvcmi.so` SHA-256:
  `3628ee50636f88da9558bd5fed7f6e36e0947c22020532404950467a6b6d2066`.
  Final hashes matched the frozen announcement; no build/product edits during play.
- PID730415: normal Load Game selected the preserved **Autosnh-run1** accepted on
  the4f candidate. Restored Week2Day1, Ash XP166,4 Imps/6 Gogs, mana5/10,
  movement319/1560, gold19450 and resources23/16/15/10/10/10. Position/fog and
  Cinderspire ownership visually matched the previous checkpoint.
- Continued one normal End Turn and a two-tile move. Day2 gold19950, mana6/10 and
  movement1360/1560 were then stored in the **new, distinct**
  `NEWGAMEgap1-compat-023` save; explicit success dialog observed. Quit normally.
- PID730571: restarted the same frozen candidate/profile and loaded that new save
  through the ordinary menu. Day2, XP166,4 Imps/6 Gogs, mana6/10,
  movement1360/1560, gold19950, resources, moved position/fog and town ownership
  matched. Quit normally again; both PIDs absent before the15-minute journey limit.
- The original `Autosnh-run1.vsgm1` SHA-256 was checked against its pre-run hash
  after **each** quit: unchanged. It was not overwritten. Both old and new saves
  remain in the idle profile. Owned Xvfb stopped; explicit final lease release sent
  to Build/Runtime at19:30:30Z.

Local evidence: `build/new-horizons-linux/testing/gap1-compat/`, including
`old-save-before.sha256`, `final-hashes.txt`, `client1.log`, `client2.log`,
`01-old-save-restored.png`, `02-new-save-success.png`, `03-new-save-reloaded.png`.
Runtime's finalized `runtime-summary.json` reports1416 samples for PID730415
(19:20:17.839987–19:26:22.488238Z) and545 for PID730571
(19:28:08.079597–19:30:28.425376Z), zero child/owned-INET positives or observer
errors. Startup gaps,250ms sampling, Unix/netlink and dummy-audio limits remain.

This establishes the exercised old-save → continue → new-save → restart/reload
compatibility route, **not** every historical save version or a graphical gap1
capture pass. No approved neutral-town diagnostic target was exposed or launched
in this test. Focused capture regression remains pending Build's explicit frozen
diagnostic identity/provenance announcement.

## Gap1 synthetic explicit-empty GUI PASS

Build subsequently approved frozen diagnostic checkpoint
`9bd41073b5f0772cac6447b3bd465a2859981c54`. Sole Tester exercised it on
2026-09-05,19:41:38–19:55:18 UTC (under the15-minute bound), with the unchanged
launcher, separate `testing/gap1-assets` and new `testing/gap1-profile`, under the
build directory. No MVP profile/save writes, product edits or builds during play.

- Client SHA-256:
  `1066015c77c5ba0e7e3b685c20730d234bea4306976913992cc80313b8c0e3a5`.
- Library SHA-256:
  `3abbe5e47bc9f0e90a38cd3e874f9ddb972921b8a8c01ab1b5aae184ba390b85`.
- Primary: `NHGap1ExplicitEmptySOD.h3m`, generated by
  `TinyH3MBuilderTest.ExportNeutralTownGarrisonFixtures`; gzip SHA-256
  `0293f64bbc68baee87ee9c4a1cbe6474888815aee0ee6147385445ac9d260af6`.
  Build's `testing/gap1-fixture-manifest.json` supplies raw identity and native
  parser/initialization/disk-byte provenance. This is synthetic diagnostic content,
  **not** a shipped original map. Only the three approved fixture maps appeared.
- PID731666: selected the explicit-empty SOD scenario normally. On day1, neutral
  Castle **Transom** showed empty army slots in its right-click popup. Orrin had
  XP40,15 Pikemen/5 Archers, mana10/10, movement1560/1560; resources
  wood20/mercury10/ore20/sulfur10/crystal10/gems10/gold20000.
  Saved **NEWGAMEpre** successfully and quit normally.
- Replacement PID731818 loaded **NEWGAMEpre** through the ordinary menu. The
  neutral-town empty popup and hero checkpoint persisted. A legal two-diagonal
  approach to the entrance captured Transom directly into its town screen, with
  **no combat screen or result**. Red ownership, empty garrison and the unchanged
  visiting hero army were visible. No turn advance was needed.
- Saved distinct **NEWGAMEpost** successfully, then used ordinary Load Game in
  the same client process. Reopened owned Transom: empty garrison and visiting
  15 Pikemen/5 Archers persisted. Day1/resources/gold/XP40/mana10 remained
  unchanged; hero movement was1278/1560 after the approach. Quit normally.
- Both client PIDs were absent before release19:55:18Z. Owned guarded Xvfb was
  stopped. Final client/library and all three fixture gzip hashes matched the
  approved identities. Separate diagnostic profile and both named saves preserved.

Local-only evidence: `build/new-horizons-linux/testing/gap1-gui/`, containing
`01-empty-neutral.png`, `02-pre-save-reloaded.png`, `03-captured-no-battle.png`,
`04-post-save-reloaded.png`, `05-post-reload-hero.png`, and both client logs.
Runtime's finalized `runtime-summary.json` records1758 samples for PID731666
(19:43:18.538547–19:50:51.331359Z) and837 for PID731818
(19:51:41.906643–19:55:17.439602Z), with no child/owned-INET positives or observer
errors; both exact process exits were observed. Startup gaps and250ms sampling
prevent an exhaustive transient process/socket claim; dummy audio remains
unverified.

**Limits:** no post-capture End Turn/income check was performed; that remains
pending. The optional17-Pikemen populated control and unspecified fixture were
not played, preserving the time bound. Their distinction remains native evidence;
unspecified guards may legitimately randomize empty. This graphical PASS covers
this explicit-empty SOD fixture, capture, and pre/post-capture persistence—not all
original maps, weekly neutral growth, campaigns, audio or other platforms.

## Gap1 follow-up — post-capture income and populated control PASS

Separately authorized bounded run,2026-09-05 19:57:48–20:01:58 UTC, PID732152,
private guarded Xvfb. Repository evidence checkpoint `0fb1bf855` was docs-only:
**no rebuild**, so tested binary identity remains `9bd41073b5f0772cac6447b3bd465a2859981c54`
with the client/library hashes above. Same approved diagnostic assets/profile.

1. Loaded **NEWGAMEpost** normally. Kingdom-resource popup showed gold20000 and
   **+1000/day**, with wood20/mercury10/ore20/sulfur10/crystal10/gems10. One
   no-spend End Turn continued to Day2 with **gold21000**, other resources
   unchanged and both owned towns retained. This closes the preceding run's
   pending post-capture turn/income check; no weekly-growth claim.
2. Returned to the main menu and started **NHGap1CustomSOD** normally. Fixture
   gzip SHA-256:
   `6ca9a316b32f1fa9038c58ecdc6b2c7d341d3cafc443b414f1cfea3c2e2489dd`.
   Neutral Castle **Dunwall** displayed a **Pack of Pikemen** in its popup—not an
   exact count there. Ordinary entrance path opened a guarded siege battle with
   **exactly17 defending Pikemen** visibly present; attacker had12 Pikemen and
   7 Archers. Unlike the explicit-empty fixture, this did not capture directly.
   Exact count was verified in battle, not inferred from the popup label.
3. Quit normally through Options → Quit to Desktop from battle. No battle/scenario
   completion claimed. PID absent, owned Xvfb stopped, explicit lease release sent
   at20:01:58Z. **NEWGAMEpre/NEWGAMEpost hashes unchanged**, no named save writes;
   final binaries and all three fixture gzip hashes matched their frozen values.

Evidence under `build/new-horizons-linux/testing/gap1-control/`:
`01-income.png`, `02-next-day.png`, `03-populated.png`, `04-guarded-battle.png`,
`client.log`, `named-before.sha256`, `final-hashes.txt`, and Runtime's independent
process observation. The optional unspecified fixture was not played; an empty
random result would not constitute failure. Same startup/transient sampling and
dummy-audio limitations apply. No product edits, builds or original executable use.
