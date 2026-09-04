# dnd-skills

Agent skills for running a D&D / TTRPG campaign with Campaign OS: planning, beat craft, places, dungeons, items, statblocks, player-facing narration, and Obsidian wiki operations.

Skills live at `.agents/skills/<name>/SKILL.md` so Claude Code, Grok, and other agents that read `.agents/skills` pick them up as-is.

## Install

Clone and symlink (or copy) into a project:

```bash
git clone https://github.com/Thedougler/dnd-skills.git
ln -s /path/to/dnd-skills/.agents/skills/<skill-name> your-project/.agents/skills/<skill-name>
```

Or clone this repo next to a campaign vault and point the agent at it.

## Skills

### Campaign architecture

| Skill | What it does |
|---|---|
| `campaign-planning` | Campaign contract, season map, horizon, and re-planning |
| `decomposing-campaign-content` | Classify a request across kinds, layers, and specialist skills |
| `llm-wiki` | Karpathy llm-wiki pattern as implemented by Campaign OS |
| `tag-taxonomy` | Controlled vocabulary for wiki tags |
| `external-references` | Cite, save, refresh, and reuse external research |

### Beats and sessions

| Skill | What it does |
|---|---|
| `writing-session-beats` | Compose Hook → Development → Cliffhanger → Climax → Resolution |
| `writing-hook-beats` | Opening-pressure beat |
| `writing-development-beats` | Non-physical change-in-situation beat |
| `writing-cliffhanger-beats` | Contest-or-peril beat |
| `writing-climax-beats` | Decisive convergence beat |
| `writing-resolution-beats` | Post-Climax fallout beat |
| `writing-cold-opens` | Pre-Hook prelude from a borrowed viewpoint |
| `writing-session-adventures` | Assemble a human DM running guide |

### World and toys

| Skill | What it does |
|---|---|
| `writing-narrative-islands` | Situation topology for sandbox play |
| `writing-places` | Locations, settlements, regions, routes |
| `writing-dungeons` | Multi-room dungeon complexes |
| `writing-items` | Notable objects the party can find, use, trade, or destroy |
| `writing-vehicles` | Named conveyances |
| `writing-statblocks` | Runnable 5e mechanics |
| `writing-traps-trials` | Traps, hazards, trials, puzzles |
| `fleshing-out-content` | Pictureable, lived-in facts before narration |
| `visual-aids` | Identity pictures and player-safe illustrations |

### Table and characters

| Skill | What it does |
|---|---|
| `theatre-of-the-mind` | All player-facing prose |
| `player-character-interview` | Twenty-question session-zero interview |
| `player-character-mechanics` | Canonical PC state and compiled projection |

### Obsidian

| Skill | What it does |
|---|---|
| `obsidian-markdown` | Wikilinks, embeds, mermaid, math, footnotes |
| `obsidian-leaflet` | Leaflet maps, markers, overlays |
| `obsidian-fantasy-statblocks` | Fantasy Statblocks fence and layouts |
| `obsidian-layout-adjustment` | Vault CSS / visual layout |

## Test content

`test-content/` holds sample Campaign OS wiki pages used to exercise the skills.
