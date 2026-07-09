---
title: "Salience Digest"
date: 2026-07-09
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

**2026-07-09** — Full dream-cycle pass (nightly). 91 wiki pages analyzed (57 concepts, 15 topics, 19 people). Vault unchanged since 2026-06-14 weekly pass. **Stage 1:** 0 new contradictions; 8 total open contradictions confirmed. Pages scanned this run: 8 pages across economics (economic-literacy, crony-capitalism-and-monetary-deformation, kyla-scanlon), health (pandemic-lessons-from-tb, tuberculosis-and-global-health), AI education (ai-in-education), forecasting/Munger (superforecasting), and Stoicism (stoic-virtues) clusters. Five existing contradictions confirmed live from direct reads: (2) `ai-in-education` states "AI can emulate relational scaffolding and lower social pressure for low-stakes failure" while `ai-tutoring-and-human-motivation` states "students eventually detect this simulation, which can lead to a flattening of motivation over time" — tension confirmed unchanged; (3) `stoic-virtues` opens "not a feeling or disposition but a practice" confirmed, consistent with existing registered tension vs. `wisdom-traditions-practice-vs-doctrine`'s dispositional framing; (4) `economic-literacy` treats hard indicators as genuine baseline ("Hard data: unemployment low, GDP growing"), `crony-capitalism-and-monetary-deformation` argues the same indicators are distorted by bubble finance — tension confirmed unchanged; (6) `superforecasting` frames fox/hedgehog distinction as "effectively an empirical validation of Munger's latticework intuition" confirmed, consistent with existing tension vs. `munger-vs-behavioral-economics`; (8) `pandemic-lessons-from-tb` Lesson 4 states "TB's history suggests no [health equity achievable without redistribution] — access to drugs is downstream of access to resources" confirmed, consistent with existing tension vs. `health-equity-without-redistribution`. No new candidates emerged. Total open contradictions: **8** (unchanged). **Stage 2:** 0 new near-duplicate cases. Vault stable at 91 pages since 2026-06-14. Case 2 #17 (tuberculosis-and-global-health inline pandemic-lessons answer vs. pandemic-lessons-from-tb) confirmed from direct read: TB topic page contains detailed 5-lesson inline answer (~300 words) that substantially duplicates primary content of pandemic-lessons-from-tb. All cases carry forward unchanged; all pending owner approval. **Stage 3:** 1 count correction. `experimental-mindset` corrected from 10 to **9** (prefix-methodology false positive). Investigation: `health-equity.md` contains `[[experimental-mindset-and-privilege]]` in its `related:` field, not `[[experimental-mindset]]`; prefix grep `[[experimental-mindset` captures this file as a false positive. The 2026-07-02 "correction" to 10 computed the prior base count (9) using prefix grep, which included health-equity.md as a false positive; when adaptive-vs-technical-challenges.md was discovered as a genuine new link (+1), the total was logged as 10. The true correction from 2026-07-02 was: base 8 genuine links (not 9) + adaptive-vs-technical-challenges.md = 9 exact links. Today's exact-string verification via `\[\[experimental-mindset\]\]` returns 9 files (adaptive-leadership, experimental-mindset-and-privilege, financial-stability-while-experimenting, experiment-theater, growth-mindset, tiny-experiments, disposition-vs-knowledge, adaptive-vs-technical-challenges, anne-laure-le-cunff) and excludes health-equity.md (which links only to `[[experimental-mindset-and-privilege]]`). Rank change: `experimental-mindset` drops from rank 8 (tied at 10 with growth-mindset, jagged-frontier, latticework-pedagogy, tuberculosis-and-global-health) to **rank 13 (tied at 9 with large-language-models and living-and-working-with-ai)**. All other 16 counts confirmed stable. Full re-verification: disposition-vs-knowledge (20 ✓), mental-models (18 ✓), health-equity (17 ✓), cognitive-atrophy-and-ai (14 ✓), mental-models-and-multidisciplinary-thinking (12 ✓), charlie-munger (11 ✓), slow-productivity (11 ✓), growth-mindset (10 ✓), jagged-frontier (10 ✓), latticework-pedagogy (10 ✓), tuberculosis-and-global-health (10 ✓), experimental-mindset (9 — corrected from 10), large-language-models (9 ✓), living-and-working-with-ai (9 ✓), tiny-experiments (8 ✓), stoic-virtues (7 ✓), superforecasting (7 ✓).

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | **18** *(corrected from 20 — prior prefix-methodology error; true exact-string count)* | ~350 | **#2 most-linked page in the vault** (displaced from co-#1 by methodology correction; disposition-vs-knowledge is now sole #1 at 20). Still the **#1 enrichment priority by thin-body/high-centrality metric**. Referenced by every major cluster (Munger, Stoicism, AI, education, forecasting, adaptive leadership, productivity). Body remains a thin properties list + model table. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence (see `munger-vs-behavioral-economics`), cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | **17** | ~400 | **3rd-most-linked page in the vault**. Body remains thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| `jagged-frontier` | **10** | ~300 | Anchor concept for the AI cluster; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`, `ai-productivity-gains-distribution`, `general-purpose-technology`, `ethan-mollick`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | **11** | ~350 | Central person page for the Munger/latticework cluster. Body is a short biography + key contributions list — well below what centrality warrants. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`, `munger-vs-behavioral-economics`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share a creation band of 2026-05-18 to 2026-06-14 (24–51 days old). Staleness does not yet differentiate meaningfully within this vault; pages are recent. Re-run this section after the next enrichment pass.

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

