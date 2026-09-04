# Adventure module

Use this branch when the walk spans more than one night, or the user
asked for a module rather than tonight.

Still a Renderer. Still assembled. The situation owns the Beat Chart;
session-plans own each night's slice.

## File

Write `adventure.<situation-slug>.md` in the same vault folder as the
owning `situation.<slug>.md`. The DM opens it in Obsidian next to the
island. Do not put modules in `_system/renderers/` — that path is
outside the vault.

`assembled_from` lists the situation and every session-plan the module
covers.

## Shape

1. **Brief** — premise, dramatic question, level/party, gravity, the
   live fronts. One screen.
2. **Chart** — embed the situation's Beat Chart sections (Dramatic
   Question, Spine, Live Branches, Climax Readiness). Do not redraw
   the chart in prose.
3. **Chapters** — one H1 per night, or a wikilink to an already
   assembled `session-guide.<NNN>`. Prefer linking a night that
   already has a guide. Assemble a missing night with the night
   workflow rather than inlining it twice.
4. **Bestiary / roster / sites** — tables of wikilinks, plus section
   embeds only for the blocks the DM will open mid-scene.
5. **Exits** — states that leave this situation for another.

A chapter is still a menu of nodes. A module that sequences nights as
"then the party goes to X" is a plot. Sequence by remaining pressure
and remaining Beat functions.

## What a module adds

- How nights hand off: which clocks, fronts, and unused beats survive
- What is true if a night is skipped
- Where the Climax gate currently sits

## What a module does not add

A second Beat Chart. A predicted route. Player-facing prose that is
not a picture. Lore appendices that duplicate owner pages.
