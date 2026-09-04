---
name: writing-statblocks
description: >-
  Statblocks — create or revise the runnable 5e mechanics for any
  NPC, creature, animal, summon, ally, boss, vehicle, or narrative
  force that can take a turn. Use when an entity needs a statblock,
  encounter prep requires new monster mechanics, or an existing
  statblock is dull, awkward to run, poorly balanced, or fails to
  express its fiction. Not the Fantasy Statblocks fence
  (`obsidian-fantasy-statblocks`) and not encounter math
  (`kind: encounter`).
---

# Writing Statblocks

Design **verb-first**: the mechanics should make the creature behave like its fiction.

A statblock is Knowledge: reusable 5e mechanical identity. An `encounter` owns quantity, placement, circumstances, and encounter difficulty. Party context may validate a design. It does not make a reusable creature party-relative.

This skill authors the `kind: statblock` page. `obsidian-fantasy-statblocks` encodes the fence. A PC is never a statblock.

## Operating words

* **Chassis** — the proven numerical skeleton you start from.
* **Usage** — how the block is meant to be run: `adversary` · `solo` · `ally` · `narrative-force`.
* **Combat role** — how it occupies a fight. Closed list, one or two values. Not `solo`.
* **Signature** — the smallest mechanic or behavior that produces identity.
* **Loop** — opener, pressure, pivot, exit.

## Workflow

### 1. Establish the chassis

Read the source entity and linked canon, `_system/schemas/statblock/`, applicable `rule` and `ruling` pages, and the closest useful existing statblocks. Before authoring or materially revising 5e numbers, follow `_system/references/exemplar-grounding.md`.

Prefer **reskin → modify → invent**.

Determine:

* intended fictional power / CR
* subtype: `monster` · `npc-combat` · `vehicle` · `hazard-stat` · `lair`
* usage: `adversary` · `solo` · `ally` · `narrative-force`
* combat role: one or two of `ambusher` · `artillery` · `brute` · `controller` · `skirmisher` · `soldier` · `support` · `leader`
* intelligence, discipline, survival instinct, and reason to fight

One entity may already have other blocks. A new combat identity is a new page.

If this block will serve a specific encounter, read that encounter and relevant PCs for edge-case validation only.

**Complete when:** one comparable chassis, one power target, one subtype, one usage, and one or two combat roles are explicit.

### 2. Define the combat identity

Write one sentence answering:

> What should fighting, aiding, escaping, bargaining with, or surviving this creature feel like?

Choose **2–4 verbs** that express that answer.

Define the loop: **Opening**, **Pressure**, **Pivot**, **Exit**.

Every signature mechanic must implement one of those verbs. Ability scores, movement, senses, defenses, and proficiencies support the same behavior.

**Complete when:** intended tactics can be predicted from the fiction and the mechanics reinforce every defining verb.

### 3. Calibrate the numbers

Consult `references/craft.md` § Numbers.

Treat CR as a **chassis benchmark**, not encounter difficulty.

**Complete when:** expected offense and effective defense sit plausibly beside comparable creatures of the target power without relying on the signature being ignored.

### 4. Build the signature

Give the creature the smallest set of mechanics that produces its identity. Consult `references/craft.md` § Signature.

Favor **decision mechanics** over extra damage. Make consequential mechanics legible. Give severe control, major denial, and encounter-changing defenses discoverable counterplay or an escape condition.

For spellcasters, turn bread-and-butter combat magic into self-contained Actions, Bonus Actions, or Reactions when practical. Keep referenced spells when the spell itself is identity or useful outside the combat loop.

Every custom mechanic uses normal 5e timing and terminology unless its complete rule is printed in the statblock.

**Complete when:** removing the creature's name would still leave recognizable gameplay identity, and its strongest mechanic creates a player decision rather than merely a larger number.

### 5. Fit the use

Consult `references/craft.md` § Use.

Adversary: default turn obvious; complexity only where it changes tactics.

Solo: contest the party's action economy; off-turn options move the fight.

Ally: one specialty, tiny choices, opportunities for PCs.

Narrative force: bounded affordances; runnable 5e timing or it is not a statblock.

Minions and special subsystems: use campaign `ruling` pages. Do not silently import another game's rule.

**Complete when:** complexity and action economy fit the chosen usage.

### 6. Make it runnable

Every ability answers, at the point of use: when, who/where, how, what happens, how long, how it ends, how often.

The creature's routine must be visible without external research.

**Complete when:** a DM seeing the page for the first time can choose its next action in seconds.

### 7. Stress-test three rounds

Mentally run: (1) its ideal opening, (2) a normal contested round, (3) a round where the party disrupts its plan or reduces it severely.

Then reverse perspective: what can players **notice, decide, and do differently** because this creature is present?

Revise until the creature remains interesting when its strongest plan fails.

**Complete when:** all three rounds are runnable, numerically plausible, tactically distinct from a generic attacker, and leave meaningful player counterplay.

### 8. Write and validate

Instantiate or patch `rules/statblock.<slug>.md` from `_system/schemas/statblock/`. Respect existing `canon` and the creative authority ladder.

Set `usage` and `combat_role`. Link `creatures:` and/or `npcs:`. Point the owning entity's Mechanics or Tactics at this page. Never write inline combat math on the entity.

Invoke `obsidian-fantasy-statblocks` for the fence.

Run `npm run doctor` from `_system/scripts/`. Repair every statblock error this change introduced.

Run `references/quality-gate.md`.

**Complete when:** the page is a valid `kind: statblock`, the fence is encoded, doctor is clean, and the six tests pass.

## Delegation

Invoke rather than reproduce:

* `obsidian-fantasy-statblocks` — fence syntax, layout, `monster:` recall
* `theatre-of-the-mind` — any player-facing prose, including `[!narration]` the table hears
* `fleshing-out-content` — the source entity has no pictureable fiction; run it on that lore page
* `writing-items` — the combatant is the object and the item page is missing
* `writing-vehicles` — the combatant is the conveyance and the vehicle page is missing
* `kind: encounter` pages — quantity, placement, circumstances, difficulty
* `kind: ruling` pages — new subsystems (one-hit minions, etc.)

Out of scope: creature lore; encounter math; PC mechanical records.

## References

| File | Read when |
|------|-----------|
| `references/craft.md` | Numbers, signature tests, usage fit |
| `references/quality-gate.md` | Six tests and page contract |
