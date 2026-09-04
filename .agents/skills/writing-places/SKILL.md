---
name: writing-places
description: >-
  Places — create or revise a spatial kind (location, settlement,
  region, or route) that needs theatre-of-the-mind orientation,
  landmarks, interactive affordances, discoveries, or meaningful
  routes. Not a dungeon complex (writing-dungeons), business, vehicle,
  situation, encounter, or spoken [!narration] craft.
---

# Writing Places

Create places the table can **picture, understand, touch, exploit, investigate, and remember**.

A place is a playable environment, not scenery. Useful specificity beats ornament. `location` is one spatial kind — a room, building, or site — not the umbrella.

Playable volume is always a spatial page. A `vehicle` or `business` links to the place; it is not the place.

`kind: dungeon` is owned by `writing-dungeons`. If the place is a multi-room dungeon complex, invoke that skill and stop.

## Scale

Apply the branch that matches `kind`. Do not run a room checklist on a region.

| Kind | Mental model | Affordances | Topology |
|---|---|---|---|
| `location` | Silhouette, landmark, one non-visual signature, exits | ≥3 combining features | Only if movement inside the site matters |
| `settlement` | Silhouette, civic landmarks, districts | Civic-scale, not every stall | Districts, gates, named routes |
| `region` | Silhouette, `geo_anchor`s, what the land does | Named sites and processes — no three-object checklist | Routes, approaches, unusual paths |
| `route` | Character of the crossing | What you can use or suffer along the way | The route *is* the topology |

A **landmark** reorients the table. `geo_anchor` is a place other pages should hang off. Do not mark furniture as `geo_anchor`.

## Workflow

### 1. Ground

Retrieve only what constrains the work: the existing page, its parent and anchors, directly relevant inhabitants, factions, history, hazards, and canon. Campaign material only when `scope: campaign`.

Check `canon`. Preserve human-authored and protected material. Read the target kind's schema and `references/section-map.md`.

If the target is `kind: dungeon` or the brief is a multi-room dungeon complex, invoke `writing-dungeons` and stop.

**Complete when:** every consequential established fact that could constrain the place is accounted for — or ownership has handed off to `writing-dungeons`.

### 2. Establish reality

Before prose, know **function**, **present use**, **trace**, and **identity** — the image or contradiction that makes this place unlike a generic example of its type.

Architecture, damage, clutter, traffic, repairs, and residue should have reasons. Temporal occurrences belong on `event`. Tonight's pressure is Work.

**Complete when:** the place could be inferred from its evidence.

### 3. Build the mental model

At the current scale:

1. overall shape, scale, or spatial character;
2. the dominant landmark;
3. one additional sensory or environmental signature;
4. obvious exits, approaches, or meaningful directions.

Use relative spatial language: above, beneath, across, behind, overlooking, through, near. Larger places recurse through districts or major areas. Fill geography fields the schema supports; leave unconstrained fields empty.

**Complete when:** a player could answer where we are, what dominates the space, and where we could go.

### 4. Seed affordances

Important sites need things to **do**. Prefer features that support several verbs and that combine.

For each affordance record: what is obvious; what interaction reveals or changes; the physical logic; the useful consequence.

Durable architecture — cover, height, chokepoints, what collapses if burned — stays on the place. Counts, morale, and staging are `kind: encounter`. Skip tactical inventory when violence is implausible.

Reward unanticipated uses from established properties. Do not script the party's solution.

**Complete when:** different PCs could reasonably choose different things to manipulate, at this scale.

### 5. Make curiosity pay

Plant incomplete signals. Reveal enough to provoke “what is that?”, not enough to answer it.

A deliberate exploration choice should be able to produce information, leverage, a route, a resource, a relationship, avoided danger, a new opportunity, or a deeper question.

Necessary conclusions need multiple independent paths. Sensible unlisted investigations that should logically reveal evidence do. Optional discoveries may stay missable.

