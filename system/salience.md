---
title: "Salience Digest"
date: 2026-06-20
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

**2026-06-20** — Full dream-cycle pass (nightly). 91 wiki pages analyzed (57 concepts, 15 topics, 19 people). Vault unchanged since prior nightly run (2026-06-19). **Stage 1:** 0 new contradictions; 8 total open contradictions confirmed. Pages scanned this run: 11 pages across education/productivity clusters — education cluster (sal-khan, jo-boaler, lisa-damour, mathematics-education, ai-in-education, ai-tutoring, cognitive-atrophy-and-ai) and productivity/focus cluster (tiny-experiments, experimental-mindset, the-one-thing, focus-vs-orientation). Three candidates explored: (1) `cognitive-atrophy-and-ai` "For novices: early AI assistance for generative tasks carries atrophy risk" vs. `ai-tutoring`/`ai-in-education` promoting AI tutoring for students — resolved as non-contradictory: Khanmigo uses Socratic method (student does cognitive work, AI does not give answers), which is the atrophy-safe use pattern; (2) `mathematics-education` (Boaler: open tasks, no timed tests, multiple valid approaches) vs. `sal-khan` (mastery learning: advance only after demonstrating mastery) — theoretical philosophical divergence, but neither page makes claims that directly negate the other's stated positions; not logged; (3) `experimental-mindset` vs. `the-one-thing` — previously explored in 2026-06-13 run and confirmed non-contradictory via orientation/execution framing in `focus-vs-orientation`; not re-logged. **Stage 2:** 0 new near-duplicate cases. Cases 1, 2 (17 confirmed), 3 carry forward unchanged. All pending owner approval. **Stage 3:** All inbound-link counts re-verified via anchored ripgrep. Methodology note: verified that filter must not exclude derivation-named files (e.g., `mental-models-and-multidisciplinary-thinking.md` correctly counted as inbound to `mental-models`; `slow-productivity-and-ai-craft.md` correctly counted as inbound to `slow-productivity`; `health-equity-without-redistribution.md` correctly counted as inbound to `health-equity`). All top-tier counts confirmed: disposition-vs-knowledge (20), mental-models (18), health-equity (17), cognitive-atrophy-and-ai (14), mental-models-and-multidisciplinary-thinking (12), charlie-munger (11), slow-productivity (11). No rank changes. Vault remains at 91 pages.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | **18** | ~350 | **#1 enrichment priority in the vault** (by enrichment-leverage: high centrality, thin body). 18 inbound links (confirmed). Referenced by every major cluster (Munger, Stoicism, AI, education, forecasting). Body remains a thin properties list + model table. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence (see `munger-vs-behavioral-economics`), cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | **17** | ~400 | **3rd-most-linked page in the vault**. Body remains thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| `jagged-frontier` | **10** | ~300 | Anchor concept for the AI cluster; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`, `ai-productivity-gains-distribution`, `general-purpose-technology`, `ethan-mollick`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | **11** | ~350 | Central person page for the Munger/latticework cluster. Body is a short biography + key contributions list — well below what centrality warrants. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`, `munger-vs-behavioral-economics`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share a creation band of 2026-05-18 to 2026-06-14 (5–32 days old). Staleness does not yet differentiate meaningfully within this vault; pages are recent. Re-run this section after the next enrichment pass.

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

