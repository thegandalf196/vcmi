# Academy map materials — revision v2

Status: Provisional; installed in source. User in-game aesthetic acceptance remains
pending; launcher delivery is recorded separately in the priority queue.

User-approved direction (UP240): preserve the existing Academy architecture and
silhouette while reducing its overly smooth finish. The first fort material edit
is in `masters/fort.png`. It was generated with the built-in image generator using
the HoMM3 Art skill and the previously authored `masters/adventure/avctowx0.png`
as its edit target. No original-game colour extraction is included.

Corresponding Village and Capitol masters are preserved with exact prompts in
`masters/`. They use their respective previously authored sprite as the edit
target, with the fort draft as a material reference only. All three returned
masters are 1254×1254 RGBA images with transparent exterior.

Root inspected each master and each before/after native 192×192 comparison:
masonry has deeper crevices and varied worn stone, roofs use less uniform
slate/teal. The existing architecture, entrance, footing and pennants are retained.
Mechanical exports use the exact prior registered master and destination boxes,
not arbitrary alpha bounds including incidental low-alpha shadow.
Runtime ownership flags and shadows must retain their existing external-resource
composition; no gameplay, entrance or blocking changes are authorized here.

`tools/export_new_horizons_academy_map_v2.py --check` reproduces exports and native
comparisons from retained authored v1 masters, independently of the active runtime
images. The importer pins `manifest.json`, including source registration, original
authored and revised master hashes, exact prompt hashes, geometry and export hashes.
It installs all three reviewed body exports, rejecting unknown replacement pixels
before changing any body. Reimporting the supplied handoff cannot revert v2.
The eight focused art tests, importer check, exporter check and independent source
review pass. The renderer's existing external ownership/shadow composition is unchanged.

The prior supplied art and its provenance remain intact. This directory does not
assign a new licence to the underlying supplied artwork or claim user acceptance.

## Exact generation prompt

Use case: precise-object-edit. Edit target: existing authored Academy adventure-map fortified town sprite. Change ONLY material finish and light/shadow texture. Keep EXACT canvas, architecture, silhouettes, tower positions and heights, teal conical roof shapes, windows, battlements, entrance, rocky footing, tiny yellow ownership flag positions, orthographic camera and transparent exterior. Make this sprite fit the rugged late-1990s prerendered Heroes III adventure map rather than looking polished and modern. Limestone masonry should be uneven and weathered: restrained ochre/earth-grey variation from stone to stone, deeply shadowed narrow mortar gaps, scattered small chipped edges and worn patches. Roof shingles dull oxidized teal/slate with subtle irregular tile color rather than uniformly shiny teal. Strengthen compact crevice shadows and selectively reduce broad smooth highlights; upper-left light direction unchanged. Ground rocks are rough angular weathered stone, subdued enough to merge into original map scenery. No redesign, no new ornaments or buildings, no thicker spires, no blanket noise or grain overlay, no artificial sharpening halo, no added border or text. Preserve dense miniature modeled fantasy rendering. One complete isolated sprite with genuinely transparent exterior. Preserve aspect ratio and framing; do not crop any tower or footing.
