# Layout

The DM uses this file three ways: a prep read, a game-day skim, and
live reference. Optimize for reference. Obsidian's outline pane is the
map.

Syntax: `obsidian-markdown`. Callout types:
`_system/references/creative-writing.md`. Spoken craft:
`theatre-of-the-mind`.

## Frontmatter

Renderer, not a kind.

```yaml
id: session-guide.010          # or adventure.<situation-slug>
generated: true
audience: [dm]
session_number: 10             # night only
assembled_from:
  - "[[session-plan.010]]"
created: YYYY-MM-DD
updated: YYYY-MM-DD
aliases:
  - "Session 10 running guide"
```

No `kind`. No `canon`. `audience: [dm]` only — player-safe pictures
are embeds, not a player page.

## Brief (one screen)

H1 is the night's name. Then, before any node:

| Block | Content |
|---|---|
| **Last Time** | `[!narration]` recap (`theatre-of-the-mind` recap branch) |
| **Tonight** | dramatic question · primary shape · one-line pressure |
| **Gravity** | table: PC · live investment |
| **Clocks / fronts** | wikilink · filled segments · next tick |
| **Roster** | NPC · Wants · Will do (from the session-plan table; do not rewrite biographies) |
| **Menu** | numbered node titles as wikilinks to their H2s |
| **Gaps** | only if diagnose left any |

The Strong Start is node 1, not a briefing. Recap hands into that
narration.

## Scan order inside a node

1. H2 title and **When**
2. `[!narration]` — speak this
3. Immediate bullets
4. Run callouts as they fire
5. Hidden only when the table probes
6. **Move on** when the state changes

Bold the scan words in **When**, **Stakes**, and Immediate. History
stays on the owner.

## OFM

- Wikilinks: `[[kind.slug|Display Name]]`. Escape `\|` in tables.
- Embeds: section or image, not the whole note.
- Callouts: `[!narration]`, `[!secret]-`, `[!danger]`, `[!tip]`,
  `[!mechanic]`. `[!hook]` only for unused possibilities.
- Collapse Hidden. Leave narration open.
- Tables for checks, roster, clocks.
- `#` headings stay outside callouts — a `##` inside a callout will
  not render as a heading.

## Mermaid

A mermaid graph is legal when five or more live branches would make
the Menu hard to scan. Nodes are beat wikilinks. Edges are states.
Skip it on a spine.

## Theatre of the mind

Immediate bullets use relative space: above, across, behind, through,
near. Name the toy. Name the exits. Counts, morale, and staging stay
on the `kind: encounter` embed.

After narration that has a discoverable or a social handle, one
`[!mechanic]` — title names the check, body is the table, fail-forward
on every row. Skills and DCs live in the mechanic.

## Length

One node ≈ one screen after the narration. Cut restatement. Cut room
history. A second `[!narration]` inside the node is for a new
arrival or a speaker, not a longer orientation.