Inbound-link counts re-verified via anchored ripgrep (unique files, excluding self-references; derivation-named files correctly included in counts — e.g., `mental-models-and-multidisciplinary-thinking.md` counted as inbound to `mental-models`, `slow-productivity-and-ai-craft.md` counted as inbound to `slow-productivity`). Vault at 91 pages. All counts confirmed stable from 2026-06-19.

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| **1** | `disposition-vs-knowledge` | **20** | ~900 words | Crown jewel: richest body among top-10; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. |
| **2** | `mental-models` | **18** | ~350 words | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Two Munger PDFs in raw/ are the primary source. |
| **3** | `health-equity` | **17** | ~400 words | Body thin relative to centrality; primary enrichment target in the health/justice cluster. Open contradiction with `pandemic-lessons-from-tb` remains. |
| **4** | `cognitive-atrophy-and-ai` | **14** | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| **5** | `mental-models-and-multidisciplinary-thinking` | **12** | ~1500 words (topic) | Well-developed topic page. |
| 6 (tied) | `charlie-munger` | 11 | ~350 words | Central person page; body unexpectedly thin for centrality — enrichment candidate. |
| 6 (tied) | `slow-productivity` | 11 | ~800+ words (topic) | Central productivity hub; topic page substantive. |
| 8 (tied) | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; contradiction with `mathematics-education` remains open. |
| 8 (tied) | `jagged-frontier` | **10** | ~300 words | Very thin body vs. centrality — **#2 AI-cluster enrichment priority**. |
| 8 (tied) | `latticework-pedagogy` | 10 | ~1000 words | Well-developed; bridges Munger cluster with behavioral science. |
| 8 (tied) | `tuberculosis-and-global-health` | **10** | ~1100 words (topic) | Well-developed topic page. Central node in the health/justice cluster. Case 2 instance #17 pending: ~300-word inline pandemic-lessons answer duplicates `pandemic-lessons-from-tb`. |
| 12 (tied) | `experimental-mindset` | 9 | ~1200 words (topic) | High centrality, well-developed. Open questions now all answered. |
| 12 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |
| 12 (tied) | `living-and-working-with-ai` | 9 | ~1500+ words (topic) | High centrality, well-developed. |
| 15 (tied) | `tiny-experiments` | 8 | ~450 words | Adequately developed for its centrality. |
| 17 (tied) | `stoic-virtues` | 7 | ~500 words | Adequately developed; open contradiction with `wisdom-traditions-practice-vs-doctrine` remains. |
| 17 (tied) | `superforecasting` | 7 | ~900 words | Well-developed; open contradiction with `munger-vs-behavioral-economics` remains. |

_Note: `social-media-and-illness-aesthetics` (created 2026-06-14) has 1 confirmed inbound link (`romanticization-of-illness`). Will accumulate links over time. Near-duplicate alert (Case 2, #16): its creation left a ~250-word duplicate in `contemporary-romanticized-illnesses` pending owner approval for compression._

---

## Newly surfaced this run

**0 new contradictions (Stage 1):**

Eleven pages scanned across the education cluster (sal-khan, jo-boaler, lisa-damour, mathematics-education, ai-in-education, ai-tutoring, cognitive-atrophy-and-ai) and productivity/focus cluster (tiny-experiments, experimental-mindset, the-one-thing, focus-vs-orientation). All 8 existing contradictions confirmed. Three candidates explored: (1) `cognitive-atrophy-and-ai` "novice AI assistance carries atrophy risk" vs. `ai-tutoring`/`ai-in-education` promoting AI tutoring for students — resolved as non-contradictory: Khanmigo's Socratic design (student does cognitive work, AI does not provide answers) is exactly the atrophy-safe use pattern the atrophy framework recommends. No contradiction. (2) `mathematics-education` (Boaler's open tasks, anti-timed-assessment model) vs. `sal-khan` (mastery learning: advance only after demonstrating mastery) — theoretical divergence in pedagogical philosophy, but neither page's specific claims directly negate the other's; `mathematics-education` does not comment on AI tutoring, and `sal-khan` does not comment on open tasks. Not logged. (3) `experimental-mindset` vs. `the-one-thing` (orientation-vs-execution tension) — previously explored in 2026-06-13 run, confirmed non-contradictory via the orientation/execution framing developed in `focus-vs-orientation`. Not re-logged.

**0 new near-duplicate cases (Stage 2):**

Vault unchanged since 2026-06-14. Cases 1, 2 (17 confirmed instances), and 3 carry forward unchanged. All pending owner approval.

**0 count corrections (Stage 3):**

All inbound-link counts confirmed stable via anchored ripgrep with correct derivation-file inclusion. Methodology clarification documented: filter must not use simple string-exclusion patterns (e.g., `grep -v 'mental-models-and'`) that would incorrectly suppress legitimate inbound linkers like `mental-models-and-multidisciplinary-thinking.md` (→ `mental-models`), `slow-productivity-and-ai-craft.md` (→ `slow-productivity`), or `health-equity-without-redistribution.md` (→ `health-equity`). Correct approach: exclude only the exact self-reference file using anchored path matching (e.g., `grep -v '/mental-models\.md$'`). Rankings unchanged. Total open contradictions: **8** (unchanged). Total near-duplicate cases: Cases 1, 2 (17 confirmed), 3 — all pending owner approval.
