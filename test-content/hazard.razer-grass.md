---
id: hazard.razer-grass
kind: hazard
subtype: environmental
scope: setting
campaign: shattered-sea
audience: [agent, dm]
canon: provisional
status: active
importance: supporting
schema: hazard@1
created: 2026-08-20
updated: 2026-08-20
aliases:
  - Razer-Grass
  - Razer Grass
sources:
  - _archive/aruhe-razor-grass.md
tags: [horror, nature, survival, blight]
locations:
  - "[[region.aruhe-the-grasslands|The Grasslands]]"
  - "[[region.aruhe|Aruhe]]"
encounters: []
dc_detection: 14
dc_save: 14
damage: 1d4 slashing per 5 ft moved (Razor Field); 2d6 slashing, DC 14 Dex half (Shatter); Glass-Choked on failed DC 14 Con (Glass Bloom)
---

# Razer-Grass

## Description

> [!narration] Player-facing description — read or adapt at the table.
> Beyond the ordinary grass, the valley turns white. Not dead-white. Winter-white. Waist-high stalks cover perhaps half an acre, pale beneath the noon sun, every blade glittering as though the first frost of the year settled here and nowhere else. There is no frost on your breath. Wind passes across the field. The grass moves. The glitter doesn't.

Razer-grass is grass armored with **opaline glass** — the plant version of [[region.aruhe|Aruhe]]'s rule: a familiar shape doing the wrong job. Grass already armors itself with silica; the [[creature.blight|Blight]] simply let it finish the job. Each blade is living pale green-white vascular tissue inside a continuous shell of cloudy white opaline silica, thickest along the margins — essentially **living grass inside a disposable glass knife**. The actual cutting edge is almost transparent; the shell's thousands of microscopic fractures scatter sunlight into the snow-white sparkle. A field reads as first snow on a hot island that has never seen frost.

The blades are dangerous. Breaking them is worse. ^[inferred — the exposure fear the design builds on: you were in danger before you understood you were in danger]

## Trigger

Contact. Razer-grass is **Difficult Terrain**; moving through intact stands cuts. Breaking a stand triggers Shatter, and Shatter triggers Glass Bloom.

## Effect

> [!danger] What happens when the hazard triggers.

**Razor Field.** Whenever a creature travels through intact Razer-grass, it takes **1d4 Slashing damage for every 5 feet it moves through the vegetation**. No saving throw — deliberately half of *Spike Growth*'s rate, because fields can be enormous and permanent. Twenty feet of forcing through averages 10 damage: enough to make somebody bloody without turning every patch into a death sentence.

**Careful Passage.** A creature can use its **action** to slowly part, brace, and negotiate the stalks. Until the start of its next turn, it can move up to **5 feet through Razer-grass without taking its movement damage**. No roll. Once players know what it is, the question becomes how much time you can afford — which is what makes predators interesting.

**Shatter.** The outer shells are brittle. A 5-foot section of intact Razer-grass shatters if any of the following occurs within it: a creature falls Prone; a creature Dashes through it; a creature is forcibly moved at least 10 feet through it; it takes Thunder damage; it takes significant Bludgeoning damage; someone deliberately tramples or smashes it. The stand goes off with a tremendous crash — a pane of glass dropped onto stone, and the stalks beside it break with it. Each creature in or within 5 feet of the shattered space makes a **DC 14 Dexterity saving throw**, taking **2d6 Slashing damage** on a failure or half on a success.

**Glass Bloom.** For one round after a section shatters, a glittering haze fills a **10-foot radius** around it. A creature that breathes within the cloud must make a **DC 14 Constitution saving throw**. On a failure it becomes **Glass-Choked** until it completes a Short or Long Rest:

- Speed reduced by 10 feet; and
- disadvantage on Constitution saving throws caused by environmental hazards.

Glass-Choked is a secondary consequence nobody was thinking about at first, and it compounds [[region.aruhe|Aruhe]]'s other environmental pressures — [[region.aruhe-the-rot|The Rot]]'s corrupted air already attacks the lungs with Constitution saves against exhaustion, so a Glass-Choked creature carries the exposure farther inland at real cost. ^[inferred — campaign-interaction design intent]

## Detection

From more than 30 feet away, Razer-grass resembles pale grass covered in frost. A creature examining it from nearby recognizes that something is wrong with a **DC 14 Wisdom (Perception or Survival)** check. On a success, it notices one or more of:

