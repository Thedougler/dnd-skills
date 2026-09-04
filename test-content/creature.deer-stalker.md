---
id: creature.deer-stalker
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
  - "Deer-Stalker"
  - "Deer Stalker"
sources:
  - "_archive/deer-stalkers.md"
  - _archive/aruhe-crown-squid.md
  - _archive/aruhe-grubnade.md
  - _archive/aruhe-razor-grass.md
  - _archive/aruhe-snakewood.md
  - _archive/aruhe-unsaid-macaw.md
tags: []
regions:
  - "[[region.aruhe|Aruhe]]"
  - "[[region.aruhe-the-quiet|The Quiet]]"
  - "[[region.aruhe-the-rot|The Rot]]"
  - "[[region.aruhe-the-grasslands|The Grasslands]]"
locations: []
factions: []
look_canon: provisional
reference_images:
  - "[[assets/creatures/deer-stalker.png|Deer Stalker]]"
player_images: []
---

# Deer-Stalker

```statblock
layout: Basic 5e Layout
name: "Deer-Stalker"
size: Large
type: monstrosity
alignment: Unaligned
ac: "15 (natural armor)"
hp: 85
hit_dice: "10d10 + 30"
speed: "40 ft., climb 20 ft."
stats: [16, 20, 16, 6, 18, 6]
saves:
  - dexterity: 8
  - wisdom: 7
skillsaves:
  - Stealth: +10
  - Perception: +7
  - Survival: +7
senses: "darkvision 120 ft., passive Perception 17"
languages: "—"
cr: 5
traits:
  - name: "Wasting Stillness"
    desc: "The deer-stalker can take the Hide action as a bonus action while in dim light, darkness, or natural foliage. If it has not moved since the start of its previous turn, it has advantage on Dexterity (Stealth) checks, and a creature searching for it cannot benefit from hearing when making its Wisdom (Perception) check. While motionless, the deer-stalker is indistinguishable from a sick deer until it speaks, attacks, or a creature sees its clawed forelimbs or forward-set eyes up close."
  - name: "Shadow Cover"
    desc: "The deer-stalker's movement makes no sound. While in dim light or darkness, moving at half its speed or less does not reveal its position to a creature from which it is hidden unless that creature sees it. The deer-stalker will not willingly enter bright light before it has hit a creature during this hunt."
  - name: "This Meal"
    desc: "When the deer-stalker first notices a creature that interrupted its feeding, or when it needs a new quarry, it chooses one creature it can see as its quarry — preferring the most isolated creature or the one that last touched its meal. It knows the direction of its quarry while the quarry is within 1 mile, and it has advantage on Wisdom (Survival) checks made to track that creature and on Wisdom (Perception) checks to hear it. Once on each of the deer-stalker's turns, when it hits its quarry with an attack while fewer than two conscious creatures other than the quarry are within 10 feet of the quarry, the attack deals an extra 7 (2d6) damage. The deer-stalker chooses a new quarry when the current quarry dies, when two or more conscious creatures other than the quarry are within 10 feet of the quarry at the start of the deer-stalker's turn, or when the deer-stalker ends its turn more than 1 mile from the quarry."
  - name: "Famished"
    desc: "The deer-stalker is Famished until it uses Feed or spends 1 minute consuming a carcass. While it is not Famished, Lost Nerve treats two qualifying creatures as enough to force a retreat."
  - name: "Lost Nerve"
    desc: "At the start of its turn, if three or more hostile creatures that are not unconscious are within 30 feet of it (two or more if it is not Famished), the deer-stalker must take the Dash or Hide action and move away. It can drag one grappled creature with it without reducing its speed. This trait does not apply if the deer-stalker has reduced a creature to 0 hit points since the start of its last turn."
actions:
  - name: "Multiattack"
    desc: "The deer-stalker makes two Claw attacks."
  - name: "Claw"
    desc: "Melee Weapon Attack: +8 to hit, reach 10 ft., one target. Hit: 12 (2d6 + 5) slashing damage. If the target is Medium or smaller, the deer-stalker can grapple it (escape DC 14) instead of dealing the attack's slashing damage. The deer-stalker can grapple only one creature at a time."
  - name: "Snatch from the Dim (Recharge 5–6)"
    desc: "The deer-stalker can use this action only while hidden in dim light, darkness, or natural foliage. It moves up to its speed without provoking opportunity attacks and makes one Claw attack. On a hit, the attack deals its normal damage and, if the target is Medium or smaller, the target is also grappled (escape DC 14). The deer-stalker can then move up to half its speed, carrying a grappled creature with it without reducing its speed. If the target is the deer-stalker's quarry, This Meal can apply."
  - name: "Feed"
    desc: "The deer-stalker feeds on a carcass or on one unconscious or dead creature within 5 feet of it. It is no longer Famished. A creature the deer-stalker is feeding on that is at 0 hit points has disadvantage on death saving throws until the deer-stalker stops feeding or is moved away."
bonus_actions:
  - name: "Borrowed Voice"
    desc: "The deer-stalker reproduces a sound it has heard, including a voice. The sound originates from its space and does not automatically reveal the deer-stalker if it is hidden, though a creature that hears the sound knows the direction. The deer-stalker prefers sounds that previously caused a specific creature to move toward their source, and it uses them out of context, looping a word or stretching a phrase. A creature that can see the original speaker knows the sound is an imitation. A creature that heard the original sound has advantage on a DC 14 Wisdom (Insight) check to recognize the imitation. After the deer-stalker uses a given sound without drawing a creature closer, it abandons that sound."
reactions:
  - name: "Silent Retreat"
    desc: "When the deer-stalker is hit by an attack, if three or more hostile creatures that are not unconscious are within 30 feet of it, or if it is not Famished, it can move up to half its speed without provoking opportunity attacks. If it ends this movement in dim light, darkness, or natural foliage, it can immediately attempt to Hide."
```

