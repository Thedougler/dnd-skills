# Callout syntax

Callouts are blockquotes with a type keyword.

```markdown
> [!narration]
> Player-facing description — read or adapt at the table.

> [!secret]- Title
> Collapsed by default. The `-` is the collapse marker.

> [!tip]+ Title
> Collapsible, open by default.

> [!note] Multi-paragraph
> First paragraph.
>
> A lone `>` line keeps the next paragraph inside the same callout.
```

A fully blank line (no `>`) ends the callout.

Types this vault uses, and the prose contract for each, live in
`CONTEXT.md` and `_system/references/creative-writing.md`.
`[!narration]` craft is `theatre-of-the-mind`.

Callout bodies are markdown. A `##` heading inside a callout does not
render as a heading. Keep titles on the `[!type]` line.
