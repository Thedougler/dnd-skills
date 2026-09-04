---
id: hazard.stillbloom
kind: hazard
subtype: environmental
scope: setting
campaign: shattered-sea
audience: [agent, dm]
canon: provisional
status: active
importance: supporting
schema: hazard@1
created: 2026-08-20
updated: 2026-08-20
aliases:
  - Stillbloom
  - Claymore Flower
sources:
  - _archive/aruhe-stillbloom.md
tags: [horror, nature, survival]
locations:
  - "[[region.aruhe-the-quiet|The Quiet]]"
  - "[[region.aruhe-the-rot|The Rot]]"
  - "[[region.aruhe|Aruhe]]"
encounters: []
dc_detection: 14
dc_save: 14
damage: 7 (2d6) piercing per volley + embedded spine (venom save DC 11 + Exposure)
---

# Stillbloom

## Description

> [!narration] Player-facing description — read or adapt at the table.
> The dull green stalk stands four feet tall, unremarkable, waxy, almost boring — until someone runs. **CRACK.** They go down. Everyone's first instinct is to run to them. And now somebody has to say: **"Don't move."** The wounded person lies fifteen feet away, awake, perhaps unable to move one leg, begging for help — and reaching them quickly may trigger the next plant. The Stillbloom does not understand surrender, panic, friendship, innocence, or rescue. It detects rapid movement and responds accordingly. Running away is aggression. Running toward your injured friend is aggression. Being shoved is aggression.

The Stillbloom is the plant version of [[region.aruhe|Aruhe]]'s rule: a familiar biological function pushed past its proper job until it becomes predatory. It should evoke **a minefield**, with a secondary undertone of an **automated sentry system** — and the important part is not merely that it explodes, but the behavior it forces from people afterward. It is not secretly malicious; nature is doing a recognizable natural thing according to a rule pushed beyond sanity.

A mature Stillbloom is roughly four feet tall, built around a tough segmented central stalk. Most of the year it is profoundly unimpressive: dull green, [[vehicle.the-narrow|Narrow]] leaves, waxy stem, little smell. Around the upper third sit several concentric rings of pale, hollow **launch bracts**, each ending in a dark needle approximately three to five inches long. The needles are not thorns — they are disposable defensive organs. Behind each exposed needle sit several immature replacements folded against the stalk; when the outer needle discharges, the next hardens and rotates into position while the plant slowly reinflates the associated pressure chamber. The visible translucent swellings beneath them are botanical pressure vessels: water and gas under enormous tension, restrained by toughened fibres.

