# Repository Guidelines

## Project structure

This repository is a documentation-only collection of D&D and Campaign OS
agent skills. Each skill is a directory under `.agents/skills/` with an
entrypoint named exactly `SKILL.md`. Supporting guidance belongs in that
skill's `references/` directory; scenario checks, when present, live in its
`evals/` directory. `test-content/` contains sample Campaign OS wiki pages
for exercising the skills. `README.md` is the user-facing catalog and install
guide.

## Creative-writing priority

The repository's primary improvement target is
`.agents/skills/theatre-of-the-mind/`. Use this skill whenever text crosses
the DM/player boundary. When revising it, preserve its camera/staging,
pointable anchors, player agency, and hidden-truth boundary. Read its required
references before changing behavior or examples. Validate player-safe prose by
reading it aloud and checking: where are we, what do we see, what is moving,
and what matters now.

## Developing skills

Keep skill directories and reference filenames in kebab-case. Start every
`SKILL.md` with YAML frontmatter containing a matching `name` and a concise
`description`, then write clear, imperative Markdown. Keep durable rules in
the entrypoint and move detailed patterns or examples into references. Link
between files with relative Markdown paths, and update the skill's reference
index when adding or renaming supporting material. Update `README.md` when a
skill is added, removed, or materially renamed.

There is no package manager, build system, or generated output in this
repository, so no build step is required. Useful checks include:

```bash
find .agents/skills -name SKILL.md
git diff --check
rg -n '^---$|^(name|description):' .agents/skills
```

For a focused change, inspect the edited skill and every linked reference
manually; confirm paths resolve and that Markdown fences, tables, callouts,
and YAML frontmatter remain intact.

## Testing and review

Use relevant files in `test-content/` as realistic Campaign OS inputs when
checking a skill's instructions. If the skill has `evals/evals.json`, run
each listed scenario as a manual or agent evaluation and verify its stated
expectations; do not infer coverage for skills without evals. Before opening
a PR, review the complete diff, check links and frontmatter, and confirm no
unrelated authored content changed.

## Commits and pull requests

Use short, imperative commit subjects that name the skill or documentation
area. Keep commits focused. A PR should explain the behavior or guidance
change, list validation commands and relevant test-content/eval scenarios,
and call out any compatibility or migration impact. Include rendered or
before/after examples when prose or formatting behavior changes.

## Agent skills

### Issue tracker

Issues live in GitHub Issues for `Thedougler/dnd-skills` (`gh` CLI). See `docs/agents/issue-tracker.md`.

### Triage labels

Default vocabulary: `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`. See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: one `CONTEXT.md` plus `docs/adr/` at the repo root. See `docs/agents/domain.md`.
