# Bestiary and recall

## Registration

A fence on a note the plugin is set to parse enters the bestiary by
the creature `name:`. Keep frontmatter `name:` (if present) identical
to the fence `name:` — a mismatch orphans recall with no error.

`bestiary: false` on a fence excludes that block from registration.

The plugin also ships a bundled 5e SRD (toggle: "Disable 5e srd").
`monster: Goblin` may resolve from that bundle, not from a vault page.

Two other creation methods exist (Save to Bestiary; Settings → Add
Creature). New pages use a git-tracked fence on a `kind: statblock`
page instead. Cache entries in the plugin's `data.json` do not
round-trip through the vault.

## Recall

```statblock
layout: Basic 5e Layout
monster: Octopus
name: "Harbor Octopus"
```

Recall is by exact name. A bare field (`name`, `hp`, `ac`, …)
**replaces** the inherited value.

```statblock
layout: Basic 5e Layout
monster: Octopus
actions+:
  - name: "Ink Cloud"
    desc: "..."
```

`field+:` **appends** to an inherited array (`traits+:`, `actions+:`,
`bonus_actions+:`, `reactions+:`). A bare `field:` replaces the whole
array. Remove one inherited entry by name with `field-:`
(e.g. `actions-:` / `- name: Bite`).

Treat `extends:` the same way as `monster:` for replace-vs-append.
