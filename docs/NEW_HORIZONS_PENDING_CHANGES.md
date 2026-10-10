# New Horizons Pending Changes

New Horizons.md is the sole canonical design specification. This document
contains only temporary amendments awaiting integration into its appropriate
sections; it is not a second permanent specification.

For each amendment record its user-approved decision, affected canonical
section, unresolved questions, and integration evidence. Remove an amendment
only after integration is verified, or an explicit decision supersedes it.
Implementation status belongs in the completion audit, not here.

The completed legacy Overrides transition is retained as history in
[NH_OVERRIDE_MIGRATION.md](NH_OVERRIDE_MIGRATION.md). Do not copy its retired
entries here and thereby recreate a permanent override layer.

## Awaiting integration

### Inteus and Halon — remaining removed starting inscriptions

Provisionally, Inteus replaces removed Bloodlust with existing Crusade! for
fresh default inscription and specialty. Apply the established +20% non-damage
specialty conversion only to Crusade!'s Spell Power-derived offensive/defensive
components, preserving its fixed terms, caps, duration, target shape and costs.
The army-wide successor is an intentional provisional change from Bloodlust's
single-target offense, not a new spell or a numerical compensation rider.
Halon replaces his removed Stone Skin default inscription with existing Guardian
Spirit. This is book-only: retain Metamagic Adept as his sole specialty, with no
additional enchantment scaling. Apply these replacements only to fresh default
books under captured explicit opt-in; preserve map books, saved/crossover and
legacy contexts, class, other development, armies and biographies. Coronius's
replacement remains a separate authored gap, not implicit approval of a proposal.

### Iron Will — recipient carry and same-Order replacement

Provisionally, an unspent and unbroken end-round Order benefit carries separately
for each eligible recipient through its next genuine completed Creature
Activation. Wait and same-activation continuations do not consume that carry;
an incapacitation that actually forfeits the activation does. Time Stop without
an activation does not expire it. Do not revive spent Charge, broken Protect or
completed Second Wind. Reissuing the same Order replaces its prior recipient
snapshot, including carried benefits, rather than preserving parallel instances.
Other Order identities keep their ordinary coexistence rules. Use the shared
effective-benefit lifetime for authoritative execution, previews and detached AI.

### Reactive Weave — independent nonstacking readiness

Provisionally, an accepted enemy Hero spell that actually affects this hero's
army arms half the normal Spell-to-Order Warcasting empowerment, rounded down,
through the end of the next round. Rejected casts and casts with no actual army
recipient do not arm it. Keep ordinary and reactive readiness independently:
the next accepted Order uses the stronger eligible bonus, never their sum, and
consumes both matching readiness candidates. A reaction must not extend or
overwrite stronger ordinary readiness; each candidate retains its own expiry.
The reactive trigger does not count as this hero accepting a Spell, advance an
alternating-action sequence, or grant a Hero Action. Apply existing consumption
perks once to the chosen readiness, not independently to both candidates.
Review readiness coexistence and affected-recipient classification in Phase2.

### Eight retired-development hero starts — explicit captured profiles

Provisionally retain each hero's current Basic faction Skill and replace its
otherwise retired generic starting development with these existing legal choices:

| Hero | Generic starting Skill | Selected Basic perk |
|---|---|---|
| Clancy | Basic Logistics | Pathfinding |
| Piquedram | Basic Logistics | Scouting |
| Thane | Advanced Learning | Scholar |
| Torosar | Basic War Machines | Master Gunner |
| Iona | Basic Learning | Scholar |
| Fiona | Advanced Logistics | Scouting |
| Ignatius | Basic Battlecraft | Tactics |
| Lacus | Advanced Battlecraft | Tactics |

Preserve Advanced parent ranks where an Advanced legacy start is being replaced;
do not invent an Advanced perk. The existing exceptional rank-advancement rule
allows the unfilled slot. All chosen parents are legal for the unchanged class
and all perks are currently active. The faction Skill replaces the retired
second generic choice; no hidden Wisdom/Mysticism/Resistance grants are added.
These are explicit default-start profiles, not a global migration policy.
Capture an optional profile collection in the hero rules, applying it only to
fresh creation with default Secondary Skills. Explicit map starting rosters,
saved/crossover initialization and captured legacy or absent-profile contexts
remain unchanged; do not apply prototype perks unconditionally to a roster
without its parent. Preserve class, army, biography, spellbook and specialty.
Reject malformed profile/perk/parent admission and unsupported old-format key
presence before enclosing serialization prefixes. Review hero differentiation
and Advanced empty-perk-slot pacing after functional coverage is established.

