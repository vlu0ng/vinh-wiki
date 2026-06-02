---
title: "Ingest Queue"
date: 2026-06-02
tags: [system, registry]
---

# Ingest Queue

A prioritized backlog of material worth ingesting next. Fed by:
- **`vinh-wiki-think`** — knowledge gaps surfaced while answering a question (what the vault couldn't answer).
- **`vinh-wiki-dream-cycle`** (salience stage) — uningested `raw/` files and under-developed pages.
- **`vinh-wiki-maintenance`** — uningested raw files (Check 4).

`vinh-wiki-ingest` reads this at the start of a session to decide what to process. Remove a row (or mark it `done`) once the gap is closed.

## Queue

| Date added | Source | What's missing / to ingest | Priority | Status |
|---|---|---|---|---|
