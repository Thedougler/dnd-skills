---
name: obsidian-fantasy-statblocks
description: >-
  Fantasy Statblocks fence, layout, or `monster:` recall on a
  `kind: statblock` page. Use when authoring or editing a `statblock`
  code block, choosing a layout, recalling a creature, or appending
  or removing inherited traits. Not the lore page (`kind: creature`)
  and not encounter math (`kind: encounter`).
---

# Fantasy Statblocks

The Fantasy Statblocks plugin renders a `statblock` fence into a
playable 5e block and keeps a name-indexed **bestiary**. Other notes
and Initiative Tracker recall from it with `monster: <name>`.

The fence lives on an existing `kind: statblock` page. Placement
is the schema (`_system/schemas/statblock/`). This skill writes
the fence, not the page home.

## Quick syntax

From `_system/schemas/statblock/template.md`:

```statblock
layout: Basic 5e Layout
name: "Roper"
size: Large
type: aberration
alignment: "Neutral Evil"
ac: 20
hp: 93
hit_dice: "11d10 + 33"
speed: "10 ft., Climb 20 ft."
stats: [18, 8, 17, 7, 16, 6]
senses: "darkvision 60 ft.; Passive Perception 16"
cr: 5
```

This campaign uses `Basic 5e Layout` only.

## What you need

| Need | Read |
|------|------|
| Bestiary registration, `monster:`, `field+:` / `field-:` | `references/bestiary.md` |
| Config keys, layouts, Settings | `references/config.md` |

Required 5e fields and WotC attack wording live on the statblock
quality gate (`_system/schemas/statblock/quality.yaml`) and the
template. This skill owns plugin mechanics.

## Workflow

### 1. Open the existing statblock page

Edit `rules/statblock.<slug>.md`. Keep `name:` in the fence aligned
with any frontmatter `name:` the plugin uses to register. A missing
page is `writing-statblocks`, not this skill.

**Complete when** the fence is on that `kind: statblock` page and
the names match.

### 2. Fill plugin keys

`layout: Basic 5e Layout`. Creature data in the template's field
set. Recall and override per `references/bestiary.md`.

**Complete when** the block renders in Obsidian and `monster: <name>`
resolves to this creature if registration is wanted.

## Out of scope

Creature lore. Encounter building. Combat identity and numbers
(`writing-statblocks`). 5e field grammar beyond what the schema
already requires.
