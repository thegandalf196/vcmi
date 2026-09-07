# Sorcery art commission — dedicated Artist worker

## User authority and outcome

**Current superseding direction:** the user rejected V2 as crude/MS-Paint-like
and supplied the miniature fantasy still-life production description. Read
[NH_SORCERY_STYLE_BRIEF.md](NH_SORCERY_STYLE_BRIEF.md) before further art.
One richly modeled high-resolution master plus native-size reductions is the
next quality gate, NOT more flat/angular studies or another full family. Prior
Renaissance-study instructions below are historical where they conflict with
this brief. No concept or visual quality has been approved.

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

Historical first-round direction (both resulting concepts rejected by user as
too modern; NOT the current approved aesthetic): an arcane
orb/celestial instrument in aged brass, indigo velvet, restrained silver-blue
light. A richly modelled object should replace the current empty geometric glyph.
Keep it distinct from elemental lightning, Nature foliage, Shadow skulls or Chaos
flames. Check the current school description/spell assignments for semantic fit.
Explore two original compact compositions before refining one coherent family;
show why each reads at native size rather than filling a large canvas with noise.

## Current user direction — new exploratory round, neither A nor B approved

User viewed downloaded Meridian/Aperture sheets and says both look too much like
Heroes: Olden Era, a more modern game. Heroes III instead has a kind of Renaissance
style, although user has not settled on exact terminology. User explicitly asks
for more attempts, then to document the chosen direction and follow it afterward.
This supersedes the initial orb/brass-emblem direction and any worker preference
for A. No concept is approved. Preserve the original drafts as rejected references;
do not just add surface noise to the same smooth orb/shield compositions.

Working interpretation to test, NOT an authoritative user style definition:
old-world fantasy painted miniature / illuminated-book / theatrical Renaissance
imagery; modelled figurative or still-life scenes, warm parchment and restrained
pigments, hand-shaped silhouettes, localized textured highlights. Avoid sleek
jewelry/product-render icons, polished spherical gems, immaculate metallic bevels,
uniform circular medallions, neon rims and modern UI gloss. Study actual original
headers AND secondary-skill pictures again for composition and object/rank changes.
A Renaissance label does not mean importing historical paintings without checking
rights or copying Heroes III's proprietary compositions.

Next deliverable is THREE genuinely different new studies, not another expensive
full family before visual choice:
1. Magician's Study: an original still life of worn books, candle and arcane
   instrument; richer object composition and warm/chiaroscuro material treatment.
2. Conjurer: expressive hand or robed magician performing subtle arcane work;
   figurative/theatrical composition rather than a jewel emblem.
3. Celestial Manuscript: original painted cosmological scene on aged parchment;
   imagery with volume and rhythm, not a flat technical wireframe diagram.

These are exploratory prompts, not approved iconography. Artist may improve the
specific composition to fit Sorcery semantics. Each study supplies a native160x96
header with required top28 transparency, selected/unselected bookmark samples and
at least32x32/82x93 skill samples. Compare at native resolution plus optional
nearest-neighbor enlargement; fix edge/alpha errors in newly authored geometry.
Use a new named revision under the existing isolated art directory. Keep source,
provenance and concise review sheets; no live import. Do not repeatedly generate
variants without inspecting results. Respect Build's quiet leases and arrange the
next bounded generation slot; reference reading/sketch planning can proceed.

Send Dispatcher the exact downloadable review-sheet paths. User will select or
reject. After explicit approval, write a compact style guide with approved example
hashes, palette/material/shape/lighting/pixel-treatment rules, rejected examples and
reasons, and how to adapt ranks/sizes without drift. Do not predeclare these
hypotheses an accepted style guide or call any draft definitive. Then finish the
full family and integration/acceptance gates below.

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

### 2026-09-07 — two complete-family concepts exported after teardown

Build released MASTERYGUI925 lease; Artist then decoded/read actual original skill
pixels offline in the allowed ignored review path. `CSkill::registerIcons` plus
enum mapping confirms Air48..50 and Sorcery78..80 in SECSK32/Secskill/SECSK82.
Read native contact: original ranks change object composition (Air scroll/book/orb;
Sorcery hat then candle/skull then flask), not merely colour. Earlier45..47/75..77
sample was correctly identified as Fire/Intelligence, not mislabeled Sorcery.
Private references remain excluded; detailed provenance in isolated README.

