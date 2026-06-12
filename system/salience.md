---
title: "Salience Digest"
date: 2026-06-12
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

**2026-06-12** — Full dream-cycle pass (nightly). 90 wiki pages analyzed (56 concepts, 15 topics, 19 people). Vault unchanged since 2026-06-07 (no new pages, no new content added since weekly pass). Inbound-link counts re-verified via exact-string grep (`[[slug]]` and `[[slug|` patterns, unique-file, excluding self-references) across all wiki/ files. **Stage 1:** 0 new contradictions; 8 total open contradictions confirmed. Reads covered 14 under-examined pages: glucose-curves, contemporary-romanticized-illnesses, ethics-of-private-beauty, stockman-2008-critique, negotiating-slow-productivity, mapping-the-jagged-frontier, adolescent-development-in-the-digital-age, developmental-strands, latticework-failure-modes, latticework-feedback-loops-outside-investing, stoicism-and-systemic-injustice, stoic-truth-telling-and-tact, compulsive-collecting, bubble-finance — all internally consistent. Notable: `mapping-the-jagged-frontier` explicitly states "Senior practitioners can map aggressively and delegate broadly — the underlying judgment is already built and can catch AI errors," aligning with `cognitive-atrophy-and-ai`'s expert-exemption position (reinforcing, not resolving, the existing open contradiction with `slow-productivity-and-ai-craft`). **Stage 2:** No new near-duplicate cases; Cases 1, 2 (15 confirmed instances), and 3 carry forward unchanged. **Stage 3:** One count correction: `mental-models` corrects from **20 to 18** (prior runs overcounted by using `[[mental-models` prefix grep, which also matched pages linking to `[[mental-models-and-multidisciplinary-thinking]]`; exact-string grep on `[[mental-models]]` yields 18 unique inbound files). This moves `mental-models` from tied #1 (with `disposition-vs-knowledge`) to sole #2. `disposition-vs-knowledge` becomes sole #1 (20 inbound, confirmed). All other counts stable.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | **18** | ~350 | **#1 enrichment priority in the vault** (by enrichment-leverage: high centrality, thin body). 18 inbound links (corrected from over-reported 20). Referenced by every major cluster (Munger, Stoicism, AI, education, forecasting). Body remains a thin properties list + model table. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence (see `munger-vs-behavioral-economics`), cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | 16 | ~400 | **3rd-most-linked page in the vault.** Body remains thin relative to centrality. One inline open-question answer (health-equity-without-redistribution) now duplicates the concept page; the parent page body itself could still be enriched with social-determinants framework depth and global health financing. |
| `jagged-frontier` | **10** | ~300 | Anchor concept for the AI cluster; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`, `ai-productivity-gains-distribution`, `general-purpose-technology`, `ethan-mollick`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | **11** | ~350 | Central person page for the Munger/latticework cluster. Body is a short biography + key contributions list — well below what centrality warrants. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`, `munger-vs-behavioral-economics`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share a creation band of 2026-05-18 to 2026-06-07 (5–25 days old). Staleness does not yet differentiate meaningfully within this vault; pages are recent. Re-run this section after the next enrichment pass.

**Exception — uningested raw articles (aging gap):** Two PDF files in `raw/articles/` remain uningested:
- `raw/articles/charlie munger - mental models Part 1.pdf`
- `raw/articles/charlie munger mental Models Part 2.pdf`

High-probability transcripts of Munger's 1994 USC "Elementary Worldly Wisdom" talk or related primary writings. Pages `mental-models`, `latticework-pedagogy`, `munger-disposition-formation`, and `mental-models-and-multidisciplinary-thinking` have been built from *Poor Charlie's Almanack* (epub) and secondary references; these PDFs may contain primary material not yet captured. Both have been in the ingest queue since 2026-06-02 at high priority.

---

## Near-duplicate flags (Stage 2)
_Owner approval required before any merge or trim._

### Case 1 · `ai-tutoring` / `ai-tutoring-and-human-motivation` — Overlapping opening sections
Both pages open with an independent Bloom's 2 Sigma exposition and a description of Khanmigo's Socratic design. `ai-tutoring-and-human-motivation`'s first section ("The Bloomian Promise…") covers Infinite Patience, Perfect Adaptability, Socratic Inquiry, and Low-Stakes Failure — substantially repeating `ai-tutoring`'s Design Principles section before diverging into the relational/motivation analysis. Estimated overlap: ~25% of `ai-tutoring-and-human-motivation`'s body.

