# Phase 1 planned-perk hold index

Updated: 2026-10-06. This is a navigation index for the planned perk entries in
`config/newHorizonsPerks.json`, not a new rule source or an amendment to the
canonical [New Horizons design](design-sources/New%20Horizons.md). That Markdown
remains the sole authority for gameplay. The queue and functional matrix record
current implementation questions and dependencies.

Registry-derived inventory: 31 Skills, 93 active rank effects, 225 active perks,
and 85 planned perks: 66 generic and 19 faction. This index covers only those 85
perks; the six inactive combat spells are tracked separately. The current
selection audit in [NH_FUNCTIONAL_COMPLETION_MATRIX.md](NH_FUNCTIONAL_COMPLETION_MATRIX.md)
reports an item-specific question or dependency for each planned perk and no
fully unblocked perk in this set. That is not evidence that the whole Version
1.0 backlog is blocked.

Status meanings:

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

No row is classified as unblocked or as merely delayed implementation without
direct supporting evidence. `needs-review` is intentional uncertainty, not a
new user question. Preserve the cited queue records rather than reopening the
same mapping without new evidence.

The table is tab-separated for simple machine extraction. `UPref` may contain
multiple comma-separated queue entries.

```text
ID	Status	UPref	Existing recorded issue / reason
new-horizons:armorer.unyielding	lack-producer	UP-167	No nonmagical forced-displacement producer; ordinary movement and spell relocation are not substitutes.
new-horizons:armorer.defiant	question	UP-136	Matrix records Defiant among Armorer perks awaiting design choices.
new-horizons:armorer.lastStand	question	UP-079	Matrix records Last Stand among Armorer perks awaiting design choices.
new-horizons:battlecraft.overwatch	question	UP-155	Teleport/Blink interaction clarification remains open.
new-horizons:battlecraft.rapidResponse	needs-review	UP-159	Relevant preparation exists; exact current hold is not restated here.
new-horizons:battlecraft.battlefieldMastery	question	UP-156	Whether an ineligible War Machine consumes the first-award opportunity remains unanswered.
new-horizons:warMachines.precisionBombardment	needs-review	UP-098	War Machines continuation reference; exact item-level hold not restated here.
new-horizons:warMachines.breachmaker	needs-review	UP-098	War Machines continuation reference; exact item-level hold not restated here.
new-horizons:warMachines.battlefieldMedic	question	UP-098	Matrix says persistence awaits clarification.
new-horizons:warMachines.fieldWorkshop	question	UP-100	Destroyed-target repair scope remains pending.
new-horizons:warMachines.counterBattery	needs-review	UP-097,UP-098	War Machines targeting/continuation references; exact current hold not restated here.
new-horizons:discipline.espritDeCorps	question	UP-152,UP-130	Composition scope awaits clarification.
new-horizons:discipline.veteranCohesion	question	UP-094	Whether the 50% trigger uses initial maximum HP or surviving-creature capacity awaits clarification.
new-horizons:discipline.heroicSpirit	question	UP-094	Extra-retaliation expiry across the immediate Morale activation awaits clarification.
new-horizons:recruitment.drillSergeant	needs-review	UP-127	Recruitment cohort/provenance family reference; exact item-level hold not restated here.
new-horizons:recruitment.fieldInstructor	needs-review	UP-127	Recruitment cohort/provenance family reference; exact item-level hold not restated here.
new-horizons:recruitment.recruiterSContacts	question	UP-126	Empty-pool eligibility for multirow external dwellings remains unresolved.
new-horizons:recruitment.reinforcementDrill	needs-review	UP-215	Readiness coexistence reference; exact item-level hold not restated here.
new-horizons:command.ironWill	question	UP-149	Recorded Command rule ruling remains pending.
new-horizons:command.crisisCommand	question	UP-150	Recorded Command rule ruling remains pending.
new-horizons:command.seizeInitiative	question	UP-151	Recorded Command rule ruling remains pending.
new-horizons:lightMagic.miracleWorker	needs-review	UP-141	Light perk reference; exact current hold is not restated here.
new-horizons:shadowMagic.plaguebearer	question	UP-113	Normal-limit definition remains pending.
new-horizons:natureMagic.mireShaper	needs-review	UP-119	Nature perk reference; exact current hold is not restated here.
new-horizons:natureMagic.worldroot	dependency	UP-117	Nature's Wrath/Worldroot base chain rules remain held.
new-horizons:natureMagic.elementalConjurer	dependency	UP-072	Depends on the unresolved Elemental Convergence terrain mapping.
new-horizons:havocMagic.demolitionist	needs-review	UP-139	Havoc perk reference; exact current hold is not restated here.
new-horizons:havocMagic.meteorologist	needs-review	UP-139	Havoc perk reference; exact current hold is not restated here.
new-horizons:havocMagic.cataclysm	needs-review	UP-111,UP-139	Havoc perk/base-spell references; exact current hold is not restated here.
new-horizons:chaosMagic.confounder	dependency	UP-043	Confusion identity/implementation is a prerequisite.
new-horizons:chaosMagic.shapeshifter	dependency	UP-066	Polymorph battle-local creature-form behavior is a prerequisite.
new-horizons:chaosMagic.fateDealer	needs-review	UP-060	Chaos perk reference; exact current hold is not restated here.
new-horizons:chaosMagic.realityBreaker	dependency	UP-179	Depends on Reality Warp; its target-scope question remains recorded.
new-horizons:chaosMagic.pandemoniumMaster	dependency	UP-123	Pandemonium identity and generic debuff counting/scaling remain prerequisites.
new-horizons:spellcraft.crossSchoolFormula	question	UP-132	Multi-school relation/eligibility interpretation remains unresolved.
new-horizons:spellcraft.concentration	question	UP-069	Target-count definition remains unresolved.
new-horizons:spellcraft.extendSpell	question	UP-134	Unusual spell-lifetime/expiry scope remains unresolved.
new-horizons:spellcraft.preciseCasting	question	UP-133	Time Stop/Earthquake scope remains unresolved despite principal cases.
new-horizons:spellcraft.counterpressure	question	UP-180	Accepted-cast effect map and no-op trigger boundary remain unresolved.
new-horizons:spellcraft.overwhelmingFormula	question	UP-121	Penetration-composition ruling remains unresolved.
new-horizons:wisdom.arcaneMemory	question	UP-054	Neutral Adventure acquisition policy remains pending.
new-horizons:wisdom.sage	question	UP-074	Pre-acquisition visit timing is recorded for both Sage rows; keep Wisdom Sage distinct from Learning Sage.
new-horizons:warcasting.enchantedCommand	question	UP-122	Shared rule decision remains pending.
new-horizons:warcasting.combatCasting	question	UP-121	Shared rule decision remains pending.
new-horizons:warcasting.reactiveWeave	needs-review	UP-215	Readiness-coexistence reference; exact current hold is not restated here.
new-horizons:warcasting.perfectRhythm	question	UP-178	Master Synthesis stacking/composition remains unresolved; prerequisite sequence work does not activate the perk.
new-horizons:logistics.rapidEmbarkation	needs-review	UP-208	Embarkation policy/geometry reference; exact current remaining hold is not restated here.
new-horizons:logistics.pursuitMarch	needs-review	UP-209,UP-193	Pursuit March references exist; exact current hold is not restated here.
new-horizons:diplomacy.mercenaryCaptain	dependency	UP-129	Deterministic recruitment/cohort provenance is a prerequisite.
new-horizons:diplomacy.loyalMercenaries	dependency	UP-129	Deterministic recruitment/cohort provenance is a prerequisite.
new-horizons:diplomacy.legendaryReputation	needs-review	UP-195,UP-129	Diplomacy implementation/provenance references; exact remaining hold is not restated here.
new-horizons:estates.prospector	question	UP-166	Gold is neither a common nor rare resource; Gold-mine eligibility/reward remains unresolved.
new-horizons:estates.merchantPrince	needs-review	UP-071	Market-selector mapping/source review exists, but the perk remains planned; exact current hold is not restated here.
new-horizons:estates.steward	question	UP-071	Two-resident stacking remains pending.
new-horizons:estates.magnate	needs-review	UP-168	Estates preparation exists; exact current item-level hold is not restated here.
new-horizons:learning.scholar	needs-review	UP-163	Learning preparation reference; exact current hold is not restated here.
new-horizons:learning.eagleEye	needs-review	UP-162	Learning preparation reference; exact current hold is not restated here.
new-horizons:learning.historian	needs-review	UP-071	Experience-source classification is recorded; exact remaining hold is not restated here.
new-horizons:learning.academicStudy	question	UP-074	First-visit/acquisition timing remains pending.
new-horizons:learning.archivist	needs-review	UP-165	Learning preparation reference; exact current hold is not restated here.
new-horizons:learning.sage	question	UP-074	Pre-acquisition visit timing is recorded for both Sage rows; keep Learning Sage distinct from Wisdom Sage.
new-horizons:learning.masterTeacher	needs-review	UP-164	Learning preparation reference; exact current hold is not restated here.
new-horizons:luck.opportunist	needs-review	UP-088	Luck perk reference; exact current hold is not restated here.
new-horizons:luck.serendipity	needs-review	UP-085	Luck perk reference; exact current hold is not restated here.
new-horizons:luck.luckyRecovery	needs-review	UP-083	Luck perk reference; exact current hold is not restated here.
new-horizons:luck.perfectFortune	needs-review	UP-081	Luck perk reference; exact current hold is not restated here.
new-horizons:divineMandate.sharedPurpose	question	UP-108	Whether success qualifies by accepted Light target overlap or both effects actually triggering remains unanswered.
new-horizons:divineMandate.divineDiscipline	needs-review	UP-108	Divine Mandate paired-recipient foundation reference; exact item-level hold not restated here.
new-horizons:divineMandate.royalStandard	needs-review	UP-108	Divine Mandate paired-recipient foundation reference; exact item-level hold not restated here.
new-horizons:divineMandate.crownAndAltar	question	UP-108	Second-action timing is resolved; paired-recipient qualification remains unanswered.
new-horizons:shroudOfMalassa.veiledMovement	lack-producer	UP-215	Movement-based reaction attack producer is absent; ordinary movement events are not equivalent.
new-horizons:shroudOfMalassa.deepFlank	needs-review	UP-174	Shroud movement/flanking reference; exact current hold is not restated here.
new-horizons:shroudOfMalassa.encircledDoom	needs-review	UP-174	Shroud flanking reference; exact current hold is not restated here.
new-horizons:shroudOfMalassa.vanish	question	UP-176	Retaliation kills and simultaneous Pursuit/Vanish allowance composition remain unresolved.
new-horizons:bloodrage.firstBlood	needs-review	UP-143	Bloodrage threshold-perk reference; exact remaining question is not restated here.
new-horizons:bloodrage.slayer	needs-review	UP-143	Bloodrage threshold-perk reference; exact remaining question is not restated here.
new-horizons:bloodrage.avatarOfRage	needs-review	UP-226,UP-143	Avatar implementation and threshold-family references; exact remaining hold is not restated here.
new-horizons:bulwarkOfTheMire.deepBulwark	lack-producer	UP-167	No canonical nonmagical forced-displacement producer exists.
new-horizons:elementalRebirth.elementalAttunement	dependency	UP-072	Depends on unresolved Elemental Convergence terrain mapping.
new-horizons:elementalRebirth.swiftRebirth	needs-review	UP-046	Rebirth first-output/provenance foundation is recorded; this does not itself implement the perk.
new-horizons:elementalRebirth.elementalMemory	needs-review	UP-046	Rebirth foundation reference; exact current item-level hold is not restated here.
new-horizons:elementalRebirth.adaptiveElement	dependency	UP-072	Depends on unresolved Elemental Convergence terrain mapping.
new-horizons:elementalRebirth.rebirthChain	needs-review	UP-046	Original-output HP metadata prerequisite is now implemented; Chain behavior/composition remains unimplemented and unspecified here.
new-horizons:elementalRebirth.perfectConvergence	dependency	UP-072	Depends on unresolved Elemental Convergence terrain mapping.
new-horizons:elementalRebirth.phoenixSpark	needs-review	UP-046	Rebirth foundation reference; exact current item-level hold is not restated here.
```

## Selection result

No fully unblocked candidate was identified within the 85 planned perk entries.
This conclusion is limited to the current queue/matrix record for these IDs; it
does not assert that all remaining Version 1.0 implementation work is blocked.
Uncertain row-level dispositions are deliberately marked `needs-review` above.

## Bounded implementation versus full activation

Independent Phase1 review identifies ordinary principal paths that can progress
without treating narrow disputed boundaries as settled: Battlefield Mastery
(ordinary stacks), Counterpressure (accepted damaging/debuffing effects), and
Last Stand (ordinary defender surviving a lethal physical creature attack).
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
