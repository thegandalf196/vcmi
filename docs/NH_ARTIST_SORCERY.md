# Sorcery art commission — dedicated Artist worker

## User authority and outcome

User explicitly authorizes a fifth worker devoted to polished original artwork,
starting with Sorcery. Use original Heroes III art as visual reference so the
result fits the game rather than drifting into modern flat-icon UI. Deliver the
whole school family, not one enlarged concept image: bookmark, selected-school
illustration, secondary-skill progression and the other currently referenced
Sorcery assets. This is an AI-assisted art commission, not a claim that a human
illustrator or an unavailable image-generation service has been hired.

Aim for release-quality art; only user visual approval plus independent technical
and in-game review can establish the final result. Existing prototype art remains
functional until replacement is reviewed. Do not label procedural drafts definitive.

Read AGENTS.md, NEW_HORIZONS_DESIGN.md, NH_WORKER_PLAN.md, NH_DELIVERY_PIPELINE.md,
assets/new-horizons/README.md and the relevant Frontend/Content handoffs first.

## Exact ownership and coordination

Artist owns only new files under `assets/new-horizons/sorcery-art/`, this charter's
append-only progress section, and ignored review output under
`build/new-horizons-linux/research/sorcery-art/`. Keep review output bounded.

Do NOT edit the shared `assets/new-horizons/generate_icons.py`, existing svg/
files, Mods/new-horizons/Images/, source C++/config, CMake, release candidates or
other workers' handoffs. These are draft-output boundaries, not permission to
leave the art permanently disconnected: provide a precise import manifest and
coordinate Frontend/Build for reviewed production replacement. Frontend retains
all non-Sorcery art and UI ownership; Artist is the sole Sorcery replacement author.
Build alone stages/commits/pushes and serializes integration/builds. Content alone
runs graphical journeys; Artist may render original standalone asset previews and
read reference images offline, but never launch or automate the game/host desktop.

Do not create a sixth worker. This fifth is Artist, not the optional unactivated
Windows Packaging worker. Preserve the active goals of all existing workers.

## Actually inspected reference and visual direction

Ignored purchaser-only reference images already exist at
`build/new-horizons-linux/research/spellbook-source/`. Read `contact-full.png`,
`Schools.def-g0-f*.png`, `SPELTAB.def-g0-f*.png` and `SpelBack.pcx.png` with the
image reader, not just filenames or dimensions. They are private references,
never distributable source art. Dispatcher inspected contact-full.png and the
existing sparse NH_sorcery_header.png before writing this brief.

Observed original visual language:
- Small painterly/pixel-finished illustrations with modelled volume, readable
  silhouettes, clustered highlights, dark creases and restrained texture.
- Header scenes occupy an aged gold-bordered field: sculpted cloud face, golden
  sun, foaming wave or tree/mountain. These are rich illustrations, not line logos.
- Bookmarks are shaded fabric/ribbons with gold embroidered motifs and cast
  shadows. Selected/unselected states have real material/value differences.
- Color and contrast fit warm parchment, aged metal and the low-resolution UI.

Do not copy those exact scenes, motifs or proprietary pixel regions. Reference
composition scale, material treatment, color relationships and pixel density.
Do not trace, recolor, embed or train a model on extracted proprietary art here.
No downloaded unlicensed art, fonts or textures. Record tool/asset provenance;
original geometry/paint outputs must have clear editable source and license.

Initial Sorcery concept direction (not a fixed user-approved emblem): an arcane
orb/celestial instrument in aged brass, indigo velvet, restrained silver-blue
light. A richly modelled object should replace the current empty geometric glyph.
Keep it distinct from elemental lightning, Nature foliage, Shadow skulls or Chaos
flames. Check the current school description/spell assignments for semantic fit.
Explore two original compact compositions before refining one coherent family;
show why each reads at native size rather than filling a large canvas with noise.

## Deliverables and exact current runtime contract

Verify these against the current Frontend API/config and actual images before
export. Current filenames/dimensions observed by Dispatcher:

| Asset | Required output |
|---|---|
| `NH_sorcery_bookmark_selected.png`, `_unselected.png` | Each80x60 RGBA; existing bookmark animation frame0 selected/frame1 unselected. Inspect hooks; these are not five generic button states. |
| `NH_sorcery_header.png` |160x96 RGBA. Preserve transparent top28 rows; original visible illustration occupies160x68. Fits first filtered-school page at existing header position, not a full new spellbook background. |
| `NH_sorceryMagic_{basic,advanced,expert}_{small,medium,large,scenarioBonus}.png` |12 images:32x32,44x44,82x93,58x64 respectively. Rank treatment legible at each size; hand-tune small outputs, not merely blur/downsample a large painting. |
| `NH_sorcery_icon.png` |64x64 standalone school emblem. |
| `NH_sorcery_{normal,pressed,highlighted,disabled}.png` |64x64 each, preserve genuine state readability and alpha. Existing button descriptor names/order must remain compatible. |
| Animation/resource integration manifest |List exact draft-to-runtime filenames, dimensions, frame roles, alpha rules and source hashes. Do not modify live descriptors independently. |

Original `Schools.def` full canvas160x96/crop160x68@(0,28); original SPELTAB is a
whole83x294 strip of five selection-state frames, NOT five separate bookmarks.
New custom-school bookmark hooks already exist; do not force these old strip
semantics onto the custom API. The secondary-skill reference must also be inspected
from the legitimate installation using existing offline asset tooling; document
actual resource names and pixels rather than invent original rank appearance.

