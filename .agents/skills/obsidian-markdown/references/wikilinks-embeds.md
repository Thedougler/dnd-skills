# Wikilinks and embeds

## Wikilinks

| Syntax | Result |
|--------|--------|
| `[[pc.mara-venn]]` | Link to that page |
| `[[pc.mara-venn\|Mara Venn]]` | Display alias |
| `[[pc.mara-venn#Gravity]]` | Heading |
| `[[pc.mara-venn#^block-id]]` | Block |

`id` matches the filename stem. Prefer `[[kind.slug|Display]]` so the
graph stays kind-prefixed and the table reads a name.

In a markdown table cell, escape the alias pipe: `[[pc.mara-venn\|Mara]]`.
An unescaped `|` is a new column.

Obsidian resolves by unique filename. Two files with the same stem need
a path prefix; this vault's kind-prefix convention makes that rare.

## Embeds

| Syntax | Result |
|--------|--------|
| `![[pc.mara-venn]]` | Full note |
| `![[pc.mara-venn#Gravity]]` | One section |
| `![[assets/maps/kalowe.webp]]` | Image |
| `![[assets/maps/kalowe.webp\|300]]` | Image at 300px wide |

Prefer a wikilink or a section embed over restating another page.
A `.base` embed is `wiki-dashboard`, not this skill.
