# OFM gotchas

Write the form that renders. The other form looks similar and breaks.

| Write | Why |
|-------|-----|
| `[[kind.slug\|Display]]` inside a table cell | An unescaped `\|` is a new column |
| `[[kind.slug]]` for an internal page | A markdown `[text](url)` link will not resolve in the graph |
| Dates as `YYYY-MM-DD` | An ISO datetime in frontmatter is not this vault's date grain |
| Tag lists as YAML `- item` lines | `tags: [a, b]` is legal YAML and a worse Properties panel |
| Quoted `"[[page]]"` in frontmatter | Bare `[[page]]` can be parsed as a nested flow |
| A lone `>` between callout paragraphs | A blank line (no `>`) ends the callout |
| Callout titles on the `[!type]` line | A `##` heading inside a callout body does not render as a heading |
| Markdown only — no `<div>`, `<br>`, comments | Inline HTML is not this vault's page surface |
