---
title: "Salience Digest"
date: 2026-07-08
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

**2026-07-08** — Full dream-cycle pass (nightly). 91 wiki pages analyzed (57 concepts, 15 topics, 19 people). Vault unchanged since 2026-06-14 weekly pass. **Stage 1:** 0 new contradictions; 8 total open contradictions confirmed. Pages scanned this run: 8 pages across art/obsession people, focus/productivity, life-design/privilege, and AI/work clusters (stephane-breitwieser, michael-finkel, the-one-thing, focus-vs-orientation, experiment-theater, experimental-mindset-and-privilege, living-and-working-with-ai, financial-stability-while-experimenting). Two candidates examined and resolved as non-contradictory: (1) `experiment-theater` (perpetual exploration as fear-driven avoidance of commitment) vs. `experimental-mindset-and-privilege` (material scarcity compressing risk tolerance) — resolved as complementary: different obstacle types (psychological vs. structural) that coexist without contradiction; experiment-theater addresses the emotional avoidance mechanism, experimental-mindset-and-privilege addresses material constraints. (2) `living-and-working-with-ai` Rule 1 ("always invite AI to the table") vs. `cognitive-atrophy-and-ai`'s novice atrophy risk — resolved as non-contradictory: the living-and-working-with-ai page's inline answer to the cognitive-atrophy open question explicitly prescribes "periodically work without AI in core domains," which is compatible with the atrophy framework; existing contradiction #1 (cognitive-atrophy-and-ai vs. slow-productivity-and-ai-craft) already captures the expert-exemption debate at the deeper level. Total open contradictions: **8** (unchanged). **Stage 2:** 0 new near-duplicate cases. All confirmed instances in pages scanned today were already documented: the-one-thing/focus-vs-orientation overlap (Case 2 #4 ✓), experiment-theater/experimental-mindset (Case 2 #1 ✓), experimental-mindset-and-privilege/experimental-mindset (Case 2 #9 ✓), living-and-working-with-ai cognitive-atrophy answer/cognitive-atrophy-and-ai (Case 2 #5 ✓), living-and-working-with-ai AI-productivity answer/ai-productivity-gains-distribution (Case 2 #10 ✓), financial-stability-while-experimenting/experimental-mindset (Case 2 #8 ✓). Vault stable at 91 pages; Cases 1, 2 (17 confirmed instances), and 3 carry forward. All pending owner approval. **Stage 3:** 1 count correction. `mental-models` corrected from 20 to **18** (prior count was inflated by prefix-methodology error in 2026-07-03 run). Investigation: files containing `[[mental-models` (prefix) = 20; files containing `[[mental-models]]` or `[[mental-models|alias]]` (exact) = 18. The 2 discrepant files are `munger-disposition-formation.md` (links only to `[[mental-models-and-multidisciplinary-thinking]]`; also has "mental-models" as a plain-text tag string — no exact `[[mental-models]]` wikilink) and `ryan-holiday.md` (links only to `[[mental-models-and-multidisciplinary-thinking]]` — no exact `[[mental-models]]` wikilink). The 2026-07-03 "correction" to 20 used prefix grep which captured these false positives; the true correction from that run was +2 exact links (stoic-justice.md and adaptive-challenge-diagnosis.md, both confirmed to have exact `[[mental-models]]` links and both in the 18), but the running total should have been 16→18, not 16→20. Rank change: `mental-models` drops from co-#1 (tied at 20 with disposition-vs-knowledge) to solo **#2** (18 links, between disposition-vs-knowledge at 20 and health-equity at 17). All other 16 counts confirmed stable. Full re-verification: disposition-vs-knowledge (20 ✓), mental-models (18 — corrected from 20), health-equity (17 ✓), cognitive-atrophy-and-ai (14 ✓), mental-models-and-multidisciplinary-thinking (12 ✓), charlie-munger (11 ✓), slow-productivity (11 ✓), growth-mindset (10 ✓), jagged-frontier (10 ✓), latticework-pedagogy (10 ✓), tuberculosis-and-global-health (10 ✓), experimental-mindset (10 ✓), large-language-models (9 ✓), living-and-working-with-ai (9 ✓), tiny-experiments (8 ✓), stoic-virtues (7 ✓), superforecasting (7 ✓).

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

