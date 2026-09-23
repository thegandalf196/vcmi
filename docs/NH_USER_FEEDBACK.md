# New Horizons — user preview feedback

## 2026-09-23 — Conversation audit and unverified regressions

The consolidated design decisions are in
[NEW_HORIZONS_OVERRIDES.md](NEW_HORIZONS_OVERRIDES.md), including rank-specific
perks, teachers, Leadership readouts, Order targeting, spellbook inspection and
the latest UI/art direction. Those decisions remain requirements regardless of
whether an older build appeared to implement them.

Keep the following reported problems in regression scope. This list records
symptoms, not established causes or fresh verification of their resolution:

- Metamagic followed by a creature action (including Defend) must not produce
  the old immediate-follow-up rejection or require a repurposed Wait button.
  Magic Arrow and non-damage spells both need coverage under typed actions.
- Restarting a scenario from battle must dismiss the previous battle UI.
- Reserve/Gating selection must tolerate no selected creature, cancellation,
  and valid selection without dereferencing creature ID -1; the missing
  Demonic Gating localization is a separate presentation defect.
- Christian entering a field battle with Pikemen and his war machine must not
  enter a siege-tower shooter path. The reported tower index -256 does not prove
  the Ballista caused it; reproduce and trace before assigning a cause.
- Human troop transfer and AI garrison swapping must respect Leadership without
  repeatedly attempting illegal moves or presenting an ordinary capacity limit
  as a generic server/fishy-request failure. Verify starting armies too.
- Adventure movement-bar fullness must correspond to actual current/maximum
  movement after the movement rework. Auto-combat slowdown needs measurement,
  not an assumed cause.
- Encoding conversion, duplicate skill identifiers, mixed Disintegrate effects,
  GUI-thread dialog waits, obsolete hero-access diagnostics, and rule-schema
  mismatches require cause-specific checks. Hiding log messages is not a fix.
- Spell acquisition must be audited across all sources and hero specialties;
  Wisdom offer frequency must be checked against the correct class and eligible
  weighted pool rather than inferred from a small number of restarts.
- Solmyr's Master Chain Lightning description must reflect its actual
  level-scaled jump retention; Shroud of Malassa's reported ineffectiveness
  remains a behavior to verify against the controlling specification.
- Orders-button clipping, oversized Halon specialty art, malformed Ward text,
  missing stat/perk icons, and Conflux portrait clipping need rendered checks.

The one-command Linux launcher remains the requested playtest entry point. It
must identify the promoted playable candidate coherently; current source, latest
commit and validated playable build are not interchangeable claims. Launcher
symlink/profile errors and engine/content schema mismatches must be tested
without replacing a known playable snapshot with an unvalidated candidate.

The immediate Tower-versus-Inferno milestone also requires checking **every
building in both factions against the scripture and Accepted overrides**, not
just Solmyr, Arcane Reservoir and Gating. Enumerate the actual two town rosters;
check each building's prerequisites, construction, triggered/passive effect,
repeat/visit restrictions, AI use where applicable, save persistence and player
feedback. Record evidence and remaining gaps per building. A few passing unique
building tests do not establish this complete-roster requirement.

Operational testing restrictions and Git authorization are separate from
game-design overrides. A documentation audit does not lift any testing hold,
authorize history rewriting, or prove that any listed defect is fixed.

## Authorized implementation: curated conveniences, rights-checked assets

User explicitly requests integrating the quick-save/load buttons and creature
ability/status icons, and asks that legal obligations not worsen. This authorizes
implementation, not assuming third-party asset permission or making legal promises.
Include these conveniences automatically in the curated edition; no optional-mod
management workflow. Preserve working F8/F9, saved-game semantics and combat rules.

Public upstream check found GitHub license metadata null and no conventional
license/readme/credits filenames in the inspected vcmi-extras branch tree. That is
an unresolved redistribution-permission question, not proof of permission or a
legal verdict. Authorship credits alone are not a license. Do not copy Extras
sprites/config/source into shipped content until exact applicable permissions are
evidenced. Do not relicense third-party artwork as New Horizons CC0 or infer that
VCMI's GPL covers separately authored extras.

If permissions cannot be established promptly, implement equivalent buttons with
the existing callback framework and original New Horizons artwork. Independently
author recognizable ability/status icons (including Undead), with editable sources,
runtime outputs and provenance/license, or reference purchaser-installed assets
without redistributing them where appropriate. Do not trace/redraw unlicensed
Extras artwork. Source comparison may identify behavior and resource mappings;
that is not asset-import approval. Keep existing GPL/component notices intact.

Owners and required acceptance:
- Frontend: implement visible Quick Save/Quick Load controls and ability/status
  presentation using existing validated commands; original art and tooltips when
  source-asset permissions remain unresolved. No gameplay mutation or layout
  overrides that hide New Horizons school/development controls.
- Build: wire reviewed config/curated registration; source/notice/asset packaging,
  scoped commits and publication. Do not enable all Extras modules implicitly.
- Content: independently review rights/provenance and normal-input acceptance:
  click-save, state change, click-load/restored state, correct unavailable states,
  F8/F9 retained, Undead/living comparison, combat spell/status icon regressions,
  layout at supported sizes. No native Windows claim from Linux tests.
- Runtime: only if a real callback/state defect emerges; otherwise no rule changes.

Integrate as a bounded usability increment without mutating released/frozen
candidate bytes. Keep remaining full-design goals active; exact implementation
status and evidence belong in each owner's handoff.

## Clarification: working shortcuts, missing Extras presentation

User confirms F8/F9 quick-save/load work; only the buttons are missing. User
identified https://vcmi.eu/Mod%20Repository/Graphical/VCMI%20extras/ as the likely
source of familiar presentation. Direct page retrieval returned403; independently
inspected public vcmi-mods/vcmi-extras repository on branch vcmi-1.7 instead:

