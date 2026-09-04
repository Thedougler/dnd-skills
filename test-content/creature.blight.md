---
id: creature.blight
kind: creature
subtype: undead
scope: setting
campaign: shattered-sea
audience: [agent, dm]
canon: provisional
status: active
importance: key
schema: creature@1
created: 2026-08-17
updated: 2026-08-20
aliases:
  - Druid Lich
  - Hinewai
sources:
  - _archive/blight.md
  - _archive/arc-blight-of-aruhe.md
  - _archive/aruhe-taking-rule.md
  - _archive/aruhe-crown-squid.md
  - _archive/aruhe-grubnade.md
  - _archive/aruhe-razor-grass.md
  - _archive/aruhe-fruits.md
  - _archive/aruhe-unsaid-macaw.md
  - _archive/aruhe-blight-hinewa.md
  - _archive/aruhe-grove-amendments.md
tags: []
regions:
  - "[[region.aruhe|Aruhe]]"
  - "[[region.karath|Karath]]"
locations:
  - "[[location.aruhe-the-clear-lake|The Clear Lake]]"
factions: []
look_canon: provisional
reference_images:
  - "[[assets/creatures/blight.jpg|Blight]]"
player_images: []
---

# Druid Lich

```statblock
layout: Basic 5e Layout
name: "Blight (Stage 1)"
size: Large
type: undead
alignment: "any alignment"
ac: 18
hp: 275
hit_dice: "34d10 + 102"
speed: "30 ft., climb 30 ft."
stats: [20, 14, 16, 17, 20, 15]
saves:
  - constitution: 9
  - wisdom: 11
skillsaves:
  - nature: 10
  - perception: 11
  - survival: 11
damage_resistances: "cold, necrotic, poison; bludgeoning, piercing, and slashing from nonmagical attacks"
condition_immunities: "charmed, exhaustion, frightened, paralyzed, poisoned"
senses: "darkvision 120 ft., passive Perception 21"
languages: "Druidic, the languages it knew in life"
cr: "19"
traits:
  - name: "Rooted Phylactery"
    desc: "While the Death Bloom remains intact, a destroyed Blight reforms at the Death Bloom in 1d10 days. Destroying the Death Bloom prevents this permanently."
  - name: "Corrupted Ground"
    desc: "The Blight can move through nonmagical plants without spending extra movement and without being slowed by them, and difficult terrain within 1 mile of the Death Bloom costs it no extra movement."
  - name: "Turn Resistance"
    desc: "The Blight has advantage on saving throws against any effect that turns undead."
spells:
  - "Spellcasting. The Blight casts spells using Wisdom as its spellcasting ability (spell save DC 19, +11 to hit) and requires no material components."
  - "At will: Druidcraft, Produce Flame, Thorn Whip"
  - "3/day each: Entangle, Moonbeam, Plant Growth, Spike Growth"
  - "2/day each: Insect Plague, Wall of Thorns"
  - "1/day each: Circle of Death, Foresight, Sunburst"
actions:
  - name: "Multiattack"
    desc: "The Blight makes two Rotten Claw attacks."
  - name: "Rotten Claw"
    desc: "Melee Weapon Attack: +11 to hit, reach 10 ft., one target. Hit: 16 (2d10 + 5) slashing damage plus 10 (3d6) poison damage."
  - name: "Acid Bloom (Recharge 5-6)"
    desc: "The Blight causes corrosive sap to erupt in a 20-foot-radius sphere centered on a point it can see within 60 feet. Each creature in that area must make a DC 19 Dexterity saving throw, taking 36 (8d8) acid damage on a failed save, or half as much damage on a successful one."
legendary_actions:
  - name: ""
    desc: "The Blight can take 3 legendary actions, choosing from the options below. Only one legendary action option can be used at a time and only at the end of another creature's turn. The Blight regains spent legendary actions at the start of its turn."
  - name: "Grasping Roots"
    desc: "Roots burst from the ground in a 10-foot square the Blight can see within 60 feet. Each creature there must succeed on a DC 19 Strength saving throw or be restrained until the end of its next turn."
  - name: "Rotten Claw (Costs 2 Actions)"
    desc: "The Blight makes one Rotten Claw attack."
  - name: "Spore Burst (Costs 2 Actions)"
    desc: "One creature the Blight can see within 30 feet must succeed on a DC 19 Constitution saving throw or be poisoned until the end of its next turn."
  - name: "Feed the Bloom (Costs 3 Actions)"
    desc: "The Blight regains 20 hit points, drawn from the Death Bloom."
```