Created two full20-PNG concept families with editable standalone SVGs and isolated
Python/Inkscape/Pillow exporter, CC0 dedication, provenance and exact per-file
source/draft/runtime hashes in `assets/new-horizons/sorcery-art/`.
Native preview paths (include80x60 and68x51 bookmarks):
- `assets/new-horizons/sorcery-art/meridian/native-review.png`
  SHA256 `8d67b80cf866c67fcba0993373eed5ee863a73675bf33a5337976176fd321d1d`.
- `assets/new-horizons/sorcery-art/aperture/native-review.png`
  SHA256 `655c4970c6e52b390f47bc9bd1cbc91eae9600e0be597bb3b188448e8f2d874a`.
- `assets/new-horizons/sorcery-art/import-manifest.json`
  SHA256 `8f0a089e99b23ae4a24230dd2c000ceeffb972f046448aa741da4d2647ca6d4b`.

Actual `python3 assets/new-horizons/sorcery-art/export.py` final EXIT0 validated40
PNGs: dimensions, RGBA, transparent exterior and header top28. Initial near-alpha
skill-border failure corrected through larger authored inset, not pixel clipping.
Artist read both native sheets: A has clearer circular glass/brass silhouette;
B angular aperture is more distinct from elemental orb imagery. Both still look
smooth/vector-finished; not yet the accepted richly finished final family. Tiny
Basic label overlap in sheet noted; runtime pixels unaffected. Full repeatability,
independent legibility, stronger material finishing, user choice/final approval,
Frontend/Build import and Content GUI are still pending. No candidate/live/shared
writes, game launch or commits. Sources/reviews bounded about1.1M/540K respectively.

Build requested new MASTERYSAVE450hard/300quit-init quiet lease immediately after
this bounded export. Artist sent PAUSED/ready ACK; no heavy batch until teardown
wake. Sending two concept paths/manifest to Frontend, Content and Dispatcher now;
request concrete direction/material/readability feedback, not approval by silence.
Next after teardown: repeatability/negative-control audit and refine chosen family
against feedback; maintain the complete original goal and all acceptance gates.

### 2026-09-07 — Dispatcher actual-pixel review, user choice pending

Dispatcher read both actual native sheets and prefers Meridian A for clearer
silhouette and glass/brass volume; this is NOT user approval. B reads as a jeweled
shield rather than a spatial instrument. Both improve on the flat prototype but
remain too smooth/vector-clean. Required refinement: warmer aged brass and velvet,
restrained deliberately placed painterly/pixel material accents (not random noise),
physical rank composition changes beyond pips, and stronger real bookmark state
contrast. Header must become a distinct narrative arcane miniature, not the emblem
on a mostly empty diagram field. Preserve both submitted drafts/manifest bytes;
next refinement belongs in a new isolated revision, not overwrite these reviews.
Dispatcher is presenting sheets and asking user A/B; actual user direction and
Build MASTERYSAVE teardown wake are still outstanding. No export/refinement during
quiet lease, no import or final-acceptance claim.

### 2026-09-07 — repeatability PASS; strict edge audit RED; Content review

After Build MASTERYSAVE verified teardown, regenerated in ignored isolated
`research/sorcery-art/repeatability/`: export EXIT0; all86 generated files exactly
match submitted originals (40SVG/40PNG/4sheets/exporter/manifest), and submitted
baseline SHA256s remain unchanged. Report `research/sorcery-art/repeatability.json`.
New read-only isolated `audit.py` passes six negative controls and validates
manifest/source hashes,40 dimensions/RGBA/header top28, unique states/ranks and
no SVG embedded/external/font content, BUT correctly returns EXIT1 under stricter
transparent-rim check:16 concept images touch canvas edge (both3small skills and
both emblem/four button sets). Alpha maxima: small top1/bottom51, medallion bottom119.
Preserved `static-audit-red.json`/`static-audit.json`; no fake technical PASS.
Repair the chosen new revision's authored geometry (inset medallion/drop shadow,
raise rank rail/small composition), not submitted concept bytes or post-clear pixels.
Full explanation/new audit path in isolated `REVIEW_STATUS.md`.

