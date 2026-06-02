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
  AGENTS.md          ← This file (read-only for you)
  index.md           ← High-level wiki overview and entry points (keep updated)
  log.md             ← Append-only session log (always append, never overwrite)
  schema.md          ← Typed-edge vocabulary for connections: frontmatter (read before connection-discovery)
  connection-discovery.md ← Registry of pages already analyzed for connections (idempotency)
  answered-questions.md   ← Registry of answered open questions (idempotency)
  contradictions.md  ← Registry of conflicting claims surfaced by dream-cycle (never silently resolve)
  ingest-queue.md    ← Prioritized backlog of raw files and gaps to ingest next
  salience.md        ← Snapshot digest of highest-leverage pages (regenerated each dream-cycle run)
  pull-log.md        ← Append-only log of local cron git pulls (written by vinh-wiki-pull.sh)
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
  related: [[RelatedPage1]], [[RelatedPage2]]   ← flat union for Obsidian graph + dashboard
  connections:                                   ← typed edges (see system/schema.md)
    - type: influenced-by
      target: related-page-1
  ---
  ```
- Concept pages: brief definition, key properties, related concepts, examples.
- Topic pages: broader overview, synthesis across multiple sources, open questions.
- People pages: who they are, key contributions, relevant works, connections.
- Every page must link back to at least one other wiki page.
- `related:` is the flat, additive union of all `connections[].target` slugs — never shrink it.
- `connections:` holds typed edges. Always read `system/schema.md` for the edge vocabulary before adding edges. Bidirectionality is mandatory: every edge needs its inverse on the target page.

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
- Never edit wiki/ concept/topic/people pages during a dream-cycle run — surface only, never resolve.
- Never shrink `related:` frontmatter — it is additive; only add targets, never remove.

## Skills Reference

Six Claude Code skills drive this vault. Each reads AGENTS.md first.

| Skill | What it does | When to use |
|---|---|---|
| `vinh-wiki-ingest` | Encodes raw/ source material into wiki/ pages | New books/articles added to raw/ |
| `vinh-wiki-maintenance` | Fixes orphans, missing frontmatter, unlinked mentions | Weekly health check |
| `vinh-wiki-connection-discovery` | Adds typed `connections:` + `related:` edges between pages | Weekly after maintenance |
| `vinh-wiki-answer-questions` | Resolves `## Open Questions` bullets into new wiki pages | Weekly after connections |
| `vinh-wiki-think` | Answers a question across the vault with citations + gap analysis | On-demand research |
| `vinh-wiki-dream-cycle` | Contradiction detection → dedup flagging → salience scoring | Nightly automated pass |

## Automation

Two scheduled routines run against `github.com/vlu0ng/vinh-wiki` (public repo):

- **Nightly (2 AM PT):** `vinh-wiki-dream-cycle` → commits to `system/` → pushes to GitHub.
- **Weekly (Sunday 7 AM PT):** `vinh-wiki-maintenance` → `vinh-wiki-connection-discovery` → `vinh-wiki-answer-questions` → commits to `wiki/` + `system/` → pushes.

A local cron (via `vinh-wiki-pull.sh`) pulls the result at 2:45 AM nightly and 8 AM Sunday, and appends an entry to `system/pull-log.md`.
