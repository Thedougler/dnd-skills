---
id: hazard.aruhe-dead-air
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
  - Dead Air
sources:
  - _archive/aruhe-caves.md
tags: [horror, survival, underground]
locations:
  - "[[region.aruhe-the-cave|The Cave]]"
encounters: []
dc_detection: 14
dc_save: 14
damage: "poisoned while in the chamber and 10 minutes after reaching clean air; suffocating on a repeated failure"
---

# Dead Air

Some low chambers of [[region.aruhe-the-cave|The Cave]] collect unbreathable gas. Dormant does **not** require the volcano still to be erupting; cave atmosphere can become dangerous through poor ventilation and biological processes. Carbon dioxide is particularly dangerous in depressions — colorless, odorless, and able to accumulate in low areas. ^[inferred — grounding from the source's cited US Geological Survey reference]

## Description

> [!narration] Player-facing description — read or adapt at the table.
> The chamber looks like every other chamber. The air does not look different. What differs: the torch flame burns low, your head aches, and breathing has become strangely deliberate. Dead cave insects collect below a particular elevation on the walls. The air has a line in it, and you are below it.

## Trigger

Entering a low chamber where unbreathable gas has collected. Prolonged exposure: after **1 minute** in a dead-air pocket, the hazard takes hold.

## Effect

> [!danger] What happens when the hazard triggers.

After 1 minute in a dead-air pocket, a creature makes a **DC 14 Constitution saving throw**. On failure: **poisoned** while remaining in the chamber and for **10 minutes** after reaching clean air. A creature that fails again while already poisoned **begins suffocating** until removed from the pocket.

The point is not invisible save-or-die gas. There are clues.

## Detection

**Tells:**

- flame burns poorly
- headache
- breathing becomes strangely deliberate
- dead cave insects collect below a particular elevation

A **DC 14 Intelligence (Nature) or Wisdom (Survival)** check recognizes the signs before prolonged exposure.

## Counterplay

> [!tip] Running this hazard — how the party can mitigate, avoid, or neutralize it.

The tells precede the save. A party that reads the flame, the headache, the deliberate breathing, or the dead-insect line can avoid prolonged exposure or leave the pocket before the minute is up. Nothing looks different when breathable air becomes bad — the point is that the signs are readable, not invisible.

## Escalation

> [!secret]- What happens if the hazard is ignored or interacted with repeatedly — collapsed by default.

Failing again while already poisoned begins suffocation until the creature is removed from the pocket. Source is silent on cumulative effects beyond that.