```statblock
layout: Basic 5e Layout
name: "Blight (Stage 2)"
size: Large
type: undead
alignment: "any alignment"
ac: 16
hp: 165
hit_dice: "22d10 + 44"
speed: "30 ft., climb 30 ft."
stats: [18, 12, 14, 15, 17, 12]
saves:
  - constitution: 6
  - wisdom: 7
skillsaves:
  - nature: 6
  - perception: 7
damage_resistances: "cold, necrotic, poison; bludgeoning, piercing, and slashing from nonmagical attacks"
condition_immunities: "charmed, exhaustion, frightened, paralyzed, poisoned"
senses: "darkvision 90 ft., passive Perception 17"
languages: "Druidic, the languages it knew in life"
cr: "13"
traits:
  - name: "Rooted Phylactery"
    desc: "While the Death Bloom remains intact, a destroyed Blight reforms at the Death Bloom in 1d10 days. Destroying the Death Bloom prevents this permanently."
  - name: "Corrupted Ground"
    desc: "The Blight can move through nonmagical plants without spending extra movement and without being slowed by them."
  - name: "Turn Resistance"
    desc: "The Blight has advantage on saving throws against any effect that turns undead."
spells:
  - "Spellcasting. The Blight casts spells using Wisdom as its spellcasting ability (spell save DC 15, +7 to hit) and requires no material components."
  - "At will: Druidcraft, Produce Flame, Thorn Whip"
  - "2/day each: Entangle, Moonbeam, Spike Growth"
  - "1/day each: Insect Plague, Wall of Thorns"
actions:
  - name: "Multiattack"
    desc: "The Blight makes two Rotten Claw attacks."
  - name: "Rotten Claw"
    desc: "Melee Weapon Attack: +7 to hit, reach 10 ft., one target. Hit: 11 (2d6 + 4) slashing damage plus 7 (2d6) poison damage."
  - name: "Acid Bloom (Recharge 6)"
    desc: "The Blight causes corrosive sap to erupt in a 15-foot-radius sphere centered on a point it can see within 60 feet. Each creature in that area must make a DC 15 Dexterity saving throw, taking 22 (4d10) acid damage on a failed save, or half as much damage on a successful one."
legendary_actions:
  - name: ""
    desc: "The Blight can take 2 legendary actions, choosing from the options below. Only one legendary action option can be used at a time and only at the end of another creature's turn. The Blight regains spent legendary actions at the start of its turn."
  - name: "Grasping Roots"
    desc: "Roots burst from the ground in a 10-foot square the Blight can see within 60 feet. Each creature there must succeed on a DC 15 Strength saving throw or be restrained until the end of its next turn."
  - name: "Rotten Claw (Costs 2 Actions)"
    desc: "The Blight makes one Rotten Claw attack."
```