- nothing large has walked through it;
- individual sparkles remain fixed when the grass moves;
- some stalks end in geometric fracture lines;
- old droplets of brown-red blood cling to the lower blades;
- wind through it makes a faint glassy tinkling rather than a rustle.

A creature that stops at the edge and closely examines an individual blade **automatically recognizes the danger**. No check. The hazard punishes heedlessness, not curiosity.

The ecosystem knows first. There are **no game trails through Razer-grass** — every trail bends around it. Except occasionally one doesn't, and that trail becomes red.

## Counterplay

> [!tip] Running this hazard — how the party can mitigate, avoid, or neutralize it.

- **Water is the intelligent countermeasure.** If a section is thoroughly soaked, its movement damage remains and Shatter still deals damage, but **Glass Bloom does not occur** — wet silica dust does not aerosolize. A *create or destroy water* spell becomes extremely valuable; after heavy rain, Razer-grass is safer to destroy. The tradeoff: wetting the white shell makes it more transparent, so **less dust, harder to see**.
- **Careful Passage** spends actions instead of hit points. Time and pressure are the currency once the party knows what it is.
- **Fire is the wrong answer.** The plant tissue burns; the silica does not. Burning leaves thousands of unsupported glass shells snapping under their own weight — **burning Razer-grass automatically triggers Shatter and Glass Bloom in each affected section**. *Fireball* transforms a hazardous meadow into a glittering airborne industrial accident. The players will only try that once.
- **Use it.** Once the party understands the grass, a pursuer that refuses to follow through the white field turns the hazard into a resource: careful passage, a barrier to route around, or a stand deliberately smashed between themselves and what is chasing them.

## Escalation

> [!secret]- What happens if the hazard is ignored or interacted with repeatedly — collapsed by default.

- **Glass-Choked exposure compounds inland pressure.** Disadvantage on environmental Constitution saves turns [[region.aruhe-the-rot|The Rot]]'s hourly corrupted-air save and any other [[region.aruhe|Aruhe]] hazard into stacking attrition for whoever carries it deeper. ^[inferred]
- **Damaged stands regrow armored.** Razer-grass responds to damage by putting more silica into its replacement growth — the Blight exaggerating a completely reasonable plant defense: *silica makes me unpleasant to eat* becomes *anything touching me will eventually learn not to touch me*.
- **Blood on snow that isn't snow.** The white field records its passage: one ruby droplet, then another, then ten, then every stalk beside the path is striped red — and the creature itself may not yet have noticed how badly it has been cut. Sometimes the party finds a field after something else crossed it: no body, just a red corridor vanishing back into ordinary grass. What walked through something every other animal knows to avoid?

## Continuity

[[region.aruhe|Aruhe]]'s fauna understand Razer-grass better than the adventurers — ecologically, not intellectually. [[creature.deer-stalker|Deer-Stalkers]] skirt it. [[creature.terror-bird|Terror-Birds]] do not charge through it. [[creature.wolfrabbit|Wolfrabbits]] leap over [[vehicle.the-narrow|Narrow]] bands rather than landing inside them. [[creature.aruhe-river-otter|River otters]] do not haul prey onto banks where it grows. Observant players can learn from the ecosystem — and later, the party can use the white field as the one barrier something chasing them will not cross.

It grows in discrete colonies inside [[region.aruhe-the-grasslands|The Grasslands]] valleys — low, waist-high islands of strange whiteness rather than a blanket over the valley floor. Stands favor ground repeatedly disturbed by grazing: animal crossings, old wallows, river bends, flood-scoured clearings, places where a [[creature.terror-bird|Terror-Bird]] charge flattened the old vegetation. Every attempt by animals to destroy it selects for thicker armor; eventually nothing grazes there. ^[inferred — habitat preference proposed by the design, not yet observed in play]

Mechanical precedents: **Razorvine** (contact slashing), half-strength **Spike Growth** (difficult terrain plus movement damage), and **Caltrops** (slowing mitigates a sharp-ground hazard), tuned to [[region.aruhe|Aruhe]]'s existing DC 14–15 environmental cluster. ([D&D 5e Wiki — Razorvine](https://dnd-5e.fandom.com/wiki/Razorvine), [D&D Beyond — Spike Growth](https://www.dndbeyond.com/sources/dnd/basic-rules-2014/spells))