## Overview

> [!narration] Player-facing description — read or adapt at the table.
A deer stands on a carcass, hips turned the wrong way, taller than a man. Forelimbs end in long claws, not hooves. It crashes into the brush, throat rattling wet, and the sweet rot of the meal hangs after it. Minutes later the same shape is already in the trees: chin dripping, eyes set forward, not blinking. It does not lean with the wind.

![[assets/creatures/deer-stalker.png]]

Blight-maddened deer. Seven to nine feet, Large, hungry. Obsession is finish the kill you interrupted, not a person. The first bolt is a ruse. What comes back hunts like a stalker and still thinks like an animal that is afraid of bigger things.

## Ecology

These were deer. The Blight cranked deer nature until it broke: the freeze, the watch, the wasting, the bolt. Hips rotated. Fore-hooves split into gripping digits with knife claws. The jaw grew incisors that do not belong in an herbivore. Rear legs stay digitigrade; the rack stays. Stillness looks like end-stage wasting — thin, wet chin, vacant forward stare, a body that forgot how to leave. When it hunts, the same broken body moves clean.

It is a predator that takes easy meat. Carcasses and dying animals bigger fauna leave are the usual meal. A single adult puts down about a hundred pounds in an hour and still looks starved. It does not contest [[creature.bear-elk|Bear-Elk]] or [[creature.terror-bird|Terror-Bird]]. Light is how those things notice it. Shadows are cover. Bright firelight is "I do not know what else is watching."

## Behavior

Solitary. Two in the same stretch ignore each other and do not share a meal. They do not herd. They do not graze.

**Meeting.** It is on a carcass or a dying animal. Disturbed, it crashes away too loud, too sick. Minutes later it has already reacquired from cover. The people who made it drop the meal are the hunting ground.

**Lock.** It fixes on whoever is most alone, or who last touched the meal. The lock holds until that creature is dead, back among ready companions, or the stalker is driven off before contact. Then it takes the next easiest body. Sleeping or unconscious creatures are not ready threats. One person awake can be enough if it has not replaced the meal; it would rather call them a step into the trees. Two people awake and it waits. Three or more ready threats and it leaves.

