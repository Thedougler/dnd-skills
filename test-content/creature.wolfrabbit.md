---
id: creature.wolfrabbit
kind: creature
subtype: monstrosity
scope: setting
campaign: shattered-sea
audience: [agent, dm]
canon: provisional
status: active
importance: supporting
schema: creature@1
created: 2026-08-17
updated: 2026-08-20
aliases:
  - "Wolfrabbit"
  - "Wolfrabbits"
sources:
  - "_archive/malformed-monsters/wolfrabbit.md"
  - _raw/wolfrabbits.md
  - _archive/aruhe-crown-squid.md
  - _archive/aruhe-grubnade.md
  - _archive/aruhe-razor-grass.md
  - _archive/aruhe-snakewood.md
  - _archive/aruhe-caves.md
tags:
  - combat
  - horror
regions:
  - "[[region.aruhe|Aruhe]]"
  - "[[region.aruhe-the-old-gardens|The Old Gardens]]"
  - "[[region.aruhe-the-quiet|The Quiet]]"
  - "[[region.midchain-east|The Eastern Midchain]]"
locations: []
factions: []
look_canon: provisional
reference_images:
  - "[[assets/creatures/wolfrabbit.png|Wolfrabbit]]"
player_images: []
provenance:
  extracted: 0.90
  inferred: 0.05
  ambiguous: 0.05
base_confidence: 0.4
lifecycle: draft
lifecycle_changed: 2026-08-19
tier: supporting
---

# Wolfrabbit

```statblock
layout: Basic 5e Layout
name: "Wolfrabbit"
size: Medium
type: monstrosity
alignment: unaligned
ac: "14 (natural armor)"
hp: 45
hit_dice: "6d10 + 12"
speed: "40 ft."
stats: [16, 18, 14, 4, 14, 6]
skillsaves:
  - Perception: +4
  - Stealth: +6
senses: "darkvision 60 ft., passive Perception 14"
languages: "—"
cr: 2
traits:
  - name: "Standing Leap"
    desc: "The wolfrabbit can long jump up to 30 feet and high jump up to 15 feet, with or without a running start. It can jump over creatures smaller than itself, and nonmagical difficult terrain on the ground does not cost it additional movement while jumping."
  - name: "Pack Rend"
    desc: "Once per turn when the wolfrabbit hits a prone creature with its Bite, the attack deals an extra 4 (1d8) piercing damage if another wolfrabbit is within 5 feet of the target."
  - name: "Blood-Scented"
    desc: "The wolfrabbit has advantage on Wisdom (Perception) checks made to locate a creature that is below its hit point maximum."
actions:
  - name: "Bite"
    desc: "Melee Weapon Attack: +5 to hit, reach 5 ft., one target. Hit: 9 (1d12 + 3) piercing damage."
  - name: "Raking Claws"
    desc: "Melee Weapon Attack: +5 to hit, reach 5 ft., one target. Hit: 8 (2d4 + 3) slashing damage."
  - name: "Pouncing Bound"
    desc: "The wolfrabbit leaps up to 30 feet to an unoccupied space it can see and makes one Raking Claws attack against a creature within 5 feet of where it lands. If the wolfrabbit began the leap at least 20 feet from the target and the attack hits, the target must succeed on a DC 13 Strength saving throw or fall prone. If the target remains standing after the attack, the wolfrabbit can immediately leap up to 10 feet to an unoccupied space it can see. This movement does not provoke an opportunity attack from that target."
bonus_actions:
  - name: "Devour the Pack"
    desc: "The wolfrabbit tears into the corpse of another wolfrabbit within 5 feet that died since the end of the wolfrabbit's previous turn. The corpse is mangled and cannot be used for this ability again. The wolfrabbit gains 7 temporary hit points and becomes Frenzied until the end of its next turn. While Frenzied, its speed increases by 10 feet and its Bite deals an extra 3 (1d6) piercing damage."
reactions:
  - name: "Frenzy Toward the Fallen"
    desc: "When another wolfrabbit the wolfrabbit can see within 30 feet drops to 0 hit points, the wolfrabbit can immediately leap up to 15 feet toward that creature without provoking opportunity attacks."
```

## Overview

> [!narration] Player-facing description — read or adapt at the table.
Wolf-sized rabbits with dark striping and spots across dark fur. The silhouette reads rabbit (long ears, whiskers, twitching nose) but the musculature underneath belongs to a hunting cat. Heavy feline shoulders and haunches drive large ripping claws. Red glowing eyes track movement. Blood and drool mat the fur around the muzzle. They move in packs of four to six through the [[region.aruhe|Aruhe]] terraces and outer jungle, hunting dawn and dusk.

![[assets/creatures/wolfrabbit.png]]

## Ecology

**[[creature.blight|The Blight]]'s corruption inverted these creatures from flight to pursuit.** The same explosive hindquarter musculature that lets a normal rabbit bolt from a fox now launches a wolf-sized body thirty feet through canopy brush. Their breeding cycle accelerated alongside their appetite. A warren produces a new litter every few weeks, and [[region.aruhe|Aruhe]]'s prey base cannot keep up. The pack turns on its own dead because it has to. The corruption did not just make them bigger. It pushed them past herbivore into committed predator.

**Home zones:** [[region.aruhe-the-old-gardens|the Old Gardens]] (collapsed terraces) into [[region.aruhe-the-quiet|the Quiet]] (outer jungle canopy). The breeding warrens honeycomb the collapsed terrace stonework. Every terrace wall has burrows running through it.

