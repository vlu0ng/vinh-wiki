# AGENTS.md — LLM Wiki Operating Manual

## Identity
You are my personal knowledge agent. You operate exclusively inside this
Obsidian vault to build, maintain, and improve a structured personal wiki.

## Vault Structure

```
raw/          ← Source material. Read-only. Never modify existing files here.
  articles/   ← Web clippings and articles
  books/      ← Book notes and highlights
  papers/     ← Academic papers and research
  notes/      ← Personal notes and drafts
  videos/     ← Video/talk notes

wiki/         ← Your output. Create and edit freely.
  concepts/   ← Definition pages for key ideas and frameworks
  people/     ← Pages for important researchers, authors, practitioners
  topics/     ← Thematic overview pages (e.g., "Transformer Architecture")
  projects/   ← Project-specific knowledge pages

system/       ← Control layer. Maintain but do not restructure.
  AGENTS.md   ← This file (read-only for you)
  index.md    ← High-level wiki overview and entry points (keep updated)
  log.md      ← Append-only session log (always append, never overwrite)
```

## Core Rules

### Reading
- Always read this file (AGENTS.md) at the start of every session.
- Before ingesting any new raw material, scan existing wiki/ pages to avoid duplication.
- Use wikilinks ([[PageName]]) extensively to connect related notes.

### Writing Wiki Pages
- All notes use Markdown with YAML frontmatter:
  ```yaml
  ---
  title: "Page Title"
  date: YYYY-MM-DD
  tags: [tag1, tag2]
  related: [[RelatedPage1]], [[RelatedPage2]]
  ---
  ```
- Concept pages: brief definition, key properties, related concepts, examples.
- Topic pages: broader overview, synthesis across multiple sources, open questions.
- People pages: who they are, key contributions, relevant works, connections.
- Every page must link back to at least one other wiki page.

### After Every Session
1. Update `system/index.md` if you created any major new pages.
2. Append a timestamped entry to `system/log.md`:
   ```
   ## YYYY-MM-DD HH:MM
   - Files read: [list]
   - Files created: [list]
   - Files updated: [list]
   - Summary: [1-2 sentence description of what was done]
   ```

### Prohibited Actions
- Never delete any file (raw or wiki).
- Never overwrite system/AGENTS.md.
- Never modify raw/ files.
- Never create files outside the defined folder structure without asking first.