- Mods/adventureMap/Content/config/widgets/adventureMap.json explicitly declares
  buttonQuickSave/buttonQuickLoad, adventureQuickSave/adventureQuickLoad bindings
  and iam-quicksave/iam-quickload artwork (small and large layouts).
- Mods/bonusIcons/mods/Bonus Icons/Content/config/bonusIcons/bonuses.json maps
  core:UNDEAD to zvs/Lib1.res/E_UNDEAD. The Bonus Icons manifest describes unit
  ability, bonus and immunity artwork.

This supports a missing optional presentation-content explanation for both
examples, not removal of quick-save/load or Undead rules. Record shortcuts as
USER-CONFIRMED working, not an open functionality failure. Review compatibility,
asset rights/attribution and exact selective configuration before curating any
Extras content; do not blindly enable every optional module or import its art.

## Windows capability preview: initial report of missing conveniences and rough art

User reports playing the new Windows release, still finding it smooth, and a
promising start. New screens/spell-school icons look very crude. User also reports
apparently missing quick-save/quick-load and creature ability/status artwork,
with Undead as an example, and asks whether curated mod selection caused this.
Likely candidate is the just-linked Windows891 capability preview; user has not
yet independently supplied its file hash, original VCMI version/profile or exact
missing-control route. Do not call this exhaustive Windows acceptance or proof
that internal transport caused the perceived smoothness.

### Evidence and open questions

- Released source891 keyBindingsConfig.json still maps adventureQuickSave to F8
  and adventureQuickLoad to F9. Current source retains both handlers; quick-load
  admission includes hasQuickSave. This is presence evidence, not a successful
  Windows quick-save/load test. Check exact released callbacks, local-game gates,
  file creation, notification, reload and keyboard/UI discovery before declaring
  it functional or absent.
- Curated edition retains the VCMI mod/content loader and required vcmi/core
  resources; it does not remove the mod mechanism. Optional UI/art packs and
  settings may differ from the user's previous installation. No attribution of
  either reported omission to a particular omitted mod is established yet.
- Creature window still builds bonus graphics through bonusToGraphics. Trace
  released Undead descriptor/resource resolution and rendered creature-window
  settings, compare upstream defaults and curated manifests. Do not confuse an
  absent icon with loss of the actual Undead gameplay property.
- New authored icons are provisional functional artwork. User feedback means
  polish remains required; do not relabel generated assets as finished art.

### Ownership and next checks

Frontend owns shortcut/control discovery and bonus-art resolution review, plus
concrete fixes and later polish within existing ownership. Runtime owns any
actual save/load/rule defect. Content independently prepares and executes bounded
checks on the exact frozen candidate through normal input under existing guards.
Build integrates fixes, preserves the released identity and keeps the full-design
feature and release lanes separate. Existing handoffs retain detailed evidence.

The shortcut-versus-button question is answered above; do not ask it again or
report quick-save/load as broken. Continue the scoped presentation comparison and
provenance review with Extras as the identified reference. Optional details about
the previous VCMI version may refine compatibility but need not block review.

## 2026-09-22 — prioritize explanatory combat logging

The user explicitly prioritizes verbose, meaningful battle-log coverage of new
interactions. Report the actor, action, outcome, and the mechanic responsible:
for example, a second or third spell cast enabled by Metamagic, or damage taken
and the amount prevented by Brace. Use clear Heroes III-style sentences rather
than technical diagnostics or a repeated New Horizons prefix.

The Brace example expresses the desired explanation style, not a requested rules
change: the canonical Brace is a preemptive strike. Attribute mitigation to the
actual reducing Order (such as Hold the Line, Riposte, or Protect).

Damage attribution must come from the actual resolved calculation, with defined
rounding and modifier ordering; do not invent prevented amounts from tooltips.
Emit gameplay messages for authoritative resolved actions, not hypothetical AI
evaluations. Expand coverage across Orders, perks, spells, and their interactions;
Metamagic and Brace are the first examples, not the entire requested scope.

The user also confirmed that the reported ee320ac39 session's orderly shutdown
was their own exit, not an unexpected closure.

## 2026-09-22 — stale Cure/Shield and combat reserve crash

The user identified Cure and Shield among spells still obtained from teachers
and hero specialties. Audit distinguishes roster membership from implementation:
Cure remains in the controlling detailed Light roster, but its legacy generic
healing/negative-dispel behavior and mastery-based 4/4/3/3 costs do not implement
the specified 4 Mana, immediate `25 + 1.5 × Spell Power` living-stack healing and
one player-chosen physical affliction removal (Poison, Disease or Bleeding).
It must not resurrect or cleanse Curse, Slow or Berserk. Hero specialties and
all learning sources need consistent migration, not only Mage Guild filtering.

Vanilla Shield is active in the live roster despite being absent from the
controlling detailed Light spell list. The earlier summary mentions Shield of
Faith, but does not supply its mechanics; the later detailed list controls.
Do not invent a replacement from the summary title alone. Cure and Shield are
not fixed by this audit; preserve this work after the immediate crash repair.

The user crashed after clicking the reserve button in combat on playable
snapshot `5639618fdfcc42d7cb0df37079adf1096b1f97e760fc1f3d9344e454e38c6308`.
The exact binary's stack trace resolves to `BattleActionsController::actionIsLegal`
in the Demonic Gate branch: an unset creature ID (-1) is dereferenced during
hover selection. The button also requests a missing Demonic Gating translation
key. The 30 passing native Gating tests validate server mechanics, not this UI
path; require regression checking of unselected, cancelled and valid selections
before claiming the combat button works.