Inbound-link counts re-verified via exact-string ripgrep (excludes self-reference, avoids prefix false positives). Vault at 91 pages. **1 count correction this run:** `mental-models` corrected to 18 (was erroneously reported as 20 since 2026-07-03 due to prefix-methodology overcounting).

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| **1** | `disposition-vs-knowledge` | **20** | ~900 words | Crown jewel: richest body among top-10; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. Sole #1 (mental-models has been corrected to 18). |
| **2** | `mental-models` | **18** *(corrected from 20 — prefix-methodology error in 2026-07-03)* | ~350 words | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Displaced from co-#1 by methodology correction. Two Munger PDFs in raw/ are the primary source. |
| **3** | `health-equity` | **17** | ~400 words | Body thin relative to centrality; primary enrichment target in the health/justice cluster. Open contradiction with `pandemic-lessons-from-tb` remains. |
| **4** | `cognitive-atrophy-and-ai` | **14** | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| **5** | `mental-models-and-multidisciplinary-thinking` | **12** | ~1500 words (topic) | Well-developed topic page. |
| 6 (tied) | `charlie-munger` | 11 | ~350 words | Central person page; body unexpectedly thin for centrality — enrichment candidate. |
| 6 (tied) | `slow-productivity` | 11 | ~800+ words (topic) | Central productivity hub; topic page substantive. |
| 8 (tied) | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; contradiction with `mathematics-education` remains open. |
| 8 (tied) | `jagged-frontier` | **10** | ~300 words | Very thin body vs. centrality — **#2 AI-cluster enrichment priority**. |
| 8 (tied) | `latticework-pedagogy` | 10 | ~1000 words | Well-developed; bridges Munger cluster with behavioral science. |
| 8 (tied) | `tuberculosis-and-global-health` | **10** | ~1100 words (topic) | Well-developed topic page. Central node in the health/justice cluster. Case 2 instance #17 pending: ~300-word inline pandemic-lessons answer duplicates `pandemic-lessons-from-tb`. |
| 8 (tied) | `experimental-mindset` | **10** | ~1200 words (topic) | High centrality, well-developed. Open questions now all answered. |
| 13 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |
| 13 (tied) | `living-and-working-with-ai` | 9 | ~1500+ words (topic) | High centrality, well-developed. |
| 15 | `tiny-experiments` | 8 | ~450 words | Adequately developed for its centrality. |
| 16 (tied) | `stoic-virtues` | 7 | ~500 words | Adequately developed; open contradiction with `wisdom-traditions-practice-vs-doctrine` remains. |
| 16 (tied) | `superforecasting` | 7 | ~900 words | Well-developed; open contradiction with `munger-vs-behavioral-economics` remains. |

_Note: `social-media-and-illness-aesthetics` (created 2026-06-14) has 1 confirmed inbound link (`romanticization-of-illness`). Will accumulate links over time. Near-duplicate alert (Case 2, #16): its creation left a ~250-word duplicate in `contemporary-romanticized-illnesses` pending owner approval for compression._

---

## Newly surfaced this run

**0 new contradictions (Stage 1):**

Eight pages scanned across art/obsession people, focus/productivity, life-design/privilege, and AI/work clusters (stephane-breitwieser, michael-finkel, the-one-thing, focus-vs-orientation, experiment-theater, experimental-mindset-and-privilege, living-and-working-with-ai, financial-stability-while-experimenting). Two candidates examined and resolved as non-contradictory: (1) `experiment-theater` psychological-avoidance mechanism vs. `experimental-mindset-and-privilege` structural-scarcity constraint — complementary obstacle types, not contradictory; both can coexist. (2) `living-and-working-with-ai` Rule 1 ("always invite AI to the table") vs. `cognitive-atrophy-and-ai`'s novice atrophy risk — the living-and-working-with-ai page explicitly prescribes "periodically work without AI in core domains" in its inline answer to the cognitive-atrophy question; the frameworks are compatible; existing contradiction #1 already captures the deeper expert-exemption debate. Total open contradictions: **8** (unchanged).

**0 new near-duplicate cases (Stage 2):**

Vault stable at 91 pages since 2026-06-14. All overlap patterns in pages scanned today (the-one-thing/focus-vs-orientation, experiment-theater/experimental-mindset, experimental-mindset-and-privilege/experimental-mindset, living-and-working-with-ai/cognitive-atrophy-and-ai, living-and-working-with-ai/ai-productivity-gains-distribution, financial-stability-while-experimenting/experimental-mindset) were already documented in Case 2. Cases 1, 2 (17 confirmed instances), and 3 carry forward unchanged. All pending owner approval.

**1 count correction (Stage 3):**

`mental-models` corrected from 20 to **18** (methodology fix). Prior count of 20 originated in 2026-07-03 run using prefix grep `[[mental-models` which captured two false positives: `munger-disposition-formation.md` (links to `[[mental-models-and-multidisciplinary-thinking]]`, not `[[mental-models]]`; also has "mental-models" as a plain-text tag but no wikilink) and `ryan-holiday.md` (links to `[[mental-models-and-multidisciplinary-thinking]]`, not `[[mental-models]]`). Exact-string verification: 18 files contain `[[mental-models]]` or `[[mental-models|alias]]`. The 2 links discovered in 2026-07-03 (stoic-justice.md and adaptive-challenge-diagnosis.md) are real and included in the 18 — the 2026-07-03 finding was correct about the new links but wrong about the total (true correction was 16→18, not 16→20). Rank change: `mental-models` drops from co-#1 (tied at 20 with disposition-vs-knowledge) to solo #2 (18). All other 16 inbound-link counts confirmed stable.