```statblock
layout: Basic 5e Layout
name: "Blight (Stage 3)"
size: Large
type: undead
alignment: "any alignment"
ac: 14
hp: 75
hit_dice: "10d10 + 20"
speed: "20 ft., climb 10 ft."
stats: [15, 10, 12, 12, 13, 10]
skillsaves:
  - nature: 3
damage_resistances: "poison; bludgeoning, piercing, and slashing from nonmagical attacks"
condition_immunities: "charmed, exhaustion, frightened, poisoned"
senses: "darkvision 60 ft., passive Perception 11"
languages: "Druidic, the languages it knew in life"
cr: "7"
traits:
  - name: "Rooted Phylactery"
    desc: "While the Death Bloom remains intact, a destroyed Blight reforms at the Death Bloom in 1d10 days. Destroying the Death Bloom prevents this permanently."
  - name: "Corrupted Ground"
    desc: "The Blight can move through nonmagical plants without spending extra movement and without being slowed by them."
actions:
  - name: "Rotten Claw"
    desc: "Melee Weapon Attack: +4 to hit, reach 5 ft., one target. Hit: 7 (1d8 + 3) slashing damage plus 4 (1d8) poison damage."
  - name: "Acid Seep (Recharge 6)"
    desc: "A 10-foot-radius patch of ground the Blight can see within 30 feet wells up with acid. Each creature there must make a DC 12 Dexterity saving throw, taking 10 (3d6) acid damage on a failed save, or half as much damage on a successful one. The patch remains as a hazard for 1 minute, and any creature that enters it or starts its turn there for the first time on a turn must make the same save."
```

## Overview

> [!narration] Player-facing description — read or adapt at the table.
The treeline opens onto a grove that should not still be standing: grass too green, fruit hanging unpicked, air sweet with rot that never finishes. At the center a single tree holds fruit that was already ripe when whoever planted it died. Roots shift in ground that looks disturbed, as if something underneath is still breathing. A voice comes from everywhere in [[region.aruhe-the-grove|The Grove]] at once, patient, asking who gave you leave to walk here.

A Blight is a druid lich whose phylactery is a **place**. This one is bound to the Death Bloom in [[region.aruhe|Aruhe]]'s interior.

When the Blight takes form it is a skeletal lich wearing [[region.aruhe-the-grove|The Grove]]: a skull, long hair heavy with vines and ripe fruit, living-wood claws, moss and unfinished rot. Tragic and furious. The island is angry through bone.

![[assets/creatures/blight.jpg]]

## Ecology

An archdruid fuses soul and body to land they mean to protect; the ritual kills them. What remains reforms at the Death Bloom while that grove stands. Smash an object-phylactery and another lich ends. A Blight does not offer that object. The dungeon *is* the phylactery.

This Blight's power drops as the Bloom takes real damage: Stage 1 while the tree is whole, Stage 2 when it is wounded, Stage 3 when it is near ruin. Destroy the Bloom and she stays dead.

Her corruption is life continuing too aggressively: growth without limits, reproduction without restraint, healing without conclusion, adaptation without ecological brakes, and rot that cannot finish. She loved life so fiercely that she made a sanctuary where life cannot complete its cycle. The same pressure turns love into possession, protection into control, abundance into excess, survival into undeath, and grief into permanence.

She did not fail at preservation — **she succeeded**. She kept roots from his bones, animals from his grave, settlers from the island, fruit on his tree, and change away from the place where she buried him. The horror is that protecting one beloved dead person became justification for freezing an entire living island around their absence. The final question is not *Can the party kill the Blight?* but **"Does love justify preventing everything else from moving on?"**

She wants [[region.aruhe|Aruhe]] inviolate in the memory of a companion who drowned in the ocean channel during their escape from the [[creature.grung|Grung]]. She carried him inland and buried him beneath [[region.aruhe-the-grove|The Grove]]; the second grave is her own. Every real fight against her chips the Bloom — the one thing she cannot regrow as fast as she is asked to defend it.

## Behavior

Those who love life are friends; those who harm life feed life instead. She cannot tolerate waste, ownership, or careless destruction. Fauna remain independent animals. She does not speak through them. Before the party reaches [[region.aruhe-the-grove|The Grove]], she remains a presence in the island's silence rather than a visible person.

She fights near the height of her strength while the Bloom is whole. Real damage on the tree, not on her body, is what drops a stage. She grows weaker and more desperate; at Stage 3 she leans on grove hazards. [[creature.grung|Grung]] patrol the reefs and will not land.

## Habitat

