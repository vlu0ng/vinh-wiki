---
title: "Salience Digest"
date: 2026-07-16
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

**2026-07-16** — Full dream-cycle pass (nightly). 91 wiki pages; vault unchanged since 2026-06-14 weekly pass (1-day gap since last logged run on 2026-07-15). **Stage 1:** 0 new contradictions; 8 total open contradictions confirmed. Pages scanned this run: 8 pages across foundational concepts (disposition-vs-knowledge, inversion), adaptive leadership (ronald-heifetz, adaptive-challenge-diagnosis), Munger/Buffett (warren-buffett, latticework-feedback-loops-outside-investing), Stoicism (stoic-justice), and art/obsession (ethics-of-private-beauty) clusters. All pages internally consistent. No new contradiction candidates emerged. Pages verified: (1) disposition-vs-knowledge and adaptive-challenge-diagnosis are consistent — both agree the knowledge-disposition gap is real and that adaptive challenge diagnosis is dispositional; they operate at theory vs. application level with no tension. (2) latticework-feedback-loops-outside-investing explicitly acknowledges superforecasting's limit ("tournament practice builds calibration, not full far-transfer"), consistent with existing contradiction #6's scope (superforecasting vs. munger-vs-behavioral-economics). (3) stoic-justice's inline answer on systemic injustice states "the framework scales inadequately without supplementation" — consistent with stoicism-and-systemic-injustice; existing contradiction #3 (stoic-virtues vs. wisdom-traditions-practice-vs-doctrine) remains the relevant Stoicism tension. (4) ethics-of-private-beauty is a well-scoped page on cultural stewardship vs. private aesthetic experience, consistent with compulsive-collecting and art-theft-and-obsession. Total open contradictions: **8** (unchanged). **Stage 2:** 0 new near-duplicate cases. Vault stable at 91 pages since 2026-06-14. Today's pages are well-scoped: ronald-heifetz and warren-buffett are compact person pages; latticework-feedback-loops-outside-investing is distinctly focused on the non-investing feedback problem; stoic-justice is the source topic page with its answer pages properly factored out. All three cases carry forward unchanged; all pending owner approval. **Stage 3:** 0 count corrections. Full verification of all 17 tracked inbound-link counts: disposition-vs-knowledge (20 ✓ — exact-string), mental-models (18 ✓ — exact-string), health-equity (17 ✓ — exact-string), cognitive-atrophy-and-ai (14 ✓ — exact-string), mental-models-and-multidisciplinary-thinking (12 ✓ — 11 exact + 1 piped in disposition-building-practices.md via `[[mental-models-and-multidisciplinary-thinking|Munger]]`), charlie-munger (11 ✓ — 10 exact + 1 piped in latticework-feedback-loops-outside-investing.md, confirmed by reading the page this run), slow-productivity (11 ✓ — exact-string), growth-mindset (10 ✓ — exact-string), jagged-frontier (10 ✓ — 9 exact + 1 piped in ai-tutoring-and-human-motivation.md), latticework-pedagogy (10 ✓ — exact-string), tuberculosis-and-global-health (10 ✓ — exact-string), experimental-mindset (9 ✓ — exact-string), large-language-models (9 ✓ — exact-string), living-and-working-with-ai (9 ✓ — exact-string), tiny-experiments (8 ✓ — exact-string), stoic-virtues (7 ✓ — exact-string), superforecasting (7 ✓ — exact-string). No rank changes.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | **18** | ~350 | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Referenced by every major cluster (Munger, Stoicism, AI, education, forecasting, adaptive leadership, productivity). Body remains a thin properties list + model table. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence (see `munger-vs-behavioral-economics`), cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | **17** | ~400 | **3rd-most-linked page in the vault**. Body remains thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| `jagged-frontier` | **10** | ~300 | Anchor concept for the AI cluster; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`, `ai-productivity-gains-distribution`, `general-purpose-technology`, `ethan-mollick`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | **11** *(10 exact + 1 piped in latticework-feedback-loops-outside-investing.md; confirmed via direct read this run)* | ~350 | Central person page for the Munger/latticework cluster. Body is a short biography + key contributions list — well below what centrality warrants. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`, `munger-vs-behavioral-economics`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share a creation band of 2026-05-18 to 2026-06-14 (32–58 days old as of 2026-07-16). Staleness does not yet differentiate meaningfully within this vault; pages are recent. Re-run this section after the next enrichment pass.

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
When open questions were answered and extracted into dedicated concept pages, the originals were not trimmed. **17 confirmed cases** (unchanged). Owner approval required for each compression individually.

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
| `contemporary-romanticized-illnesses` ("How Social Media Changes the Pattern" section) | `social-media-and-illness-aesthetics` | ~250 |
| `tuberculosis-and-global-health` (open-Q on pandemic lessons) | `pandemic-lessons-from-tb` | ~300 |