Inbound-link counts re-verified via exact-string ripgrep (excludes self-reference, avoids prefix false positives). Vault at 91 pages. **1 count correction this run:** `experimental-mindset` corrected to 9 (was erroneously reported as 10 since 2026-07-02 due to prefix-methodology overcounting; health-equity.md links to `[[experimental-mindset-and-privilege]]`, not `[[experimental-mindset]]`).

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| **1** | `disposition-vs-knowledge` | **20** | ~900 words | Crown jewel: richest body among top-10; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. Sole #1. |
| **2** | `mental-models` | **18** *(corrected from 20 in 2026-07-08 run — prefix-methodology error)* | ~350 words | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Two Munger PDFs in raw/ are the primary source. |
| **3** | `health-equity` | **17** | ~400 words | Body thin relative to centrality; primary enrichment target in the health/justice cluster. Open contradiction with `pandemic-lessons-from-tb` remains. |
| **4** | `cognitive-atrophy-and-ai` | **14** | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| **5** | `mental-models-and-multidisciplinary-thinking` | **12** | ~1500 words (topic) | Well-developed topic page. |
| 6 (tied) | `charlie-munger` | 11 | ~350 words | Central person page; body unexpectedly thin for centrality — enrichment candidate. |
| 6 (tied) | `slow-productivity` | 11 | ~800+ words (topic) | Central productivity hub; topic page substantive. |
| 8 (tied) | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; contradiction with `mathematics-education` remains open. |
| 8 (tied) | `jagged-frontier` | **10** | ~300 words | Very thin body vs. centrality — **#2 AI-cluster enrichment priority**. |
| 8 (tied) | `latticework-pedagogy` | 10 | ~1000 words | Well-developed; bridges Munger cluster with behavioral science. |
| 8 (tied) | `tuberculosis-and-global-health` | **10** | ~1100 words (topic) | Well-developed topic page. Central node in the health/justice cluster. Case 2 instance #17 pending: ~300-word inline pandemic-lessons answer duplicates `pandemic-lessons-from-tb`. |
| 13 (tied) | `experimental-mindset` | **9** *(corrected from 10 — prefix-methodology false positive in 2026-07-02 run; health-equity.md links to `[[experimental-mindset-and-privilege]]` only)* | ~1200 words (topic) | High centrality, well-developed. Open questions now all answered. Rank drops from 8 (tied at 10) to 13 (tied at 9). |
| 13 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |
| 13 (tied) | `living-and-working-with-ai` | 9 | ~1500+ words (topic) | High centrality, well-developed. |
| 16 | `tiny-experiments` | 8 | ~450 words | Adequately developed for its centrality. |
| 17 (tied) | `stoic-virtues` | 7 | ~500 words | Adequately developed; open contradiction with `wisdom-traditions-practice-vs-doctrine` remains. |
| 17 (tied) | `superforecasting` | 7 | ~900 words | Well-developed; open contradiction with `munger-vs-behavioral-economics` remains. |

