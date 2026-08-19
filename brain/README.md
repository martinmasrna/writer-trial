# Library conventions

This repo is a knowledge library: documents that steer agents, written to the standard in the writer's `library-document.md`. This file defines the repo's mechanics; it is not itself library knowledge and is never loaded as such.

## Layout

- `index.md` — the only file always loaded into an agent's context. One entry per document.
- `*.md` at root — the documents. Nothing else lives at root.
- `_sources/` — raw material documents were distilled from. Immutable once a document cites it.
- `_reviews/` — review trails, one file per delivered document per pass.

## Naming

- Documents: kebab-case, named for the subject as a consumer would look for it (`the-reader.md`, `marketing-psychology.md`). No dates, no versions — git is the history.
- Sources: keep the original filename.
- Reviews: `<document-name>--YYYY-MM-DD.md`.

## Document frontmatter

Every document starts with:

```
---
description: <1-2 lines: what this covers and when an agent should load it>
source: _sources/<file>.md
---
```

The description is the retrieval mechanism — it is what the index shows and what an agent decides relevance from. Write it for that decision, not as a summary.

## index.md

One entry per document, generated from frontmatter — path plus description, nothing more. The document's frontmatter is the single source of truth; whoever delivers or edits a document updates its index entry in the same commit.

## Linking

Documents link down to their source (`_sources/...`) for the full derivations, per the spec. Documents may link to each other by relative path when one builds on another; the index never substitutes for these links.
