# Post-submission verification — concepts remain unaccepted

After Build MASTERYSAVE teardown, copied only exporter into isolated ignored
`build/new-horizons-linux/research/sorcery-art/repeatability/` and ran there.
Actual export EXIT0. Compared all86 generated files (40SVG +40PNG +4sheets +
exporter +manifest) byte-for-byte to submitted sources: all identical. Original
submitted files were also checked against saved SHA256 baseline and preserved.
Evidence: `research/sorcery-art/repeatability.json` under ignored Linux build root.
This supersedes README's chronological 'repeatability not yet checked' statement.

A new, stricter read-only `audit.py` binds sources/PNGs to manifest, checks all
sizes/modes/top margins, unique states/ranks and forbidden SVG external/raster/font
content. Six synthetic negative controls reject wrong size/mode, blank, opaque,
dirty header margin and clipped edge. It also requires a completely clear exterior
pixel rim for non-header assets. **Actual audit EXIT1 / RED** on16 concept PNGs:
both families'3 small skills and emblem/4buttons touch a canvas edge with partially
transparent antialiasing. Small skill top maximum alpha1/bottom51; medallion bottom
maximum119. Existing dimension/transparency checks had not detected this stricter
edge condition. Do not claim these concepts ready for production import.

Preserved reports: `static-audit.json` and `static-audit-red.json` in ignored review
root. The submitted concept PNG/SVG/exporter/manifest bytes remain unchanged.
Next chosen revision must move rank rail upward/inset small composition and inset
medallion/drop-shadow; fix geometry, do not clear a clipped silhouette post-render.
Re-run strict audit and repeatability against new revision with unchanged originals.

Mean masked luminance on native bookmarks: A selected61.588/unselected49.737;
B selected63.562/unselected51.069. This measures a difference, NOT evidence the
selection is sufficiently legible in composed UI. Dispatcher already identified
subtle states and requested stronger material/value difference. Actual-size
Content review and explicit user visual approval remain mandatory.

Dispatcher's pixel review prefers A, but that is NOT user choice or approval.
They are asking the user A/B. Need a richer unique header scene, deliberately
placed aged-brass/velvet pixel finishing and physically distinct rank progression.
Do not overwrite either submitted concept while waiting. No live integration,
product edits, game launch or commits by Artist. All other workers retain goals.