### Loynis and Zubin — authored offensive-enchantment replacements

Loynis provisionally replaces removed Prayer with the existing Light Crusade!
for fresh default inscription and specialty. Crusade! is the authored successor
to army-wide Prayer. Apply +20% only to its Spell Power-derived Attack, Defense,
Initiative and Magical Damage Reduction components, once before existing floors
and caps. Preserve fixed bases, duration, target eligibility, costs and actions.
Zubin provisionally replaces removed Precision with existing Sorcery Focus Magic
for fresh default inscription and specialty. Apply +20% only to its numerical
Spell Power-derived penetration component; preserve fixed10%, cap20%, duration3,
first-shot handling, post-hit Arcane Breach marks and mark cap3. Neither conversion
adds a separate Masterful spell or hero-level rider. Preserve current class,
biography, starting Skills/army, map-prescribed books and captured legacy rules.
Existing legitimately inscribed combat-spell casting governs their known starts;
these replacements grant no unknown spell or ordinary acquisition exemption.
Review high-tier starting impact and enchantment/perk composition in Phase2/3.

### Halon — additional Metamagic capacity without additional mastery

The selected Metamagic Adept specialty grants exactly one additional use per
combat at each actual learned Metamagic rank. Preserve Halon's selected Basic
Metamagic/Basic Spellcraft start and existing specialty bonus; do not restore
Mysticism. Basic/Advanced/Expert capacities become2/3/4, respectively, while
actual mastery remains Basic/Advanced/Expert. Extra capacity does not unlock
Expert-only Grand Metamagic or bypass its perk requirement. A hero without
the learned faction Skill receives no capability merely from a capacity bonus.
Keep ordinary heroes'1/2/3 capacity unchanged. Accepted follow-up consumption,
pending grant expiry, cancellation and Counterspell semantics remain unchanged.
Separate capacity from rank across authoritative transitions, detached forecasts
and UI. Capture any changed rules/state admission explicitly; unsupported old
formats must reject unrepresentable state before writing prefix bytes, not lose
the fourth use silently. Review this provisional clarification after focused
Basic/Advanced/Expert and saved-state controls. Halon's removed Stone Skin start
is a separate unimplemented replacement decision, not addressed by this repair.

### War Machines — selected shots, overflow geometry and repair scope

Precision Bombardment provisionally locks a Catapult's explicitly selected legal
wall/gate/tower part. Basic War Machines retains its existing manual control;
the perk's distinct benefit is that an accuracy miss causes no damage instead
of redirecting to another part. Preserve accuracy, damage-quality and Siege
rolls; it grants no guaranteed hit. Stop later shots once the selected part is
destroyed rather than silently choosing another target. Ordinary unselected and
captured legacy behavior remains unchanged.

Breachmaker uses this explicit outer-line neighbor order:
bottom tower — bottom wall — below gate — gate — over gate — upper wall — upper
tower. The central keep is not an outer neighbor. Only destruction of a wall or
gate by an actual controlled hero Catapult strike qualifies. Use applied final
structural damage exceeding its positive pre-hit HP; carry floor(excess/2) once
to the surviving destructible adjacent part with lowest positive current HP,
breaking ties by fixed fortification order. No further overflow or repeated
Siege scaling occurs. Primary tower hits, spells, creature abilities, zero
excess and non-Catapult damage do not trigger it. Destroying the chosen neighbor
tower also removes its real defensive shooter through ordinary authority.

Field Workshop repairs existing surviving damaged allied war machines and
friendly defended-town structures, including towers, using full ordinary
Siege-scaled Tent output capped by missing HP. It does not rebuild destroyed
structures or restore fallen war machines. Resolve structural tower targeting
before treating its hex as an ordinary creature-healing target. Preserve normal
troop healing and reduced-output extra-activation rules; casualty restoration
and affliction cleansing do not apply to repairs. Actual HP state, manual/AI
structure-only eligibility, previews and wall-sprite refresh must be delivered,
not merely target labels. These choices are provisional; focused implementation
and native evidence must precede canonical integration.

### Recruitment training — provisional stack-level interpretation

Drill Sergeant, Field Instructor and Reinforcement Drill operate on the whole
resulting strategic stack after a positive direct recruitment into the hero's
army, including recruitment into an existing matching stack. No per-creature
cohort accounting or additive duplicate training bonuses is introduced.
Same-hero splits and merges preserve training receipts; merging combines
eligibility/trained flags without multiplying bonuses. Drill Sergeant retains
the later pending deadline when two eligible stacks merge. Slot reordering is
not a transfer. Actual army-boundary transfers permanently remove Field
Instructor and Reinforcement Drill eligibility/benefits from the moved portion;
Drill Sergeant follows the troops because its wording does not require continued
residence with the recruiter. Internal temporary detachment is not a boundary.

