---
id: creature.aruhe-crown-squid
kind: creature
subtype: monstrosity
scope: setting
campaign: shattered-sea
audience: [agent, dm]
canon: provisional
status: active
importance: supporting
schema: creature@1
created: 2026-08-20
updated: 2026-08-20
aliases:
  - "Great Crown Squid"
  - "Crown Squid"
  - "Colossal Tree Squid"
sources:
  - _archive/aruhe-crown-squid.md
  - _archive/aruhe-snakewood.md
tags:
  - horror
  - apex-predator
regions:
  - "[[region.aruhe|Aruhe]]"
  - "[[region.aruhe-the-quiet|The Quiet]]"
  - "[[region.aruhe-the-rot|The Rot]]"
  - "[[region.aruhe-the-old-gardens|The Old Gardens]]"
  - "[[region.aruhe-the-grasslands|The Grasslands]]"
  - "[[region.aruhe-the-river|The River]]"
locations:
  - "[[location.aruhe-the-long-reach|The Long Reach]]"
  - "[[location.aruhe-the-clear-lake|The Clear Lake]]"
factions: []
look_canon: provisional
reference_images: []
player_images: []
---

# Great Crown Squid

```statblock
layout: Basic 5e Layout
name: "Great Crown Squid"
size: Gargantuan
type: monstrosity
alignment: unaligned
ac: "17 (rubbery natural armor)"
hp: 283
hit_dice: "21d20 + 63"
speed: "20 ft., climb 50 ft."
stats: [24, 20, 17, 7, 20, 6]
saves:
  - dex: 11
  - con: 9
  - wis: 11
skillsaves:
  - Perception: 17
  - Stealth: 11
  - Athletics: 13
senses: "darkvision 120 ft., passive Perception 27"
languages: "—"
cr: 17
traits:
  - name: "Canopy Camouflage"
    desc: "While among foliage, branches, or hanging roots, the squid can Hide even when only lightly obscured. If it hasn't moved since the end of its previous turn, it has advantage on Dexterity (Stealth) checks. This is cephalopod camouflage expressed through 5e's normal hiding mechanics rather than invisibility."
  - name: "Eight-Eyed Awareness"
    desc: "The squid has advantage on Wisdom (Perception) checks relying on sight and cannot be surprised while conscious unless the creature surprising it is inside its Mouth-Blind Zone."
  - name: "Mouth-Blind Zone"
    desc: "The squid cannot visually perceive a creature within 10 feet directly beneath the center of its mantle unless that creature is grappled by the squid or touching one of its arms. Against the squid, such a creature counts as unseen, and the squid cannot make opportunity attacks against it."
  - name: "Spider-Braced"
    desc: "While at least three primary arms are touching solid surfaces, the squid cannot be knocked prone or moved against its will."
  - name: "Buoyant Mantle"
    desc: "The squid takes no falling damage while its gas mantle remains intact and falls no faster than 60 feet per round. It cannot use this trait to fly."
  - name: "Siege Predator"
    desc: "The squid deals double damage to objects and structures. Nonmagical plant growth never costs it additional movement."
  - name: "Selected Prey"
    desc: "The squid has advantage on its first Hookline attack each turn against a creature that has no conscious ally within 10 feet of it. This is the jumping-spider brain made mechanically visible: isolation invites attack."
actions:
  - name: "Multiattack"
    desc: "The squid makes three attacks, only one of which may be a Beak attack."
  - name: "Hookline Tentacle"
    desc: "Melee Weapon Attack: +11 to hit, reach 80 ft., one creature. Hit: 18 (2d10 + 7) slashing damage, and the target is grappled (escape DC 19). Until the grapple ends, the target is also restrained. The squid can maintain up to four Hookline grapples simultaneously. A Hookline can itself be attacked: AC 15, 15 hit points, immunity to poison and psychic damage. Destroying one ends that grapple but does not meaningfully reduce the Crown Squid's combat ability; it has dozens."
  - name: "Crushing Arm"
    desc: "Melee Weapon Attack: +13 to hit, reach 20 ft. Hit: 25 (4d8 + 7) bludgeoning damage. The squid may grapple the target (escape DC 19) or push it 20 feet."
  - name: "Beak"
    desc: "Melee Weapon Attack: +13 to hit, reach 10 ft., one creature grappled by the squid. Hit: 33 (4d12 + 7) piercing damage."
  - name: "Reel"
    desc: "Each creature grappled by a Hookline is pulled up to 30 feet directly toward the Crown Squid."
  - name: "Canopy Pounce (Recharge 5-6)"
    desc: "The squid moves up to its climb speed without provoking opportunity attacks, provided it ends that movement touching a tree or similarly massive structure. At any two points during this movement it may make a Hookline attack."
legendary_actions:
  - name: ""
    desc: "The Crown Squid can take 3 legendary actions, choosing from the options below. Only one legendary action option can be used at a time and only at the end of another creature's turn. The Crown Squid regains spent legendary actions at the start of its turn."
  - name: "Skitter"
    desc: "The squid moves up to 20 feet using its climb speed without provoking opportunity attacks."
  - name: "Hookline"
    desc: "The squid makes one Hookline Tentacle attack."
  - name: "Reel"
    desc: "One creature grappled by the squid is pulled up to 20 feet toward it."
  - name: "Rip Through (Costs 2 Actions)"
    desc: "The squid tears apart a 10-foot cube of nonmagical wood or vegetation within reach. Creatures in that area make a DC 19 Dexterity saving throw, taking 18 (4d8) bludgeoning damage and falling prone on a failure, or half damage on success. The destroyed area becomes difficult terrain."
```