_Note: `social-media-and-illness-aesthetics` (created 2026-06-14) has 1 confirmed inbound link (`romanticization-of-illness`). Will accumulate links over time. Near-duplicate alert (Case 2, #16): its creation left a ~250-word duplicate in `contemporary-romanticized-illnesses` pending owner approval for compression._

---

## Newly surfaced this run

**0 new contradictions (Stage 1):**

Eight pages scanned across economics (economic-literacy, crony-capitalism-and-monetary-deformation, kyla-scanlon), health (pandemic-lessons-from-tb, tuberculosis-and-global-health), AI education (ai-in-education), forecasting/Munger (superforecasting), and Stoicism (stoic-virtues) clusters. No new contradiction candidates emerged. Five existing contradictions confirmed live from direct reads: contradiction #2 (ai-in-education vs. ai-tutoring-and-human-motivation — AI relational scaffolding claim vs. eventual student detection and motivation flattening); contradiction #3 (stoic-virtues opening claim "not a feeling or disposition but a practice" confirmed unchanged); contradiction #4 (economic-literacy uses hard indicators as baseline for vibecession analysis; crony-capitalism-and-monetary-deformation argues those same indicators are distorted by bubble finance); contradiction #6 (superforecasting frames fox/hedgehog finding as "empirical validation of Munger's latticework intuition" — confirmed in tension with munger-vs-behavioral-economics); contradiction #8 (pandemic-lessons-from-tb Lesson 4 states TB history "suggests no" on health equity without redistribution — confirmed in tension with health-equity-without-redistribution). Total open contradictions: **8** (unchanged).

**0 new near-duplicate cases (Stage 2):**

Vault stable at 91 pages since 2026-06-14. Case 2 instance #17 (tuberculosis-and-global-health inline pandemic-lessons answer vs. pandemic-lessons-from-tb) confirmed from direct read: the TB topic page contains a detailed 5-lesson inline answer (~300 words) that substantially duplicates pandemic-lessons-from-tb's primary content. Cases 1, 2 (17 confirmed instances), and 3 carry forward unchanged. All pending owner approval.

**1 count correction (Stage 3):**

`experimental-mindset` corrected from 10 to **9** (methodology fix). Prior count of 10 originated in 2026-07-02 run which found adaptive-vs-technical-challenges.md as the "10th" inbound link; however, the base count of "9" used in that correction was inflated by prefix grep which counted health-equity.md as a false positive (`[[experimental-mindset-and-privilege]]` matches the `[[experimental-mindset` prefix). True exact-string count: 9 files (adaptive-leadership, experimental-mindset-and-privilege, financial-stability-while-experimenting, experiment-theater, growth-mindset, tiny-experiments, disposition-vs-knowledge, adaptive-vs-technical-challenges, anne-laure-le-cunff). The 2026-07-02 discovery of adaptive-vs-technical-challenges.md was correct (link is real), but the count correction should have been 8→9 not 9→10. Same false-positive mechanism as the mental-models correction in the 2026-07-08 run. Rank change: `experimental-mindset` drops from rank 8 (tied at 10) to **rank 13 (tied at 9 with large-language-models and living-and-working-with-ai)**. All other 16 inbound-link counts confirmed stable.
