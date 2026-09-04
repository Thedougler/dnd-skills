---
id: creature.snakewood
kind: creature
subtype: plant
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
  - "Snakewood"
sources:
  - _archive/aruhe-snakewood.md
tags:
  - horror
  - ambush-predator
regions:
  - "[[region.aruhe|Aruhe]]"
  - "[[region.aruhe-the-quiet|The Quiet]]"
  - "[[region.aruhe-the-rot|The Rot]]"
  - "[[region.aruhe-the-old-gardens|The Old Gardens]]"
locations: []
factions: []
look_canon: provisional
reference_images: []
player_images: []
---

# Snakewood

```statblock
layout: Basic 5e Layout
name: "Snakewood"
size: Huge
type: plant
alignment: unaligned
ac: "15 (layered woody stems)"
hp: 127
hit_dice: "15d12 + 30"
speed: "0 ft."
stats: [20, 14, 15, 2, 15, 3]
skillsaves:
  - Perception: 5
  - Stealth: 5
condition_immunities: "prone"
senses: "blindsight 60 ft. while in contact with vegetation, passive Perception 15"
languages: "—"
cr: 6
traits:
  - name: "False Appearance"
    desc: "While the Snakewood remains motionless among vegetation, it is indistinguishable from an ordinary mass of large jungle vines."
  - name: "Root-Anchored"
    desc: "The Snakewood cannot willingly move its root crown and can't be knocked prone or moved against its will. Its articulated body can strike anywhere within 60 feet of the root crown, provided continuous branches, trunks, or other substantial vegetation connect it to that space. Its speed is 0 while it still behaves like an arboreal predator."
  - name: "Distributed Body"
    desc: "A creature grappled by the Snakewood can attack the grasping bundle directly. The bundle has AC 15 and 15 hit points. If destroyed, that grapple immediately ends. Damage dealt to a grasping bundle doesn't reduce the Snakewood's hit points. At the beginning of the Snakewood's next turn, neighboring vines can form a replacement bundle."
  - name: "Load Sharing"
    desc: "When one of the Snakewood's grasping bundles is destroyed, another creature currently grappled by the Snakewood is immediately pulled 5 feet toward the canopy."
actions:
  - name: "Multiattack"
    desc: "The Snakewood makes one Snatching Jaws attack and either uses Constrict or Reel."
  - name: "Snatching Jaws"
    desc: "Melee Weapon Attack: +8 to hit, reach 60 ft., one Large or smaller creature. Hit: 12 (2d6 + 5) piercing damage, and the target is grappled (escape DC 16). Until this grapple ends, the target is restrained. The Snakewood can grapple no more than two creatures simultaneously."
  - name: "Reel"
    desc: "The Snakewood pulls each creature grappled by it up to 20 feet toward the canopy. If this movement leaves the victim unsupported, it hangs suspended."
  - name: "Constrict"
    desc: "One creature grappled by the Snakewood takes 16 (2d10 + 5) bludgeoning damage. If the target is already suspended at least 10 feet above the ground, the damage increases to 21 (3d10 + 5)."
  - name: "External Digestion"
    desc: "One creature grappled by the Snakewood must make a DC 15 Constitution saving throw. On a failed save, pale digestive tissue pushes between the jaw-vines and the target takes 18 (4d8) acid damage. On a successful save, it takes half as much. A creature damaged this way continues to take 7 (2d6) acid damage at the start of each of its turns until the grapple ends or a creature uses an action to scrape or wash away the digestive sap. The Snakewood normally doesn't use this until prey has been hauled into the canopy."
reactions:
  - name: "Reflexive Snare"
    desc: "When a creature within 60 feet of the Snakewood that the plant can sense falls prone, jumps, falls, or is forcibly moved, the Snakewood can make one Snatching Jaws attack against it."
```

## Overview

> [!narration] Player-facing description — read or adapt at the table.
> At first it is only another rope-vine among thousands: dull green-brown, leafless beneath the canopy, thick as a man's arm where several stems twist together.
>
> Then a branch thirty feet overhead bends.
>
> The vine does not fall.
>
> **It strikes.**
>
> Half a dozen stems separate in flight, opening around one another like fingers. They meet around the prey with a wet wooden clap. What looked like one vine becomes two jaws, then a coil, and the thing on the ground is suddenly going upward.
>
> There is no head behind it. No eyes. No throat.
>
> Just sixty feet of vegetation tightening through the trees.

A Huge predatory liana on [[region.aruhe|Aruhe]] that uses the canopy as a skeleton. At rest it is an especially large bundle of ordinary-looking lianas; the snake appears only when it moves, and its "head" is whichever five or six leading vines are currently braided into a wedge-shaped striking structure. It follows [[region.aruhe|Aruhe]]'s rule of familiar organisms pushed past their proper job rather than arbitrary fantasy monsters. Runnable identity: [[creature.snakewood|Snakewood]].

## Ecology

**What it is.** Each "Snakewood" is not a single vine but a clonal colony grown from one root crown: dozens of genetically identical stems fused through natural grafting until water, sugars, and electrical signals pass between them. There is no single spinal vine. Cut one and the others simply take its load.

**The canopy as skeleton.** It is a liana that took the normal evolutionary cheat of "let the trees hold my weight" and pushed it until the vine no longer merely climbs through the canopy — it uses the canopy as a skeleton. Twenty or thirty different contact points support the body: hooked tendrils grip branches, others release, and the body redistributes its weight from tree to tree. Its movement resembles a python flowing over branches, but mechanically it is more like a suspension bridge dismantling and rebuilding itself one cable at a time.