Content independently read both native sheets after teardown: advisory preference
A for controlled arcane instrument/cohesion; B reads faceted gem mount, not opening.
Agrees cleaner/smoother than target, needs stronger32px rank distinction, stronger
compact bookmark states, richer purposeful header and sheet label-spacing fix.
This corroborates Dispatcher critique, not user approval or in-game acceptance.
Content is inspecting manifest/export provenance. Artist notifies owners of actual
repeatability PASS and stricter edge RED. Waiting for Dispatcher's arranged user
A/B direction before creating a distinct refined revision; no live import pending
those gates, no silent overwrite of reviewed concepts. No current heavy batch.

### 2026-09-07 — Frontend actual-pixel critique received

Frontend actually viewed both native sheets: advisory A preference at32 and68x51,
B narrower lens reads more badge. Visually consistent header top28 is not GUI
acceptance. Requests crisp roughly3px rank chips/spacing plus stronger physical
rank progression, localised brass wear/creases and directional highlights,
structured velvet folds/stitching, curved glass reflection/depth rather than round
white glint, a coherent richer160x68 instrument/cloth scene, and stronger compact
tab fabric/value/edge separation. Aligns with Content/Dispatcher review. No user
choice or approval supplied; Frontend explicitly asks to await Dispatcher direction
before generating variants. Recorded for selected revision; waiting on arranged
user-review wake, no new batch or live import.

### 2026-09-07 — independent static audit corroboration

Content independently checked all40 PNG/SVG hashes, dimensions, RGBA, source tags,
two20-runtime-path sets, descriptor frame ordering and clear header top28; reports
`sorcery-concepts-independent.json/log`. It independently reproduces the same16
outer-edge alpha contacts. Correct classification: **edge-clearance RED**, not
proof that underlying geometry is clipped. Artist audit's `edge clipping` label
is conservative shorthand for its explicit transparent-rim requirement; do not
claim proven silhouette truncation. Next revision still needs safe authored rim.
Content did not rerasterize: Artist's86-file repeatability PASS remains separate,
not independent repeatability verification. No user approval, graphical acceptance
or live import. Build deferred the planned boundary GUI; user-direction wait remains
active and wake owner remains Dispatcher/Build.

### 2026-09-07 — user rejects A/B; three new illustrative studies

Actual user feedback rejects BOTH A/B as modern/OldenEra-like. All worker A
preferences are superseded. Read updated current-direction charter and again
actually viewed original header/tab and Air/Sorcery secondary-skill contacts.
Created new isolated `renaissance-studies-v2/paint.py` with hand-placed native-pixel
polygons/material planes and editable SVG groups, Pillow only; no image model,
noise, proprietary pixels/compositions or external art/fonts/textures. Three
new subjects, not surface variants of orb/shield: worn-book/candle/dividers still
life, expressive conjuring hand/curtains/floating leaf, cosmological painted folio.

Build granted one120s offline slot. Initial export EXIT1 immediately at header
edge guard (cloth touches canvas), preserved in ignored `v2-export-evidence.json`.
Authored scene inset and repositioned hand, no alpha erasure. Build granted ONE
<=10s retry: actual EXIT0 exports15 samples with RGBA, clear exterior rim and
header top28 guards. Slot explicitly released/Pillow process finished before
Build next TRACE compile. No repeat batch. Original A/B baseline SHA256s rechecked
unchanged. No live/shared/candidate edits, GUI or commits.

Artist actually read all3 native sheets. New compositions are distinct and avoid
modern glossy orb/badge, but angular planes remain rough; these are composition
studies, not achieved painterly finish or user-approved Renaissance style. Exactly
five assets each:160x96 header,80x60 two bookmarks,32x32 and82x93 skill samples;
no ranks/full family predeclared before choice. Sheets also show68x51 compact tabs.
Exact downloadable paths under `assets/new-horizons/sorcery-art/renaissance-studies-v2/`:
- `study/native-review.png`, SHA256
  `643a2f168cc91aaa69245ad5b34e79f4ca19e14a89107733f04908b8c6063635`.
