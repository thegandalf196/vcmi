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