The memorial grove at [[region.aruhe|Aruhe]]'s heart: [[region.aruhe-the-grove|The Grove]], on a shelf above [[location.aruhe-the-clear-lake|The Clear Lake]]. Root network and corrupted fauna through [[region.aruhe-the-rot|The Rot]] and inward. She does not leave the island. Live expedition: [[situation.aruhes-hungry-isle|Aruhe's Hungry Isle]].

## Lore

> [!secret]- What is actually known about this creature
> Hinewai was once an immensely powerful elven archdruid from a small, isolated island village. Almost all autobiographical memory has decayed; what remains is hatred of the [[creature.grung|Grung]], hatred of invaders and takers, love of life, love of [[region.aruhe|Aruhe]], and love for the companion she escaped with and lost. Hinewai is a Māori feminine name associated with water, but she may no longer remember it. She was captured on [[region.karath|Karath]], drugged into hatchery work, and fled with her companion across the ocean channel. He drowned during that escape within sight of freedom. She carried him inland and buried him beneath [[region.aruhe-the-grove|The Grove]], then made the second grave her own and bound herself into the ground. [[creature.grung|Grung]] name the island [[region.aruhe|Hungry Isle]] from one survivor's telling. Archived drafts retain earlier variants as evidence, not competing current history.

> Her bearing at [[region.aruhe-the-grove|The Grove]] is calm, proud, ancient, and courteous to respectful admirers. She may genuinely enjoy people who stop to admire [[region.aruhe|Aruhe]]'s beauty, answer questions about its animals, or approach as careful guests. That warmth disappears cleanly when someone harms the garden. She states natural consequences rather than threatening, and concrete verbs — take, break, cut, kill, carry, eat, drink, leave, return, grow, feed — fit what remains of her vocabulary. The accusation *you do not protect this place; you own it* reaches the contradiction she cannot resolve.

Sailors know two things: best landfall in the region, and nothing that took from it came back.

## Tactics

> [!tip] Running this creature — see the linked statblock for the runnable loop.
Swap chassis when the Death Bloom takes real damage: [[creature.blight]] → [[creature.blight]] → [[creature.blight]]. Body HP is not the gate.

## Variants

Stage 1 / 2 / 3 are the same being as the Bloom degrades. Not subspecies.

## Relationships

- [[region.aruhe|Aruhe]] — her garden and grave.
- [[region.karath|Karath]] — the camp she fled.
- [[creature.grubnade|Grubnade]] — her corruption made bomb: volatile plant oils in the discharge, regenerative capacity fused with paedogenesis. Nothing can safely eat them.
- [[hazard.razer-grass|Razer-Grass]] — her corruption of grass's silica armor: a familiar shape doing the wrong job. Grass already made itself unpleasant to eat; she let it finish becoming glass.
- The miracle fruit ([[item.redheart-berry|Redheart Berry]], [[item.lion-citrus|Lion Citrus]], [[item.stonepear|Stonepear]], [[item.giants-guava|Giant's Guava]], [[item.ghost-plum|Ghost Plum]], [[item.whisper-fig|Whisper Fig]], [[item.breathmelon|Breathmelon]], [[item.quickeye-berry|Quickeye Berry]], [[item.skybladder|Skybladder]], [[item.rotheart|Rotheart]]) — she did not invent new nature, she removed its brakes. Every fruit exaggerates a recognizable biological mechanism (extreme fruit-cell enlargement, concentrated sugars/pigments/stimulants/metabolites, lignified stone cells, gas-filled aerenchyma, optical wax, plant hormones, extreme stress-response chemistry) instead of inventing alien biology.
- Island fauna are her rewritten ecosystem, not allies she commands by name. A [[creature.aruhe-crown-squid|Crown Squid]] hunts like a [[creature.aruhe-crown-squid|Crown Squid]]. She does not remotely pilot animals.
- [[creature.unsaid-macaw|Unsaid Macaw]] — corruption without intent. She did not deliberately create psychic parrots; flock communication crossed into thought-perception on its own. The garden's harmless end.
