---
title: "Salience Digest"
date: 2026-07-15
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

**2026-07-15** — Full dream-cycle pass (nightly). 91 wiki pages; vault unchanged since 2026-06-14 weekly pass (1-day gap since last logged run on 2026-07-14). **Stage 1:** 0 new contradictions; 8 total open contradictions confirmed. Pages scanned this run: 10 pages across AI/economics (ai-productivity-gains-distribution, general-purpose-technology), Stoicism/ethics (stoicism-and-systemic-injustice, stoic-truth-telling-and-tact), health/TB (tb-eradication-requirements), productivity (pseudo-productivity, negotiating-slow-productivity), leadership (adaptive-vs-technical-challenges), and economics (sound-money, crony-capitalism) clusters. All pages internally consistent. No new contradiction candidates emerged. Pages verified internally consistent: ai-productivity-gains-distribution and general-purpose-technology are complementary (distributional political economy vs. definitional GPT properties — no tension); stoicism-and-systemic-injustice and stoic-truth-telling-and-tact operate on different dimensions (collective justice critique vs. honest speech ethics) and are consistent; tb-eradication-requirements aligns with health-equity-without-redistribution's framing (political/IP reform as key levers) while acknowledging the structural constraints that pandemic-lessons-from-tb emphasizes — the nuance is already captured in existing contradiction #8; pseudo-productivity and negotiating-slow-productivity are an explicitly complementary diagnosis/tactics pair; adaptive-vs-technical-challenges is consistent with adaptive-leadership; sound-money and crony-capitalism are complementary Stockman-cluster definitional pages consistent with the existing contradiction #4. Total open contradictions: **8** (unchanged). **Stage 2:** 0 new near-duplicate cases. Vault stable at 91 pages since 2026-06-14. All three cases carry forward unchanged; all pending owner approval. **Stage 3:** 0 count corrections. Methodology note: earlier grep using `-v 'jagged-frontier.md'` (substring match) produced a false count of 8 for jagged-frontier by also excluding `mapping-the-jagged-frontier.md`; full-path exclusion `-v '/wiki/concepts/jagged-frontier.md'` confirms 9 exact-string hits + 1 piped (ai-tutoring-and-human-motivation.md) = **10**, consistent with all prior runs. All 17 top-tier and mid-tier inbound-link counts verified stable: disposition-vs-knowledge (20 ✓), mental-models (18 ✓), health-equity (17 ✓ — exact-string confirmed), cognitive-atrophy-and-ai (14 ✓), mental-models-and-multidisciplinary-thinking (12 ✓ — 11 exact + 1 piped in disposition-building-practices.md via `[[mental-models-and-multidisciplinary-thinking|Munger]]`), charlie-munger (11 ✓ — 10 exact + 1 piped), slow-productivity (11 ✓), growth-mindset (10 ✓), jagged-frontier (10 ✓ — prefix confirmed), latticework-pedagogy (10 ✓), tuberculosis-and-global-health (10 ✓), experimental-mindset (9 ✓), large-language-models (9 ✓), living-and-working-with-ai (9 ✓), tiny-experiments (8 ✓), stoic-virtues (7 ✓), superforecasting (7 ✓). No rank changes.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | **18** | ~350 | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Referenced by every major cluster (Munger, Stoicism, AI, education, forecasting, adaptive leadership, productivity). Body remains a thin properties list + model table. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence (see `munger-vs-behavioral-economics`), cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | **17** | ~400 | **3rd-most-linked page in the vault**. Body remains thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| `jagged-frontier` | **10** | ~300 | Anchor concept for the AI cluster; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`, `ai-productivity-gains-distribution`, `general-purpose-technology`, `ethan-mollick`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | **11** *(10 exact + 1 piped in latticework-feedback-loops-outside-investing.md; confirmed via prefix search)* | ~350 | Central person page for the Munger/latticework cluster. Body is a short biography + key contributions list — well below what centrality warrants. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`, `munger-vs-behavioral-economics`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share a creation band of 2026-05-18 to 2026-06-14 (31–57 days old as of 2026-07-15). Staleness does not yet differentiate meaningfully within this vault; pages are recent. Re-run this section after the next enrichment pass.

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