- `conjurer/native-review.png`, SHA256
  `617ca132ac7afbe491fd4f7c2df5ec0b17acbc5f05571cef1a40e4765444e8da`.
- `manuscript/native-review.png`, SHA256
  `35f4093e11869b10468864c8cbf24d41d1b88fbf986df20ef8b6d2a8e0615a5f`.
- `manifest.json`, SHA256
  `25da26944492557d0523d530d94772d113178af27da8aed6338e54d79dbfd836`.

New README/REVIEW_STATUS document tools, CC0/provenance, actual inspection,
partial binding contract and limits. No rerasterization/repeatability forV2 yet;
A/B86-file repeatability does not transfer. Sending exact paths to Dispatcher,
Frontend and Content for actual visual review/user choice. Next: receive concrete
choice/rejection, then approved-example style guide and chosen-family refinement;
all20 final assets, technical repeatability/independent GUI and explicit final
user approval still required. No further heavy batch without Build coordination.

### 2026-09-07 — Frontend actual V2 sheet review

Frontend actually viewed all3 V2 sheets: distinct illustrative subjects replace
orb/shield; header/topmargin/compact pair visually fit existing contract, not GUI
proof. Remaining hard facets are not finished painting. Study32 is cramped and
book risks reading Knowledge; retain instrument/candle distinction if chosen.
Conjurer32 silhouette is recognisable but anatomy/floating page need refinement.
Manuscript32 reads folio while celestial scene is largely lost. Tab states still
rely mainly on cloth value, requiring later composed-book review. No style/user
approval, full-family request or import authorization. Record these concrete
caveats for whichever direction user chooses; await arranged choice/rejection.

### 2026-09-07 — Content independent V2 static PASS, no visual acceptance

Tester actually read all3 native sheets and full paint.py/README/REVIEW_STATUS.
Independent `commands-static/sorcery-v2-independent.json` checks15 PNG/SVG pairs:
hashes, dimensions, RGBA, clear rim, top28 and allowed SVG geometry/no external
references PASS. Subject distinction confirmed; angular planes are not finished
painterly treatment,32px details limited and ranks unassigned. No independent
regeneration, GUI, full-family or user-choice claim. Corrected V2 README's stale
'Retry awaits Build slot' to explicitly historical wording with actual later retry0;
preserved initial RED, all reviewed art/source/manifest bytes unchanged. Next still
Dispatcher-arranged user choice/rejection before style guide or further batches.

### 2026-09-07 — superseding painting brief; capability gate, not more batches

User rejects angular V2 as well as glossy A/B. Read full NH_SORCERY_STYLE_BRIEF;
all prior worker preferences/technical style comments are historical, no approved
motif. Current goal requires one credible high-resolution original master plus
actual44/32 reductions before full-family work. Frontend confirms reserved live
paths and the corrected sequence. No new flat/pixel batch generated.

Actual bounded capability inspection: GIMP3.2.2, Inkscape, ImageMagick, Pillow and
NumPy available; Blender/Krita/POV-Ray/LuxCore/Mitsuba executables and bpy/mitsuba/
torch/diffusers/trimesh/pyrender/vtk/moderngl modules not found. Local apt metadata
reports Blender not installed, candidate5.0.1+dfsg-1ubuntu1. No installation,
download, GUI or image-generation service used. GIMP presence is not evidence of
agent manual-painting skill; do not claim brushwork or a human commission.

Isolated `PRODUCTION_METHOD_REVIEW.md` gives concrete options and honest limits.
Recommended test: user/admin authorizes Blender install or supplies executable,
then Build schedules bounded headless render of one originally modeled still-life
scene at768 square, native44/32 reductions and editable .blend/source/material/
lighting settings. Proposed book/warding-key/cloth motif is merely a new hypothesis,
NOT user choice. Physical renderer availability still cannot guarantee painterly
quality; actual proof must be inspected/approved. Alternatives: user-run original
scene or real rights-cleared layered artist master; no invented hired artist,
paid service/account/proprietary upload. Asked user for Blender approval/location
and sending requirements to Dispatcher/Build/Frontend. Next executable step once
method available: verify headless renderer and request bounded proof-render slot.
All full-family, reproducibility, integration, sole Content GUI and final explicit
user-approval requirements remain open. Preserve rejected drafts/candidates.

