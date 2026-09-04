---
name: writing-dungeons
description: >-
  Dungeons — create or revise a multi-room dungeon complex as an
  explorable system. Use when a kind: dungeon needs topology, zones,
  Room Index, entrances, loops, landmarks, living ecology, or
  exploration logic; or when a dungeon is linear, inert, hard to
  navigate, or hard to run. Not a single room (writing-places), not
  tonight's roster, not spoken [!narration] craft.
---

# Writing Dungeons

Build a dungeon as an **explorable system**: topology, inhabitants,
information, affordances, dangers, and rewards let players form plans
and change what happens. The DM runs the place; the players choose the
route.

A **dungeon** is a spatial kind. One `kind: dungeon` page owns durable
spatial topology, zones, Room Index, landmarks, physical logic, typical
inhabitants and use, and persistent affordances. Rooms stay in the Room
Index unless a room needs independent geography or reuse outside the
dungeon.

`writing-places` owns other spatial kinds. This skill owns `kind:
dungeon`. Place craft still applies at room and dungeon-wide scale —
mental model, affordances, curiosity — inside this workflow.

## Path

| Job | Run |
|---|---|
| New complex | every step |
| Topology-only repair | 1 → 3 → 8 → 9 |
| Keying repair | 1 → 5 → 6 → 8 → 9 |
| Living-ecology repair | 1 → 4 → 8 → 9 |

## Workflow

### 1. Retrieve

Read `_system/schemas/dungeon/` and `references/section-map.md`. Load
the existing page if any, parent geography, relevant PCs and gravity,
situation or session-plan, factions, and constraining canon. Campaign
material only when `scope: campaign`.

Before original challenge or combat math, follow
`_system/references/exemplar-grounding.md`.

Resolve:

- **purpose** — what it was built for and what it is now
- **reason** — why these PCs would risk entry; link gravity when possible
- **budget** — one scene, one session, multi-session, or revisitable site
- **experience** — tone, danger, weirdness, exploration density
- **constraints** — locked canon, exclusions, map or source limits

If the brief is unclear, ask the DM once. Before heavy keying, state the
**spine**: premise, objective, zones, topology, active forces, signature
interaction, payoff. Resolve consequential disagreement; then fill
reversible detail.

**Complete when:** purpose, PC reason, budget, experience, constraints,
and spine are unambiguous.

### 2. Make the place coherent

Design **function → history → present state**.

For each zone: why it exists; how builders or inhabitants moved; what
changed, broke, flooded, collapsed, grew, or was repurposed; who uses it
now and what traces that leaves; one **landmark** for orientation.

Architecture communicates history. Doors, stairs, drains, defenses,
storage, sightlines, wear, refuse, shrines, repairs, and damage imply
how the place works without exposition.

**Complete when:** every major zone has a practical reason to exist, a
present use or abandonment logic, and a recognizable identity.

### 3. Build meaningful topology

Default to **loops**, not dead-end branches.

- Multiple approaches when scale permits — obvious, risky, hidden,
  social, vertical, damaged — that differ in risk, information,
  resources, faction contact, or position
- Branches reconnect so choice matters
- Multi-level sites need more than one useful level connection;
  occasional skip-level or surface links reward mastery
- Secrets as shortcuts, escape, ambush, or bypass — not the only path
- Elevation, sightlines, sound, water, shafts, and destructible
  boundaries let rooms affect one another
- Linear segments only when sequence itself has purpose; return to
  choice afterward
- Mandatory chokepoints are fragile. Required obstacles get multiple
  viable approaches; fiction-supported improvisation stays valid

Telegraph route tradeoffs. Players need enough signal to prefer a path
for a reason.

**Complete when:** the main objective has at least two materially
different approaches where scale permits, a useful loop or
cross-connection exists, and the party can retreat or reroute without
the design collapsing.

### 4. Populate a living dungeon

Separate **belongs here** from **is here tonight**.

On the dungeon page: durable inhabitants, territories, movement logic,
environmental processes, and typical use. Tonight's roster, alert state,
patrol placement, encounter counts, and immediate pressure live in Work
(`situation`, `encounter`, session-plan).

When the concept supports it, give multiple active forces with
incompatible wants. For each intelligent group: want now; territory or
resources; fear or unsolved problem; offer or knowledge; response when
the party shifts the balance.

Include someone or something that can be communicated with when the
fiction allows. Mix residents, intruders, predators, hazards, remnants,
and opportunists.

For revisitable sites, decide how abandoned territory, casualties,
stolen resources, opened routes, and faction victories alter later
delves. Mint `event` or `clock` only when existing thresholds are met.

**Complete when:** the dungeon can react to intrusion without assuming a
fixed room-by-room sequence.

### 5. Key rooms as decision surfaces

A keyed room is a **decision surface**, not a lore dump. Order facts as
play reveals them:

1. **Immediate** — obvious on entry; strongest identity and actionable features
2. **Features** — objects, terrain, creatures as types, exits, landmarks, affordances
3. **Investigation** — what closer attention, touch, tools, or talk expose
4. **Consequences** — what changes when used, damaged, bypassed, triggered, or ignored
5. **Connections** — clues, routes, sounds, sightlines, or relationships beyond the room

Significant rooms need at least three combining affordances (obvious /
reveals / logic / consequence). Connective rooms may be exits plus one
cue.

Favor manipulable features. Define physical truth; do not prescribe the
solution. Quiet rooms still orient, foreshadow, offer resources, show
consequence, change pace, or give a safe-ish choice.

**Complete when:** the DM can scan each key, know what players perceive
first, and adjudicate plausible interaction from stated physical logic.