Plants genuinely use stored elastic and hydraulic energy for extraordinarily rapid movement — bunchberry flowers explosively catapult pollen, and white mulberry stamens have been measured releasing stored elastic energy in less than 25 microseconds, propelling pollen at more than half the speed of sound. ([PubMed — a record-breaking pollen catapult](https://pubmed.ncbi.nlm.nih.gov/15889081/)) Pushing that from "absurdly fast botanical catapult" to "supersonic poisoned dart launcher" is exactly the sort of biological exaggeration the island already uses.

The root system is equally important. Stillblooms form wide, shallow mats packed with mechanosensitive tissue. Real plants perceive mechanical stimulation and propagate electrical/calcium signals through their tissues; touch-sensitive species respond remarkably quickly. ([PMC — rapid movements in plants](https://pmc.ncbi.nlm.nih.gov/articles/PMC7817606/)) [[region.aruhe|Aruhe]] has pushed that from **touch detection** into **vibration classification**:

- A falling leaf means nothing.
- Rain means nothing.
- A mouse means nothing.
- A [[creature.human|Human]] carefully placing one foot after another means nothing.
- A thirty-pound animal suddenly bolting means **fire**.

**Lifecycle.** Stillblooms are **monocarpic**: one flowering in their entire lives. For approximately twenty years they accumulate nutrients underground — strong real analogues exist in bamboo, which can remain vegetative for decades before synchronous flowering, and agaves, which spend decades storing resources for a single enormous reproductive event. ([PMC — the bamboo flowering cycle](https://pmc.ncbi.nlm.nih.gov/articles/PMC7180196/)) Then, over several weeks, the central stalk produces one enormous pale flower — cream-white with a faint green center, almost obscenely beautiful. After pollination, the plant dies. Twenty years of investment for perhaps ten days of reproduction explains why natural selection has gone completely insane around protecting it.

**Dead things are useful.** The Stillbloom does not directly eat prey — scavengers do that for it. Blood, dung, discarded tissue, decay, and eventually skeletal remains enrich the soil immediately over its root mat. The plant has effectively evolved a little ecosystem that converts frightened animals into fertilizer. The venom has a strong real-world basis in curare: plant-derived, producing skeletal-muscle paralysis through neuromuscular blockade. ([PMC — structural mechanism of muscle nicotinic receptor block by curare](https://pmc.ncbi.nlm.nih.gov/articles/PMC9531584/))

**Naming.** Stillbloom is the canonized name, replacing the former **Claymore Flower** — an ordinary plant-name that fits [[region.aruhe|Aruhe]]'s terse naming style and only becomes horrible once the players understand what "still" means. Discarded alternatives: Stillthorn, Startlethorn, Hushbloom, Watchthorn, Deadstill. ^[noncanon — naming options rejected in the design document]

## Trigger

A **charged mature stalk** fires when a **Small or larger grounded creature** within **20 feet**:

- moves more than 10 feet during one turn;
- takes the Dash action;
- jumps or falls;
- is forcibly moved 10 or more feet; or
- performs another violent physical movement at the DM's discretion.

**Safe movement.** A creature moving **10 feet or less per turn** does not trigger it. Flying creatures that never touch the root mat do not trigger it.

## Effect

> [!danger] What happens when the hazard triggers.

**Detonation.** Every creature within **15 feet** of the plant makes a **DC 14 Dexterity saving throw**. On a success, no damage — the creature gets below, behind, or between the worst of the volley. On a failure: **7 (2d6) piercing damage**, one spine embeds itself, and the creature must make the venom save below.

**Reload.** The plant cannot fire again for **1 minute**. Its collapsed air sacs visibly swell during this time — the reload is the hazard's solvable window.

**Cover.** Half and three-quarters cover apply normally to the Dexterity save. Total cover prevents the volley.

**Poison immunity.** Prevents the venom effects, but not the piercing damage.

**Venom — Exposure.** Every time a creature is struck, its **Exposure** increases by 1. Its Constitution save DC is **11 + current Exposure** — so the first embedded spine is DC 12, then 13, 14, 15, and so on. A **successful save** keeps the venom localized around the wound: the struck limb becomes temporarily numb. A **failed save** spreads the venom and advances the victim one step on the Paralytic Spread track:

| Spread | Effect |
| --- | --- |
| **0 — Local** | Only the struck limb is affected. |
| **1 — Systemic** | The creature is **Poisoned**. |
| **2 — Motor Failure** | **Poisoned and Restrained** as voluntary muscle control begins failing. |
| **3 — Paralysis** | **Paralyzed**. |

Deliberately not the full Paralyzed condition on the first failed save — in 5e that condition is brutal: the victim is incapacitated, has Speed 0, automatically fails Strength and Dexterity saves, attacks against them have advantage, and adjacent hits become automatic critical hits. ([SRD 5.2 — conditions](https://media.dndbeyond.com/compendium-images/srd/5.2/SRD_CC_v5.2.pdf)) The escalating DC is the point: the players can **feel the venom winning**.

**Local paralysis.** No hit-location subsystem — use the fiction of where the spine struck. A numbed **arm** cannot wield something, perform somatic components with that hand, or contribute to a two-handed weapon. A numbed **leg** reduces Speed by 10 feet and prevents the Dash action. If both legs are numb, Speed becomes 5 feet. Local numbness lasts 10 minutes after the final exposure — less severe than formal Paralysis while still producing the moment where the fighter pulls the barb out of their shoulder and discovers their sword arm simply doesn't answer anymore.

**Recovery.** At the end of each of its turns, a creature at Spread 2 or 3 repeats the Constitution save; success reduces Spread by one step. After **1 minute** without another Stillbloom hit, Spread drops by one additional step. After **10 minutes**, Exposure returns to 0 and local paralysis ends. An effect that neutralizes poison clears the venom normally. This keeps a paralyzed PC rescuable instead of turning one unlucky environmental encounter into a death sentence.

## Detection

**DC 14 Wisdom (Perception)** notices the launch-spines, punctured carcasses, and strange paths taken by scavengers.

**DC 14 Intelligence (Nature) or Wisdom (Survival)** identifies the root vibration system and realizes slow movement is safe. Watching local scavengers for 1 minute reveals this automatically.

**The unsettling ecological tell.** Around a Stillbloom patch, small scavengers behave strangely — not frightened, *careful*. A clever little carrion-eater walks between the stems with exaggerated slowness: place a forefoot, stop, look around, take another step, stop. It reaches a carcass covered in black punctures and starts eating. Something larger approaches: the scavenger freezes. The larger animal bolts. **CRACK.** Every bird in the party should flinch. Thirty seconds later, the scavenger resumes eating. That teaches the players almost everything without a Nature check.

## Counterplay

> [!tip] Running this hazard — how the party can mitigate, avoid, or neutralize it.

- **Move slowly.** Ten feet per turn or less is the whole rule once it is understood.
- **Spend the reload.** The exact **one-minute reload** makes the plant solvable: throw a rock, send an expendable object across the roots, use *mage hand* to disturb something, deliberately provoke the volley — **CRACK** — and the party has ten rounds to run. That transforms it from "make a saving throw because the DM said so" into a genuine environmental system.
- **Fly over.** Anything that never touches the root mat is safe.
- **Manage the venom.** Spread out within the patch (the volley only reaches 15 feet), use poison immunity and *neutralize poison* intelligently, and obey rescue discipline: reaching the wounded person *quickly* is exactly what the flowers are waiting for.
- **Use it.** A learned Stillbloom patch is a barrier pursuers cannot run across — a shove, *thunderwave*, or a Frightened creature's forced flight all become weapons aimed at the trigger radius.

## Escalation

> [!secret]- What happens if the hazard is ignored or interacted with repeatedly — collapsed by default.

- **The best encounter is not "walk across the flowers".** Once learned, the horror inverts: the party retreats through [[region.aruhe-the-quiet|The Quiet]] knowing a patch is ahead and how to cross it — ten feet, stop, ten feet, stop — while something behind them moves. A [[creature.deer-stalker|Deer-Stalker]] appears in the vegetation. Nobody can run. The [[creature.deer-stalker|Deer-Stalker]] does not know what the flowers are. Or perhaps, worse, *it does*. ^[ambiguous — the design deliberately leaves open whether the larger fauna has learned]
- **The hazard rewrites ordinary encounters.** A shove becomes terrifying. *Thunderwave* becomes terrifying. Being Frightened and having to flee becomes terrifying. A companion falling unconscious twenty feet away becomes terrifying. A [[creature.terror-bird|Terror-Bird]] charging into the patch might produce the loudest five seconds of the entire expedition. ^[inferred — encounter-design intent from the draft]
- **Weaponization.** The players can eventually turn that knowledge against whatever chases them — the field is a weapon once nobody else knows the rule.

## Continuity

Stillblooms are principally a **Quiet → Rot transitional species** — game trails and sunbreaks, not throughout [[region.aruhe-the-grasslands|The Grasslands]]. [[region.aruhe-the-rot|The Rot]] already establishes that [[region.aruhe|Aruhe]]'s roots can detect creatures and transmit information, so exaggerated root mechanosensation belongs naturally there. Keeping them out of the main Grasslands preserves the conceptual space for [[hazard.razer-grass|Razer-Grass]]: Razer-Grass says *"the beautiful field itself cuts you"*; Stillbloom says *"the field is perfectly safe. Just don't move."* Two very different fears.

The hazard is run with **trap rules**, not as a creature — the same shape 5e uses for environmental threats: trigger, detection, avoidance/disarming, effect. The 2014 Basic Rules use a "fusillade of poisoned darts" as an example trap hazard. ([D&D Beyond — Basic Rules](https://www.dndbeyond.com/sources/dnd/basic-rules-2014/running-the-game)) DC 14 sits inside [[region.aruhe|Aruhe]]'s existing environmental DC 13–15 cluster rather than inventing a new difficulty scale.

The ecosystem knows the rule before the adventurers do. Small scavengers cross patches with exaggerated slowness and feed on the punctured carcasses; the party can learn from watching them — and later weaponize the white-hot center of an otherwise ordinary encounter.