**Rapid hydraulic motion.** Snakewood does not continuously "flex muscles." Sections are cocked under hydraulic tension and release explosively — an [[region.aruhe|Aruhe]] exaggeration of mechanisms that genuinely exist in plants. Venus flytraps can close in less than half a second; Snakewood has taken rapid hydraulic movement and touch-response and applied it to enormous pre-tensioned stems.

**Feeding.** The temporary jaws don't chew. Once they clamp around something, pale glandular tendrils evert between them and flood the enclosed prey with proteolytic sap — the botanical equivalent of a sea star partially digesting prey outside its body before drawing the food inward.

**Scale.** Sixty feet is roughly two and a half times the length of a reliably measured giant python (wild record 23 ft 8 in; longest Guinness-recorded captive 25 ft 2 in).

## Behavior

**Appearance is motion.** At rest Snakewood should not resemble a snake. Its rapid motion is an [[region.aruhe|Aruhe]] exaggeration of genuine plant mechanisms; it stays fast without becoming animal-like.

**Hunting.** It does not attack groups indiscriminately. It waits for one body to pass beneath the portion of canopy where its strike is easiest — a lone traveler is ideal, a wounded animal better, something already falling almost irresistible. It usually takes one creature and withdraws rather than fighting an adventuring party. If the first strike misses, the "head" instantly disassembles into six ordinary vines and the entire sixty-foot body starts flowing backward through the canopy. It can't flee from its root, but finding the root crown among sixty feet of jungle is another matter: the party isn't chasing the monster, they're following the monster backward to discover what part of the forest it actually is.

**The metaphor.** The source frames the horror as industrial entanglement — being caught in machinery — not snakes and not strangulation. A single little tendril catches you; then another takes tension; then another. Struggling doesn't persuade anything to let go; it transfers your weight deeper into the mechanism. Cut one strand and the neighboring strands instantly inherit its load. The prey is reeled upward like something caught in a winch. Snakewood makes almost no sound: no roar, no hiss, just someone's boots leaving the ground.

**Tells the players can learn.** A Snakewood hunting territory becomes recognizable once you've survived one:
- **DC 13 Nature** — several different-looking vines are actually shoots of the same plant.
- **DC 14 Survival** — animal trails conspicuously avoid walking directly beneath certain branches.
- **DC 15 Perception** — vines above the trail aren't hanging under their own weight; several are visibly under tension.
- **DC 16 Nature** — parallel compression scars on branches show where the plant repeatedly braces itself before striking.
- **Best clue of all** — no carcasses, only things that fell off carcasses: a snapped antler, one boot, a bit of harness, a handful of feathers. Everything edible went upward.

## Habitat

Primarily [[region.aruhe-the-quiet|The Quiet]], which already emphasizes a sealed, silent canopy where sight dies within a few paces — making an overhead predator especially appropriate. Specimens grow larger but less healthy-looking in [[region.aruhe-the-rot|The Rot]]. [[region.aruhe-the-old-gardens|The Old Gardens]] can contain younger specimens, but the sixty-foot adults stay farther inland so they don't replace [[creature.vine-lash|Vine Lash]].

## Lore

> [!secret]- What is actually known about this creature — collapsed by default.
> Design intent follows [[region.aruhe|Aruhe]]'s rule: take a recognizable organism and push some authentic part of its nature until it performs the wrong ecological job. Snakewood is almost completely mundane underneath — a liana whose biology genuinely matches the structural premise. Design grounding in the source: Smithsonian Natural History Museum (liana flexible stems, climbing structures, dependence on surrounding trees), Kew Gardens (Venus flytrap rapid hydraulic movement), Smithsonian Science Education Center (starfish external digestion), Guinness World Records (giant-python scale comparison).
>
> The design brief also specifies what Snakewood is not: no eyes, no breathing, no hiss imitation. When the jaw opens, tiny, pale, intensely sweet-smelling flowers line the inner surfaces of the grasping vines where an animal expects gums and teeth; the jaw closes and the flowers disappear.
>
> The two concept images in the source are external URLs; no assets promoted yet.

## Tactics

> [!tip] Running this creature — see the linked statblock for the runnable loop.
> Runnable loop: [[creature.snakewood|Snakewood]]. Combat identity (catch → reel → crush → digest) lives on the statblock page. Ecology that is not mechanical: the pursuit is investigative, not a chase — follow the monster backward to the root crown. Snakewood sometimes steals kills from [[region.aruhe|Aruhe]]'s other predators through its Reflexive Snare, which is excellent ecology.

## Variants

- **Younger specimens** — found in [[region.aruhe-the-old-gardens|The Old Gardens]]; the sixty-foot adults stay farther inland.
- **Larger, less healthy specimens** — found in [[region.aruhe-the-rot|The Rot]].

## Relationships

- **[[creature.vine-lash|Vine Lash]]** — the escalation of the same family. [[creature.vine-lash|Vine Lash]] is the warning ("some vines attack"); Snakewood is the later revelation ("no — some vines hunt"). Snakewood's adults stay inland partly so they don't replace [[creature.vine-lash|Vine Lash]].
- **[[creature.wolfrabbit|Wolfrabbits]]** — learn its strike zones and deliberately drive prey beneath them.
- **[[creature.deer-stalker|Deer-Stalkers]]** — refuse to pass under mature Snakewood, revealing its location by giving apparently harmless stretches of trail an absurdly wide berth.
- **[[creature.terror-bird|Terror-Birds]]** — too large to be normal prey; young Snakewoods occasionally grab one and get ripped completely out of the canopy.
- **[[creature.aruhe-crown-squid|Colossal Tree Squid]]** — eats Snakewood, not the reverse. Seeing sixty feet of predatory vine hanging shredded from a branch tells adventurers that something higher in the canopy food chain was hungry; [[faction.dravosi-crown|the Crown]] Squid stays the real apex.
