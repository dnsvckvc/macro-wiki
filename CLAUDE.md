# LLM Wiki — Schema & Workflow Instructions

This is a wiki maintained by Claude Code. The current working directory **is** the wiki root — `index.md`, `log.md`, `overview.md`, and the `sources/`, `entities/`, `concepts/`, `syntheses/` subdirectories all live here.

The slash commands (`/wiki-ingest`, `/wiki-query`, `/wiki-lint`, `/wiki-graph`) are installed at user level and are available in any session. They follow the workflows defined below.

## Slash Commands

| Command | What to say |
|---|---|
| `/wiki-ingest` | `ingest raw/my-article.md` |
| `/wiki-query` | `query: what are the main themes?` |
| `/wiki-lint` | `lint the wiki` |
| `/wiki-graph` | `build the knowledge graph` |

Or describe in plain English:
- *"Ingest this file: raw/papers/attention-is-all-you-need.md"*
- *"What does the wiki say about transformer models?"*
- *"Check the wiki for orphan pages and contradictions"*
- *"Build the graph"*

---

## Directory Layout

```
.                # the wiki root (cwd)
├── CLAUDE.md    # this file
├── index.md     # catalog of all pages — update on every ingest
├── log.md       # append-only chronological record
├── overview.md  # living synthesis across all sources
├── sources/     # one summary page per source document
├── entities/    # people, companies, projects, products
├── concepts/    # ideas, frameworks, methods, theories
├── syntheses/   # saved query answers
├── raw/         # immutable source documents — never modify these
└── graph/       # auto-generated graph data
```

---

## Page Format

Every wiki page uses this frontmatter:

```yaml
---
title: "Page Title"
type: source | entity | concept | synthesis
tags: []
sources: []       # list of source slugs that inform this page
last_updated: YYYY-MM-DD
---
```

Use `[[PageName]]` wikilinks to link to other wiki pages.

---

## Ingest Workflow

Triggered by: *"ingest <file>"* or `/wiki-ingest`

Steps (in order):
1. Read the source document fully using the Read tool
2. Read `index.md` and `overview.md` for current wiki context
3. Write `sources/<slug>.md` — use the source page format below
4. Update `index.md` — add entry under Sources section
5. Update `overview.md` — revise synthesis if warranted
6. Update/create entity pages for key people, companies, projects mentioned
7. Update/create concept pages for key ideas and frameworks discussed
8. Flag any contradictions with existing wiki content
9. Append to `log.md`: `## [YYYY-MM-DD] ingest | <Title>`
10. **Post-ingest validation** — check for broken `[[wikilinks]]`, verify all new pages are in `index.md`, print a change summary

### Source Page Format

```markdown
---
title: "Source Title"
type: source
tags: []
date: YYYY-MM-DD
source_file: raw/...
---

## Summary
2–4 sentence summary.

## Key Claims
- Claim 1
- Claim 2

## Key Quotes
> "Quote here" — context

## Connections
- [[EntityName]] — how they relate
- [[ConceptName]] — how it connects

## Contradictions
- Contradicts [[OtherPage]] on: ...
```

### Domain-Specific Templates

If the source falls into a specific domain (e.g., personal diary, meeting notes), use a specialized template instead of the default generic one above:

#### Diary / Journal Template
```markdown
---
title: "YYYY-MM-DD Diary"
type: source
tags: [diary]
date: YYYY-MM-DD
---
## Event Summary
...
## Key Decisions
...
## Energy & Mood
...
## Connections
...
## Shifts & Contradictions
...
```

#### Meeting Notes Template
```markdown
---
title: "Meeting Title"
type: source
tags: [meeting]
date: YYYY-MM-DD
---
## Goal
...
## Key Discussions
...
## Decisions Made
...
## Action Items
...
```

---

## Query Workflow

Triggered by: *"query: <question>"* or `/wiki-query`

Steps:
1. Read `index.md` to identify relevant pages
2. Read those pages with the Read tool
3. Synthesize an answer with inline citations as `[[PageName]]` wikilinks
4. Ask the user if they want the answer filed as `syntheses/<slug>.md`

---

## Lint Workflow

Triggered by: *"lint the wiki"* or `/wiki-lint`

Use Grep and Read tools to check for:
- **Orphan pages** — wiki pages with no inbound `[[links]]` from other pages
- **Broken links** — `[[WikiLinks]]` pointing to pages that don't exist
- **Contradictions** — claims that conflict across pages
- **Stale summaries** — pages not updated after newer sources
- **Missing entity pages** — entities mentioned in 3+ pages but lacking their own page
- **Data gaps** — questions the wiki can't answer; suggest new sources

Output a lint report and ask if the user wants it saved to `lint-report.md`.

---

## Graph Workflow

Triggered by: *"build the knowledge graph"* or `/wiki-graph`

Generate the graph data manually:
1. Use Grep to find all `[[wikilinks]]` across every file in the wiki
2. Build a node/edge list (one node per page; one edge per wikilink)
3. Optionally infer additional implicit relationships, tagged INFERRED with a confidence score
4. Write `graph/graph.json` with `{nodes, edges, built: today}`
5. Write `graph/graph.html` as a self-contained vis.js page (nodes colored by type, interactive, searchable)

If the `llm-wiki-agent` repo is cloned locally, you can also run `python <agent-path>/tools/build_graph.py --open` for a Python-driven build with Louvain community detection.

---

## Naming Conventions

- Source slugs: `kebab-case` matching source filename
- Entity pages: `TitleCase.md` (e.g. `OpenAI.md`, `SamAltman.md`)
- Concept pages: `TitleCase.md` (e.g. `ReinforcementLearning.md`, `RAG.md`)
- Source pages: `kebab-case.md`

## Index Format

```markdown
# Wiki Index

## Overview
- [Overview](overview.md) — living synthesis

## Sources
- [Source Title](sources/slug.md) — one-line summary

## Entities
- [Entity Name](entities/EntityName.md) — one-line description

## Concepts
- [Concept Name](concepts/ConceptName.md) — one-line description

## Syntheses
- [Analysis Title](syntheses/slug.md) — what question it answers
```

## Log Format

Each entry starts with `## [YYYY-MM-DD] <operation> | <title>` so it's grep-parseable:

```
grep "^## \[" log.md | tail -10
```

Operations: `ingest`, `query`, `lint`, `graph`
