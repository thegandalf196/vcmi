# Phase 1 planned-perk hold index

Updated: 2026-10-08. This is a navigation index for the planned perk entries in
`config/newHorizonsPerks.json`, not a new rule source or an amendment to the
canonical [New Horizons design](design-sources/New%20Horizons.md). That Markdown
remains the sole authority for gameplay. The queue and functional matrix record
current implementation questions and dependencies.

Registry-derived inventory: 31 Skills, 93 active rank effects, 232 active perks,
and 78 planned perks: 59 generic and 19 faction. This index covers only those 78
perks; the six inactive combat spells are tracked separately. The current
selection audit in [NH_FUNCTIONAL_COMPLETION_MATRIX.md](NH_FUNCTIONAL_COMPLETION_MATRIX.md)
historically reported item-specific questions or dependencies. The user has now
resolved Battlefield Mastery and Last Stand. Mastery is now source/native verified
and active (removed from this planned-only table); Last Stand is now source/native
verified and active too. Perfect Rhythm is also active after its seven focused
and eleven adjacent native cases pass; the old same-tier Master Synthesis
composition hold is inapplicable. That is not evidence that the whole
Version1.0 backlog is blocked.

Status meanings:

- `implementation-ready`: user answered the recorded design questions; source
  work is still missing.
- `in-progress`: source/AI/focused validation is underway, not completed coverage.

- `question`: the cited records identify an explicit rule, composition, timing,
  scope, or policy question.
- `dependency`: the cited records identify a prerequisite, producer, or base
  feature that is absent or still held.
- `lack-producer`: a required runtime trigger/state producer is absent; do not
  substitute a tooltip or infer one from a neighboring perk.
- `needs-review`: the registry entry remains planned and a relevant queue
  pointer exists, but the exact current blocker was not independently restated
  in this bounded index. Do not infer that the mechanic is ambiguous or fully
  blocked from this label.

Implementation-ready/in-progress rows require explicit supporting canonical
rules or direct user rulings. Do not retain a question when the existing authored
rules already settle it; a hypothetical exception is not itself a design hold.
`needs-review` is intentional uncertainty, not a
new user question. Preserve the cited queue records rather than reopening the
same mapping without new evidence.

The table is tab-separated for simple machine extraction. `UPref` may contain
multiple comma-separated queue entries.

