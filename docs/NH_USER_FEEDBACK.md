# New Horizons — user preview feedback

## Windows capability preview: missing familiar VCMI conveniences and rough art

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

Ask user whether F8/F9 fail or the expected buttons are missing, where the Undead
icon used to appear (creature information window versus battlefield marker), and
which VCMI version/optional UI packs they used. These details refine reproduction;
static review and default-profile tests need not stop while awaiting them.
