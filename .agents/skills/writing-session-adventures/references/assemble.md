# Assemble

Compile presentation from owners. Patch the owner before restating it.

## Inventory

From the session-plan (night) or situation (module), list every:

- beat in `beats:`
- situation in `situations:` and in the Situations body
- NPC, place, encounter, item, vehicle, clock, front named in play
- PC in `pcs:`
- Illustration named on the session-plan

Read each owner. Note: runnable, needs presence, missing, or
unrunnable.

**Complete when:** the list matches the plan and every row has a
status.

## Transclude

Prefer, in order:

1. `[[kind.slug|Display Name]]` for identity
2. `![[kind.slug#Section]]` when the DM needs the owner's text inline
   (Beat Chart, encounter math, a parent `[!narration]`, a statblock)
3. a session-local sentence on this Renderer when the fact is only true
   tonight

Copying a durable fact onto the guide makes a second canon. If the
guide must paraphrase to scan, keep the wikilink beside the paraphrase.

Full-page embeds dump too much. Section embeds only.

## Missing prep

| Gap | Move |
|---|---|
| No session-plan / no Beat Chart | `writing-session-beats` (grill if the night is unauthored) |
| Beat missing or unrunnable | the matching `writing-*-beats` skill |
| Place / dungeon / item / vehicle / statblock / trial missing | its owner skill |
| Owner exists, no signature / Surface / toy | `fleshing-out-content` |
| Narration missing | `theatre-of-the-mind` on the parent, then embed |
| Encounter math missing | `kind: encounter` page |

Write the diagnostic on the guide under **Gaps** only when the DM must
see it tonight. Leave a stub node (`**When:**` + wikilink + "unrunnable
— see Gaps") rather than inventing the missing beat.

## Narration inventory

For each node, list every place, person, creature, and notable object
the table will need to imagine. Each needs one Establish on first
sight. A change in the world is a Continue. A crossing is a Transition.

Source narration from the owner's stocked facts. Session-local smoke,
boarding, or weather may be written here.

## Secrets

A secret stays unbound from one room. The node records who *can* say it
and what physical trace exists. The DM still picks the channel in play.

A conclusion the table must reach needs three independent clues on
different owners (`writing-session-beats/references/audits.md`).
The guide only points at those clues; it does not mint a fourth.

## Night-only pressure

A session-plan Situations section that has no `kind: situation` page
stays a node on this guide. Do not mint a situation to make the walk
look official.