## Overview

> [!narration] Player-facing description — read or adapt at the table.
> The branch above you changes color. It is not a branch. Something closes around your ankle — not a vine, a wet little tightening, then a hook punches through your boot. Your feet leave the ground. You are thirty feet up before anyone understands what is happening.

A Gargantuan arboreal cephalopod that lives in the crowns of [[region.aruhe|Aruhe]]'s enormous trees: approximately 60–80 feet from mantle-tip to the ends of its eight principal arms, with hair-thin-to-rope-thick hunting tentacles able to extend another 80–120 feet downward. It does not swing like an ape; it **flows from tree to tree like an enormous jumping spider**. It does not roar and does not threaten. A [[creature.human|Human]] is not an opponent — a [[creature.human|Human]] is approximately the size category of prey it normally lifts out of the undergrowth.

## Ecology

**What it is.** A mature Great Crown Squid is a Gargantuan arboreal cephalopod, 60–80 feet from mantle-tip to the ends of its eight principal arms; the oldest individuals may be larger. Its mantle is grotesquely broad rather than hydrodynamic: a translucent, lobed structure resembling a swollen squid mantle crossed with a seed pod and a spider abdomen. Much of that apparent bulk is not flesh — it is an enormous collection of gas chambers.

The eight principal arms are the animal's "legs": each immensely muscular, ending in broad gripping pads and hooked suckers. At rest, perhaps five are anchored to separate trunks while three lie loose. Underneath hangs the feeding apparatus: the beak, radula, and a forest of much finer extensible tentacles — some only finger-thick despite being dozens of feet long.

**Biological grounding.** The ingredients are real. Colossal squid possess hooked arms and tentacles; the long feeding tentacles seize prey, after which the eight arms surround and guide it to the beak. Colossal-squid tentacle hooks swivel, while arm hooks are deeply seated to maintain purchase on struggling prey (Te Papa). Cephalopods already control skin color and texture using chromatophores, reflective cells, and muscular papillae, so the squid's nearly supernatural camouflage is an exaggeration of something cephalopods genuinely do (Smithsonian Ocean).

**The gas mantle.** The squid is buoyancy-assisted rather than freely flying. Symbiotic fermentative microbes live in gas-gill chambers: blood brings them carbohydrate-rich waste products, the microbes generate hydrogen-rich gas, and specialized countercurrent tissues separate and compress it into the mantle sacs. Its gas mantle removes most of its effective weight while its arms provide anchorage and propulsion — the animal still weighs several tons if killed, but a living one feels to the trees like something weighing a few hundred pounds. It cannot truly fly. It can, however, **almost not fall**: if all eight arms release, the mantle slowly sinks or rises between the trees while the animal spreads its limbs looking for another purchase. A four-ton predator can launch across a fifty-foot canopy gap almost silently. Because the thing supporting it is gas rather than bone and muscle, its locomotion feels deeply wrong — trees should bend under something this large; they barely move. (Real precedent: the Portuguese man o' war's pneumatophore is a gas-filled biological float; biological hydrogen production through microbial fermentation is real.)

**Apex-predator mosaic.** A Crown Squid requires several adjacent mature trees because it rarely trusts its whole mass to one — a natural range restriction. [[creature.aruhe-river-otter|River Otters]] create an especially good ecological boundary: a Crown Squid that lets a grabber trail into occupied water is liable to discover six enormous otters pulling the other direction, so mature squids recognize open water as unsafe. On land [[faction.dravosi-crown|the Crown]] Squid is at the top: [[creature.terror-bird|Terror-Birds]] are dangerous prey, [[creature.bear-elk|Bear-Elk]] are very dangerous prey, [[creature.wolfrabbit|Wolfrabbits]] are snacks, and a humanoid is food.