Drill Sergeant gives +1 Morale in the first actual combat during recruitment
day through day+6 inclusive, consuming eligibility even if immunity or a cap
prevents a benefit. Field Instructor gives surviving original strategic troops
+1 Creature Attack only after completing their first combat under the recruiter,
including a retained retreat/surrender army, and only while continuously in that
hero's army. Reinforcement Drill includes Champions: at accepted battle entry,
the lowest original army slot among eligible newly recruited stacks consumes
the hero's one weekly use and receives +2 flat Initiative in round1 only.
Recruitment may arm a resulting stack again, but never stack the same bonus.

Both paid recruitment and genuine free external-dwelling recruitment qualify;
creature transfers, rewards, resurrection, Diplomacy joins, Necromancy, summons
and merely increasing a dwelling pool do not. Existing category, Leadership,
payment and pool validation remain unchanged. Required pending/trained creature
feedback, typed receipts, save guards and shared combat/AI stat consumption
must be implemented and focused evidence accepted before canonical integration.
These choices are provisional under the user's explicit judgment policy.

### Merist and Labetha — provisional defensive specialty replacements

Under the user's provisional-rule authorization, replace removed Stone Skin
in fresh default starts and specialties with ordinary Hydra's Vitality for
Merist and Guardian Spirit for Labetha. Merist retains a Nature-oriented defense
spell for living Fortress troops; Guardian Spirit also protects Labetha's
nonliving Elementals. Apply +20% only to each spell's SP-derived numerical
component. Hydra's fixed25%, maximum50%, three-round duration and regeneration
rate remain unchanged; Guardian Spirit's fixed50HP and two-round duration remain
unchanged. Preserve existing School/perk staging, other profiles, map books and
captured legacy contexts. These are authored provisional identities, not the
workbook's undefined Masterful variants. Independent review and focused live/
detached/default/map/legacy/save evidence must precede canonical integration.

## Integrated history

### Contacts, Phoenix Spark, Arcane Memory and Aenain — 2026-10-09 (integrated)

The canonical rows now record owned-entry/first-empty-row growth, actual scroll
completion and ordinary acquisition, and fixed battle-start Phoenix substitution
with once-use placement semantics. The hero section records Aenain's SP-only
Frailty replacement and preserved default/map/legacy boundaries. Independently
reviewed production and fixture repairs link14567; exact retry2 principal34618
passes42/42 in13.975s and adjacent26046 passes23/23 in8.785s, zero failures,
errors or skips. Initial failed logs/XML remain private. Provisional choices
remain reviewable in the second-look ledger; implementation and playable
delivery are distinguished in the queue.

### Sage catalog and four Frailty specialties — 2026-10-09 (integrated)

Both Sage rows now state the eligible undisplayed catalog, saved school labels,
ordinary learning/map-ban rules, deterministic selection, first built-Guild
visit receipt and separate reveal rows. The canonical hero-profile audit names
Cuthbert, Olema, Mirlanda and Xsi's existing Frailty replacement, SP-component
conversion, unchanged caps and preserved default/map/legacy boundaries.
Independent source review and exact native70790 pass36/36, including Sage10,
Frailty11 and Shared Purpose15; adjacent61175 passes12/12 after linked38972.
Eligibility, initial corpse provenance and variant prerequisites were preserved
through reviewed fixture-only repairs. These provisional choices remain in the
second-look ledger; other missing hero identities remain separate gaps.

### Thant — authored provisional specialty replacement — 2026-10-09 (integrated)

Integrated into the canonical hero starting-profile audit: existing Re-animate
replaces removed Animate Dead in fresh default starts and specialty, +20% only
to its SP-derived restoration component. Fixed220, temporary casualty rules,
map-prescribed spellbooks, legacy contexts and other profile choices remain.
Source review and ten principal cases pass in native88843; fifteen adjacent
controls pass in3070 after linked25787. Broader casualty/cap composition remains
in the second-look ledger; no new rendered or playable acceptance is inferred.

### Polymorph impossible-footprint restoration — 2026-10-09 (integrated)

Provisional decision under the user's authorization to resolve rule ambiguity:
Polymorph normally restores its original body after two rounds or Dispel, using
the approved nearest legal position when necessary. If no legal position for
the original footprint exists anywhere, retain the current form, surviving HP
and position; retry safe restoration at later round boundaries. Never overlap
another stack, delete creatures or heal them to force restoration. This is an
exceptional delayed restoration, not a new normal duration or a successful
immediate Dispel. It must be represented accurately in status/help text.