**Hunting pattern:** the pack stalks from terrace brush and launches from elevation, closing thirty feet in a single bound. They hunt dawn and dusk and do not chase retreating prey far. They know the island provides.

## Behavior

They hunt dawn and dusk in packs of four to six. They stalk from terrace brush and launch from elevation. They do not chase retreating prey far. They know the island provides. They leap [[vehicle.the-narrow|Narrow]] [[hazard.razer-grass|Razer-Grass]] bands rather than landing inside them.

**Pack Frenzy:** When a pack member falls, the survivors enter a cannibalistic frenzy — Devour the Pack grants temporary HP and a speed/damage boost, while Frenzy Toward the Fallen lets them leap toward fallen allies without provoking opportunity attacks.

**Standing Leap:** Can long jump up to 30 feet and high jump up to 15 feet, with or without a running start. Can jump over creatures smaller than itself, and nonmagical difficult terrain on the ground does not cost additional movement while jumping.

**Blood-Scented:** Advantage on Wisdom (Perception) checks to locate creatures below their hit point maximum.

## Habitat

Home zones: [[region.aruhe-the-old-gardens|The Old Gardens]] into [[region.aruhe-the-quiet|The Quiet]] on [[region.aruhe|Aruhe]]. The breeding warrens honeycomb the collapsed terrace stonework. Every terrace wall has burrows running through it.

Also found in: [[region.midchain-east|Midchain East]], [[region.aruhe|Aruhe]] coastal forests.

At [[location.aruhe-the-old-mouth|The Old Mouth]] on the lower [[region.aruhe-the-old-gardens|Old Gardens]], warrens stop abruptly along one wall at the point where daylight disappears — wolfrabbits refuse to den below it. Whatever lives down there outranks the thing that hunts up here.

## Lore

> [!secret]- What is actually known about this creature — collapsed by default.
Source is silent.

## Tactics

> [!tip] Running this creature — see the linked statblock for the runnable loop.
Runnable loop: [[creature.wolfrabbit]] (individual) or  (pack of 4-6 as coordinated unit). Ecology that is not mechanical: packs of four to six, dawn/dusk, elevation launches, they do not chase far, pack frenzy on fallen allies.

### Individual Tactics (CR 2)

**Opener:** Pouncing Bound from 30 ft — leap, Raking Claws, potential prone on DC 13 Str save. If target stays standing, immediate 10 ft leap to reposition.

**Pressure:** Multiattack not available; alternates Bite (+5, 1d12+3) and Raking Claws (+5, 2d4+3). Pack Rend: once/turn when hitting prone target with Bite and another wolfrabbit within 5 ft, +1d8 piercing.

**Pivot:** Devour the Pack (bonus action) on fallen ally within 5 ft — 7 temp HP, Frenzied (speed +10, Bite +1d6) until end of next turn. Frenzy Toward the Fallen (reaction): when ally drops within 30 ft, leap 15 ft toward them without provoking.

**Exit:** Do not chase retreating prey far. Know the island provides.

### Pack Tactics (CR 5 encounter, 4-6 individuals)

Coordinate Pouncing Bounds to surround. Focus fire on prone targets via Pack Rend. When one falls, survivors frenzy — action economy spikes. Blood-Scented tracks wounded PCs across battlefield.

## Variants

Source is silent.

## Relationships

The drop names [[region.aruhe|Aruhe]], [[region.aruhe-the-old-gardens|The Old Gardens]], [[region.aruhe-the-quiet|The Quiet]], [[region.midchain-east|Midchain East]], and the [[creature.blight|Blight]]. Those pages are not minted from this drop.

- **[[creature.aruhe-crown-squid|Crown Squid]]** — prey. The canopy apex lifts them from the undergrowth as snacks.
- **[[creature.snakewood|Snakewood]]** — mutual strategy. Wolfrabbits learn its strike zones and deliberately drive prey beneath them.
- **[[creature.grubnade|Grubnade]]** — the one smell that aborts a pounce. A mature [[creature.grubnade|Grubnade]] in foliage makes the pack break off.
- **[[hazard.razer-grass|Razer-Grass]]** — crossed by leap, never landed in. A pack that clears a [[vehicle.the-narrow|Narrow]] white band keeps its momentum and its feet.

## Statblock Reference

**Individual Wolfrabbit (CR 2):** `statblock.wolfrabbit`
- Medium monstrosity, unaligned
- AC 14 (natural armor), HP 45 (6d10 + 12)
- Speed 40 ft.
- Stats: [16, 18, 14, 4, 14, 6]
- Skills: Perception +4, Stealth +6
- Senses: darkvision 60 ft., passive Perception 14
- Traits: Standing Leap, Pack Rend, Blood-Scented
- Actions: Bite (+5, 1d12+3), Raking Claws (+5, 2d4+3), Pouncing Bound (leap 30 ft + Raking Claws, DC 13 Str prone)
- Bonus: Devour the Pack (cannibalize fallen ally -> 7 temp HP + Frenzied: speed +10, Bite +1d6)
- Reaction: Frenzy Toward the Fallen (ally drops within 30 ft -> leap 15 ft toward them)

**Pack Encounter (CR 5, 4-6 individuals):** Coordinated Pouncing Bounds, Pack Rend focus fire, cascading Devour the Pack frenzies.
