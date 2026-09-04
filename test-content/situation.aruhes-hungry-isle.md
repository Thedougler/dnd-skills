---
id: situation.aruhes-hungry-isle
kind: situation
subtype: expedition
scope: campaign
campaign: shattered-sea
audience: [agent, dm]
canon: provisional
status: active
importance: major
schema: situation@1
created: 2026-08-18
updated: 2026-08-22
aliases:
  - Aruhe's Hungry Isle
  - The Aruhe Shipwrecking
  - Aruhe Narrative Island
sources:
  - _archive/aruhe-hungry-isle.md
  - _archive/aruhe-hungry-isle-narration-condition.md
  - _archive/aruhe-hungry-isle-run-guide.md
  - _archive/aruhe-grubnade.md
  - _archive/aruhe-fruits.md
  - _archive/aruhe-blight-hinewa.md
  - _raw/aruhe-dungeon.md
summary: An Outer Aruhe rescue before a later optional return to the Death Bloom.
tags: []
dramatic_question: Can the crew recover the living castaways across Outer Aruhe and find a route home before the wreck and its shelter fail?
fronts: []
clocks: []
locations:
  - "[[location.aruhe-the-clear-lake|The Clear Lake]]"
  - "[[region.aruhe-the-grove|The Grove]]"
  - "[[region.aruhe-the-rot|The Rot]]"
  - "[[region.aruhe-the-quiet|The Quiet]]"
  - "[[region.aruhe-the-grasslands|The Grasslands]]"
  - "[[region.aruhe-the-old-gardens|The Old Gardens]]"
  - "[[region.aruhe-the-beach|Aruhe Beach]]"
beats:
  - "[[beat.past-the-teeth|Past the Teeth]]"
  - "[[beat.aruhe-the-landing|The Landing]]"
  - "[[beat.aruhe-two-in-shade|Two in the Shade]]"
  - "[[beat.aruhe-plenty|Plenty]]"
  - "[[beat.aruhe-the-count|The Count]]"
  - "[[beat.aruhe-mute-country|Mute Country]]"
  - "[[beat.aruhe-fires-fail|The Fires Fail]]"
npcs:
  - "[[npc.sandro|Sandro]]"
  - "[[npc.nino|Nino]]"
  - "[[npc.nona-black-jaw|Nona Black-Jaw]]"
factions:
  - "[[faction.grung-clans|Grung Clans]]"
hooks: []
relationships:
  - target: "[[situation.the-aruhe-rescue|The Aruhe Rescue]]"
    type: related_to
  - target: "[[region.aruhe|Aruhe]]"
    type: related_to
  - target: "[[creature.blight|Druid Lich]]"
    type: related_to
  - target: "[[event.aruhe-wreck|The Aruhe Wreck]]"
    type: related_to
  - target: "[[location.aruhe-the-clear-lake|The Clear Lake]]"
    type: related_to
  - target: "[[dungeon.aruhe-wilderness-megadungeon|Aruhe Wilderness Mega-Dungeon]]"
    type: related_to
provenance:
  extracted: 0.88
  inferred: 0.1
  ambiguous: 0.02
base_confidence: 0.37
lifecycle: draft
lifecycle_changed: 2026-08-18
tier: supporting
---

# Aruhe's Hungry Isle

## Situation

**[[npc.sandro|Sandro]], [[npc.nino|Nino]], and scattered castaways want a route home; [[faction.grung-clans|Grung Clans]] want the reef watched and the sand untouched; the [[creature.blight|Druid Lich]] wants [[region.aruhe|Aruhe]] inviolate — before the wreck fails and the island's pressure reaches the landing.**

- **Dramatic question:** Can the crew recover the living castaways across [[region.aruhe|Outer Aruhe]] and find a route home before the *[[vehicle.vethka|Vethka]]* shelter fails?
- **If ignored:** The signal fires stop, the *[[vehicle.vethka|Vethka]]* shelter gives way, and unrecovered castaways join the island's count. The reef remains a possible landing, but a live rescue and the safest route home close with the smoke.

If anyone takes fruit from [[region.aruhe|Aruhe]], nearby animals attack them. The fruit itself is not cursed.

> [!secret]- What is actually happening
> [[creature.grung|Grung]] are attacked on sight. The Death Bloom is graves, tree, and ritual ground together — not a detachable object. Destroying it ends the Blight. Leaving it preserves the sanctuary and its killings. This is the island expedition. [[situation.the-aruhe-rescue|The Aruhe Rescue]] owns [[region.midchain|The Midchain]] captive trail and the smoke clock that can *lead here*.