Affected canonical section: Chaos School / Polymorph, restoration and duration.
Second-look question: whether another explicit no-space policy is preferable.
Integrated into Chaos / Polymorph together with the Phantom body/Integrity
distinction and explicit Shapeshifter independent draws/whole-stack Army Value.
These reasoned interpretations remain in the second-look ledger. Production
implementation and focused evidence remain separately tracked; integration of
wording is not gameplay completion.

### Elemental Convergence terrain completion — 2026-10-09 (integrated)

User approves Earth for Dirt, inland Sand and Wasteland, and Water for Swamp
and coastal battlefields including coastal Sand. Integrated into the canonical
Experimental Values terrain table, with captured coastal battlefield context
taking precedence over forced Sand. Runtime and AI implementation of the spell
and its terrain-dependent perks remain UP072 work, not completed coverage.

### Battlefield Mastery and Last Stand scope — 2026-10-06 (integrated)

User resolves Battlefield Mastery's award in favor of the first eligible ordinary
stack: an ineligible War Machine leaves it available. Last Stand protects ordinary
stack health, not clones/Phantom Integrity; when lethal retaliation triggers it,
the surviving attacker's current activation ends. Integrated into both canonical
perk rows. Production completion and delivery remain separate in UP-156/UP-079.

### Both Cabir forms are ranged — 2026-10-06 (integrated)

User explicitly directs both Cabir and Cabir Master to shoot. Apply to the
canonical Academy creature roster/ability section; this supersedes inherited
basic Gremlin melee-only gameplay. Preserve both forms' elemental defenses and
Master's repair ability. Ranged art and ordinary ammunition/targeting must be
implemented together; no implication of No Melee Penalty is granted.
Integrated into the canonical Academy creature ability paragraph and roster row.
Source/runtime and art acceptance remain tracked in UP-265; this document change
does not claim shooting animations or playable delivery are complete.

### Barehanded Cabir and repair abilities — 2026-10-06 (integrated)

User explicitly removes the golden pot/fire vessel from both forms. Both get
Fire resistance and Water weakness; Cabir Master repairs Golems and Gargoyles.
Integrated into the canonical Academy creature presentation/ability rule,
superseding the initial unchanged-gameplay restriction for these specified
abilities only. User subsequently approves provisional50% less Fire damage and
25% more Water/Frost damage, and healing plus restoration of fallen creatures
within a surviving stack. These answers are integrated in the same canonical
rule. The canonical implementation prototype now specifies one repair per
combat, 10 HP per acting Cabir Master and a normal creature activation. These
remain tunable values; implementation and artwork status remain in UP253.

### Cabir replacement — 2026-10-06 (integrated)

User-approved decision: replace Academy's Gremlins and Master Gremlins with
original Cabir and Cabir Master artwork and names, retaining the current
creatures' gameplay initially. Integrate into the canonical Academy roster;
do not invent new stats or abilities from the Heroes VII reference. Full
base/upgraded battle animation sets and all creature presentation bindings are
required, not just portraits. Original artwork must use HoMM3 Art, including
provisional assets. Integrated into the canonical creature roster and its
Academy presentation rule. Implementation and delivery are tracked in UP248;
the approved standing-frame draft is not a completed runtime animation set.

### Academy visual identity — 2026-10-05 (integrated)

The user supplied the Academy definitive art handoff and requested integration.
Its visual direction is integrated into the canonical Tower section: Academy
display name and scholarly sandstone presentation, existing Tower identity and
New Horizons gameplay preserved. The user separately confirmed Sand as Academy's
native terrain; existing authored map terrain is not repainted. Original retained pixels remain externally
referenced. Asset integration and playable evidence are tracked in UP-235.

### Crown and Altar automatic second-action bonus — 2026-10-05 (integrated)

In response to predeclaring a pair target versus redesigning the perk, the user
preferred the less-clicky option. The canonical perk now automatically boosts
the second action's rating-derived components by20% on friendly recipients
also affected by the first, in either pair direction. No additional button,
target-preselection dialog or retrospective first-action change is introduced.
The first action is unchanged. Integration verified in the Divine Mandate perk
pool; its planned registry description is synchronized. Runtime implementation,
recipient provenance, AI and focused evidence remain work tracked in UP108/
UP023, not claimed complete by this specification change.

### Commanding Presence effective lifetime — 2026-10-02 (integrated)