**Proposed:** Trim `ai-tutoring-and-human-motivation`'s opening to a 2-sentence cross-reference to `ai-tutoring`, then pick up with the relational-gap analysis. Owner approval required.

### Case 2 · Structural pattern: inline answers duplicated in concept pages
When open questions were answered and extracted into dedicated concept pages, the originals were not trimmed. **15 confirmed cases.** Owner approval required for each compression individually.

| Page | Duplicated in concept page | Estimated inline word count |
|---|---|---|
| `experimental-mindset` (open-Q on experiment theater) | `experiment-theater` | ~350 |
| `adaptive-leadership` (open-Q on psychological safety) | `adaptive-leadership-and-psychological-safety` | ~300 |
| `stoic-justice` (open-Q on systemic injustice) | `stoicism-and-systemic-injustice` + `stoic-truth-telling-and-tact` | ~450 combined |
| `the-one-thing` (open-Q on tunnel vision) | `focus-vs-orientation` | ~400 |
| `living-and-working-with-ai` (open-Q on cognitive atrophy) | `cognitive-atrophy-and-ai` | ~300 |
| `disposition-vs-knowledge` (open-Q on wisdom traditions) | `wisdom-traditions-practice-vs-doctrine` | ~350 |
| `health-equity` (open-Q on IP and health equity) | `intellectual-property-and-health-equity` | ~150 |
| `experimental-mindset` (open-Q on financial stability) | `financial-stability-while-experimenting` | ~200 |
| `experimental-mindset` (open-Q on privilege) | `experimental-mindset-and-privilege` | ~150 |
| `living-and-working-with-ai` (open-Q on AI productivity gains) | `ai-productivity-gains-distribution` | ~200 |
| `adaptive-leadership` (open-Q on adaptive challenge diagnosis) | `adaptive-challenge-diagnosis` | ~150 |
| `mental-models-and-multidisciplinary-thinking` (open-Q on Munger vs. behavioral economics) | `munger-vs-behavioral-economics` | ~150 |
| `health-equity` (open-Q on redistribution) | `health-equity-without-redistribution` | ~200 |
| `economic-literacy` (open-Q on literacy at scale) | `economic-literacy-at-scale` | ~150 |
| `economic-literacy` (open-Q on Scanlon's optimism limits) | `scanlon-optimism-limits` | ~200 |

**Proposed for each confirmed case:** Compress the inline answer to a 1–2 sentence summary + wikilink to the concept page.

### Case 3 · `slow-productivity-and-ai-craft` / `cognitive-atrophy-and-ai` — Mechanism section overlap *(flagged 2026-06-07)*
~35% body overlap in "The Atrophy Mechanism" section, "Where AI Actually Helps" table, and core heuristic. Proposed: compress mechanism section to 2-sentence cross-reference + `[[cognitive-atrophy-and-ai]]` link; collapse the parallel table; retain only Newport-specific content (three-principle vulnerability analysis and flywheel argument). Owner approval required before trimming.

---

## Surfacing for the dashboard
_Top 10+ pages by salience score (inbound edges × body depth bonus; feeds `wiki-dashboard.html` node sizing)._

Inbound-link counts re-verified via exact-string grep (unique files, excluding self-references). Vault stable at 90 pages. **One count correction this run: `mental-models` corrects from 20 to 18** (prior overcounting via prefix-match grep; exact `[[mental-models]]` search yields 18). `disposition-vs-knowledge` is now sole #1 (20). `mental-models` moves to sole #2 (18).

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| **1** | `disposition-vs-knowledge` | **20** | ~900 words | **Sole #1** (corrected — `mental-models` drops to 18). Crown jewel: richest body among top-10; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. |
| **2** | `mental-models` | **18** | ~350 words | **Sole #2** (corrected from 20 — prior prefix-grep overcounting). Still the **#1 enrichment target in the vault** by thin-body/high-centrality metric. |
| 3 | `health-equity` | 16 | ~400 words | Body thin relative to centrality; primary enrichment target in the health/justice cluster. Open contradiction with `pandemic-lessons-from-tb` remains. |
| 4 | `cognitive-atrophy-and-ai` | 13 | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| **5** | `mental-models-and-multidisciplinary-thinking` | **12** | ~1500 words (topic) | Well-developed topic page. |
| 6 (tied) | `charlie-munger` | 11 | ~350 words | Central person page; body unexpectedly thin for centrality — enrichment candidate. |
| 6 (tied) | `slow-productivity` | 11 | ~800+ words (topic) | Central productivity hub; topic page substantive. |
| 8 (tied) | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; contradiction with `mathematics-education` remains open. |
| 8 (tied) | `jagged-frontier` | **10** | ~300 words | Very thin body vs. centrality — **#2 AI-cluster enrichment priority**. |
| 8 (tied) | `latticework-pedagogy` | 10 | ~1000 words | Well-developed; bridges Munger cluster with behavioral science. |
| 8 (tied) | `tuberculosis-and-global-health` | **10** | ~1100 words (topic) | Well-developed topic page. Central node in the health/justice cluster; bridges romanticization-of-illness, health-equity, pandemic-lessons-from-tb, and IP/health-equity pages. |
| 12 (tied) | `experimental-mindset` | 9 | ~1200 words (topic) | High centrality, well-developed. Open questions now all answered. |
| 12 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |
| 12 (tied) | `living-and-working-with-ai` | 9 | ~1500+ words (topic) | High centrality, well-developed. |
| 15 (tied) | `tiny-experiments` | 8 | ~450 words | Adequately developed for its centrality. |
| 17 (tied) | `stoic-virtues` | 7 | ~500 words | Adequately developed; open contradiction with `wisdom-traditions-practice-vs-doctrine` remains. |
| 17 (tied) | `superforecasting` | 7 | ~900 words | Well-developed; open contradiction with `munger-vs-behavioral-economics` remains. |

_Note: New concept pages from the 2026-06-07 weekly pass (health-equity-without-redistribution, economic-literacy-at-scale, scanlon-optimism-limits, munger-vs-behavioral-economics, financial-stability-while-experimenting, experimental-mindset-and-privilege, ai-productivity-gains-distribution, adaptive-challenge-diagnosis) all have 1–4 inbound links and will accumulate over time._

---

## Newly surfaced this run

**0 new contradictions (Stage 1):**

No new contradictions detected after reads of 14 under-examined pages across four clusters: glucose/metabolic health (glucose-curves); illness narrative (contemporary-romanticized-illnesses); art/aesthetics (ethics-of-private-beauty, compulsive-collecting); economics (stockman-2008-critique, bubble-finance); productivity (negotiating-slow-productivity); AI/work (mapping-the-jagged-frontier); adolescent development (adolescent-development-in-the-digital-age, developmental-strands); Munger/latticework (latticework-failure-modes, latticework-feedback-loops-outside-investing); Stoicism (stoicism-and-systemic-injustice, stoic-truth-telling-and-tact). All internally consistent.

Notable structural observation: `mapping-the-jagged-frontier` states "Senior practitioners can map aggressively and delegate broadly — the underlying judgment is already built and can catch AI errors." This is a third page (after `cognitive-atrophy-and-ai` and `mapping-the-jagged-frontier`) explicitly aligning with the expert-exemption position against `slow-productivity-and-ai-craft`'s "even experts need ongoing productive struggle" claim. The existing open contradiction (logged 2026-06-02) holds; this is a reinforcing observation, not a new contradiction. Total open contradictions: **8** (unchanged).

**0 new near-duplicate cases (Stage 2):**

Cases 1, 2 (15 confirmed), and 3 carry forward unchanged. All pending owner approval.

**1 count correction (Stage 3):**

`mental-models` corrects from **20 to 18** — prior runs used a `[[mental-models` prefix grep that incorrectly matched pages containing `[[mental-models-and-multidisciplinary-thinking]]` links (specifically `munger-disposition-formation.md` and `ryan-holiday.md`; confirmed to link only to the topic page, not the concept page). Exact-string grep on `[[mental-models]]` and `[[mental-models|` yields 18 unique inbound files. The 2026-06-09 "correction" from 18 to 20 was itself an overcounting artifact. `mental-models` moves from tied #1 to sole #2; `disposition-vs-knowledge` is now sole #1 (20 inbound, confirmed). All other counts stable.
