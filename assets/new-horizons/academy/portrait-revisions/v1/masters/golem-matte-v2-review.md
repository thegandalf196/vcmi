# Golem matte V2 review — 2026-10-06

These built-in ImageGen geometry-only edits are retained as **unapproved,
rejected runtime candidates**. They do not close UP-251 and must not be
registered. The original V1 masters/mattes and runtime bindings are unchanged.

The exact edit prompts are beside the masters:

- `ironGolem-matte-v2.prompt.txt`
- `stoneGolem-matte-v2.prompt.txt`

The 58×64 binary masks in `../mattes/ironGolem-v2.png` and
`../mattes/stoneGolem-v2.png` were mechanically reduced from these masters
with the existing LANCZOS resize and threshold-at-128 rule. Each mask was
checked for exact reproducibility from its master.

Review used the ignored native and nearest-neighbor 8× comparisons in
`build/nh-up251-validation/golem-matte-v2-review/`, compositing only the
external original frame over the currently authored Academy backdrop. No
original-color creature pixels are stored here.

- `ironGolem` internal ID 32 uses external frame 34, displayed as the Stone
  Golem. V2 changes 30 native mask pixels (28 white-to-black, 2 black-to-white),
  but the pale/snow-like fringe around the head and shoulder remains visible;
  this is not a material correction.
- `stoneGolem` internal ID 33 uses external frame 35, displayed as the Iron
  Golem. V2 changes 94 native mask pixels (84 white-to-black, 10 black-to-white)
  and visibly nicks genuine dark forearm/armor contour; do not install it.

The originals and both V2 attempts are preserved for comparison. Native-size
acceptance, correct runtime bindings, playable delivery, and user visual
acceptance remain pending.