### 2026-09-07 — authorized Blender method; ONE actual master proof

User approved installation; independently verified Blender5.0.1. Authored isolated
`still-life-proof-v3/scene.py` original curved page/rounded leather/old silver key/
cloth mesh geometry, material shaders, lights and camera; no reference inputs,
image-generation tool or manual-painting claim. `reduce.py` provides straightRGBA
native outputs with premultiplied-alpha Lanczos filtering, no stretching.

Build explicitly granted ONE180sTERM/+10kill CPU2threads32samples768 render.
Actual command: `timeout --signal=TERM --kill-after=10s 180s blender --background
--factory-startup --threads 2 --python assets/new-horizons/sorcery-art/still-life-proof-v3/scene.py -- --samples 32`.
Actual EXIT0 elapsed18s; reduce.py EXIT0; pgrep exact blender empty, slot released.
No second render. Log/exit in ignored `research/sorcery-art/v3/`. Deprecation
warnings for future Blender6.0 use_nodes preserved, not a current render failure.

Metadata scan caught RAW master path metadata (privacy RED). Kept raw PNG/.blend/
settings private and locally ignored; created clean master-review PNG with identical
RGBA pixels, no metadata; regenerated native reductions from clean pixels only.
All5 review PNG metadata dictionaries empty, `v3/image-audit.json`. No private .blend
or raw file publication permission; corresponding original scene.py available,
.blend remains editable but must receive independent privacy review first.

Artist actually read master and native sheet. Real object volume, thickness,
reflections, folds and lighting are now present. NOT yet user-approved painterly
quality; left page notation mostly hidden (suspected normal/solidify ordering),
fine32sample shading grain and key contact/junction need review. Book dominates32,
Sorcery-versus-Knowledge identity unproven. No motif approval, style guide or full
family inferred. Fixed renderer settings do not prove repeatability; rerender not
performed. Full provenance/limits/command in new V3 README.

Exact safe download paths under
`assets/new-horizons/sorcery-art/still-life-proof-v3/output/`:
- `master-review.png`768square SHA256
  `92837278c0101bd83f6b727990c89d3f630572da787c7ee9796e77f3741c909f`.
- `native-review.png`actual44/32/82x93 sheet SHA256
  `3bcfead9ef6ecbde1746fbdb0fe74a0f8b921ae95254bdf5b6ab97545056f45f`.
- Individual `native-44.png`, `native-32.png`, `slot-82x93.png` and hash manifest.

Notify Dispatcher/Frontend/Content with safe paths for actual user quality review,
not raw master/.blend. Next external event: explicit quality/motif feedback; no
rerender/full family before coordinated decision. Build now reserves BEnegative/
restore/clean6 job, Artist no heavy work. All final20-family, reproducibility,
Frontend/Build integration, sole Content GUI and explicit final user approval
remain required; rejected rounds and frozen candidates preserved.

Frontend independently actually viewed cleaned V3 master/native: clear physical
volume/occlusion/material separation improvement, book/cloth read44/32; key becomes
weak gray page detail32. Large paper areas/regular text still feel rendered rather
than painted; grain/page-block edge require user quality judgment. No approval or
extra render requested. Preserve proof/clean pixel identity; wait user feedback
before family/style guide/import. Dispatcher/Content sent safe paths and requested
non-goal feedback wake; no heavy work during BE lease.

Dispatcher actually read V3 master/native and is arranging user review by SCP.
Advisory critique, NOT approval: book-first/key weak32; blank left page and regular
right dash marks feel unfinished/procedural; materials too new and light too soft
for strong fantasy chiaroscuro; tighter native composition may help. Preserve
exact proof, no extra render/full family before actual user feedback and Build
slot. Dispatcher explicitly owns relaying that user quality/motif direction.