User-approved decision: its negative-Morale floor ends for a recipient when
that recipient's Order benefit is spent or broken. It does not persist solely
because the Order snapshot remains until round end. Examples include a consumed
Charge, a broken/exhausted Protect pair, and the end of Second Wind's extra
activation. Affected canonical section: Command perk pool, Commanding Presence.
No unresolved lifetime question remains. Integrated into the canonical Command
perk pool's Commanding Presence row. Implementation and validation belong in
UP-142, not in this amendment.

### Polymorph footprint relocation — 2026-09-30 (integrated)

The user chose relocation to the nearest legal position when a replacement
footprint cannot fit at the original hex. Integrated into canonical Polymorph:
do not exclude the form solely for its original-position footprint; retain
ownership, allegiance and current Initiative queue position. Runtime coverage
and the shared form/HP foundation remain tracked under UP-066.

### Paradox Shield and damage caps — 2026-09-30 (integrated)

The user selected the existing physical cap: Paradox Shield adds ten percentage
points after the spell's own formula cap, but total Physical Damage Reduction
still cannot exceed 80%. Magical protection can reach 90%, subject to its
ordinary 95% total cap. This clarification is integrated into the canonical
Shield of Chaos section; implementation evidence belongs in UP-063.

### Hand of Fate secondary mitigation — 2026-09-30 (integrated)

User-approved decision: after selecting the secondary recipient uniformly from
the surviving friendly/enemy pool, apply that recipient's own magical defenses
to the hit whose base is half the primary target's actual HP loss. Defenses do
not affect selection and must not cause a reroll. This clarification is integrated
into the detailed Chaos / Hand of Fate section of New Horizons.md.
Runtime implementation and delivery remain tracked in the priority queue.

### School-rank spell potency — 2026-09-27 (integrated)

Basic, Advanced, and Expert rank in each of the six Magic Schools must
progressively strengthen applicable spells of that school, in addition to
gating ordinary acquisition of higher spell levels. A legitimately inscribed
spell remains castable without the rank. Begin with a modest, coherent
Heroes V-like damage rule: improve the coefficient that multiplies Spell Power,
not merely flat base damage. Expert rank does not automatically grant Mass
versions; those remain perk-granted. For non-damage spells, choose meaningful
effect-appropriate rank improvements, with explicit exceptions instead of a
blind numerical multiplier. The initial authored coefficient ladder (provisional
balance) is: no School rank 100%, Basic 115%, Advanced 130%, Expert 145% of
the spell's Spell Power coefficient. Apply it before existing integer rounding;
preserve flat base terms, caps, costs, target shape, mitigation, and specialty
rules. For a multi-school spell, use the highest applicable rank once, never
stack the schools. Adventure Spells remain neutral and unscaled. Saved magic
rules version 3 carries the ladder; v1/v2 saves retain 100% so an ongoing game
does not silently change its formulas. Numeric healing, temporary HP, and
restoration may follow the same coefficient principle where the formula has an
actual Spell Power term. Discrete/binary spells need authored rank variants or
an explicit exception. The shared rule is now in the canonical Markdown Magic
Skills section; implementation and validation of specific spell effects remain
tracked in UP-027.

The five amendments approved before 2026-09-27 were integrated into the
canonical DOCX: Spell Lock duration stacking, Arcane Acquisition target
semantics, generic Faction-Skill combat statuses, consume-on-use Metamagic and
its accompanying perks, and ordinary Mage / Arch Mage melee penalties. The
edited document passed ZIP integrity and a complete 191-page LibreOffice render;
the affected pages were visually inspected without clipping or overlap.

### Bulwark of the Mire perk rules — 2026-09-27 (integrated)

Affected canonical section: Fortress faction Skill, Bulwark of the Mire perk
table. User-approved changes integrated into the repaired canonical
`New Horizons.md`:

- Toxic Spines: “the first melee attacker each round” is tracked separately
  for **each Defending Bulwark stack**, not once per hero army. That attacker
  must suffer Bulwark reflection before receiving physical Poison. Its base
  damage is `max(1, floor(actual reflected HP damage / 4))`; on the victim's
  next three real activations it deals base, `floor(1.5 × base)`, then
  `2 × base` physical damage. A new application with equal or higher base
  replaces the old potency and restarts three ticks; a weaker application is
  ignored. Poison does not stack. Cure removes it; ordinary Dispel does not.
- Immovable: its first-physical-creature-hit 25% final-damage reduction applies
  **only while the particular Bulwark stack is Defending**. Track the first
  qualifying hit separately per stack per round.

The repaired Markdown contains both clarified rows, checked against the perk
registry with no unapproved cell differences. The original DOCX remains an
archival conversion reference. No design choice remains open for these rules.