**Proposed for each confirmed case:** Compress the inline answer to a 1–2 sentence summary + wikilink to the concept page.

### Case 3 · `slow-productivity-and-ai-craft` / `cognitive-atrophy-and-ai` — Mechanism section overlap *(flagged 2026-06-07)*
~35% body overlap in "The Atrophy Mechanism" section, "Where AI Actually Helps" table, and core heuristic. Note from 2026-06-19 run: these two pages also show a minor classification divergence — `cognitive-atrophy-and-ai` labels "generating initial drafts then substantially revising" as "Low" atrophy risk; `slow-productivity-and-ai-craft` labels the same use as "Medium — depends on whether revision builds judgment." This nuance is part of the Case 3 overlap pattern. Proposed: compress mechanism section to 2-sentence cross-reference + `[[cognitive-atrophy-and-ai]]` link; collapse the parallel table; retain only Newport-specific content (three-principle vulnerability analysis and flywheel argument). Owner approval required before trimming.

---

## Surfacing for the dashboard
_Top 10+ pages by salience score (inbound edges × body depth bonus; feeds `wiki-dashboard.html` node sizing)._

Inbound-link counts verified via exact-string and prefix ripgrep (excludes self-reference, captures piped wikilinks). Vault at 91 pages. **0 count corrections this run.** charlie-munger confirmed at 11 (10 exact + 1 piped in latticework-feedback-loops-outside-investing.md — read directly this run); jagged-frontier confirmed at 10 (9 exact + 1 piped — ai-tutoring-and-human-motivation.md); health-equity confirmed at 17 (exact-string); mental-models-and-multidisciplinary-thinking confirmed at 12 (11 exact + 1 piped — disposition-building-practices.md via `[[mental-models-and-multidisciplinary-thinking|Munger]]`).

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| **1** | `disposition-vs-knowledge` | **20** | ~900 words | Crown jewel: richest body among top-10; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. Sole #1. |
| **2** | `mental-models` | **18** | ~350 words | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Two Munger PDFs in raw/ are the primary source. |
| **3** | `health-equity` | **17** | ~400 words | Body thin relative to centrality; primary enrichment target in the health/justice cluster. Open contradiction with `pandemic-lessons-from-tb` remains. |
| **4** | `cognitive-atrophy-and-ai` | **14** | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| **5** | `mental-models-and-multidisciplinary-thinking` | **12** *(11 exact + 1 piped; confirmed)* | ~1500 words (topic) | Well-developed topic page. |
| 6 (tied) | `charlie-munger` | 11 *(10 exact + 1 piped; confirmed this run)* | ~350 words | Central person page; body unexpectedly thin for centrality — enrichment candidate. |
| 6 (tied) | `slow-productivity` | 11 | ~800+ words (topic) | Central productivity hub; topic page substantive. |
| 8 (tied) | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; contradiction with `mathematics-education` remains open. |
| 8 (tied) | `jagged-frontier` | **10** *(9 exact + 1 piped; confirmed)* | ~300 words | Very thin body vs. centrality — **#2 AI-cluster enrichment priority**. |
| 8 (tied) | `latticework-pedagogy` | 10 | ~1000 words | Well-developed; bridges Munger cluster with behavioral science. |
| 8 (tied) | `tuberculosis-and-global-health` | **10** | ~1100 words (topic) | Well-developed topic page. Central node in the health/justice cluster. Case 2 instance #17 pending: ~300-word inline pandemic-lessons answer duplicates `pandemic-lessons-from-tb`. |
| 13 (tied) | `experimental-mindset` | **9** | ~1200 words (topic) | High centrality, well-developed. Open questions now all answered. |
| 13 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |
| 13 (tied) | `living-and-working-with-ai` | 9 | ~1500+ words (topic) | High centrality, well-developed. |
| 16 | `tiny-experiments` | 8 | ~450 words | Adequately developed for its centrality. |
| 17 (tied) | `stoic-virtues` | 7 | ~500 words | Adequately developed; open contradiction with `wisdom-traditions-practice-vs-doctrine` remains. |
| 17 (tied) | `superforecasting` | 7 | ~900 words | Well-developed; open contradiction with `munger-vs-behavioral-economics` remains. |