The first expedition can resolve in [[region.aruhe|Outer Aruhe]]: recover the castaways the crew reaches and find a route home from the reef. The Death Bloom is not required. [[npc.sandro|Sandro]] and [[npc.nino|Nino]] remain in the wreck's shade unless play changes their position; the scattered castaways are prepared possibilities from the wider wreckage, not replacements for them. A later return may confront [[creature.blight|Hinewai]] at the Death Bloom and decide whether destroying her is worth destroying the sanctuary she made. Until the party reaches [[region.aruhe-the-grove|The Grove]], [[creature.blight|Hinewai]] stays offstage: silent birds and independent fauna carry her presence without giving animals her voice.

The rescue topology covers [[region.aruhe-the-beach|The Beach]], the lower edge of [[region.aruhe-the-old-gardens|The Old Gardens]], and the [[region.aruhe-the-quiet|Quiet]] edge. The linked [[dungeon.aruhe-wilderness-megadungeon|Aruhe Wilderness Mega-Dungeon]] owns [[region.aruhe|Aruhe]]'s broader route system and local spatial detail. This situation owns the rescue pressure, the lessons castaways carry, the route home, and the choice to return.

> [!narration]
> *Past the reef gap the water calms under three limestone walls, their faces cut with stair steps gone green under vine. The wind brings salt, bruised citrus, and no birds.*
>
> *On the shingle a [[vehicle.vethka|Vethka]] proa lies broken on one side, outrigger snapped, ribs hung with wet cloth. A cooking fire has gone to grey ash beside the hull. Water jars stand in the surviving shade. Fresh footprints run from the wreck to the tideline, then stop at the first terrace.*
>
> *[[npc.sandro|Sandro]] and [[npc.nino|Nino]] still use that shade. Inland the jungle is a solid green wall. Nothing shows past the first trunks. The air coats the roof of the mouth, fruit rotting under fruit still ripening.*

## Forces

| Actor | Wants | Why | Next action | Tell |
|-------|-------|-----|-------------|------|
| `[[npc.sandro]]` | Get [[npc.nino\|Nino]] off alive | Knows the shoreline and Tomo; not the interior | Keep signal fires; stay off the first terrace | Bent hook; will not cross the moss |
| `[[npc.nino]]` | Leave without crossing the garden line | He will not step onto the first terrace | Stay in hull shade | Silence; stops at the first terrace |
| [[region.aruhe\|Aruhe]] castaway at the Gardens (possible) | Survive long enough to be found | Saw animals turn after a castaway took fruit | Hold to a refuge | Fruit left untouched |
| [[region.aruhe\|Aruhe]] castaway at the terraces (possible) | Reach help while a predator holds the route | A predator still owns the climb | Stay near a defensible break and signal when safe | A clear line, disturbed earth, and signs of a fight |
| [[region.aruhe\|Aruhe]] castaway at the [[region.aruhe-the-quiet\|Quiet]] edge (possible) | Stay together and find the way back | Learned to wait out territories and read the mute trails | Keep to a refuge or game-trail seam | No birdsong, careful fire, and marks that avoid a patrol |
| `[[faction.grung-clans]]` | Watch the reef; never land | Inherited enemy of this sand | Patrol boats; refuse landfall | Hulls on the gap; no footprints inland |
| `[[creature.blight]]` | Keep [[region.aruhe\|Aruhe]] inviolate in a drowned companion's memory | Protection turned punishment | Stay bound at [[region.aruhe-the-grove\|The Grove]] | Quiet island; no birdsong |
| `[[npc.nona-black-jaw]]` | An answer to [[pc.perrin-black-jaw\|Perrin]]'s survey | A Tangle anchor, or proof the island cannot be entered | Wait on the commission | The survey exists; she is not on [[region.aruhe-the-beach\|The Beach]] |

Every load-bearing actor can advance the situation without the party.

## Gravity

Declining is legitimate. The island stays hungry.

