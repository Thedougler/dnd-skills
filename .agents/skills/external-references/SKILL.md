---
name: external-references
description: External references — use when durable work cites, saves, refreshes, or reuses a web page, paper, video, repository, dataset, or other external research resource. Use the managed source corpus instead when exact publication content must be locally ingested.
---

# External references

Persist external research as `kind: reference` when another page, later task,
or recheck must cite the resource as a node.

## 1. Classify

Load the `reference` schema and template.

Use `reference` for external evidence represented locally by provenance and a
faithful digest.

Use `source` + `source-entry` when the resource needs managed local ingestion,
exact searchable source text, ingest policy, or forks.

Complete when the resource has exactly one evidence model.

## 2. Resolve identity

Prefer a persistent or versioned identifier when available. Resolve the
canonical URL, then search existing references by persistent identifier,
canonical URL, and title before minting a page.

One external resource has one reference node unless independently citable
versions must deliberately remain distinct.

Complete when no duplicate node exists and the reference identity is stable.

## 3. Ground

Read the actual resource. Record its provenance and the representation being
summarized. For mutable material, preserve an immutable snapshot or version
when available.

Write only claims supported by the resource. Use source-native locators for
consequential findings.

Complete when every consequential finding can be traced back to the external
resource.

## 4. Distill

Write the template's Summary, Findings, and applicable Limitations.

Make Summary self-contained enough to survive retrieval without the surrounding
wiki. Keep interpretation and Campaign-OS application on the consuming Work or
Knowledge page.

Complete when the reference can be retrieved and understood without fetching
the external resource, while remaining recognizably faithful to it.

## 5. Cite

Add the reference to a page's `sources:` only where it actually grounds that
page. Use ordinary prose links when it is merely related or inspirational.

Complete when every durable use has the intended relationship and no
unsupported claim gained authority from the reference.

## 6. Validate

Run `npm run reference -- check <id|--all>`, Doctor, and link checks where
applicable. Refresh the `sources` retrieval index after writes.

Complete when validation passes, the reference is retrievable by title and
subject, and no duplicate or provenance diagnostic remains.
