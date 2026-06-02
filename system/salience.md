---
title: "Salience Digest"
date: 2026-06-02
tags: [system, digest]
---

# Salience Digest

A "what to look at next" digest, **regenerated each `vinh-wiki-dream-cycle` run** (this file is overwritten below the header each time — it is a snapshot, not an append-only log). Ported from [gbrain](https://github.com/garrytan/gbrain)'s salience scoring.

Each page is scored on cheap structural signals:
- **Inbound edges** — how many other pages point to it (`[[slug]]` mentions + `connections` targets). High = central.
- **Body depth** — approximate length / section count. Low = thin.
- **Staleness** — days since frontmatter `date:`.
- **Open questions** — unanswered `## Open Questions` bullets present.
- **Orphan** — zero inbound links.

## Last run

_Not yet generated. Run `vinh-wiki-dream-cycle` to populate._

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

## Surfacing for the dashboard
_Top pages by salience score (feeds optional `wiki-dashboard.html` node sizing)._