## Behavior

**Eight-eyed sensory psychology** (behavioral, not anatomical — the squid shape stays recognizably intact). Jumping spiders have eight eyes divided into jobs: [[vehicle.the-narrow|Narrow]]-field, exceptionally high-resolution principal eyes and broad secondary eyes good at noticing movement (PubMed). [[faction.dravosi-crown|the Crown]] Squid exaggerates this: two enormous forward eyes perform rangefinding and microscopic target inspection; three secondary pairs ring the mantle, continuously passing moving objects to [[npc.cosimo-verantio|the Principal]] pair. The result is effectively 360-degree awareness — but not eight identical magic cameras. When something moves, one little lateral eye notices; then, without its body moving at all, the enormous principal eyes slowly roll around inside the transparent head until they are looking at it. **That movement is the tell.**

**Mouth-Blind Zone.** Immediately beneath the beak, between the bases of the arms, the eye fields overlap badly. The safest place relative to a Crown Squid is horrifyingly close to its mouth — that should matter mechanically.

**The modern fear: you have already been selected.** The conscious horror is arachnophobia; the deeper [[region.aruhe|Aruhe]] horror is ubiquitous surveillance and automated targeting. Not "someone is following me" — the [[creature.deer-stalker|Deer-Stalker]] owns that territory. The party walks beneath it for perhaps several minutes; eight eyes have tracked everyone — who trails behind, who limps, who repeatedly separates, who carries the most meat, who is smallest. The players never make the momentous decision to enter combat. One character makes a Perception check and fails.

**Combat loop.** Watch → select → hook → lift → reel → beak. The creature should not normally descend and exchange attacks with five adventurers. If the party cuts the line before the victim reaches the mouth, [[faction.dravosi-crown|the Crown]] Squid does not become enraged — it becomes **interested**. That failed grab tells it something about the herd; it immediately relocates and tries a different individual. When actually wounded badly (below half HP), it stops treating the party as ordinary prey and begins a full jumping-spider pursuit: it stays above them, anticipates routes rather than following directly, crosses gaps with Canopy Pounce, and demolishes vegetation that would slow it. The important distinction from the [[creature.terror-bird|Terror-Bird]]: the [[creature.terror-bird|Terror-Bird]]'s first explosive charge is its commitment, and escaping that charge can end the encounter; [[faction.dravosi-crown|the Crown]] Squid's psychology is the opposite — **[[faction.dravosi-crown|the Crown]] Squid likes a chase**.

**Signs that one lives here** (the encounter is avoidable after players learn the ecology). DC 14 Wisdom (Survival) recognizes that something extremely large is using the upper canopy; DC 17 identifies the unmistakable hunting signs; DC 20 Wisdom (Perception), or passive Perception 20, can find a motionless adult before it attacks. The signs: sucker scars seventy feet above the ground, circles arranged in sequences no claw could make; strips of bark removed upward rather than downward; a mature tree leaning thirty degrees from where something uprooted it and discarded it; polished fragments of antler on the forest floor with no carcass nearby; and places where the undergrowth holds lots of prey tracks but no tracks showing what killed them. Nothing walked down to eat them. They went up.

## Habitat

The vertical ecosystem of [[region.aruhe|Aruhe]]'s gigantic trees: the established canopy is already hundred-foot-scale in ordinary stretches, with extraordinary growth throughout the island. [[region.aruhe-the-quiet|The Quiet]] is especially suitable — visibility dies within a few paces, hearing is unreliable, and its enormous trees and root curtains establish exactly the vertical ecosystem this thing needs. A Crown Squid requires several adjacent mature trees, which gives it a natural range restriction.

| Region | Crown Squid behavior |
|---|---|
| **Old Gardens** | Mature animals usually absent; trees are too interrupted. Juveniles occasionally hunt the upper terraces. |
| **[[region.aruhe-the-quiet\|The Quiet]]** | Prime habitat — where the species becomes a major threat. |
| **[[region.aruhe-the-rot\|The Rot]]** | Largest and oldest animals. More sessile because prey is abundant. |
| **Grasslands** | Refuses to cross broad openings except under extreme hunger. No anchor points. |
| **River valleys** | Hunts from the jungle bank but rarely extends a grabber over deep water. |
| **Clear Lake** | Forested margins only. Open shoreline is refuge from it. |
| **[[region.aruhe-the-grove\|The Grove]]** | Does not cross the mourner line. |

