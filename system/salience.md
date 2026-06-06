---
title: "Salience Digest"
date: 2026-06-06
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

**2026-06-06** — Full dream-cycle pass (nightly). 82 wiki pages analyzed (48 concepts, 15 topics, 19 people). No new wiki pages have been added since the 2026-06-05 run. Vault is structurally stable. Inbound-link counts re-verified via ripgrep pattern-match on `[[slug` prefix across all wiki/ files — confirmed unchanged from the 2026-06-04 full scan. **Stage 1:** Zero new contradictions detected; 4 prior contradictions remain open. **Stage 2:** Zero new near-duplicate cases; 8 flagged cases (Case 1 + 7-instance structural pattern) remain pending owner approval. **Stage 3:** Rankings confirmed stable — `mental-models` remains #1 (19 inbound, ~350 words) and the single highest-leverage enrichment target in the vault.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | 19 | ~350 | **#1 enrichment priority in the vault.** Highest inbound count of any page; body remains a thin properties list + model table. Referenced by every major cluster. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence, cross-domain worked examples. |
| `health-equity` | 13 | ~400 | **3rd-most-linked page in the vault.** Body thinner than centrality warrants. One unanswered open question remains ("Is health equity achievable without global wealth redistribution?"). Inline IP-answer near-duplicate case also pending trim. |
| `jagged-frontier` | 9 | ~300 | Anchor concept for all AI pages; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share the same creation band (2026-05-18 to 2026-06-02, now 4–19 days old). Staleness does not yet differentiate meaningfully within this vault; all pages are recent. Re-run this section after the next enrichment pass.

**Exception — uningested raw articles (aging gap):** Two PDF files in `raw/articles/` remain uningested:
- `raw/articles/charlie munger - mental models Part 1.pdf`
- `raw/articles/charlie munger mental Models Part 2.pdf`

These are high-probability transcripts of Munger's 1994 USC "Elementary Worldly Wisdom" talk or related primary writings — the foundational source for the latticework framework. Pages `mental-models`, `latticework-pedagogy`, `munger-disposition-formation`, and `mental-models-and-multidisciplinary-thinking` have been built from *Poor Charlie's Almanack* (epub) and secondary references; these PDFs may contain primary material not yet captured. Both have been in the ingest queue since 2026-06-02 at high priority.

---

## Near-duplicate flags (Stage 2)
_Owner approval required before any merge or trim._

### Case 1 · `ai-tutoring` / `ai-tutoring-and-human-motivation` — Overlapping opening sections
Both pages open with an independent Bloom's 2 Sigma exposition and a description of Khanmigo's Socratic design. `ai-tutoring-and-human-motivation`'s first section ("The Bloomian Promise…") covers Infinite Patience, Perfect Adaptability, Socratic Inquiry, and Low-Stakes Failure — substantially repeating `ai-tutoring`'s Design Principles section before diverging into the relational/motivation analysis. Estimated overlap: ~25% of `ai-tutoring-and-human-motivation`'s body.

**Proposed:** Trim `ai-tutoring-and-human-motivation`'s opening to a 2-sentence cross-reference to `ai-tutoring`, then pick up with the relational-gap analysis. The concept page carries the deeper treatment; the opener should signal the dependency, not re-explain it.

### Case 2 · Structural pattern: inline answers duplicated in concept pages
When open questions were answered and extracted into dedicated concept pages, the originals were not trimmed. **7 cases confirmed (7 prior + 0 new this run).** Owner approval required for each compression individually.