### 6. Make information, danger, and reward legible

- **Clues** — environment reveals history, hazards, routes, rivalries,
  shortcuts. Required conclusions need redundant paths.
- **Danger** — telegraph severe threats before commitment. Lethality is
  interesting when risk is chosen and escape is possible.
- **Challenges** — traps, hazards, and trials are interesting when found,
  understood, exploited, bypassed, or disarmed. Mint independent pages
  via `writing-traps-trials` when the mechanism is a node.
- **Rewards** — specific treasure, knowledge, allies, territory,
  shortcuts, leverage, tools, or transformations. Major rewards behind
  risk, curiosity, mastery, or hard choices — not only the final room.
- **Secrets** — shortcuts, hidden chambers, advantageous positions,
  alternate solutions, or re-readings of earlier areas.

**Complete when:** players can detect major risks, discover why the place
matters, and gain concrete advantages from exploration without a missed
roll stalling the delve.

### 7. Vary pressure

Contrast combat with exploration, negotiation, hazards, strange
interaction, discovery, respite, navigation, and treasure. Avoid every
key being a fight or every danger a hidden save.

- Enemies use terrain the PCs can also turn
- Sound, light, doors, distance, and verticality change fights
- Some threats can be avoided, bargained with, redirected, or fled
- Strong PC capabilities that genuinely apply bypass problems; reward
  mastery instead of silently countering it
- Time or resource pressure needs a concrete source and a fiction for
  rest cost

Reusable combat identity is `writing-statblocks`. This fight's counts,
terrain use, objectives, and morale are `kind: encounter`.

**Complete when:** the dungeon pressures multiple kinds of decision and
no single encounter mode dominates by accident.

### 8. Persist

Patch or mint `dungeon.<slug>.md` from `_system/schemas/dungeon/`.
Folder by authority: `world/` or `campaign/`. `id` matches the stem.
New designs: `canon: provisional`. Fill existing sections — see
`references/section-map.md`. Do not invent a second outline.

Rooms stay in the Room Index unless a room needs its own geography page
via `writing-places`.

Invoke rather than reproduce:

- `theatre-of-the-mind` — Overview and room entry `[!narration]`
- `fleshing-out-content` — structure sound but still generic; before
  spoken pictures
- `writing-traps-trials` — independent trap, hazard, or trial nodes
- `writing-statblocks` — combat identity
- `writing-items` — notable treasure nodes
- `writing-places` — a room that must exist as its own spatial page
- `obsidian-leaflet` — map fence; qualitative geography stays canonical
- `visual-aids` — identity picture for the look
- `kind: encounter` — tonight's staging
- `kind: clue` — only when a mystery must cite the information as a node
- `kind: event` / `kind: clock` — named temporal change or countdown

Do not put tonight's roster, party-tuned difficulty, estimated session
counts, wandering encounter queues, loot parcels, or victory scripts on
this Knowledge page.

Run doctor from `_system/scripts/`. Apply
`_system/schemas/dungeon/quality.yaml`.

**Complete when:** one authoritative dungeon page exists; each fact has
one owner; a session plan can cite the dungeon without inventing spatial
logic.

### 9. Gate

Run the player-side passes:

- **Route** — multiple approaches, a retreat, a useful loop or shortcut;
  no accidental single points of failure
- **Agency** — major pre-dice decisions change exposure, information,
  allies, resources, position, or consequence
- **Mastery** — learning map, factions, hazards, or mechanisms yields
  later leverage
- **Interaction** — each major zone has manipulable features with
  adjudicated consequences
- **Signals** — severe danger, hidden opportunity, and necessary
  information have discoverable tells
- **Ecology** — inhabitants travel, eat, guard, communicate, retreat,
  reinforce, and react without play-breaking contradiction
- **Capability** — flight, climbing, scouting, divination, forced entry,
  teleport, shapechange, and destructive magic change the dungeon
  honestly when relevant
- **Key** — map and Room Index agree; exits, secrets, vertical links,
  and hazards are glance-findable
- **Run** — unexpected entry order, alliance with an intended enemy,
  skipped centerpiece, and revisit after retreat still produce coherent
  play

Then apply `_system/schemas/dungeon/quality.yaml`.

**Complete when:** every pass succeeds or the DM has deliberately
accepted the remaining constraint as a feature of this dungeon.

## Who may invoke

Fire when a `kind: dungeon` is missing, unplayable, linear, inert, or
being revised as a dungeon complex.

Expected callers: `writing-narrative-islands`, `writing-session-beats`,
`campaign-planning`, `writing-places` (when the place is a dungeon),
`writing-vehicles` (multi-room playable interior that is a dungeon),
`writing-traps-trials` (host dungeon missing).

`theatre-of-the-mind` and `obsidian-leaflet` do not fire this skill.

## Delegation

- `theatre-of-the-mind` — all player-facing prose, including spoken `[!narration]`
- `fleshing-out-content` — presence on a structurally sound dungeon
- `writing-traps-trials` — challenge mechanisms
- `writing-statblocks` — combat identity
- `writing-items` — notable treasure
- `writing-places` — standalone room/site pages spun out of the index
- `obsidian-leaflet` — map fence syntax
- `visual-aids` — reference image or named illustration
- `kind: encounter` — tonight's staging
- `kind: clue` / `mystery` — discoveries a mystery must cite
- `kind: event` / `kind: clock` — named temporal change

Out of scope: single-room places; other spatial kinds; Beat Charts;
spoken-prose craft; party-relative difficulty as dungeon truth;
tonight's roster on the Knowledge page.