```text
ID	Status	UPref	Existing recorded issue / reason
new-horizons:armorer.unyielding	lack-producer	UP-167	No nonmagical forced-displacement producer; ordinary movement and spell relocation are not substitutes.
new-horizons:armorer.defiant	question	UP-136	Applied debuffs versus intrinsic nonmagical retaliation blockers, and No Quarter's linked Morale penalty, remain unresolved.
new-horizons:battlecraft.overwatch	question	UP-155	Teleport/Blink interaction clarification remains open.
new-horizons:battlecraft.rapidResponse	question	UP-159	Precedence versus earned immediate Morale/Quartermaster/Second Wind activations remains unresolved; narrow ruling requested.
new-horizons:warMachines.precisionBombardment	question	UP-098	Basic War Machines already selects attackable structural parts; distinct perk benefit remains unresolved.
new-horizons:warMachines.breachmaker	question	UP-098	Fortification neighbor geometry and central-keep participation remain unresolved; enum order is not adjacency.
new-horizons:warMachines.battlefieldMedic	question	UP-098	Matrix says persistence awaits clarification.
new-horizons:warMachines.fieldWorkshop	question	UP-100	Destroyed-target repair scope remains pending.
new-horizons:warMachines.counterBattery	question	UP-097,UP-098	Automatic enemy-machine tower preference versus additional manual targeting remains unresolved; multiplier alone is incomplete.
new-horizons:discipline.espritDeCorps	question	UP-130	Mixed-faction versus Undead-presence composition penalties remain unresolved; UP152 is a retired duplicate.
new-horizons:discipline.veteranCohesion	question	UP-094	Battle-start maximum HP versus surviving-creature capacity changes the principal below-50% trigger; choice remains unanswered.
new-horizons:discipline.heroicSpirit	question	UP-094	Extra retaliation surviving the immediate Morale activation and expiring on the following activation remains unresolved; generic next-activation expiry would erase it immediately.
new-horizons:recruitment.drillSergeant	question	UP-127	Whole merged-stack bonus versus strict recruited-cohort provenance remains unresolved.
new-horizons:recruitment.fieldInstructor	question	UP-127	Merged-stack versus recruited-cohort scope remains unresolved; required UI depends on that rule.
new-horizons:recruitment.recruiterSContacts	question	UP-126	Empty-pool eligibility for multirow external dwellings remains unresolved.
new-horizons:recruitment.reinforcementDrill	question	UP-127	Newly recruited stack identity after merging remains unresolved; UP215 cross-reference alone did not establish its hold.
new-horizons:command.ironWill	question	UP-149	Same-command reissue replacing existing recipient carries versus separate nonstacking instances remains unresolved.
new-horizons:command.crisisCommand	question	UP-150	Free Order after complete action resolution versus interruption between hits remains unresolved.
new-horizons:command.seizeInitiative	question	UP-151	Currently active recipient eligibility determines additional activation versus moving a pending normal activation; canonical conflict remains unresolved.
new-horizons:lightMagic.miracleWorker	question	UP-141	25% increase to restoration HP versus resulting integer creature count remains unresolved.
new-horizons:shadowMagic.plaguebearer	question	UP-113	Normal-limit definition remains pending.
new-horizons:natureMagic.mireShaper	question	UP-119	Five-patch absolute cap versus sixth perk patch remains unresolved; narrow ruling requested.
new-horizons:natureMagic.worldroot	dependency	UP-117	Nature's Wrath/Worldroot base chain rules remain held.
new-horizons:natureMagic.elementalConjurer	dependency	UP-072	Depends on the unresolved Elemental Convergence terrain mapping.
new-horizons:havocMagic.demolitionist	question	UP-139	Structural-perk stacking and fixed-landmark destructibility remain unresolved; baseline structural producer is verified.
new-horizons:havocMagic.meteorologist	question	UP-139	Structural stacking and fixed-landmark destructibility remain unresolved.
new-horizons:havocMagic.cataclysm	question	UP-111,UP-139	Eligible magical-obstacle and fixed-landmark filters remain unresolved.
new-horizons:chaosMagic.confounder	implementation-ready	UP-043	User settles trapped Wander -> Defend, sole legal result may repeat, negative Morale consumes Confusion, and Confusion removes Berserk; missing Confusion producer remains the implementation prerequisite.
new-horizons:chaosMagic.shapeshifter	dependency	UP-066	Polymorph battle-local creature-form behavior is a prerequisite.
new-horizons:chaosMagic.fateDealer	question	UP-060	Two collateral draws with replacement versus distinct targets remains unresolved; base eligible pool is settled.
new-horizons:chaosMagic.realityBreaker	dependency	UP-179	Depends on Reality Warp; its target-scope question remains recorded.
new-horizons:chaosMagic.pandemoniumMaster	dependency	UP-123	Pandemonium identity and generic debuff counting/scaling remain prerequisites.
new-horizons:spellcraft.crossSchoolFormula	question	UP-132	Multi-school relation/eligibility interpretation remains unresolved.
new-horizons:spellcraft.concentration	question	UP-069	Target-count definition remains unresolved.
new-horizons:spellcraft.extendSpell	question	UP-134	Unusual spell-lifetime/expiry scope remains unresolved.
new-horizons:spellcraft.preciseCasting	question	UP-133	Time Stop/Earthquake scope remains unresolved despite principal cases.
new-horizons:spellcraft.counterpressure	question	UP-180	Accepted-cast effect map and no-op trigger boundary remain unresolved.
new-horizons:wisdom.arcaneMemory	question	UP-054	Neutral Adventure acquisition policy remains pending.
new-horizons:wisdom.sage	question	UP-074	Pre-acquisition visit timing is recorded for both Sage rows; keep Wisdom Sage distinct from Learning Sage.
new-horizons:warcasting.reactiveWeave	question	UP-215	Half-strength readiness replacing versus stacking with stronger existing readiness remains unresolved.
new-horizons:logistics.rapidEmbarkation	question	UP-103,UP-208	Navigation composition: 10% final boarding cost versus halved 5% remains unresolved.
new-horizons:logistics.pursuitMarch	question	UP-104,UP-209,UP-193	Daily recovery cap and zero-effective-recovery use consumption remain unresolved.
new-horizons:diplomacy.mercenaryCaptain	dependency	UP-129	Deterministic recruitment/cohort provenance is a prerequisite.
new-horizons:diplomacy.loyalMercenaries	dependency	UP-129	Deterministic recruitment/cohort provenance is a prerequisite.
new-horizons:diplomacy.legendaryReputation	question	UP-195,UP-129	Monthly use on refusal/zero admission versus positive join remains unresolved.
new-horizons:estates.prospector	question	UP-166	Gold is neither a common nor rare resource; Gold-mine eligibility/reward remains unresolved.
new-horizons:estates.merchantPrince	question	UP-071	Visitor/garrison qualification, holder stacking and eligible exchange types remain unresolved.
new-horizons:estates.steward	question	UP-071	Two-resident stacking remains pending.
new-horizons:estates.magnate	question	UP-168	Visit/week-start ownership, capture and multiple-holder stacking remain unresolved.
new-horizons:learning.scholar	question	UP-163	One-holder reciprocal scope, no-transfer use and canonical spellbook-order representation remain unresolved.
new-horizons:learning.eagleEye	question	UP-162	Winner-only versus other combat participants' eligibility remains unresolved.
new-horizons:learning.historian	question	UP-071	Primary-XP reward classification for Chest/Tree/mixed rewards remains unresolved.
new-horizons:learning.academicStudy	question	UP-074	First-visit/acquisition timing remains pending.
new-horizons:learning.archivist	dependency	UP-165,UP-054	Neutral Adventure-scroll acquisition policy remains unresolved; combat-only partial cannot complete full scope.
new-horizons:learning.sage	question	UP-074	Pre-acquisition visit timing is recorded for both Sage rows; keep Learning Sage distinct from Wisdom Sage.
new-horizons:learning.masterTeacher	question	UP-164	Whether Mentor must also be selected remains unresolved; two recipient identities are required.
new-horizons:luck.opportunist	question	UP-088	Movement-only continuation from reactions versus own activation remains unresolved.
new-horizons:luck.serendipity	question	UP-085	Round-one eligibility for the first-attack +2 Luck bonus remains unresolved; narrow corrected ruling requested.
new-horizons:luck.luckyRecovery	question	UP-083	Generic/Sylvan 10% recovery stacking versus shared single effect remains unresolved.
new-horizons:divineMandate.sharedPurpose	question	UP-108	Whether success qualifies by accepted Light target overlap or both effects actually triggering remains unanswered.
new-horizons:divineMandate.divineDiscipline	question	UP-108,UP-149	Same-Order reissue replacing versus separate nonstacking carried instances remains unresolved.
new-horizons:divineMandate.royalStandard	question	UP-108	Protection to scheduled expiry versus ending with broken/spent Order benefit remains unresolved.
new-horizons:divineMandate.crownAndAltar	question	UP-108	Second-action timing is resolved; paired-recipient qualification remains unanswered.
new-horizons:shroudOfMalassa.veiledMovement	lack-producer	UP-215	Movement-based reaction attack producer is absent; ordinary movement events are not equivalent.
new-horizons:shroudOfMalassa.deepFlank	question	UP-174	Distinct melee sides from current positions versus accepted-hit history and reset window remains unresolved.
new-horizons:shroudOfMalassa.encircledDoom	question	UP-174	Positional side contacts versus attack-history count/reset window remains unresolved.
new-horizons:shroudOfMalassa.vanish	question	UP-176	Retaliation kills and simultaneous Pursuit/Vanish allowance composition remain unresolved.
new-horizons:bloodrage.firstBlood	question	UP-143	First Elite/Champion death overlap with Slayer producing two/three/four increments remains unresolved.
new-horizons:bloodrage.slayer	question	UP-143	First Blood overlap on the first Elite/Champion death remains unresolved.
new-horizons:bloodrage.avatarOfRage	question	UP-226,UP-143	Blood Scent attack-local cap qualification versus stored Rage remains unresolved.
new-horizons:bulwarkOfTheMire.deepBulwark	lack-producer	UP-167	No canonical nonmagical forced-displacement producer exists.
new-horizons:elementalRebirth.elementalAttunement	dependency	UP-072	Depends on unresolved Elemental Convergence terrain mapping.
new-horizons:elementalRebirth.swiftRebirth	question	UP-046	Precedence versus earned Morale activation and multi-spawn tie order remain unresolved.
new-horizons:elementalRebirth.elementalMemory	question	UP-046	Inherited Morale versus Elemental immunity remains unresolved.
new-horizons:elementalRebirth.adaptiveElement	dependency	UP-072	Depends on unresolved Elemental Convergence terrain mapping.
new-horizons:elementalRebirth.rebirthChain	question	UP-046	Exact first-output HP producer exists; secondary-output inheritance of other Rebirth perks remains unresolved.
new-horizons:elementalRebirth.perfectConvergence	dependency	UP-072	Depends on unresolved Elemental Convergence terrain mapping.
new-horizons:elementalRebirth.phoenixSpark	question	UP-046	Greater Essence composition with the fixed 25% replacement remains unresolved.
```

