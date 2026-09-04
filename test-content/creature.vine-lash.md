---
id: creature.vine-lash
kind: creature
subtype: plant
scope: setting
campaign: shattered-sea
audience: [agent, dm]
canon: provisional
status: active
importance: supporting
schema: creature@1
created: 2026-08-18
updated: 2026-08-20
aliases:
  - "Vine Lash"
sources:
  - _archive/vine-lash.md
  - _archive/aruhe-snakewood.md
summary: Shoulder-thick Aruhe vine. Island growth turned predatory. Hangs over trails.
tags: []
regions:
  - "[[region.aruhe|Aruhe]]"
  - "[[region.aruhe-the-old-gardens|The Old Gardens]]"
  - "[[region.aruhe-the-quiet|The Quiet]]"
locations: []
factions: []
relationships:
  - target: "[[creature.blight|Druid Lich]]"
    type: related_to
  - target: "[[region.aruhe-the-old-gardens|The Old Gardens]]"
    type: related_to
provenance:
  extracted: 0.9
  inferred: 0.1
  ambiguous: 0.0
---

# Vine Lash

```statblock
layout: Basic 5e Layout
name: "Vine Lash"
size: Medium
type: plant
alignment: unaligned
ac: "12 (natural armor)"
hp: 52
hit_dice: "8d8 + 16"
speed: "10 ft., climb 10 ft."
stats: [14, 8, 14, 1, 10, 1]
damage_vulnerabilities: "fire"
condition_immunities: "blinded, deafened, frightened"
senses: "blindsight 30 ft. (blind beyond this radius), passive Perception 10"
languages: "—"
cr: 3
traits:
  - name: "False Appearance"
    desc: "While the vine lash remains motionless, it is indistinguishable from ordinary jungle vines."
  - name: "Spider Climb"
    desc: "The vine lash can climb difficult surfaces, including upside down on ceilings, without needing to make an ability check."
actions:
  - name: "Multiattack"
    desc: "The vine lash makes two Tendril attacks."
  - name: "Tendril"
    desc: "Melee Weapon Attack: +4 to hit, reach 15 ft., one target. Hit: 7 (2d4 + 2) bludgeoning damage, and the target is grappled (escape DC 12). The vine lash can grapple up to two creatures at a time."
  - name: "Constrict"
    desc: "Each creature grappled by the vine lash takes 9 (2d6 + 2) bludgeoning damage."
```

## Overview

> [!narration] Appearance
> Jungle vine, shoulder-thick, hanging like every other vine. No leaves. No fruit. Rope in a canopy.

Blight-animated plant. Chassis [[creature.vine-lash]].

## Ecology

Not a transplant. [[creature.blight|Druid Lich]] turned what was already growing. Feeds on blood and bone meal through the root network. Thickest where terrace stone gives anchors and the canopy gives height.

## Behavior

Does not move until something walks under. Then it whips, wraps, squeezes.

## Habitat

[[region.aruhe-the-old-gardens|The Old Gardens]] into [[region.aruhe-the-quiet|The Quiet]]. Collapsed terrace walls. Game trails and water.

## Lore

Source is silent.

## Tactics

See [[creature.vine-lash]].

## Variants

Source is silent.

## Relationships

- [[creature.blight|Druid Lich]] — animator.
- [[creature.strangler-fig|Strangler Fig]] — another [[region.aruhe|Aruhe]] plant hunter.
- [[creature.snakewood|Snakewood]] — the escalation of the same family. Vine Lash is the warning ("some vines attack"); [[creature.snakewood|Snakewood]] is the later revelation ("no — some vines hunt"). [[creature.snakewood|Snakewood]]'s sixty-foot adults stay farther inland so they don't replace Vine Lash in [[region.aruhe-the-old-gardens|The Old Gardens]].
