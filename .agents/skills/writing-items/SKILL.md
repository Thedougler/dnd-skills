---
name: writing-items
description: >-
  Items — create or revise a notable object the party can find, use,
  trade, or destroy. Use when awarding loot, tailoring treasure, pricing
  or crafting gear, writing a curse, sentience, artifact, or evolving
  reward, or checking attunement and campaign fit. Not inventory
  stackables, not a statblock, not spoken [!narration] craft.
---

# Writing Items

Create objects that feel native to the world, express a **Signature**
through mechanics, and give players a new choice.

An **item** is a notable object. One `kind: item` page owns lore and
5e item rules. Mint the page when another page, a query, or play must
cite the object. Stackable gear stays PC structured data.

**Signature** is the smallest mechanic or behavior that produces
identity.

## Path

| Object | Run |
|---|---|
| Mundane notable | 1 → 2 → 4 → 6 → 8 → 9 |
| Magical | every step; load only the special branch that applies |

Acquisition is a retrieval fact — reward, purchase, sale, craft, quest
object, curse, sentient, artifact, or evolving. It is not a frontmatter
field.

## Workflow

### 1. Retrieve

Read `_system/schemas/item/`. Before authoring or materially revising 5e item math, follow `_system/references/exemplar-grounding.md`. Retrieve the target PC if any,
campaign-plan, relevant situation or session, world canon, existing
Signature gear, and at least three same-rarity comparators when the
item is magical. Include the closest spell or class feature when the
effect resembles one.

**Complete when:** wielder or play role, tier, acquisition mode,
constraining canon, and comparators (if magical) are known.

### 2. Write the Signature

One sentence: the physical object, its distinctive verb, and why it
belongs here. One Signature. Further properties only reinforce it.

For a bespoke reward, connect to established gravity. Prefer a new
verb, situational leverage, transformation, or tradeoff.

**Complete when:** the mechanics can be predicted from the fiction and
the fiction recognized from the mechanics.

### 3. Set the envelope

Provisional rarity from tier, then compare the actual effect.

Check frequency × magnitude, action economy, attack / damage / AC /
save / DC / healing, control, defense, mobility, information, challenge
bypass, concentration, stacking, out-of-combat spam, attunement cost,
and the strongest PC synergy.

Attunement is a scarce-slot cost. Broadly optimal effects sit weaker
than narrow ones. Untested homebrew sits slightly low.

Read `references/baseline.md` when a rarity ceiling or value is
needed. Read `references/abuse.md` for any activated, charged, or
scaling property.

**Complete when:** the item sits beside same-rarity comparators and its
strongest synergy and obvious abuse cases survive review.

### 4. Make it runnable

State each property's trigger, action type, prerequisite, target /
range, roll or DC, duration, uses or charges, recharge, and the
edge-case a stranger-DM will hit. A spell-on-item distinguishes
casting the spell from producing its effect.

Bookkeeping earns its time. Charges, tables, and escalating states
stay only when players will feel them.

Mundane: state what the object is, what it affords, and any condition
that matters in play.

**Complete when:** a DM who did not design it can run normal use and
likely edge cases without inventing a rule.

### 5. Special branch

If the item is consumable, cursed, sentient, evolving, artifact, or a
set piece, read that heading in `references/branches.md`.

The complication deepens the Signature.

**Complete when:** every special property changes play in a fictionally
coherent, administrable way.

### 6. Reveal and embed

This skill owns the cut. `fleshing-out-content` stocks first-sight
facts. `theatre-of-the-mind` writes the player-facing prose.

If handling, wear, or lived-in identity is thin, invoke
`fleshing-out-content` before the Appearance callout.

1. **First sight** — `[!narration]` Appearance. Material identity only.
2. **Handling** — what responds to touch or use.
3. **Known mechanics** — Properties the character is entitled to know.
4. **Lore** — fragments in History, earned through play.
5. **DM truth** — `[!secret]-` Secrets.

Invoke `theatre-of-the-mind` for the Appearance callout. Give it
first-sight facts only.

Two or three material details, a creator or origin, an original
purpose, and at least one connection to an existing person, faction,
place, event, practice, or hook when canon supports it.

**Complete when:** the player can picture it, the DM knows why it
exists, and first-sight prose contains only first-sight facts.

### 7. Price and place

When commerce or crafting matters, read `references/baseline.md` plus
`references/market.md` or `references/crafting.md`. Report separately:

1. **rules baseline**
2. **campaign transaction**
3. **availability**

For rewards, read `references/reward.md`.

**Complete when:** the DM knows how the item enters play and what any
quoted value represents.

### 8. Persist

Patch or mint `item.<slug>.md` from `_system/schemas/item/`. Folder by
authority: `world/` for setting truth, `campaign/` for party-specific
truth. `id` matches the stem.

New designs: `canon: provisional`. PC relevance lives in relationships
and body prose.

If the object can take a turn, invoke `writing-statblocks` and link
that block. Item rules that never take a turn stay in `## Mechanics`.

If the object exists but lacks handling, wear, or lived-in identity,
invoke `fleshing-out-content`.

If the item has a look and needs an identity picture, invoke
`visual-aids`.

If crafting, acquisition, destruction, loss, or awakening must be
queried as an occurrence, mint an `event`. The item page stays
timeless.

If a recurring need cannot fit the schema, propose a schema update.

Run the vault doctor from `_system/scripts/`. Apply
`_system/schemas/item/quality.yaml`.

**Complete when:** one authoritative item page exists and canon,
audience, schema, and time rules remain intact.

### 9. Gate

`_system/schemas/item/quality.yaml`. Revise until every applicable
check passes.

## Who may invoke

Fire when an item is missing, unrunnable, or being revised as an item.

Expected callers: `writing-session-beats`, `writing-narrative-islands`,
`campaign-planning`, `player-character-mechanics` (reconcile, when loot
becomes a notable object).

`theatre-of-the-mind` does not fire this skill.
`writing-statblocks` fires it only when the combatant is the object
and the item page is missing.

## Delegation

- `theatre-of-the-mind` — all player-facing prose, including spoken `[!narration]`
- `fleshing-out-content` — object exists but still feels generic
- `writing-statblocks` — the object takes a turn
- `visual-aids` — reference image or named illustration
- `kind: event` — named temporal occurrences
- `kind: npc` — the spirit is independently a person

Out of scope: inventory stackables; spoken-prose craft; combat math on
this page.

## References

| File | Read when |
|---|---|
| `references/baseline.md` | Rarity value, craft time, attunement slots |
| `references/market.md` | Purchase, sale, or bargaining |
| `references/crafting.md` | Someone is making the item |
| `references/reward.md` | Bespoke loot or treasure spotlight |
| `references/branches.md` | Consumable, curse, sentient, evolving, artifact, or set |
| `references/abuse.md` | Activated, charged, or scaling properties |