## Selection result

Bounded Armorer/Discipline readiness audit,2026-10-06: four additional planned
rows above are checked against actual canonical wording, queue questions and
production seams. These are principal trigger/scope/lifetime choices, not
cosmetic or broad Phase2 concerns. No complete implementation-ready item is
established. Esprit de Corps points to UP130; UP152 is a retired duplicate.
Command UP149/150/151 additionally confirm principal reissue, interrupt timing
and active-recipient eligibility decisions, not missing generic producers.
Combined46 planned rows now have refreshed evidence; do not repeatedly remap
these seven while their recorded choices remain unanswered. Remaining37 indexed
rows are not newly certified by this bounded pass.

Final uncertain-row audit,2026-10-06: twelve additional planned rows (including
Rapid Response) now have exact queue/canonical holds restated above. Combined
with the prior27-row audit,39 planned perks have refreshed item-specific
evidence. The other44 already indexed rows are not newly certified by this
bounded pass. No unresolved `needs-review` row remains in the table; this does
not prove every Version1.0 feature outside this perk table is blocked. The six
inactive combat identities below also retain actual decisions; Polymorph's
approved nearest-legal relocation is implemented, not a new question or missing
prerequisite. Do not rerun these architecture maps without new rule evidence.

Bounded canonical/queue/source audit,2026-10-06:27 planned entries across
War Machines, Recruitment, Logistics, Estates, Learning, Nature/Havoc, Luck and
Elemental Rebirth have item-specific holds restated above. This audit adds no
implementation credit and does not certify the remaining56 planned entries as
blocked. Baseline structural/Quicksand/Rebirth producers and separate Sylvan
Luck perks are not substitutes for their planned perk behavior. Recruitment's
Reinforcement Drill hold points to UP127, not merely UP215. Narrow rulings for
Rapid Response precedence and Mire Shaper's cap are requested; corrected generic
Serendipity question concerns +2 Luck on the first attack, never an extra Hero
Action. Do not repeat these mapped neighborhoods while awaiting those decisions.

