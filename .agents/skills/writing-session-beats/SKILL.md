---
name: writing-session-beats
description: >-
  Compose Hook, Development, Cliffhanger, Climax, and Resolution beats
  into a Beat Chart. Use when prepping a session, turning a situation
  into a spine or field, resequencing after play, gating a Climax, or
  auditing agency, gravity, rhythm, and continuity.
---

# Composing Session Beats

Compose **pressure, not plot**. The DM is the runtime.

The Beat Chart is dramatic grammar (Hook → Development ↔ Cliffhanger →
Climax → Resolution). The sandbox is **irrigation**: gravity →
obstacles → player choice → changed state → next appropriate beat.

The output is **prepared dramatic possibility**. The table determines
actuality. This skill owns composition **between** beats.
`writing-session-beats` is the composer — there is no `composing-beats`
skill.

## Contract

A successful composition:

1. begins from compiled campaign state and a dramatic question worth playing
2. anchors every prepared beat to established gravity via a Link of Relevance
3. composes atomic `kind: beat` pages rather than duplicating them
4. preserves rhythm and escalation along every prepared path without scripting decisions
5. exposes only branches justified by materially different world states
6. enters the Climax only when earned; Resolution depends on the actual result

## Delegation

Invoke rather than reproduce:

- `writing-hook-beats` — opening pressure
- `writing-development-beats` — information, relationships, leverage, revelations
- `writing-cliffhanger-beats` — contest, peril, pursuit, confrontation
- `writing-climax-beats` — decisive convergence
- `writing-resolution-beats` — fallout
- `writing-traps-trials` — challenges inside a beat
- `writing-statblocks` — reusable combat identity
- `writing-places` — unplayable or missing location, settlement, region, or route
- `writing-dungeons` — missing or unrunnable multi-room dungeon complexes
- `writing-items` — missing or unrunnable notable objects
- `writing-vehicles` — missing or unrunnable named conveyances
- `fleshing-out-content` — a beat's people, places, or objects exist but have no presence
- `theatre-of-the-mind` — all player-facing prose, including spoken `[!narration]`
- `writing-session-adventures` — assemble the at-table running guide
- `kind: encounter` pages — encounter math

Beats are `kind: beat` pages, instantiated from
`_system/schemas/beat/template.md`. Session-tied beats live in
`wiki/sessions/<NNN>/` beside that night's running guide. The situation
owns the Beat Chart when a situation page exists. Otherwise the chart
lives on that session-plan and dies with it.

Out of scope: the at-table running guide (`writing-session-adventures`);
entity pages (use their schemas; places go through `writing-places`;
dungeons go through `writing-dungeons`; items go through
`writing-items`; vehicles go through `writing-vehicles`); art and
battlemaps; moving Campaign Now; flipping canon past what
reconciliation owns.

## Gravity

Retrieve gravity from PC pages and the campaign-plan Party Goals.
Every prepared beat records a **Link of Relevance** in `## Player
Gravity` and lists the PCs in `pcs:`.

Prepared material is possibility. Played material becomes
authoritative through reconciliation. After a session, re-orchestrate
from the updated vault, never from what the chart predicted.

## References

| File | Read when |
|------|-----------|
| `references/composition.md` | Core model, Spine vs Field, branch discipline |
| `references/climax-gate.md` | Climax readiness |
| `references/audits.md` | Agency, gravity, validation gate |
| `references/runtime-surface.md` | Writing the chart onto the situation or session-plan |
| `references/rhythm-and-pacing.md` | Beats per session, pacing the active path |

## Workflow

Detail: `references/composition.md`.

### 1. Compile the current playable state

Smallest authoritative set: PCs and gravity, situation, actors,
threats, prior consequences, existing beats, dramatic question.

**Complete when** every needed fact is vault-supported or marked as new prep.

### 2. State the dramatic question

One question whose answer would materially change the situation.

**Complete when** it names a real conflict, permits two different
answers, player action can influence which becomes true, and answering
it would justify a Climax.

### 3. Map player gravity

Only established investments. Never manufacture backstory to make prep
convenient.

**Complete when** every beat intended for advance prep can carry a
concrete Link of Relevance.

### 4. Determine the current Beat position

A new session does not automatically imply a new Hook.

**Complete when** exactly one next structural function (or the Climax
gate) is identified.

### 5. Choose Spine or Field

Spine when direction is clear. Field when several materially different
states remain live.

**Complete when** every retained branch is a distinct playable state
and none exists to predict a player method.

### 6. Compose atomic beats

Context packet per beat, delegate to its `writing-*-beats` skill,
instantiate from the beat template, wikilink from the chart.

**Complete when** every required beat exists as a valid atomic page.

### 7. Connect beats by state

Transitions follow achievable world states. Shared invariants
reconverge branches.

**Complete when** every edge is a state, not an assumed decision.

### 8. Audit rhythm

Beat grammar on every prepared path.

**Complete when** every plausible path alternates coherently and no
beat pads a quota.

### 9. Audit escalation

Later beats are more consequential, not merely larger.

**Complete when** no two adjacent beats perform the same dramatic job.

### 10. Gate, write, validate

Climax gate (`references/climax-gate.md`). Write the chart
(`references/runtime-surface.md`). Run `references/audits.md`. Run
`npm run doctor` from `_system/scripts/`.

**Complete when** every applicable gate passes and doctor is clean.

## Governing principle

> **Prepare the terrain. Follow the gravity. Let the players choose the river.**