An environmental signal stays on the place when it is only texture. Mint `kind: clue` when a `mystery` or another page must cite that information as a node. Do not author mystery pages.

**Complete when:** curiosity can change knowledge, options, resources, risk, or position.

### 6. Give exploration topology

When movement matters, create meaningful spatial choices: multiple approaches, loops, shortcuts, vertical connections, unusual paths, or areas that differ in risk, distance, access, or reward.

Signal enough that the choice has content. A blank left/right fork is not exploration. Stop adding routes when they cease to create distinct decisions.

Name a `route` if you would name it in the world.

Mint a spatial page when another page, a named route, a situation, the geography graph, or a future query must cite it.

**Complete when:** learning the place can improve how the players move through or exploit it — or movement at this scale does not matter.

### 7. Make it alive

Show occupants through **typical activity and spoor**, not tonight's roster.

Ask what happens here without the PCs; what evidence leaks from nearby people, creatures, factions, or processes; what changes when disturbed; what remembers the PCs afterward.

Named imminent change is a pending event or a situation tide. Physical process (rust, flood, squatters as a type) may live on the page.

**Complete when:** the place behaves like something that exists between descriptions.

### 8. Write the page

Instantiate or patch the target kind from `_system/schemas/<kind>/`. Fill existing sections — see `references/section-map.md`. Do not add a second outline.

`locations:` on other pages still means `kind: location`. Wikilink settlements, regions, dungeons, and routes in the body.

If the place is structurally sound but still generic, invoke
`fleshing-out-content` before any spoken picture.

When `[!narration]` is needed, invoke `theatre-of-the-mind` with the
Surface facts and one toy. Stop at a reaction point.

For a `leaflet` fence, invoke `obsidian-leaflet`. Qualitative geography remains canonical.

If a feature is a trap, hazard, or trial, invoke `writing-traps-trials`.

If the place has a look and needs an identity picture, invoke `visual-aids`.

**Complete when:** the DM can scan the page, establish the shared image, follow whichever feature the players engage, and adjudicate an unexpected interaction without searching through prose.

## Who may invoke

Fire this skill when a location, settlement, region, or route is missing, unplayable, or being revised as a place. Expected callers: `writing-narrative-islands`, `writing-session-beats`, `campaign-planning`, `writing-traps-trials`, `writing-dungeons` (standalone room spun out of a Room Index).

Do not fire from `theatre-of-the-mind` or `obsidian-leaflet`. For dungeon complexes, fire `writing-dungeons` instead.

## Quality gate

Test from the players' side, at this scale:

- **Picture** — stable image from a few anchors
- **Orient** — meaningful directions and exits
- **Touch** — things worth acting on
- **Infer** — function, history, occupants, or danger through evidence
- **Explore** — curiosity exposes genuine discoveries
- **Choose** — alternatives produce different consequences
- **Exploit** — established properties support unprescribed use
- **Remember** — a landmark, image, behavior, or consequence distinguishes it later
- **Run** — the next needed fact is findable at a glance

Then apply `_system/schemas/<kind>/quality.yaml`. Remove details that satisfy none of these tests.

## Delegation

- `writing-dungeons` — multi-room dungeon complex / `kind: dungeon`
- `theatre-of-the-mind` — all player-facing prose, including spoken `[!narration]`
- `fleshing-out-content` — existing place is still generic; run before `[!narration]`
- `writing-traps-trials` — challenge mechanisms
- `obsidian-leaflet` — map fence syntax
- `visual-aids` — reference image or named illustration
- `kind: encounter` — tonight's staging
- `kind: clue` / `mystery` — discoveries a mystery must cite
- `kind: event` — named temporal occurrences

Out of scope: `dungeon`, `business`, and `vehicle` pages; Beat Charts; spoken-prose craft; widening `locations:` to other spatial kinds.

## References

| File | Read when |
|---|---|
| `references/section-map.md` | Writing a specific kind — which sections this skill owns |