### 2026-09-07 — actual user V3 direction; V4 illustrative test/geometry RED

User says V3 is undoubtedly closer but still too photorealistic. Read updated
style brief: retain modeled volume, change finish toward illustration; no motif/
family approval. New isolated `illustrated-proof-v4/` source uses broad authored
object-space pigment fields (no noise/filter), restrained specular, selected silver
accent geometry, stronger grouped warm lighting, richer blue/carmine, larger key,
tighter camera and corrected left-page normals/flowing sepia phrases. Actual
procedural shader/render method, NOT claimed hand painting. V3 exact manifest
hashes rechecked unchanged; no live writes.

Build granted ONE180s/+10CPU2thread32sample768 render; actual EXIT0 elapsed19s,
reduce0, exactBlenderPID none, slot released. Read real master/native comparison.
Actual **geometry RED**: enlarged tilted key bow intersects corrected left page,
leaving broken-U silhouette. Render0/metadata success is not visual PASS. Preserve
V4 source/output bytes and `research/sorcery-art/v4/visual-red.json`. CleanPNG
metadata empty/raw-clean master pixels identical verified. No user-quality claim
or presentation of that defect as deliberate illustration.

Requested Build one separate repair-only<=60s/+10 slot, NOT started. Prepared new
`illustrated-proof-v4-keyfix/scene.py` SHA256
`da808e2d52f3c2809ad23111fccba9d90c31fd24d49404fd858c4122bb7d64a8`:
exactly one geometry line changes key plane to z.875/XYrotation0, all V4 style,
materials/light/camera unchanged; reduce.py remains hashf7f934. Source syntax0.
Await explicit Build GO before render. Then inspect complete bow/contact/master
and native44/32 comparison before Dispatcher user quality review. No full family,
style acceptance or repeatability inferred; all final gates remain open.

### 2026-09-07 — one authorized V4 geometry repair inspected, ready for user review

Build reverified exactda808e2d scene/f7f934 reduction and one-line delta, granted
ONE60sTERM/+10kill CPU2threads32sample768 repair. Actual render EXIT0 elapsed19s,
reduce0, exactBlenderPID none; slot released. No subsequent render. Read actual
master and native comparison: bow now complete closed loop; prior broken-U/page
intersection not visible. This is visual repair evidence, not comprehensive mesh
collision certification or painting acceptance. Grain/contact/regular writing and
still-rendered appearance remain explicit quality limits.

V3 and firstV4 all manifest hashes rechecked unchanged. All6 clean review PNGs have
empty metadata; raw/clean master RGBA identity verified. Raw master/.blend/settings
private/ignored pending independent privacy review; no publish permission inferred.
Evidence `research/sorcery-art/v4-keyfix/{render.log,exit.txt,audit.json}`; actual
method/provenance/limits recorded in new keyfix README. No rerender-repeatability
claim, live edits, game launch or commits.

Safe paths under `assets/new-horizons/sorcery-art/illustrated-proof-v4-keyfix/output/`:
- `master-review.png`768square SHA256
  `3d9aa573ddab127df63bc23f268913c6f23e44e327388dd83304c77cf1ab63e0`.
- `native-comparison.png`actualV3/V4 44/32 SHA256
  `b73962242af65e500d319f4fa4682a834f99c46e26fe6d4cb743dfd5423bb10d`.
Sending Dispatcher/Frontend/Content these exact files for actual user comparison,
not raw exports. User's 'closer but too photorealistic' is the only current quality
direction, not motif/final approval. Next arranged external event: explicit user
feedback before further render/family/style-guide expansion; all20-family technical,
integration, soleContent composedGUI and explicit final approval still required.

Frontend actually viewed V4keyfix master/native comparison: larger closed bow/shaft
makes key more identifiable32 than V3; warm paper/blue cover/red cloth separation
retained. Continuous bow visible, not full geometry proof. Grain/contact shadow
and matte uniform key material remain user-quality questions, not visual PASS.
No additional batch/style guide/import requested. Honest shader/render versus
manual-painting distinction retained; await arranged actual user feedback.
