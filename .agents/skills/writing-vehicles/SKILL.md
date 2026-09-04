---
name: writing-vehicles
description: >-
  Vehicles — create or revise a named conveyance the party can board,
  contest, or travel in. Use when writing a ship, boat, wagon, carriage,
  airship, spelljammer, war machine, or other transport; especially for
  ownership, crew, operation, customization, upkeep, playable interiors,
  voyages, or vehicle combat. Not a place, not a statblock, not spoken
  [!narration] craft.
---

# Writing Vehicles

Make the vehicle a **working asset**: something the party can recognize,
board, operate, exploit, damage, repair, change, and remember.

A **vehicle** is a named conveyance. One `kind: vehicle` page owns
identity, operation, ownership, crew context, capabilities, upkeep, and
customization. Mint the page when another page, a query, or play must
cite the conveyance. Playable interior is a linked `location` or
`dungeon`. If it can take a turn, combat math lives on a linked
`statblock` subtype `vehicle`.

**Weight** scales every step: incidental · recurring asset · campaign
centerpiece. Add only systems that create decisions.

## Path

| Weight | Run |
|---|---|
| Incidental | 1 → 2 → 3 → 8 → 9 |
| Recurring | every step that the play needs; skip combat unless it takes a turn |
| Centerpiece | every step; load travel, upkeep, and customization when they matter |

## Workflow

### 1. Retrieve

Read `_system/schemas/vehicle/`. Load the existing page if any, relevant
campaign or world canon, and the PCs or campaign-plan when the party
owns or depends on it. Before authoring or materially revising 5e combat
or travel math, follow `_system/references/exemplar-grounding.md`.

Resolve:

- **relationship** — owned, hired, borrowed, pursued, captured, enemy, home
- **weight** — incidental, recurring, centerpiece
- **mode** — land, water, air, astral, planar, subterranean, or stranger
- **play** — transport, exploration, cargo, social space, crew operation,
  customization, upkeep, combat
- whether its **interior** is genuinely playable
- whether it can **take a turn**

Preserve human decisions and established canon.

**Complete when:** you know why this vehicle deserves a page and which
play branches it actually needs.

### 2. Give it physical identity

Build one coherent physical model before mechanics.

Establish the few details players will repeatedly perceive or manipulate:

- silhouette, scale, materials, and construction
- propulsion and what physically produces motion
- control surface — reins, wheel, tiller, helm, pedals, ritual circle
- boarding and access
- passenger and cargo reality
- characteristic motion, sound, vibration, smell, wake, tracks, or exhaust
- visible wear, repairs, markings, trophies, or modifications
- one limitation that follows from how it works

Then expose **affordances**: parts characters can climb, open, hide in,
secure, overload, cut loose, repair, jettison, reinforce, sabotage, or
use creatively.

Incidental vehicles may need only 1–2. Recurring or centerpiece vehicles
should present several distinct affordances. Detail earns its place
through interaction, choice, mechanics, consequences, or memory.

**Complete when:** a DM can picture the object in motion and answer what
characters can physically do with it.

### 3. Make operation legible

For every important function, connect:

**part → operator → action → effect → failure**

Cover only functions that matter in play: movement and steering;
braking, anchoring, landing, docking, or mooring; propulsion; lookout,
navigation, communication; cargo handling; weapons or defenses;
emergency repair; unusual magical or technological systems.

State **what capability degrades** when hands or parts are missing.
Crew jobs create opportunities, not chores. Competent ordinary operation
stays routine; stations, checks, and resource decisions come forward
when circumstances become dangerous.

Named crew who matter as people are linked or minted `npc` pages.
Undifferentiated hands stay crew.

**Complete when:** the DM knows who makes the vehicle work, what they
do, and what changes when somebody or something fails.

### 4. Scale the playable volume

A vehicle is not a spatial kind.

If characters merely sit on or in it, keep physical facts concise here.

If its interior can be meaningfully explored, defended, boarded,
infiltrated, searched, fought through, modified by room, or revisited as
a place, mint a linked spatial page: `writing-places` for a single
`location`, `writing-dungeons` for a multi-room `dungeon`.

The spatial page owns durable topology, landmarks, cover, chokepoints,
access, verticality, rooms, and environmental affordances. This page
owns conveyance identity, operation, ownership, crew, capabilities, and
the relationship to that interior.

Design important spaces around function. Give each space a reason
characters might go there during play.

**Complete when:** any playable interior is usable without turning this
page into an illegal place page.

### 5. Give ownership consequences

For a recurring party vehicle, determine what owning it changes:

- cargo or passenger opportunities
- access to routes or environments otherwise hard to reach
- functional space — storage, workshop, galley, quarters, shrine
- legal status, registration, docking, reputation, debts, enemies
- crew relationships
- salvage, trade, smuggling, exploration, piracy, rescue, transport
- an attachment worth protecting

Prefer benefits and complications that generate adventure. The vehicle
should expand what the party can attempt, not merely cut travel time.

