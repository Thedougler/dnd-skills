---
id: vehicle.hcs-ordinance
kind: vehicle
subtype: ship
scope: setting
campaign: shattered-sea
audience: [agent, dm]
canon: established
status: active
importance: supporting
schema: vehicle@1
created: 2026-08-17
updated: 2026-08-19
aliases:
  - "HCS Ordinance"
  - "Ordinance"
  - "The Ordinance"
sources:
  - _archive/hcs-ordinance.md
summary: Three-deck Crown first-rate; 96 guns; Knighton's private fleet. Commanded by Corbin Knighton. Intercepted the Uncertainty in Session 09.
tags: []
ship_class: ship of the line
crew_capacity: 240
cargo_capacity: 160 tons
speed: 50 miles/day fair wind
npcs:
  - "[[npc.corbin-knighton|Corbin Knighton]]"
locations: []
statblocks: []
factions:
  - "[[faction.dravosi-crown|The Dravosi Crown]]"
relationships:
  - target: "[[faction.dravosi-crown|The Dravosi Crown]]"
    type: related_to
  - target: "[[vehicle.hcs-sovereign|HCS Sovereign]]"
    type: related_to
  - target: "[[item.letters-of-marque|Letters of Marque]]"
    type: related_to
provenance:
  extracted: 0.85
  inferred: 0.05
  ambiguous: 0.1
base_confidence: 0.37
tier: supporting
---

# HCS Ordinance

```statblock
name: hcs ordinance
size: Gargantuan
type: vehicle
ac: 14
hp: 650
```

> [!narration] Overview
> Gun decks rise above a grey hull in three rows. Fourteen ports a side on each deck, shut. A white stripe at the main deck. Crown flags on three tall masts. The bow statue is [[deity.tyr|Tyr]], blind, in robes, gold scales. She is not fast. She does not need to be.

Built at [[region.harwick|Harwick]] in [[faction.dravosi-crown|the Crown]] Islands. 210 feet on the waterline. When launched she was the largest Crown hull in [[region.shattered-sea|The Shattered Sea]]. She does not patrol. She is a court on the water: cases, rulings, and a name that ends pirate gangs for miles.

> [!secret]- Flagship contradiction
> The draft itself says [[vehicle.hcs-sovereign|HCS Sovereign]] supersedes this entry as the definitive Tier 4 Crown flagship. The *Ordinance* may still exist as a secondary vessel or may have been refit or renamed. Do not collapse the two. Confirm before seating her in a scene.^[ambiguous]

## Stats

| Property | Value |
|---|---|
| **Class** | Ship of the line |
| **Crew** | 50 min / 240 full |
| **Cargo** | 160 tons (typically impound) |
| **Speed** | 50 miles/day good wind; 20 poor; poor maneuverability |
| **Guns** | 96: 84 × 24-lb long cannon; 12 × 12-lb chasers |

Decks bow to stern: weather (quarterdeck, Admiralty Court deckhouse); upper gun (14/side, admiral's cabin); main gun (14/side, Registry Vault); lower gun (14/side, waterline); orlop; hold.

## Crew

Commanded by [[npc.corbin-knighton|Corbin Knighton]] — "the new one in charge of the knights," dispatched by [[npc.rupert-knighton|Rupert Knighton]]. Admiral's staff and signals complement exist as roles.

## Facilities (draft Bastion mapping)

- **Admiralty Court** — once per Bastion Turn: one Crown instrument (commission, revocation, warrant, impound, or [[item.letters-of-marque|Letters of Marque]]). Passive: Crown officers have advantage on Intimidation vs parties under Crown law.
- **Registry Vault** — certified copies, forgeries, named registrations. Forgery detection DC 18 Investigation. Passive paper trail of ports and inspections.
- **Gunner's Magazine** — specialist shot order for the next fight. Criticals deal full cannon damage. Never misfired, per draft.

## Relationships

- [[faction.dravosi-crown|The Dravosi Crown]] — commissioning authority.
- [[vehicle.hcs-sovereign|HCS Sovereign]] — live flagship; do not merge.
- [[settlement.tidefall|Port Tidefall]] and HCS Constancy appear in the draft Connections list and are not minted.

## Continuity

- Session 09: intercepted the *[[vehicle.uncertainty|Uncertainty]]* on [[region.midchain|The Midchain]] approach hunting [[npc.shepherd-grigori|Shepherd Grigori]], carrying [[npc.aleksander-malone|Aleksander Malone]]. [[npc.corbin-knighton|Corbin Knighton]] accepted the merchant cover, restrained [[npc.aleksander-malone|Malone]], and stood the warship off for [[settlement.calveno|Calveno]].
