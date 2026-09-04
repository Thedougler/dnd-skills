---
name: player-character-mechanics
description: >-
  Player-character mechanics — use when a task needs to know what a
  PC can do now, or when a PC's class/level, abilities, HP/resources,
  proficiencies, conditions, features, inventory, equipment, spells,
  actions, or rests change and its canonical character state or
  compiled PC projection must be read, updated, repaired, or refreshed.
---

# Player-character mechanics

Make **what can this PC do right now?** a cheap, reliable question.

The canonical PC owns character-specific **build state**. Reusable
mechanics stay on `rule` / `spell` / `item` pages. **Table state** is
Runtime. The **PC projection** materializes both. Agents run this
**between sessions**. During play the DM narrates; the transcript is
evidence.

## Sources of truth

For `pc.<slug>`:

- `campaign/pc.<slug>.md` — identity, gravity, `pc-state` fence
- linked `rule` / `spell` / `item` / `equipment` pages and playable `source-entry` spells — reusable definitions
- `_system/schemas/pc/` — field contract; read before writing
- `_system/state/pcs/pc.<slug>.runtime.json` — table state
- `_system/state/pcs/pc.<slug>.json` — projection; never canon

Discover the compiler and doctor from the environment
(`package.json`, `--help`). Do not cache command names here.

A `pc-sheet` fence is view config. It is not a second record.

## 1. Resolve the PC

1. explicit wikilink or path
2. exact `campaign/pc.<slug>.md`
3. exact lexical lookup among `kind: pc`
4. broader retrieval only if identity is ambiguous

Read `canon` before editing. If there is no `kind: pc` page, stop.
Origination is `player-character-interview`. Do not mint a parallel
record.

**Complete when:** exactly one existing PC is resolved, or the
absence/identity conflict is explicit.

## 2. Load the projection

Read the PC and its projection. If the projection is missing or its
hash no longer matches the `pc-state` + runtime it claims, run the
configured compiler. On compiler failure, inspect diagnostics. If no
compiler exists, resolve only what this task needs from canon and
report the gap — do not invent a projection.

Follow source pages only for unresolved capabilities or full rule
text.

**Complete when:** every mechanical claim the task needs is traceable
to the PC, runtime, or a linked canonical source.

## 3. Own each fact once

- **PC / `pc-state`:** character-building choices, scores, listed
  proficiencies, class/feat/species/background, possessions,
  equipped/attuned, known/prepared spells, stated `hp_max` / hit
  dice / AC override, play-established lasting patches.
- **Source pages:** spell text, item mechanics, class/feature/feat
  rules. Link them; do not paste a second definition.
- **Runtime file:** current HP, temp HP, death saves, expended
  resources, concentration, conditions.
- **Projection:** modifiers, proficiency bonus, save/skill totals,
  AC/HP when derivable, attacks, slot *counts*, denormalized
  summaries. Diagnostics instead of guesses.

**Complete when:** each changed fact has one owner.

## 4. Patch from play evidence

Agents write between sessions. Reconciliation reads `present`
transcript discourse.

Promote **next-session-true** facts onto `pc-state` (remaining HP
stays in runtime; inventory/prep/attunement/lasting resources that
would still be true tomorrow go to build state). Discard in-combat
expenditures that reset when the next fight starts.

A rest restores resources only when that rest `event` is `occurred`.
Unresolved rest rules are diagnostics.

Play-established loot/spend/prepare/attune may be patched. Ability
scores, species, class/level, feats, and subclass picks are
human/player decisions — propose them.

If loot must be cited as a node, invoke `writing-items`, then link
the page from possessions.

Do not append a Session Log. History is events and session-reports.

**Complete when:** canon states the new character once, with no
copied rule text.

## 5. Compile

Run the configured PC compiler after any mechanical write. v1
resolves a closed set (scores, proficiency, listed proficiencies,
HP from hit dice + CON or stated max, AC from override or equipped
armor + Dex, stated speeds/senses, slot counts, spell *links*,
equipped weapon attacks). Features and items are links and
diagnostics, not inferred action cards.

**Complete when:** the projection is current and every unresolved
mechanical question is a diagnostic.

## 6. Serve

Answer capability questions from the projection first. For several
PCs, load each projection. For session prep, give the smallest
sufficient slice: defenses, senses/movement, high-impact skills,
attacks, limited resources, concentration or major spells, relevant
gear.

The DM sheet (`--sheet`) is a read view of the same object.

**Complete when:** the consumer has the smallest sufficient character
context without dropping a mechanically consequential option.

## 7. Validate

Schema validation, compiler, doctor, projection diagnostics, linked
sources exist, renderer holds no authoritative data. Refresh QMD
through the configured indexing workflow when content it indexes
changed.

## Done

One PC owns each character-specific fact. Reusable mechanics stay on
source pages. Projection is current. Unresolved mechanics are
diagnostics. Human view and agent answers consume the same
projection.
