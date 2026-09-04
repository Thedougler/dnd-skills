---
name: tag-taxonomy
description: >
  Enforce consistent tagging across the Campaign OS wiki using the controlled vocabulary
  in _system/config/taxonomy.md (24 canonical tags). Use this skill when the user says "fix
  my tags", "normalize tags", "clean up tags", "tag audit", "what tags should I use", "tag
  taxonomy", or whenever you're creating or updating wiki pages and need to choose tags. Also
  trigger when the user asks about tag conventions, wants to add a new tag to the taxonomy,
  or says "my tags are a mess". Always consult this skill's taxonomy file before assigning
  tags to any wiki page.
---

# Tag Taxonomy — Controlled Vocabulary for Wiki Tags

You are enforcing consistent tagging across the wiki by normalizing tags to the campaign's controlled vocabulary — a tight set of **24 canonical tags**. Tags name **play texture and campaign forces** — never type, place, faction, habitat, or frontmatter axes (those have fields, folders, links, and body sections).

## Before You Start

1. **Resolve config** — follow the Config Resolution Protocol in `llm-wiki/SKILL.md` (inline `@name` override → walk up CWD for `.env` → `~/.obsidian-wiki/config` → prompt setup). This gives `OBSIDIAN_VAULT_PATH` (the `wiki/` root) and, for Campaign OS, `OBSIDIAN_SCHEMA_SOURCE`.
2. Derive the repository root (the vault root's parent) and set `TAXONOMY_FILE="$REPO_ROOT/_system/config/taxonomy.md"`. **Confirm that file exists before changing a page** — it is the canonical tag list. If it is missing, report the missing authority and stop.
3. Read `$TAXONOMY_FILE` in full — the canonical tags, aliases, the "Do not put these in tags" carriers, and the migration table.
4. Orient: skim `$OBSIDIAN_VAULT_PATH/index.md` for scope if unfamiliar.

The taxonomy file is the source of truth. It is grounded in a full-vault audit: **Texture** tags (`maritime`, `intrigue`, `exploration`, `mystery`, …) are the workhorse; **Motif** (`dravosi-crown`, `drowned-maw`, `umberlee`, `blight`) names the four campaign forces; **Table** has `recurring` and `consumable`. Everything else observed in the wild — ecology adjectives, subtypes, place and faction names, session/season/operational one-offs — is a migration drop onto a field, folder, link, or body section. The vocabulary stays small on purpose; a fact that has a home is not a tag.

## Reserved System Tags

`visibility/` is a reserved tag group with special rules. These tags are **not** domain or type tags and are managed separately from the taxonomy vocabulary:

| Tag | Purpose |
|---|---|
| `visibility/public` | Explicitly public — shown in all modes (same as no tag) |
| `visibility/internal` | Team-only — excluded in filtered query/export mode |
| `visibility/pii` | Sensitive data — excluded in filtered query/export mode |

**Rules for `visibility/` tags:**
- They do **not** count toward the 5-tag limit
- Only one `visibility/` tag per page
- Omit entirely when content is clearly public — no tag needed
- Never add `visibility/internal` just because content is technical; use it only for genuinely team-restricted knowledge
- When running a tag audit, report `visibility/` tag usage separately — do not flag them as unknown or non-canonical

When normalizing tags, leave `visibility/` tags untouched — they are not subject to alias mapping.

## Mode 1: Tag Audit

When the user wants to see the current state of tags:

### Step 1: Scan canonical pages

Glob `$OBSIDIAN_VAULT_PATH/**/*.md`, excluding what canonical page discovery excludes: `_raw/`, `_archive/`, `wiki/.obsidian/`, `wiki/assets/`, `wiki/sources/` (managed corpora), renderer output, and the ledgers (`index.md`, `log.md`, `hot.md`). Extract the `tags:` field from YAML frontmatter (inline `tags: [a, b]` or list form `tags:\n  - a`). Note: the `---` frontmatter delimiter can be misparsed as a `--` tag — a tag that looks like dashes is a parser artifact, not a real page problem.

### Step 2: Classify against the taxonomy

For each tag found, bucket it:

- **Canonical** — in the taxonomy's canonical tables
- **Alias** — in an alias column; note the canonical form it maps to
- **Migration** — in the migration table; note the rename target or the carrier (field/folder/id/body section) that makes it droppable
- **Unknown** — in none of the above

Flag separately:

- **Over-tagged pages** — more than 5 non-`visibility/` tags
- **At-cap violations** — 5 tags where most violate the taxonomy (worth fixing, not just noting)

Do **not** flag untagged pages as a defect. The taxonomy states canonical pages are mostly `tags: []` — empty is correct until a page has real texture. Only list untagged pages whose body clearly has texture worth a tag.

### Step 3: Report

```markdown
## Tag Audit Report

### Summary
- Pages scanned: 636 | tagged: 325 | untagged: 309
- Unique tags: 159 | canonical: 24 | aliases: ~30 | migration/drop: ~100 | unknown: N

### Non-Canonical Tags Found (sample)
| Current Tag | → Canonical / Action | Pages Affected |
| ----------- | -------------------- | -------------- |
| `naval`     | → `maritime`         | 4              |
| `beast`     | drop (`subtype`)     | 9              |
| `aquatic`   | drop (Habitat body)  | 5              |
| `maw`       | → `drowned-maw`      | 0              |

### Unknown Tags (not in taxonomy)
| Tag          | Pages | Recommendation                   |
| ------------ | ----- | -------------------------------- |
| `song`       | 1     | Drop — creature body             |

### Over-Tagged Pages
| Page                     | Tag Count | Tags                 |
| ------------------------ | --------- | -------------------- |
| `settlement.tidefall.md` | 6         | maritime, dravosi-crown, naval, … |
```

## Mode 2: Tag Normalization

When the user wants to fix the tags:

### Step 1: Run the audit (above)

### Step 2: Apply fixes

For each page with non-canonical tags, one at a time:

1. Read the page's frontmatter (and enough body to judge intent)
2. Replace alias tags with their canonical form from the taxonomy
3. Apply migration entries: rename targets as specified; **drop** tags whose fact a field, folder, ID, link, or body section already carries (the carrier is named in the migration table)
4. If the page has > 5 tags, drop the least relevant — texture beats place/kind/habitat duplicates
5. Write the updated `tags:` field

**Example (settlement page):**

```yaml
# Before
tags: [maritime, dravosi-crown, naval, inspection, checkpoint, calders-tooth]
# After
tags: [maritime, politics]   # dravosi-crown → factions: field; naval → maritime;
                             # inspection/checkpoint → politics; calders-tooth → within: field
```

**Example (creature page):**

```yaml
# Before
tags: [beast, aquatic, predator]
# After
tags: []                     # beast is the subtype; aquatic/predator live in Ecology/Habitat
```

### Step 3: Handle unknowns

For tags that aren't in the taxonomy and aren't aliases or migration entries:

- Used on **2+ pages** → propose adding it to the taxonomy (see Mode 4), then ask the user
- Used on **1 page** → drop it or replace with the closest canonical tag
- Ask the user before making changes to unknown tags

### Step 4: Update taxonomy

If new canonical tags were agreed upon, append them to `$TAXONOMY_FILE` in the correct section, with a one-line "use for", aliases, and a migration entry for superseded spellings. The vocabulary should stay small — prefer mapping onto an existing tag over adding one.

## Mode 3: Tagging a New Page

When you're creating a wiki page and need to choose tags:

1. Read `$TAXONOMY_FILE`
2. Select tags by page kind — **never** tag the kind, subtype, place, faction, habitat, or any frontmatter axis:
   - **Creature / hazard:** 1–2 texture tags; habitat and behaviour stay in the **Ecology** and **Habitat** body sections
   - **Item:** texture + `consumable` if it is used up (`potion`/`tool`/`wondrous` go in `subtype`)
   - **Region / location / settlement:** texture (+ a motif only if the force is the page's central pressure)
   - **Quest / hook / situation / beat / event:** texture
   - **Faction / deity / vehicle / NPC / PC:** usually `tags: []`; a motif only when the force defines the page
   - **Rules / session / campaign machinery:** `recurring` when a returning element is the point; otherwise `tags: []`
3. Max 5 tags, canonical only — never aliases
4. If no existing tag fits, leave `tags: []` or check whether an addition is worth proposing (Mode 4)

## Mode 4: Adding a New Tag

When the user wants to add a tag to the vocabulary:

1. Check the taxonomy's canonical tags, aliases, and migration table — an existing tag usually covers the concept; prefer mapping onto it
2. If genuinely new: confirm it is not a kind, subtype, place, faction, status, session id, frontmatter axis, or creature-habitat body fact, and that it will be used on 2+ pages
3. Add it to `$TAXONOMY_FILE` in the correct section (Texture, Motif, or Table) with the canonical name, a one-line "use for", and any aliases to redirect
4. Add a migration entry for any current spellings it supersedes

## After Any Tag Operation

1. **`log.md`** — append a one-line ledger entry to `$OBSIDIAN_VAULT_PATH/log.md`:
   ```
   - [TIMESTAMP] TAG_NORMALIZE tags_renamed=N pages_modified=P new_tags_added=N note="…"
   ```
   (Audit-only: `- [TIMESTAMP] TAG_AUDIT tags_normalized=N unknown_tags=M pages_modified=P`)
2. **`hot.md`** — read `$OBSIDIAN_VAULT_PATH/hot.md` (create from the `wiki-ingest` template if missing). Add one Recent Activity line — e.g. "Tag taxonomy: normalized tags across N pages." Keep at most 3 Recent Activity entries. Update the `updated` timestamp.
3. **Doctor** — for every canonical page whose frontmatter you edited, run `npm run doctor -- --file <page>` (repeat the flag per page) or `npm run doctor -- --fix`; resolve any findings before yielding.
4. **QMD refresh** — QMD is a search index, not the source of truth. If `$QMD_WIKI_COLLECTION` is empty or unset, skip this step. Run it only after this skill has written or rewritten vault markdown. If QMD refresh fails, do not roll back the vault changes; report the QMD status separately.

Use `$QMD_CLI` if set; otherwise use `qmd`, from the repository root:

```bash
${QMD_CLI:-qmd} update
```

If the output says vectors are needed or embeddings may be stale, run:

```bash
${QMD_CLI:-qmd} embed
```

Verify the collection with either:

```bash
${QMD_CLI:-qmd} ls "$QMD_WIKI_COLLECTION"
```

or, when a specific page path is known:

```bash
${QMD_CLI:-qmd} get "qmd://$QMD_WIKI_COLLECTION/<page>.md" -l 5
```

Record one of:
- `QMD refreshed: update + embed + verified`
- `QMD refreshed: update only + verified`
- `QMD skipped: QMD_WIKI_COLLECTION unset`
- `QMD skipped: qmd CLI unavailable`
- `QMD failed: <short error summary>`
