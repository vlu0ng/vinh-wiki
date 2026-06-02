---
title: "Connection Schema"
date: 2026-06-02
tags: [system, schema, spec]
---

# Connection Schema

Defines the **typed-edge vocabulary** for the vinh-wiki knowledge graph. Ported from [gbrain](https://github.com/garrytan/gbrain)'s typed-edge model into markdown frontmatter. Read by `vinh-wiki-connection-discovery` (writes edges) and `vinh-wiki-dream-cycle` (reads edges to find contradictions).

## Two frontmatter fields, one source of truth

Every wiki page may carry **two** linking fields. They are not redundant — each serves a different consumer:

```yaml
related: [[carol-dweck]], [[mathematics-education]]   # FLAT union — Obsidian graph + wiki-dashboard.html
connections:                                           # TYPED edges — the knowledge graph
  - type: influenced-by
    target: carol-dweck
  - type: applies-to
    target: mathematics-education
```

- **`related:`** — the flat, untyped, de-duplicated **union** of every `connections[].target`. Backward-compatible: Obsidian's graph view and `wiki-dashboard.html` both parse only this field. **Never remove a target from `related:` that still has a `connections` edge.**
- **`connections:`** — the typed edges. Each entry is `{ type, target }` where `target` is a page slug (no `[[ ]]`, no `.md`).

**Invariant:** `related:` MUST equal `{ [[t]] for t in connections[].target }` ∪ (any legacy hand-authored links). When you add a `connections` edge, add its target to `related:` in the same edit.

## Edge-type vocabulary

Pick the **most specific** type that fits. If nothing fits, use `related` (the untyped fallback). Each type has an **inverse** written on the target page (bidirectionality is mandatory).

| Type | Meaning | Inverse (on target) |
|---|---|---|
| `influenced-by` | Source's ideas derive from / build on target | `influenced` |
| `critiques` | Source argues against / problematizes target | `critiqued-by` |
| `extends` | Source elaborates or generalizes target | `extended-by` |
| `contradicts` | Source makes a claim incompatible with target | `contradicts` (symmetric) |
| `applies-to` | Source is a framework/method applied in target's domain | `application-of` |
| `authored` | Person/org produced the work (topic/source) | `authored-by` |
| `founded` | Person founded org/institution | `founded-by` |
| `advises` | Person advises/partners another person/org | `advised-by` |
| `example-of` | Source is a concrete instance of target concept | `has-example` |
| `related` | Untyped thematic link (fallback only) | `related` (symmetric) |

Symmetric types (`contradicts`, `related`) use the same type on both pages. All others use the inverse.

## Rules

- **Additive only.** Adding `connections:` must never shrink `related:`. Legacy pages with `related:` but no `connections:` are valid; backfill them opportunistically, never destructively.
- **Slugs, not wikilinks, inside `connections`.** `target: carol-dweck`, not `target: [[carol-dweck]]`.
- **Closest type wins; `related` is the escape hatch** — do not invent new type names without adding them to this table first.
- **Bidirectional.** Every edge gets its inverse on the target page in the same session.