| Page | Duplicated in concept page | Estimated inline word count |
|---|---|---|
| `experimental-mindset` (open-Q on experiment theater) | `experiment-theater` | ~350 |
| `adaptive-leadership` (open-Q on psychological safety) | `adaptive-leadership-and-psychological-safety` | ~300 |
| `stoic-justice` (open-Q on systemic injustice) | `stoicism-and-systemic-injustice` + `stoic-truth-telling-and-tact` | ~450 combined |
| `the-one-thing` (open-Q on tunnel vision) | `focus-vs-orientation` | ~400 |
| `living-and-working-with-ai` (open-Q on cognitive atrophy) | `cognitive-atrophy-and-ai` | ~300 |
| `disposition-vs-knowledge` (open-Q on wisdom traditions) | `wisdom-traditions-practice-vs-doctrine` | ~350 |
| `health-equity` (open-Q on IP and health equity) | `intellectual-property-and-health-equity` | ~150 |

**Proposed for each:** Compress the inline answer to a 1–2 sentence summary + wikilink to the concept page. The concept page becomes canonical; the page retains the question header and a brief pointer.

---

## Surfacing for the dashboard
_Top 10 pages by salience score (inbound edges × body depth bonus; feeds `wiki-dashboard.html` node sizing)._

Inbound-link counts re-verified via ripgrep; no changes from 2026-06-04 full scan. No new pages added since 2026-06-04.

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| 1 | `mental-models` | 19 | ~350 words | **Highest centrality in vault** — thin body makes it the single highest-leverage enrichment target. |
| 2 | `disposition-vs-knowledge` | 17 | ~900 words | Crown jewel — most-linked concept after `mental-models`; richest body; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. |
| 3 | `health-equity` | 13 | ~400 words | 3rd-most-linked page; body thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| 4 | `cognitive-atrophy-and-ai` | 12 | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| 5 | `mental-models-and-multidisciplinary-thinking` | 11 | ~1500 words (topic) | Well-developed topic page; centrality is high but body likely adequate. |
| 6 | `slow-productivity` | 10 | ~800+ words (topic) | Central productivity hub; topic page likely substantive. |
| 7 | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; could be enriched with replications debate and structural-support nuance. |
| 8 | `charlie-munger` | 10 | unknown | Central person page; check body depth on next enrichment pass. |
| 9 | `jagged-frontier` | 9 | ~300 words | Very thin body vs. high centrality — **#2 enrichment priority** behind `mental-models`. |
| 10 | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level; effectively tied with `jagged-frontier` as a top AI-cluster enrichment target. |

_Note: `tuberculosis-and-global-health` (9 inbound, topic page, ~1000+ words) and `latticework-pedagogy` (9 inbound) also sit at rank 9–10 but are well-developed. The thin-body targets — `jagged-frontier` and `large-language-models` — are the higher-leverage enrichment bets._

---

## Newly surfaced this run

**No new contradictions (Stage 1):** All 4 prior contradictions confirmed still open. Targeted scan of six under-examined clusters (glucose, superforecasting/latticework, growth-mindset/math, disposition, adolescent development, Stockman critique) found no new conflicting claims. No contradiction to record. Contradiction pairs remain: (1) `cognitive-atrophy-and-ai` vs. `slow-productivity-and-ai-craft` on expertise exemption from atrophy risk; (2) `ai-in-education` vs. `ai-tutoring-and-human-motivation` on whether AI relational emulation works; (3) `stoic-virtues` vs. `wisdom-traditions-practice-vs-doctrine` on virtue as action vs. disposition-builder; (4) `vibecession`/`economic-literacy` vs. `bubble-finance`/`crony-capitalism-and-monetary-deformation` on whether hard economic indicators are reliable baselines or distorted signals.

**No new near-duplicate cases (Stage 2):** All 8 prior cases confirmed still open. No new structural overlap detected.

**Salience rankings stable (Stage 3):** Inbound-link counts re-verified via ripgrep; confirmed unchanged for all top pages. `mental-models` remains #1 (19 inbound) and the primary enrichment target. `latticework-pedagogy` also confirmed at 9 inbound (same tier as `jagged-frontier`, `large-language-models`, `tuberculosis-and-global-health`). Next highest-leverage action: ingest the two Munger PDFs in `raw/articles/` to potentially enrich the vault's most-linked concept page.