Inbound-link counts verified via exact-string and prefix ripgrep (excludes self-reference, captures piped wikilinks). Vault at 91 pages. **0 count corrections this run.** charlie-munger confirmed at 11 (10 exact + 1 piped); jagged-frontier confirmed at 10 (9 exact + 1 piped — ai-tutoring-and-human-motivation.md); health-equity confirmed at 17 (exact-string); mental-models-and-multidisciplinary-thinking confirmed at 12 (11 exact + 1 piped — disposition-building-practices.md via `[[mental-models-and-multidisciplinary-thinking|Munger]]`).

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| **1** | `disposition-vs-knowledge` | **20** | ~900 words | Crown jewel: richest body among top-10; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. Sole #1. |
| **2** | `mental-models` | **18** | ~350 words | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Two Munger PDFs in raw/ are the primary source. |
| **3** | `health-equity` | **17** | ~400 words | Body thin relative to centrality; primary enrichment target in the health/justice cluster. Open contradiction with `pandemic-lessons-from-tb` remains. |
| **4** | `cognitive-atrophy-and-ai` | **14** | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| **5** | `mental-models-and-multidisciplinary-thinking` | **12** *(11 exact + 1 piped; confirmed)* | ~1500 words (topic) | Well-developed topic page. |
| 6 (tied) | `charlie-munger` | 11 *(10 exact + 1 piped; confirmed)* | ~350 words | Central person page; body unexpectedly thin for centrality — enrichment candidate. |
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

Ten pages scanned across AI/economics (ai-productivity-gains-distribution, general-purpose-technology), Stoicism/ethics (stoicism-and-systemic-injustice, stoic-truth-telling-and-tact), health/TB (tb-eradication-requirements), productivity (pseudo-productivity, negotiating-slow-productivity), leadership (adaptive-vs-technical-challenges), and economics (sound-money, crony-capitalism) clusters. No new contradiction candidates emerged. All pages internally consistent. Notable examinations: (1) tb-eradication-requirements and existing contradiction #8 — the TB eradication page provides quantitative specificity ($22B/year delivery, $300/course endTB MDR-TB cure, PIH >85% cure rates) that supports health-equity-without-redistribution's "substantial progress" framing while acknowledging the structural/funding constraints that pandemic-lessons-from-tb emphasizes; this nuance is fully within the already-registered contradiction's scope and does not create a new one. (2) stoicism-and-systemic-injustice's "truth-telling as structural disruption" section and stoic-truth-telling-and-tact — both acknowledge that individual truth-telling at scale can produce structural change; no tension, they complement each other by addressing collective-justice limits vs. honest-speech ethics respectively. (3) negotiating-slow-productivity references Heifetz's holding-environment concept in the organizational context — consistent with adaptive-leadership and adaptive-vs-technical-challenges (pseudo-productivity could be classified as an adaptive challenge requiring behavioral change, and the page provides both tactical individual strategies and organizational structural prescriptions consistent with Heifetz's framework). Total open contradictions: **8** (unchanged).

**0 new near-duplicate cases (Stage 2):**

Vault stable at 91 pages since 2026-06-14. Today's pages are well-scoped and distinct: pseudo-productivity (diagnosis) vs. negotiating-slow-productivity (tactics) are explicitly designed as a pair; stoicism-and-systemic-injustice and stoic-truth-telling-and-tact cover different dimensions of Stoic ethics in practice; tb-eradication-requirements is a detailed policy synthesis distinct from tuberculosis-and-global-health (topic overview), health-equity-without-redistribution (sufficiency argument), and pandemic-lessons-from-tb (pandemic parallels); adaptive-vs-technical-challenges is a compact foundational concept distinct from adaptive-leadership (topic) and adaptive-challenge-diagnosis (extension). Cases 1, 2 (17 confirmed instances), and 3 carry forward unchanged. All pending owner approval.

**0 count corrections (Stage 3):**

All 17 inbound-link counts for top-tier and mid-tier pages verified stable (see full list in "Surfacing for the dashboard" section above). Methodology note: using `-v 'jagged-frontier.md'` (substring exclusion) incorrectly filtered out `mapping-the-jagged-frontier.md` from the jagged-frontier count, producing a false count of 8 instead of 9 exact-string hits; the correct full-path exclusion `-v '/wiki/concepts/jagged-frontier.md'` confirms 9 exact + 1 piped = **10** — consistent with all prior runs. No correction needed to the salience table.