This pays off the existing Long Reach language that things **hang in the jungle curtain and drop from the root canopy** — Crown Squids are one of the things that sentence was warning about all along.

## Lore

> [!secret]- What is actually known about this creature — collapsed by default.
> The name: the **Great Crown Squid**, usually shortened to **Crown Squid**, renamed from the **Colossal Tree Squid** ("tree squid" sounds slightly comedic; "Crown Squid" sounds like an animal somebody could genuinely have named after discovering that the crowns of [[region.aruhe|Aruhe]]'s enormous trees are its habitat). It preserves [[region.aruhe|Aruhe]]'s naming pattern: ordinary words for something that becomes horrible once you understand what they mean.
>
> The island's established rule is not "invent random monsters" but **take a recognizable animal and push some authentic part of its nature until it performs the wrong ecological job**. [[faction.dravosi-crown|the Crown]] Squid is a recognizable cephalopod doing the job of a canopy apex predator.
>
> Design references from the source: Te Papa colossal-squid anatomy; Smithsonian Ocean cephalopod camouflage; PubMed on jumping-spider vision and on biological hydrogen production; Q?rius on the Portuguese man o' war. The three source images (a Te Papa tentacle-hook photograph and two concept images) are external URLs in the source file; no assets promoted yet.

## Tactics

> [!tip] Running this creature — see the linked statblock for the runnable loop.
> Runnable loop: [[creature.aruhe-crown-squid|Great Crown Squid]]. Ecology that is not mechanical: [[faction.dravosi-crown|the Crown]] Squid functions as an [[region.aruhe|Aruhe]] **hazard** rather than a bag of 283 hit points. Escape is geographical, not numerical — reach broad open ground, get into sufficiently deep water, pass beneath terrain too low for its body, force it to cross a grassland valley with no canopy connection, or hurt it badly enough that elephant-sized food stops looking worth the calories. It is an apex predator, not a fantasy villain: it does not hate adventurers and does not defend [[region.aruhe|Aruhe]] out of ideology. The [[creature.blight|Blight]] does not remotely pilot the animal.
>
> Fleeing into a Grassland cut is wonderfully [[region.aruhe|Aruhe]]: escaping the thing in the trees means running into the territory where the [[creature.terror-bird|Terror-Bird]] waits for things to leave cover. [[region.aruhe-the-grasslands|The Grasslands]] already treat open sky as bait. [[faction.dravosi-crown|the Crown]] Squid gives [[region.aruhe-the-quiet|The Quiet]] a new fundamental rule: **the floor is not where the jungle's largest predator lives.**

## Variants

- **Juveniles** — hunt the upper terraces of [[region.aruhe-the-old-gardens|The Old Gardens]] occasionally; mature animals are usually absent there because the trees are too interrupted.
- **Oldest and largest** — found in [[region.aruhe-the-rot|The Rot]], where they are more sessile because prey is abundant.

## Relationships

- **[[creature.aruhe-river-otter|River Otters]]** — ecological boundary. A grabber trailed into occupied water meets six enormous otters pulling the other direction; mature squids treat open water as unsafe. Apex-predator mosaic rather than one monster dominating everything.
- **[[creature.terror-bird|Terror-Bird]]** — dangerous prey, and the opposite psychology: [[faction.dravosi-crown|the Crown]] squid likes a chase; the [[creature.terror-bird|Terror-Bird]]'s first charge is its commitment. Grassland cuts trade one threat for the other.
- **[[creature.bear-elk|Bear-Elk]]** — very dangerous prey.
- **[[creature.wolfrabbit|Wolfrabbits]]** — prey; snacks lifted from the undergrowth.
- **[[creature.snakewood|Snakewood]]** — prey. Colossal Tree Squids eat [[creature.snakewood|Snakewood]], not the reverse; a shredded sixty-foot predatory vine hanging from a branch marks the real apex.
- **[[creature.deer-stalker|Deer-Stalker]]** — deliberately different horror territory: pursuit ("someone is following me") vs surveillance and automated targeting ("you have already been selected").
- **[[creature.blight|Druid Lich]]** — she does not remotely pilot the animal. A Crown Squid hunts like a Crown Squid.
- **[[location.aruhe-the-long-reach|The Long Reach]]** — the jungle-curtain language ("things hang in the overhang and drop on what passes below") is paid off here.