- [[pc.perrin-black-jaw|Perrin Black-Jaw]] — [[npc.nona-black-jaw|Nona]]'s survey: can this island be an anchor, or is it permanently unusable?
- [[pc.jean-claude-tabarnack|Jean-Claude Tabarnack]] — [[creature.grung|Grung]] history. The island attacks [[creature.grung|Grung]] on sight.
- [[pc.delmar-fisk|Delmar Atticus Fisk]] — [[settlement.calveno|Calveno]] crew on the wreck. Rescue is crew obligation; salvage is a second pull.
- [[pc.catarina-davirelli|Catarina Da'Virelli]] — Corruption that reshapes biology at scale.
- [[pc.crissdalynn-khinriss|Crissdalynn Khinriss]] — A place-bound artifact. Pattern before anyone names it.

## Bridges

- **Reef gap and wreck.** Weather, wreckage, or a heading east of [[region.karath|Karath]]. Reveals two survivors. Cost: a landing on [[region.aruhe-the-beach|The Beach]].
- **Castaway signs.** An improvised refuge, a marked terrace, or a silent trail can reveal a living castaway beyond the hull. It offers a different lesson and a route-home clue. Cost: time away from the wreck and its fires.
- **[[pc.perrin-black-jaw|Perrin]]'s survey.** [[npc.nona-black-jaw|Nona]]'s commission. Reveals the terrace question. Cost: going inland.
- **[[region.karath|Karath]] channel patrols.** Contact that will not land. Reveals the inherited enemy. Cost: [[creature.grung|Grung]] attention.
- **Wake of [[situation.the-aruhe-rescue|The Aruhe Rescue]].** Smoke, port talk, or a chart note. Losing the rescue clock does not erase the island.

## Affordances

- [[npc.sandro|Sandro]] and [[npc.nino|Nino]]: hear testimony, protect, rescue from the wreck, or leave them in place (Tomo, fruit, wreck, shoreline vs jungle). They do not begin inland.
- **Scattered castaways:** recoverable people, not required explainers. Testimony, observation, or another approach can reveal them.
- **Outer [[region.aruhe|Aruhe]] rescue sites:** [[region.aruhe-the-beach|The Beach]] offers extraction and the wreck's testimony; [[region.aruhe-the-old-gardens|The Old Gardens]] offer temptation and a possible recovery; the [[region.aruhe-the-quiet|Quiet]] edge offers a final recovery and a choice to go deeper. The broader route system belongs to [[dungeon.aruhe-wilderness-megadungeon|Aruhe Wilderness Mega-Dungeon]].
- **Route home:** signal fires, a reef approach, a marked trail, and whatever vessel or escort the crew brings can combine into an extraction. A first expedition need not reach [[region.aruhe-the-grove|The Grove]].
- Miracle fruit ([[item.redheart-berry|Redheart Berry]], [[item.lion-citrus|Lion Citrus]], [[item.stonepear|Stonepear]], [[item.giants-guava|Giant's Guava]], [[item.ghost-plum|Ghost Plum]], [[item.whisper-fig|Whisper Fig]], [[item.breathmelon|Breathmelon]], [[item.quickeye-berry|Quickeye Berry]], [[item.skybladder|Skybladder]], [[item.rotheart|Rotheart]]) works as its item pages state.
- [[creature.grubnade|Grubnades]]: living traps in the flowers. Predators have burn scars and walk around them. Plucking one to throw works.
- Outer [[region.aruhe|Aruhe]] can stand as a complete rescue: Beach, Gardens, and Quiet edge. The crew may leave after a route home, or choose a later return. The [[dungeon.aruhe-wilderness-megadungeon|Aruhe Wilderness Mega-Dungeon]] holds the wider expedition topology. Combat clears temporary space; no band stays tame.
- **Outer [[region.aruhe|Aruhe]] tables:** use [[random-table.aruhe-beach-navigation|Aruhe Beach Navigation Table]], [[random-table.aruhe-old-gardens-navigation|Old Gardens Navigation Table]], and [[random-table.aruhe-quiet-navigation|Quiet Navigation Table]] when the rescue zooms into 30-minute route checks.
- Death Bloom: destroy, leave, or bargain with what [[region.aruhe-the-grove|The Grove]] still is.
- Knowledge, mapped routes, and ruin fragments open later approaches. They do not script one.

## Tide

| State | Cause | What changes | Visible evidence | What opens or closes |
|---|---|---|---|---|
| Shelter live | [[npc.sandro\|Sandro]] and [[npc.nino\|Nino]] keep fires while the hull and provisions hold | The wreck remains a visible extraction point; inland castaways can still be sought | Smoke, open-sky fish, and prints that stop at the first terrace | A live rescue and a route-home attempt remain open |
| Shelter failing | Time, hunger, and interior pressure reach the landing | Fires shorten, the hull becomes unsafe, and a castaway may abandon a refuge or become harder to reach | Grey ash, fewer fish, fresh tracks near the wreck, and a darkening reef gap | Delay closes the safest rescue window; inland clues remain possible |
| First expedition resolved | Castaways are recovered, their fate is accepted, and a route home is found | The rescue can end without the Death Bloom changing state | Survivors, route marks, and accounts of what lies inland | The optional return to the Death Bloom opens; it is never required |

## Wake

If the first expedition resolves in [[region.aruhe|Outer Aruhe]], recovered castaways leave through [[region.aruhe-the-beach|The Beach]] with a route home. [[npc.sandro|Sandro]] and [[npc.nino|Nino]] are not relocated by preparation; if rescued, they depart from the wreck. A partial rescue leaves names, trails, or warnings for a later attempt. The [[region.aruhe-the-grove|Death Bloom]] remains untouched unless the crew chooses a later return. If the Bloom eventually falls, corruption recedes over weeks and the island can become usable, including [[npc.nona-black-jaw|Nona]]'s survey. If it stands, the memorial endures. Feeds [[situation.the-aruhe-rescue|The Aruhe Rescue]] and [[faction.grung-clans|Grung Clans]] patrol doctrine.

## Beat Chart

**Run:** [[session-guide.010|Session 10 running guide]]

Prepared possibility. Session 10 live slice. Death Bloom is not tonight.

- **Dramatic question:** Can the crew recover the living castaways before [[region.aruhe|Aruhe]] takes them?
- **Player Gravity:**
  - [[pc.delmar-fisk|Delmar]] — [[settlement.calveno|Calveno]] crew on this wreck
  - [[pc.perrin-black-jaw|Perrin]] — [[npc.nona-black-jaw|Nona]]'s survey
  - [[pc.jean-claude-tabarnack|Jean-Claude]] — island attacks [[creature.grung|Grung]] on sight
  - [[pc.catarina-davirelli|Catarina]] — biology reshaped at scale
  - [[pc.crissdalynn-khinriss|Crissdalynn]] — pattern in a place-bound system
- **Current State:** *[[vehicle.uncertainty|Uncertainty]]* on [[settlement.sparhold|Sparhold]] heading, likely to pass. 487 left [[settlement.calveno|Calveno]]; 290 at [[region.karath|Karath]]; 149 hit this reef. [[npc.sandro|Sandro]] and [[npc.nino|Nino]] still in the hull.
- **Active Beat:** none until they steer for the smoke ([[beat.past-the-teeth|Past the Teeth]]).
- **Beat Field:**
  - [[beat.past-the-teeth|Past the Teeth]] — entry: prize stays, heading south
  - [[beat.aruhe-the-landing|The Landing]] — entry: they steer for the smoke
  - [[beat.aruhe-two-in-shade|Two in the Shade]] — entry: keel on the shingle
  - [[beat.aruhe-plenty|Plenty]] — entry: they climb the first risers
  - [[beat.aruhe-the-count|The Count]] — entry: a take, a defense, or a living inland sign
  - [[beat.aruhe-mute-country|Mute Country]] — entry: they reach mute canopy; optional one middle bite if they push
  - [[beat.aruhe-fires-fail|The Fires Fail]] — gated Climax
- **Live Branches:**
  - **they extract from the Beach without climbing** → skip inland; Climax may still earn on people + gap
  - **they take fruit** → nearby animals attack; same beats, louder
  - **they push inland from mute canopy** → one middle bite on [[beat.aruhe-mute-country|Mute Country]], not a seventh slot
  - **they never land** → this chart unused
- **Climax Readiness:**
  - Question: ready
  - Investment: ready
  - Opposition: missing until they land
  - Understanding: missing until wreck testimony
  - Leverage: missing until they have a route home
  - Stakes: ready once fires are visible
  - Possibility: ready
  - Convergence: missing until people, gap, and time occupy the same landing
- **Unused Possibilities:** Death Bloom / [[region.aruhe-the-grove|The Grove]] — later voluntary return.

## Notes

Run-guide checks after the cold open, if they turn east or follow wreckage.

| Check | DC | Failure reads as | Pass |
|---|---|---|---|
| Survival | 14 | a rich island | cultivated terraces and fruit that still hangs |
| Perception | 13 | jungle | reef and beach, then terraces, then closed sight lines |
| Investigation | 15 | a wreck | [[pc.perrin-black-jaw\|Perrin]]'s Tangle-anchor question |
| Insight | 12 | two castaways | [[npc.sandro\|Sandro]] will risk the shore; [[npc.nino\|Nino]] will not cross the garden line |
| Persuasion | 13 | they stay put | testimony: Tomo, the fruit, the wreck |
| Nature | 14 | the garden | the cultivation is deliberate |

Exit: the crew can leave from [[region.aruhe-the-beach|The Beach]] with the survivors it recovered and a route home. The Death Bloom remains a later, optional return; no Open Strait run-guide is minted here.
