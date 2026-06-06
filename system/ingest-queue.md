---
title: "Ingest Queue"
date: 2026-06-06
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
| 2026-06-02 | dream-cycle (salience) | `raw/articles/charlie munger - mental models Part 1.pdf` — uningested PDF; likely primary Munger mental-models transcript (1994 USC talk or similar). Would enrich `mental-models`, `latticework-pedagogy`, `munger-disposition-formation`, `mental-models-and-multidisciplinary-thinking`. | high | open |
| 2026-06-02 | dream-cycle (salience) | `raw/articles/charlie munger mental Models Part 2.pdf` — Part 2 of same source. | high | open |
| 2026-06-02 | dream-cycle (salience) | `wiki/concepts/jagged-frontier.md` — thin body (~300 words) vs. 7 inbound links; enrich with worked domain examples, BCG study details, frontier-movement dynamics, open questions. | medium | open |
| 2026-06-02 | dream-cycle (salience) | `wiki/concepts/large-language-models.md` — thin body (~250 words) vs. 6 inbound links; enrich with transformer history, capability trajectory, failure mode catalog, societal framing. | medium | open |
| 2026-06-02 | dream-cycle (salience) | `wiki/concepts/mental-models.md` — body (~350 words) underweight vs. 7+ inbound links; enrich the latticework construction process, known failure modes (see `latticework-failure-modes`), and behavioral-economics convergence. Full vault scan (2026-06-04) revised inbound estimate to 19 — now the #1 most-linked page in the vault. **Priority upgraded to high.** | high | open |
| 2026-06-04 | dream-cycle (salience) | `wiki/concepts/health-equity.md` — body (~400 words) thin vs. 13 inbound links (newly revealed as 3rd-most-linked page). Enrich with: social-determinants framework depth, global health financing, community health worker model details. Also: one unanswered open question ("Is health equity achievable without global wealth redistribution?") that should be answered as a concept page. | medium | open |
| 2026-06-04 | dream-cycle (salience) | `wiki/topics/economic-literacy.md` — two unanswered open questions: (1) "How do you build economic literacy at scale without the content being captured by political narratives?" (2) "Scanlon's framing is optimistic (economies trend toward okay-ness). How does that hold up against structural inequality and climate risk?" — the second is directly related to the new Scanlon vs. Stockman contradiction (see `system/contradictions.md` row 2026-06-04). Answering these would produce 1–2 new concept pages and partially address the economic-indicators contradiction. | medium | open |
