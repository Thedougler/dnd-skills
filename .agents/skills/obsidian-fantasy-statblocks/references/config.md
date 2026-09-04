# Config keys and layouts

## Per-block keys

```yaml
layout: Basic 5e Layout
name: "Roper"
dice: true
columns: 2
source: "Homebrew"
bestiary: true
```

`dice: true` turns on Dice Roller for this block. A vault-wide
"Integrate dice roller" setting exists in Plugin Settings.

## Layouts

This campaign uses **Basic 5e Layout** only. Fate Core, Pathfinder
2e, and 13th Age built-ins do not apply.

Custom layouts are a Settings-tab concern (Import / Add / Duplicate).
This vault has none yet. Write `layout: Basic 5e Layout`.

## Settings screen

Community plugins → Fantasy Statblocks:

- General: export PNG, dice integration, render wikilinks, disable
  bundled 5e SRD, debug
- Note parsing: parse frontmatter, bestiary folders
- Layout: default layout, custom layouts
- Homebrew creatures: import / add / filter

Point bestiary folders at wherever this vault's `kind: statblock`
pages actually live (`rules/` under the current layout). A folder
list that does not contain those pages will not auto-register them.