_Note: `social-media-and-illness-aesthetics` (created 2026-06-14) has 1 confirmed inbound link (`romanticization-of-illness`). Will accumulate links over time. Near-duplicate alert (Case 2, #16): its creation left a ~250-word duplicate in `contemporary-romanticized-illnesses` pending owner approval for compression._

---

## Newly surfaced this run

**0 new contradictions (Stage 1):**

Eight pages scanned across foundational concepts (disposition-vs-knowledge, inversion), adaptive leadership (ronald-heifetz, adaptive-challenge-diagnosis), Munger/Buffett (warren-buffett, latticework-feedback-loops-outside-investing), Stoicism (stoic-justice), and art/obsession (ethics-of-private-beauty) clusters. No new contradiction candidates emerged. All pages internally consistent. Notable examinations: (1) disposition-vs-knowledge and adaptive-challenge-diagnosis are consistent — disposition-vs-knowledge provides the theoretical basis (knowledge-disposition gap, Dreyfus expertise progression, character education evidence) while adaptive-challenge-diagnosis is a precise application (the diagnostic skill is itself dispositional, not merely propositional). (2) latticework-feedback-loops-outside-investing and superforecasting — the former explicitly describes the latter's limit as "calibration and aggregation, not full far-transfer," which is compatible with existing contradiction #6 (superforecasting frames Tetlock as validating Munger's latticework; munger-vs-behavioral-economics frames Tetlock as contrasting with Munger). The feedback-loops page takes the complementary view (forecasting tournaments as the best non-investing feedback substitute) without weighing in on the Munger validation vs. contrast question. (3) stoic-justice's systemic-injustice inline answer acknowledges Stoicism's structural limits — consistent with stoicism-and-systemic-injustice; existing contradiction #3 (stoic-virtues vs. wisdom-traditions-practice-vs-doctrine on virtue-as-practice vs. virtue-as-disposition) remains the operative Stoicism tension. (4) ethics-of-private-beauty examines the Kantian disinterestedness claim alongside the cultural stewardship obligation — internally consistent and distinct from compulsive-collecting's psychological lens. Total open contradictions: **8** (unchanged).

**0 new near-duplicate cases (Stage 2):**

Vault stable at 91 pages since 2026-06-14. Today's pages are well-scoped and distinct: ronald-heifetz and warren-buffett are compact biographical pages; adaptive-challenge-diagnosis extends adaptive-leadership with a diagnostic tool (already registered as Case 2 instance #11); latticework-feedback-loops-outside-investing is explicitly scoped to the non-investing domain and complements rather than duplicates disposition-building-practices; stoic-justice is the source topic page whose inline answers are already factored into Case 2 instances #3 and #14. Cases 1, 2 (17 confirmed instances), and 3 carry forward unchanged. All pending owner approval.

**0 count corrections (Stage 3):**

All 17 inbound-link counts verified stable via exact-string ripgrep (full-path exclusions for self-reference). Piped-wikilink counts for charlie-munger (latticework-feedback-loops-outside-investing.md confirmed by direct read this run), jagged-frontier (ai-tutoring-and-human-motivation.md, confirmed in prior runs), and mental-models-and-multidisciplinary-thinking (disposition-building-practices.md, confirmed in prior runs) all carry forward unchanged. No rank changes.