The user has cleared Battlefield Mastery and Last Stand for implementation.
Mastery is now active with4/4 focused and16/16 adjacent native cases passing;
Last Stand is now active with13/13 principal and22/22 activated adjacent cases.
This conclusion is limited to the current queue/matrix record for these IDs; it
does not assert that all remaining Version 1.0 implementation work is blocked.
The former uncertain row-level dispositions now have exact holds above.

## Bounded implementation versus full activation

Independent Phase1 review identifies ordinary principal paths that can progress
without treating narrow disputed boundaries as settled: Battlefield Mastery
(ordinary stacks), Counterpressure (accepted damaging/debuffing effects), and
Last Stand (ordinary defender surviving a lethal physical creature attack).
Subsequent user answers clear Battlefield Mastery and Last Stand for full
implementation; their historical partial/inactive restriction below no longer
applies. Counterpressure remains partial/inactive pending its separate answer.
These are candidates for **Partial, inactive** implementation, not permission
to activate a perk with an undocumented exclusion or claim completed coverage.
Counterpressure is the next selected partial slice; its no-op Dispel boundary
still needs the presented answer. Reuse UP180's accepted-effect map rather than
re-explore architecture. This index is navigation, not gameplay authority.

## Missing combat identities

Canonical/queue review found no newer ruling clearing these existing holds:

| Identity | Queue | Remaining decision |
|---|---|---|
| Confusion | UP043 | Impossible behavior, sole Confounder result and consumed activation |
| Polymorph | UP066 | Phantom conversion and reversion when no original footprint fits |
| Reality Warp | UP179 | Beneficiary-side ownership of transferred effects |
| Pandemonium | UP123/191 | Repeated debuff counting and per-debuff perk composition |
| Nature's Wrath | UP117 | Chaining range, healthy/blocked conduction and resisted continuation |
| Elemental Convergence | UP072 | Terrain mapping, including coastal Sand |