**Complete when:** losing, improving, or changing the vehicle would
materially change campaign play — or ownership is not in scope.

### 6. Add upkeep only when it produces choices

Maintenance is **friction**, not taxation.

Track a need only when players choose: spend now or risk trouble, carry
the spare or extra cargo, hire expertise or improvise, sail damaged or
lose time repairing.

Useful triggers: significant damage; overload or hard use; hostile
terrain or weather; a long demanding voyage; a known fault neglected;
unusual fuel, feed, ammunition, air, magic, or consumables.

For a tracked fault: **symptom → consequence → repair requirement →
escalation**.

When persistent deterioration needs a countdown, link a `clock`. When a
named future repair, arrival, breakdown, or other occurrence crosses the
event threshold, mint an `event`. Vehicles do not acquire timestamps.

**Complete when:** every tracked maintenance burden can make the players
choose between competing priorities — or no upkeep is tracked.

### 7. Leave room for customization

Recurring vehicles should accumulate player fingerprints.

Define a few meaningful **upgrade surfaces**: propulsion or handling;
protection; cargo or passenger capacity; specialized rooms; weapons or
defenses; sensors, navigation, communications, stealth; environmental
capability; support craft or tools; comfort, prestige, disguise, or
intimidation.

A good upgrade changes at least one capability **and** the imagined
object. Prefer new verbs, access, tradeoffs, or reliability over
anonymous numerical bonuses. Costs may include space, weight, crew,
visibility, maintenance, scarcity, money, power, or another capability.

An installed component stays part of the vehicle unless it needs
independent narrative identity. A named object other pages must cite may
be a linked `item`. Let upgrades arise from play.

**Complete when:** players can imagine ways to make *this* vehicle
increasingly theirs — or customization is not in scope.

### 8. Persist

Patch or mint `vehicle.<slug>.md` from `_system/schemas/vehicle/`.
Folder by authority: `world/` for setting truth, `campaign/` for
party-specific truth. `id` matches the stem. New designs:
`canon: provisional`.

Fill existing schema sections. Do not invent a second outline.

If the interior is playable, invoke `writing-places` for a `location`
or `writing-dungeons` for a multi-room `dungeon`, then link it.
If the vehicle can take a turn, invoke `writing-statblocks` and link
`statblock` subtype `vehicle`. Hull AC/HP and combat actions stay off
this page.

If the object exists but lacks handling, wear, or lived-in identity,
invoke `fleshing-out-content` before any spoken picture.

If `[!narration]` is needed, invoke `theatre-of-the-mind` with
first-sight facts only.

If the vehicle has a look and needs an identity picture, invoke
`visual-aids`.

If crafting, acquisition, destruction, loss, refit, or a named voyage
must be queried as an occurrence, mint an `event`. The vehicle page
stays timeless.

When travel is central, the vehicle defines capabilities and limits;
routes, situations, encounters, clocks, events, and session plans own
the journey content. Never reduce an important voyage to one check
whose only outcomes are “arrive” or “arrive slower.”

If a recurring need cannot fit the schema, propose a schema update.

Run the vault doctor from `_system/scripts/`. Apply
`_system/schemas/vehicle/quality.yaml`.

**Complete when:** one authoritative vehicle page exists and canon,
audience, schema, spatial split, and time rules remain intact.

### 9. Gate

Apply `_system/schemas/vehicle/quality.yaml`. Then the **weight test**:

- incidental vehicles remain light
- recurring assets expose repeated interaction
- centerpiece vehicles support ownership, evolution, and sustained play
- no subsystem exists solely because a larger vehicle *could* have one

Revise until every applicable check passes.

**Complete when:** the DM can run the vehicle as a tangible,
understandable, consequential object and the players can form plans
about it rather than merely travel inside it.

## Who may invoke

Fire when a vehicle is missing, unrunnable, or being revised as a
vehicle.

Expected callers: `writing-session-beats`, `writing-narrative-islands`,
`campaign-planning`, `writing-statblocks` (when the combatant is the
conveyance and the vehicle page is missing).

`theatre-of-the-mind` does not fire this skill.
`writing-places` does not write vehicle pages.

## Delegation

- `writing-places` — single-room playable interior as `location`
- `writing-dungeons` — multi-room playable interior as `dungeon`
- `writing-statblocks` — the vehicle takes a turn
- `theatre-of-the-mind` — all player-facing prose, including spoken `[!narration]`
- `fleshing-out-content` — vehicle exists but still feels generic
- `visual-aids` — reference image or named illustration
- `writing-items` — a notable installed component needs its own node
- `kind: event` — named temporal occurrences
- `kind: clock` — tracked deterioration or countdown pressure
- `kind: encounter` — this particular battle
- `kind: npc` — named crew who matter as people

Out of scope: spatial pages; combat math on this page; spoken-prose
craft; inventory of every bolt; predicted voyage plots.
