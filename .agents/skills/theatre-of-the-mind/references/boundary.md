# Player boundary

The owning parent and current table state supply the world. This skill decides
which part of that world the player can receive through the current surface.
It does not invent a second world inside player-facing prose. Read this file
whenever a scene contains hidden truth, automatic knowledge, a specific
interaction, a creature effect, or an unresolved player choice.

## Evidence-of-access gate

Before putting a detail on the player-facing page, name its legitimate channel:

1. **Current sensory access:** a character can see, hear, smell, touch, or
   otherwise sense it from the current position, angle, and state.
2. **Established automatic knowledge:** the character's known expertise,
   culture, background, magic, or prior experience supports recognition. Do not
   invent a specialty to make a detail convenient.
3. **Declared and resolved interaction:** the player declared an action and the
   fiction or mechanic resolved it. Describe only what that result exposed.
4. **Earned public canon:** the parent or prior play has already made the fact
   public and relevant. Preserve its certainty and ownership.

If no channel applies, cut the detail and stop or route to the owning
content-stock skill. An uncertainty marker does not create access: an inference
is permissible only when it follows from named perceivable evidence or
established knowledge. Source silence cannot be filled with a genre default.
Recheck the object's interaction state: visible, held/inspected,
recognized/used, or recurrent/intelligent. A character holding an intact
stonepear can receive its established exterior and weight; holding it does not
reveal the inside, underside, function, history, contents, taste, temperature,
texture, or magic. Do not write “skin barely yields,” “grit under the skin,” or
equivalent interior information until the surface is actually exposed and the
result is resolved.

Current sensory access also has a boundary. A sightline does not expose the
far side; a hand on a handle does not inspect the room beyond a door; a sound
does not identify its source without evidence. Questions and player actions
earn closer detail. Mechanics can establish an effect, but do not backfill
unresolved fiction with its likely explanation.

## Fresh phrasing gate

The parent and references provide facts and technique, not wording to repeat.
Make a terse fact inventory in fragmentary keywords with provenance and access;
never copy source sentences into that inventory. Set source and reference prose
aside, group facts by the target contract rather than source order, and draft
with a different subject order, syntax, verbs, and comparisons. Compare the
result against the polished parent and every read expert excerpt for suspicious
phrase or sentence overlap, recognizable clauses, distinctive metaphors,
callouts, or matching section order across paragraphs. Rewrite; merely swapping
synonyms sentence by sentence is not enough. Preserve proper names, necessary
measurements, and irreducible game terms only when changing them would alter
identity or accuracy. “Copy the move, leave the setting” means copy the
technique, never the words. The sole narrow exception is an established
in-world quotation, inscription, or document the user explicitly requests
verbatim; identify its owner and quotation. Expert table lines in `experts.md`
are instructional analysis, not player-facing text to echo.

## Standalone knowledge scope

Unless the user explicitly asks for identified or player-known properties, a
standalone portrait is a cold player-appearance and observable-state layer.
Parent audience labels such as `[agent, dm]` do not grant player knowledge.
Include all established descriptive states needed to recognize the subject,
including state-qualified physical views such as a cut cross-section, but keep
exact effects, durations, speeds, actions, DCs, rarity, attunement, curses,
private biology or history, tactics, hidden causes, learned route rules, and
secret identities out. Render a separately requested mechanics layer only after
the description and only within the explicitly granted knowledge state.
Complete means complete for the target portrait contract, never every parent
heading.

## Manifestation, inference, mechanics

Keep these layers separate, especially for creatures, auras, hazards, magic,
and illusions:

- **Visible manifestation:** body, posture, behavior, buildup, and sensory or
  physical effects the characters actually experience now.
- **Permissible inference:** a character's qualified reading of named
  perceivable evidence or established knowledge (“it may be warded,” “the air
  seems to thin”). “May” or “seems” cannot rescue a detail with no evidence;
  players still decide what it means. Do not turn mood into certainty.
- **Mechanic or secret:** exact radius, DC, condition, HP, damage, save,
  recharge, hidden ability, source, or true consequence. Keep these in
  `[!mechanic]` or collapsed `[!secret]-` until the parent, character
  knowledge, earned public canon, or a resolved interaction makes them public.

On a first look at a monster, expose only body, visible behavior, posture, and
sensory effects actually experienced. Do not announce an exact 30-foot aura or
suffocation before contact merely because the stat block contains them.
Telegraph danger with an observable buildup — breath frosting, moths dropping,
grass paling, a cough after someone enters — then resolve the mechanic when the
table acts. A later public reveal may state the rule in the appropriate wrapper.

## Player agency

Never write what a PC thinks, feels, wants, decides, intends, remembers
incorrectly, concludes, or chooses to investigate. Do not narrate a route,
trust, surrender, victory, death, or other unresolved outcome. Show the
stimulus and leave the response to the player.

NPC and faction behavior may pursue established goals. The world may change
because of a resolved mechanic or an established pressure. A player-facing
surface stops at the next meaningful decision; do not append an “if they hold”
or “if anyone touches it” branch to spoken text.

If a description gives the table a false mental model, correct it directly.
Communication must not become a hidden challenge. Do not hide obvious geometry,
conspicuous danger, or normal expertise to manufacture mystery.

## Parent, canon, and stock

Read the owning parent before drafting. Established and locked facts remain the
authority. Preserve beliefs as beliefs; do not promote a possibility to canon
because it makes a cleaner image.

If the parent lacks a signature, first-sight facts, and one usable property,
invoke `fleshing-out-content` before this prose pass. Select only facts that
pass the access gate. The stock pass may add reversible texture, but may not
decide hidden truth, player action, or an unresolved consequence. Keep hidden
truth in `[!secret]-`.