## Iteration and technical review

1. Inspect original references and current bindings; record a short style/palette/
   material analysis and contract. No game launch or original-executable access.
2. Create two original draft motifs and native-size preview sheets. Include the
   full160x96 header, both bookmarks and at least small/large skill samples. Provide
   optional enlarged nearest-neighbor views separately; never use enlargement to
   disguise illegibility at native scale. Tell Dispatcher the exact preview paths.
3. Refine the chosen direction into the entire family. Prefer layered editable
   painting/vector source with explicit materials and hand-tuned pixels over
   flat primitives plus random noise. Use only available tools; never claim a
   render/image-generation service was used if it was not.
4. Validate all dimensions, alpha/top-margin, frame/state ordering, absence of
   clipped edges and small-size rank recognition. Supply reproducible exports,
   source/runtime hashes and provenance. Artist's isolated exporter must not
   regenerate other artists' outputs or modify purchaser references.
5. Frontend reviews integration and reserves live Sorcery paths for replacement;
   Build imports only approved files and adapts shared generation/audit manifests
   in coordination. Content checks real composed spellbook/skill UI on a frozen
   candidate, including old/new school navigation, frames and rank sizes.
6. Obtain user visual review. Address concrete requested revisions. If awaiting
   user/Tester feedback, arrange a wake and use harness-compliant waiting; do not
   endlessly generate variants or call unfinished work complete.

## Acceptance

- Cohesive original Sorcery family covers every listed runtime asset and state.
- Observable improvement over current crude prototypes at actual UI scale, using
  the reference's shaded/material-rich treatment without copying its artwork.
- Editable source, export route, attribution/license/provenance and checksums exist;
  no original assets or unclear third-party rights in distributable outputs.
- Frontend/Build integration is recorded and independent in-game visual/layout/
  behavior checks pass. Static mockups alone are insufficient.
- User explicitly approves the visual direction/final family. Missing approval
  remains unaccepted, not a fabricated legal or artistic completion claim.

## Goal prompt

```text
/goal Create, refine and integrate the complete original Sorcery school art family specified by docs/NH_ARTIST_SORCERY.md: selected/unselected bookmark, filtered-school illustration, all Basic/Advanced/Expert skill sizes, emblem and button states. Inspect actual original Heroes III reference pixels offline and existing runtime bindings, then author richly shaded material-aware art fitting that visual language without copying proprietary pixels/compositions. Own only the charter's isolated draft/export/review paths; no shared generator/live assets/product edits, no game launch or commits. Supply two native-size concept directions, refine a cohesive family, maintain editable sources/provenance/license and deterministic exports. Coordinate Frontend/Build integration and Content's sole graphical acceptance; preserve existing candidate bytes and other workers' goals. Require actual-size legibility, correct alpha/dimensions/states, independent in-game review and explicit user visual approval before calling the family definitive or complete. Record progress/evidence/next action in the charter. Use available tools honestly; no fictitious human commission or image-generation capability. Follow harness wait/safety rules while awaiting arranged reviews.
```

## Artist progress

Artist appends concise dated checkpoints here: references inspected, changed draft
files, native-size preview paths, export checks, review feedback and exact next task.

### 2026-09-07 13:04 UTC — reference/contract inspection; quiet lease

Read baseline/design, worker/pipeline, art README and relevant current handoffs.
Actually viewed purchaser-only contact-full, all four Schools frames, all five
SPELTAB frames and SpelBack with image reader, plus current live Sorcery header.
Observed compact clustered light/dark modelling, ochre edge wear, directional
fabric folds and tiny gold stitching; current Sorcery is an empty outlined glyph.
No reference pixels were copied or exported. Secondary-skill pixel inspection is
still pending; existing local offline decoder has been read, not rerun.

Verified current CSpellWindow custom hooks: frame0 selected/frame1 unselected,
80x60 with aspect-preserving compact-six-school scaling (review must include this),
header at117,74 plus offsets on first page. Live button JSON orders normal,
pressed, disabled, highlighted. Skill config names match charter. Sorcery spell
assignments include antiMagic, clone, dimensionDoor, dispel, forceField, teleport,
magicMirror and visions: instrument/controlled-space motifs fit better than
lightning or flames. Proposed original directions for upcoming native drafts:
A, a cradled blue-glass orb with asymmetrical brass meridian and indigo cloth;
B, a silver-blue lens suspended inside a folded brass spatial aperture. Distinct
silhouettes, not reused original school scenes. No direction is approved yet.

Build explicitly holds heavy generation during MASTERYGUI925 quiet lease
(600s hard /450s quit-init). No shared assets, source, generator, candidates or
other workers' files changed by Artist. Next after Build teardown wake: inspect
actual secondary-skill pixels offline, then author two native-size concepts in
isolated paths, deterministic exports and precise hash/import manifest. Build is
wake owner; Frontend/Dispatcher receive drafts, Content alone performs later GUI
review. User final approval and all integration/graphical gates remain pending.

### 2026-09-07 — Frontend coordination ACK

Frontend explicitly reserves Sorcery replacement ownership and preserves live
prototypes. Its runtime review specifies compact six-school bookmarks at **68x51**
in addition to native80x60; both belong on concept/review sheets. It confirms exact
header top28 transparency and all four skill sizes. Frontend/Build will coordinate
selective generation/import protection only after user approval and Content GUI;
Artist must not change the shared generator. Frontend requests a wake with both
native concepts and import manifest. Build teardown wake remains outstanding;
no heavy export started during the quiet lease.
