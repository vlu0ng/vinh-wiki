# Claude Code Instructions — vinh-wiki

This is an Obsidian knowledge vault operated in the Karpathy LLM Wiki style.

**Always start every session by reading `system/AGENTS.md` fully before taking any action.**

The full operating manual is in `system/AGENTS.md`. Follow it precisely.

## Quick Reference: Core Workflows

### Ingest Raw Material
```
Ingest all unprocessed files in raw/articles/ (i.e., files not yet referenced in any wiki/ page).
For each file:
1. Read the content.
2. Identify key concepts, people, and topics.
3. Create or update appropriate pages in wiki/concepts/, wiki/people/, and wiki/topics/.
4. Use [[wikilinks]] to connect pages.
5. Update system/index.md if you create a major new page.
6. Append a summary to system/log.md when done.
```

### Synthesize a Topic
```
Review all wiki pages and raw files related to [TOPIC].
Create or update wiki/topics/[topic-name].md with:
- A comprehensive synthesis of what I know
- Key concepts with [[wikilinks]]
- Open questions and gaps
- Sources referenced
Then update system/index.md and log.md.
```

### Health Check & Maintenance
```
Perform a health check on the wiki/:
1. Find orphan pages (no inbound [[wikilinks]]) and suggest where to link them. Implement the links.
2. Find missing frontmatter and add it.
3. Find pages that reference the same concept without linking — add wikilinks.
4. Identify any raw/ files that have not yet been ingested and list them.
5. Log all changes in system/log.md.
```

### Query / Research Mode  (→ `vinh-wiki-think`)
```
Given everything in wiki/, answer this question: [YOUR QUESTION]
Cite specific wiki pages and note if the information is incomplete or needs more sources.
After answering, suggest 1-2 follow-up pages to create or enrich.
```
The `vinh-wiki-think` skill formalizes this: a synthesized answer with inline `[[citations]]`
plus an explicit `## Knowledge Gaps` section that can be queued to `system/ingest-queue.md`.

### Dream Cycle  (→ `vinh-wiki-dream-cycle`)
```
Run the dream cycle on the wiki/:
1. Detect contradictions between connected pages → record in system/contradictions.md (surface, don't resolve).
2. Flag near-duplicate concept/people pages → propose merges for approval (never delete).
3. Regenerate the salience digest in system/salience.md (what to enrich / revisit next).
4. Append uningested raw + under-developed pages to system/ingest-queue.md.
5. Log all changes in system/log.md.
```

## Connection Schema

Connections are **typed** (gbrain-style). See `system/schema.md` for the edge vocabulary.
Every page carries two linking fields: the flat `related:` union (Obsidian + dashboard) and a
typed `connections:` block (the knowledge graph). `related:` is additive — never shrink it.

## Weekly Automation

The weekly cadence (`maintenance` → `connection-discovery` → `answer-questions` → `dream-cycle`)
is run hands-off via `/schedule` routines. Each pass appends to `system/log.md`, keeping the
cadence auditable.
