---
id: npc.aleksander-malone
kind: npc
subtype: heresy-hunter
scope: setting
campaign:
audience:
  - agent
  - dm
canon: established
status: active
importance: major
schema: npc@1
created: 2026-08-17
updated: 2026-08-19
aliases:
  - "Aleksander Malone"
  - "Malone"
  - "Cleric Malone"
sources:
  - _archive/aleksander-malone.md
  - _archive/aleksander-malone-2.md
  - _archive/aleksander-malone-narration-appearance.md
  - _archive/arc-malones-verdict.md
  - _archive/the-hound-of-god.md
summary: Dravosi Crown heresy-hunter and Tyr zealot hunting Shepherd Grigori without waiting for Crown confirmation.
tags: []
factions:
  - "[[faction.dravosi-crown|The Dravosi Crown]]"
locations:
  - "[[location.blackrule|Blackrule]]"
  - "[[settlement.sarns-landing|Sarn's Landing]]"
npcs:
  - "[[npc.shepherd-grigori|Shepherd Grigori]]"
relationships:
  - target: "[[npc.shepherd-grigori|Shepherd Grigori]]"
    type: related_to
provenance:
  extracted: 0.9
  inferred: 0.08
  ambiguous: 0.02
base_confidence: 0.37
tier: supporting
---

# Aleksander Malone

```statblock
layout: Basic 5e Layout
name: "Aleksander Malone"
size: Medium
type: humanoid (elf)
alignment: "Lawful Neutral"
ac: "18 (half plate, blessed)"
hp: 195
hit_dice: "26d8 + 78"
speed: "30 ft."
stats: [20, 14, 16, 12, 20, 13]
saves:
  - con: 7
  - wis: 9
skillsaves:
  - insight: 9
  - perception: 9
  - religion: 5
  - stealth: 6
condition_immunities: "Charmed, Frightened"
senses: "Passive Perception 19"
languages: "Common, Elvish"
cr: 14
traits:
  - name: "Regeneration"
    desc: "Malone regains 20 hit points at the start of his turn. If Malone takes necrotic damage, this trait doesn't function at the start of his next turn. Malone dies only if he starts his turn with 0 hit points and doesn't regenerate."
  - name: "Heretic's Bane"
    desc: "Malone has advantage on saving throws against spells and abilities used by fiends and undead. When he hits a fiend or undead with a weapon attack, the attack deals an extra 4 (1d8) radiant damage."
  - name: "Sneak Attack (1/Turn)"
    desc: "Malone deals an extra 7 (2d6) damage when he hits a target with a weapon attack and has advantage on the attack roll, or when another enemy of the target is within 5 feet of it, that enemy isn't incapacitated, and Malone doesn't have disadvantage on the attack roll."
  - name: "Spellcasting"
    desc: "Malone is a 7th-level spellcaster. His spellcasting ability is Wisdom (spell save DC 17, +9 to hit with spell attacks). At will: Guidance, Sacred Flame (3d8), Thaumaturgy. 2/day each: Bless, Command, Hold Person. 1/day each: Dispel Magic, Banishment."
actions:
  - name: "Multiattack"
    desc: "Malone makes three attacks: any combination of blessed longsword and blessed bayonet attacks."
  - name: "Blessed Longsword"
    desc: "Melee Weapon Attack: +9 to hit, reach 5 ft., one target. Hit: 9 (1d8 + 5) slashing damage plus 9 (2d8) radiant damage."
  - name: "Blessed Bayonet"
    desc: "Ranged Weapon Attack: +9 to hit, range 20/60 ft., one target. Hit: 7 (1d4 + 5) piercing damage plus 9 (2d8) radiant damage."
  - name: "Bayonet Barrage (Recharge 5–6)"
    desc: "Malone hurls a fan of blessed bayonets in a 30-foot cone. Each creature in that area must make a DC 17 Dexterity saving throw, taking 28 (8d6) radiant damage on a failed save, or half as much damage on a successful one."
bonus_actions:
  - name: "Action Surge (1/Short Rest)"
    desc: "Malone can take one additional action on his turn, in addition to his regular action and a possible bonus action."
  - name: "Spiritual Weapon (2/Day)"
    desc: "Malone conjures a spectral mace within 60 feet. For 1 minute, as a bonus action on each of his turns, he can move the weapon up to 20 feet and make a melee spell attack (+9 to hit) against a creature within 5 feet of it, dealing 14 (2d8 + 5) force damage on a hit."
  - name: "Channel Divinity: Rebuke the Unclean (1/Short Rest)"
    desc: "Each fiend and undead within 30 feet of Malone must succeed on a DC 17 Wisdom saving throw or be turned for 1 minute. A turned creature must spend its turns moving as far away from Malone as possible and cannot take reactions. It can only Dash or try to escape effects preventing movement. A fiend or undead of CR 2 or lower that fails is destroyed instead."
reactions:
  - name: "Guided Judgment (2/Short Rest)"
    desc: "Immediately after missing with an attack roll, Malone can reroll the die and must use the new roll."
  - name: "Withdraw by Judgment (1/Day)"
    desc: "When Malone is reduced below 49 hit points, he can teleport up to 30 feet to an unoccupied space he can see without provoking opportunity attacks, and does not return to the fight this encounter."
```

