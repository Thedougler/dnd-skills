---
name: writing-session-adventures
description: >-
  Running guides — assemble a human DM control panel for a session or
  adventure from existing session-plans, beats, and wiki owners. Use
  when writing a session run guide, adventure module, at-table DM
  reference, or assembling tonight to run. Not beat composition, not
  reconciliation.
---

# Running Guides

Assemble a **control panel** the DM runs from. The table never sees this
file. Every fact the DM needs sits where play needs it.

The guide is a Renderer ([ADR-0005](../../../docs/adr/0005-session-lifecycle.md),
[ADR-0013](../../../docs/adr/0013-content-classification.md)). Work and
Knowledge stay on their owners. The guide is the **walk**.

Missing prep is a diagnostic. Assemble does not invent the night.

## Contract

A successful guide:

1. opens on a one-screen brief the DM can run from if the rest never loads
2. walks prepared nodes as a menu of world states, not a plotted path
3. transcludes or wikilinks owners instead of copying them
4. speaks every theatre-of-the-mind change in `[!narration]` titled Narration
5. puts Immediate facts in scan range and Hidden facts in `[!secret]-`
6. names Move On as states, not player decisions

## Narration

Theatre of the mind is spoken. Write a `[!narration]` for every scene
change, crossing, first sight, and change in an already-seen thing.
Invoke `theatre-of-the-mind` for the craft. Durable narration lives on
the parent and is embedded here. Session-local continues and
transitions may live on this Renderer.

**Complete when:** a listener who heard only the narration could name
where they are, who is present, and what they could touch.

## Scene block

One H2 per node. Obsidian's outline *is* the control panel.

```markdown
## N. Title — [[beat.slug|Beat]]

**When:** world-state that makes this node live
**Stakes:** what is gained or lost
**Gravity:** [[pc.slug|Name]] — established investment

> [!narration] Narration
> What the table perceives. Read or adapt.

### Immediate
- landmark, occupants, toys, exits — actable now

### Hidden
> [!secret]- What is actually happening
> Truth behind the surface.

### Run
> [!mechanic] Title of the check
> | Check | When | DC | Fail-forward |
> |-------|------|----|--------------|
> | …     | …    | …  | play moves   |

> [!danger] If violence starts
> Who fights, flees, or calls. Tactical shape.

> [!tip] Running [[npc.slug|Name]]
> **Wants:** …
> **Voice / tell:** …
> **Opening:** mid-task · first line (a question)

**Move on:** **state** → [[beat.next|Next]]
```

Drop empty subsections. Embed a parent `[!narration]` or encounter
section when it is already the authority. Write nested narration when
an NPC or item arrives inside the node.

Full OFM recipe: `references/layout.md`.

## Scale

| Scale | Source | File |
|---|---|---|
| **Night** | `kind: session-plan` plus tonight's beats | `wiki/sessions/<NNN>/session-guide.<NNN>.md` |
| **Module** | a `kind: situation` and its Beat Chart | beside that situation page: `adventure.<situation-slug>.md` |

Module form: `references/module.md`.

## Workflow

### 1. Ground

Read the session-plan (night) or situation (module). Read every linked
beat, situation, NPC, place, encounter, item, clock, and front. Read the
Beat Chart on the owning situation.

**Complete when:** every named in-play thing has an owner page, or is
listed as missing.

### 2. Diagnose

Read `references/assemble.md`. Invoke the owner skill for missing or
unrunnable Work. Invoke `fleshing-out-content` when a seen thing
has no presence. Do not fill the guide with invented canon.

**Complete when:** every in-play entity is runnable or an explicit
diagnostic.

### 3. Map the walk

Order nodes by likely play. Label them a menu. Key each node. Edges are
world states. Recap and Strong Start first. Unused possibilities and
exits last.

**Complete when:** every plan beat and situation is a node or an unused
possibility, and every edge is a state.

### 4. Write the control panel

Read `references/layout.md`. Brief first, then scene blocks. Invoke
`theatre-of-the-mind` for every player-facing prose block. Invoke
`obsidian-markdown` for wikilinks, embeds, and callouts.

**Complete when:** a DM who has not opened another page can recap,
open, run each prepared node, and find the next node from a state.

### 5. Pictures and items

Invoke `visual-aids` assemble for in-play `player_images` and named
session-plan Illustrations. Store illustrations with this renderer.

**Complete when:** every in-play `player_images` entry is on the guide,
and each named illustration is generated or explicitly skipped.

### 6. Gate

Read `references/quality-gate.md`. Mark `generated: true`. Run doctor
from `_system/scripts/` if any owner pages were patched.

**Complete when:** every gate passes.

## Who may invoke

Fire when the outcome is a table-ready running guide or adventure
module. Expected callers: the user asking to run tonight;
`writing-session-beats` after a chart exists; `decomposing-campaign-content`
when the outcome is a playable night; `visual-aids` assemble.

Do not fire from `theatre-of-the-mind`. If the session-plan or Beat
Chart is missing, invoke `writing-session-beats` (and grill if the
night itself is unauthored) and stop.

## Delegation

- `writing-session-beats` — missing or uncomposed beats / chart
- `theatre-of-the-mind` — every player-facing prose block, `[!narration]`, and spoken line
- `obsidian-markdown` — wikilink, embed, callout punctuation
- `fleshing-out-content` — owner exists but has no presence
- `visual-aids` — assemble player-safe pictures and named illustrations
- `writing-places` / `writing-dungeons` / `writing-items` /
  `writing-vehicles` / `writing-statblocks` / `writing-traps-trials` —
  missing or unrunnable owners
- `kind: encounter` — combat math
- `player-character-mechanics` — what the PCs can do now

Out of scope: composing the Beat Chart; minting canon; moving Campaign
Now; player-safe handouts as a separate product; reconciliation.

## References

| File | Read when |
|------|-----------|
| `references/assemble.md` | Inventory, transclude, missing-prep diagnostics |
| `references/layout.md` | Brief, OFM, scan order, mermaid |
| `references/quality-gate.md` | Final runnability tests |
| `references/module.md` | Multi-session adventure module |