**Night.** Almost never seen by day. Daylight is exposure. It hunts the dim edge after dark. It will not walk into the bright ring of a fire. Once it is already on someone and still hungry, light and noise will not make it let go.

**Voice.** It plays back sounds it has heard, including voices. It watches what makes this prey move. Favorite lure: a companion calling that person's name, after it has heard that work. It uses the sound wrong — out of context, a word on a loop, wet, held too long. It will throw a line from last night's fire, or last week's. That is how long it has been sitting in the dark. It drops a lure that stops drawing anyone closer. Answering is not a curse. Walking to the sound is walking to it.

**Hunger.** It always looks empty. Until it replaces the lost meal it may stay against two ready threats. After it feeds — a short messy feed on a downed creature, or meat left for it — it goes back to taking only one. Any meat starts it eating. A snack buys minutes. A real carcass buys the hour. If your scent is still the nearer meal when it finishes, the hunt is not over. Leave while it feeds.

**After a kill.** This hunt ends. Another deer-stalker only starts if someone interrupts *that* one's food.

## Habitat

[[region.aruhe-the-quiet|The Quiet]] into [[region.aruhe-the-rot|The Rot]] on [[region.aruhe|Aruhe]], and inside the eight-foot grass of [[region.aruhe-the-grasslands|The Grasslands]]. Thick cover: closed canopy, grass walls, pale rock at [[location.aruhe-the-clear-lake|The Clear Lake]]. In a valley they stand in the blades and do not lean with the wind. They skirt [[hazard.razer-grass|Razer-Grass]] stands — the one green thing on the island even a deer-stalker does not walk through.

## Lore

> [!secret]- What is actually known about this creature — collapsed by default.
Not a witch. Not a former person. Not named for any mainland hunger-spirit. The Blight made a deer finish meals the way a wasting deer forgets to run, then gave it the claws to do it. Sailors who come back from [[region.aruhe-the-quiet|The Quiet]] remember a deer that bolted from a kill and a voice later that belonged to someone at their fire. [[creature.grung|Grung]] already treat that band as mute close and do not walk it.

## Tactics

> [!tip] Running this creature — see the linked statblock for the runnable loop.
Runnable loop: [[creature.deer-stalker]]. Ecology that is not mechanical: interrupt a carcass, crash-ruse, night return, playback of old talk, bait-and-leave, solitary, hides from larger fauna.

## Variants

Adults are seven to nine feet. Smaller sightings are younger animals, not a second species.

## Relationships

- [[creature.blight|Druid Lich]] — the corruption that rebuilt the deer.
- [[creature.grubnade|Grubnade]] — the one thing it steps around. A learned predator; it has the burn scars to show for it.
- [[hazard.razer-grass|Razer-Grass]] — skirted, like the [[creature.grubnade|Grubnade]]. A learned predator.
- [[creature.bear-elk|Bear-Elk]] / [[creature.terror-bird|Terror-Bird]] — things it will not be seen by. It yields carcasses to them.
- [[region.aruhe-the-quiet|The Quiet]], [[region.aruhe-the-rot|The Rot]], [[region.aruhe-the-grasslands|The Grasslands]], [[location.aruhe-the-clear-lake|The Clear Lake]] — cover and watering-hole still-hunts.
- [[creature.aruhe-crown-squid|Crown Squid]] — deliberately different horror territory. The deer-stalker owns "someone is following me"; [[faction.dravosi-crown|the Crown]] squid owns surveillance and automated targeting — you were already selected.
- [[creature.unsaid-macaw|Unsaid Macaw]] — deliberately different horror territory. The deer-stalker repeats what was already spoken; the macaw says what was never spoken aloud. One steals voices, the other steals the unsaid.
- [[creature.snakewood|Snakewood]] — refused to pass under. Deer-Stalkers give mature [[creature.snakewood|Snakewood]] stretches an absurdly wide berth, revealing the ambusher's location by the shape of their avoidance.