> [!narration] First Impression
> *Tall and spare, a High Elf in a Crown-service coat that has been through worse than tailoring can hide. The wool carries salt and something older. Seams gone pale at the shoulders, patched at the elbows with leather that matches nothing else on him. His hands are steady and unused to stillness, resting open at his sides the way a man's do when he expects to need them.*
>
> *Before he speaks again, fingers touch his lips. Quick as a blessing. His eyes have already finished with whoever he is looking at.*

Cleric of [[deity.tyr|Tyr]]. Held in reserve by the [[faction.dravosi-crown|The Dravosi Crown]] for **heresy**, not ordinary crime. Modeled on Alexander Anderson (Hellsing): zealotry delivered with grim joy. Every killing he frames as righteous judgment.

## Wants

- **Right now:** Confirm heresy, then act on his own judgment. No handler. Word reaches him; he goes.
- **Long term:** Be [[faction.dravosi-crown|the Crown]]'s answer once [[faction.khlysty|Khlysty]] is confirmed inside [[faction.dravosi-crown|Dravosi]]. Do not wake that thread until the GM chooses.

> [!tip] Playing Tips
> Iron will, absolute conviction. Scripture cadence, grim laughter, mid-sermon energy — not a subtle interrogator. Signature line as written. He answers to no one moment-to-moment; the leash is long by design.
> Combat: mercilessly precise cleric / fighter / rogue stacking (Channel Divinity as [[deity.tyr|Tyr]]'s judgment, Action Surge, rogue precision and mobility). Run [[npc.aleksander-malone|Malone]]; do not add supernatural resilience beyond that block.

## What They Know

- Crown doctrine and heresy briefs he is given.
- How to find a guilty man by who flinches at God (his method, not a spell).
- The standing arrangement: no handler. [[faction.dravosi-crown|Dravosi]] tried; the handler did not survive contact. Crown proverb: their dog needs a long leash, and a handler will only get bit.

He will share freely that he hunts heresy for [[faction.dravosi-crown|the Crown]]. He will not discuss the public-space mistake unless pressed by someone with rank.

## Relationships

- [[faction.dravosi-crown|The Dravosi Crown]] — reserved asset for confirmed heresy. Not a day-to-day officer.
- [[deity.tyr|Tyr]] — cleric.
- [[npc.shepherd-grigori|Shepherd Grigori]] / [[faction.khlysty|Khlysty]] — the reason he is loosed. Hunt already live from earlier houses, not Knighton.
- [[location.blackrule|Blackrule]] — chapterhouse he chose; not exile.

## Levers

- **Confirmed heresy.** That is the warrant. Ordinary crime does not move him.
- **Ranked Crown word** that a target is guaranteed-guilty. He aims cleanly only then.
- **A handler assignment** is not a lever — it is how people die.
- **Scripture or [[deity.tyr|Tyr]]'s law** argued in good faith may slow him; mockery will not.

> [!secret]- Secrets
> [[faction.dravosi-crown|the Crown]] loosed him once in a relatively public space: [[settlement.sarns-landing|Sarn's Landing]]. Ugly results. That incident is why he is reserved now, and why heresy must be confirmed before he sails. He still believes the violence was judgment. The archived verdict fiction is tone, not a locked body count.

> [!danger] If Violence Starts
> He does not hesitate. He treats the fight as a sacrament already underway. The statblock's regeneration and withdrawal threshold are the important counterplay.

## If Left Alone

He stays at [[location.blackrule|Blackrule]] until word of heresy reaches him, then goes on his own judgment. Once [[faction.khlysty|Khlysty]] infiltration of [[faction.dravosi-crown|Dravosi]] is confirmed, he is [[faction.dravosi-crown|the Crown]]'s answer. The hunt is already live. See [[situation.grigori-ascension|Grigori's Ascension]], [[situation.the-aruhe-rescue|The Aruhe Rescue]], [[season.02|Season 2]].

## Mechanics

- Statblock: [[npc.aleksander-malone|Malone]] — link only; combat math lives there.
- Class stack as fiction: cleric ([[deity.tyr|Tyr]]) + fighter durability/Action Surge + rogue precision/mobility.

## Continuity

- Season 02 flags him as surfacing with [[npc.shepherd-grigori|Grigori]].
- [[region.aruhe|Aruhe]] rescue table: hunt for [[npc.shepherd-grigori|Grigori]] south; board-and-inspect cutter in the main channel.
- Session 09: boarded the *[[vehicle.uncertainty|Uncertainty]]* under [[npc.corbin-knighton|Corbin Knighton]], hunting [[npc.shepherd-grigori|Grigori]]. Used confession magic; [[pc.delmar-fisk|Delmar]] confessed while [[pc.catarina-davirelli|Catarina]] resisted and staged an [[deity.umberlee|Umberlee]] laugh. [[npc.corbin-knighton|Corbin]] reined him in and the warship stood off for [[settlement.calveno|Calveno]].
