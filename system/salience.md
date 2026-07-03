---
title: "Salience Digest"
date: 2026-07-03
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

**2026-07-03** — Full dream-cycle pass (nightly). 91 wiki pages analyzed (57 concepts, 15 topics, 19 people). Vault unchanged since 2026-06-14 weekly pass. **Stage 1:** 0 new contradictions; 8 total open contradictions confirmed. Pages scanned this run: 13 pages across teenage development cluster (lisa-damour, adolescent-development-in-the-digital-age, developmental-strands, teenage-girl-development), art-theft/obsession cluster (compulsive-collecting, ethics-of-private-beauty), glucose cluster (glucose-curves, glucose-revolution), Stoicism cluster (stoic-justice, stoicism-and-systemic-injustice), and AI/work cluster (adaptive-leadership, general-purpose-technology, mapping-the-jagged-frontier, ai-productivity-gains-distribution, latticework-pedagogy). All clusters internally consistent. Teenage development cluster is cohesive: developmental-strands supplies the theoretical framework, teenage-girl-development applies it across seven strands, adolescent-development-in-the-digital-age extends it to the digital context. Art-theft/obsession: compulsive-collecting and ethics-of-private-beauty are complementary pages building on the Breitwieser case from opposite analytical angles (psychology vs. ethics). Glucose: glucose-curves and glucose-revolution are tightly paired, glucose-curves being the key concept page and glucose-revolution the full framework page — consistent. Stoicism: stoic-justice raises the systemic-injustice open question; stoicism-and-systemic-injustice directly answers it — consistent. AI/work: mapping-the-jagged-frontier, ai-productivity-gains-distribution, and latticework-pedagogy all consistent with each other and with the AI cluster; latticework-pedagogy's treatment of superforecasting research aligns with the superforecasting page (same "validates Munger's latticework intuition" framing), consistent with existing contradiction #6 between superforecasting and munger-vs-behavioral-economics. No new contradiction candidates identified. All 8 existing contradictions remain open and unchanged. **Stage 2:** 0 new near-duplicate cases. Vault stable at 91 pages since 2026-06-14. Cases 1, 2 (17 confirmed instances), and 3 carry forward unchanged. All pending owner approval. **Stage 3:** 1 count correction detected. `mental-models` re-verified via anchored ripgrep (`[[mental-models` prefix): **20 confirmed** (up from 18 recorded in all prior passes). Two previously-missed inbound links discovered: (1) `wiki/topics/stoic-justice.md` contains `[[mental-models]]` in its frontmatter `related:` field (page created 2026-05-19; link always present); (2) `wiki/concepts/adaptive-challenge-diagnosis.md` contains `[[mental-models]]` in both frontmatter `related:` and body text (page created 2026-06-07; link always present). These links were missed because prior passes focused on the core Munger cluster and did not verify Stoicism or adaptive leadership pages for mental-models backlinks. `mental-models` now ties `disposition-vs-knowledge` at 20 — **co-#1 most-linked page in the vault** (up from rank 2 at 18). This strengthens the enrichment case: `mental-models` is the most central thin-body page in the vault. All other 16 counts confirmed stable.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | **20** *(corrected — was 18)* | ~350 | **#1 enrichment priority in the vault** (by enrichment-leverage: highest centrality, thin body). Now tied with `disposition-vs-knowledge` at 20 inbound links — **co-#1 most-linked page in the vault**. Referenced by every major cluster (Munger, Stoicism, AI, education, forecasting, adaptive leadership). Body remains a thin properties list + model table. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence (see `munger-vs-behavioral-economics`), cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | **17** | ~400 | **3rd-most-linked page in the vault**. Body remains thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| `jagged-frontier` | **10** | ~300 | Anchor concept for the AI cluster; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`, `ai-productivity-gains-distribution`, `general-purpose-technology`, `ethan-mollick`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | **11** | ~350 | Central person page for the Munger/latticework cluster. Body is a short biography + key contributions list — well below what centrality warrants. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`, `munger-vs-behavioral-economics`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share a creation band of 2026-05-18 to 2026-06-14 (19–46 days old). Staleness does not yet differentiate meaningfully within this vault; pages are recent. Re-run this section after the next enrichment pass.

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

Inbound-link counts re-verified via wikilink-anchored ripgrep (`[[slug` prefix pattern; excludes plain-text prose mentions). Vault at 91 pages. **One count correction this run: `mental-models` corrected to 20 (was 18).** Two missed links: `stoic-justice.md` (frontmatter `related:`) and `adaptive-challenge-diagnosis.md` (frontmatter `related:` + body). Both links have always been present; discovered during this run's broader cluster scan. `mental-models` now co-#1 with `disposition-vs-knowledge`.

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| **1 (tied)** | `disposition-vs-knowledge` | **20** | ~900 words | Crown jewel: richest body among top-10; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. |
| **1 (tied)** | `mental-models` | **20** *(corrected from 18)* | ~350 words | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Now co-#1 most-linked page. Two Munger PDFs in raw/ are the primary source. |
| **3** | `health-equity` | **17** | ~400 words | Body thin relative to centrality; primary enrichment target in the health/justice cluster. Open contradiction with `pandemic-lessons-from-tb` remains. |
| **4** | `cognitive-atrophy-and-ai` | **14** | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| **5** | `mental-models-and-multidisciplinary-thinking` | **12** | ~1500 words (topic) | Well-developed topic page. |
| 6 (tied) | `charlie-munger` | 11 | ~350 words | Central person page; body unexpectedly thin for centrality — enrichment candidate. |
| 6 (tied) | `slow-productivity` | 11 | ~800+ words (topic) | Central productivity hub; topic page substantive. |
| 8 (tied) | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; contradiction with `mathematics-education` remains open. |
| 8 (tied) | `jagged-frontier` | **10** | ~300 words | Very thin body vs. centrality — **#2 AI-cluster enrichment priority**. |
| 8 (tied) | `latticework-pedagogy` | 10 | ~1000 words | Well-developed; bridges Munger cluster with behavioral science. |
| 8 (tied) | `tuberculosis-and-global-health` | **10** | ~1100 words (topic) | Well-developed topic page. Central node in the health/justice cluster. Case 2 instance #17 pending: ~300-word inline pandemic-lessons answer duplicates `pandemic-lessons-from-tb`. |
| 8 (tied) | `experimental-mindset` | **10** | ~1200 words (topic) | High centrality, well-developed. Open questions now all answered. Count corrected in 2026-07-02 run (was 9; 10th link from `adaptive-vs-technical-challenges.md`). |
| 13 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |
| 13 (tied) | `living-and-working-with-ai` | 9 | ~1500+ words (topic) | High centrality, well-developed. |
| 15 | `tiny-experiments` | 8 | ~450 words | Adequately developed for its centrality. |
| 16 (tied) | `stoic-virtues` | 7 | ~500 words | Adequately developed; open contradiction with `wisdom-traditions-practice-vs-doctrine` remains. |
| 16 (tied) | `superforecasting` | 7 | ~900 words | Well-developed; open contradiction with `munger-vs-behavioral-economics` remains. Wikilink count confirmed 7. |

_Note: `social-media-and-illness-aesthetics` (created 2026-06-14) has 1 confirmed inbound link (`romanticization-of-illness`). Will accumulate links over time. Near-duplicate alert (Case 2, #16): its creation left a ~250-word duplicate in `contemporary-romanticized-illnesses` pending owner approval for compression._

---

## Newly surfaced this run

**0 new contradictions (Stage 1):**

Thirteen pages scanned across teenage development cluster (lisa-damour, adolescent-development-in-the-digital-age, developmental-strands, teenage-girl-development), art-theft/obsession cluster (compulsive-collecting, ethics-of-private-beauty), glucose cluster (glucose-curves, glucose-revolution), Stoicism cluster (stoic-justice, stoicism-and-systemic-injustice), and AI/work cluster (adaptive-leadership, general-purpose-technology, mapping-the-jagged-frontier, ai-productivity-gains-distribution, latticework-pedagogy). All clusters internally consistent. Teenage development: all three pages form a coherent chain — developmental-strands (theory) → teenage-girl-development (applied Damour) → adolescent-development-in-the-digital-age (digital extension). Art-theft: compulsive-collecting and ethics-of-private-beauty are complementary pages on the Breitwieser case from different angles (psychology vs. ethics) — not contradictory. Glucose: consistent pair. Stoicism: stoic-justice's open question answered directly by stoicism-and-systemic-injustice — consistent. AI/work: mapping-the-jagged-frontier aligns with cognitive-atrophy-and-ai on the novice/expert distinction (consistent with existing contradiction #1's framing); latticework-pedagogy's Tetlock reference aligns with superforecasting ("validates Munger's latticework intuition") — consistent with existing contradiction #6 framing. No new contradiction candidates identified. Total open contradictions: **8** (unchanged).

**0 new near-duplicate cases (Stage 2):**

Vault stable at 91 pages since 2026-06-14. Cases 1, 2 (17 confirmed instances), and 3 carry forward unchanged. All pending owner approval.

**1 count correction (Stage 3):**

`mental-models` wikilink count corrected to 20 (was 18 in all prior passes). Two previously-missed inbound links discovered: (1) `wiki/topics/stoic-justice.md` → `[[mental-models]]` in frontmatter `related:` (link predates 2026-06-14 vault freeze; page created 2026-05-19); (2) `wiki/concepts/adaptive-challenge-diagnosis.md` → `[[mental-models]]` in frontmatter `related:` and body text (page created 2026-06-07). Both links were missed because prior verification passes focused on the core Munger/latticework cluster and did not systematically verify Stoicism-cluster and adaptive-leadership-cluster backlinks to `mental-models`. `mental-models` now ties `disposition-vs-knowledge` at 20 — co-#1 most-linked page in the vault (up from rank 2 at 18). This strengthens the case for enrichment: the page is simultaneously the most-linked and the thinnest among the top-5. Verified via `grep -rl "[[mental-models" wiki/ | grep -v "wiki/concepts/mental-models.md"` (20 results). All other 16 counts confirmed stable: health-equity (17 ✓), cognitive-atrophy-and-ai (14 ✓), mental-models-and-multidisciplinary-thinking (12 ✓), charlie-munger (11 ✓), slow-productivity (11 ✓), growth-mindset (10 ✓), jagged-frontier (10 ✓), latticework-pedagogy (10 ✓), tuberculosis-and-global-health (10 ✓), experimental-mindset (10 ✓), large-language-models (9 ✓), living-and-working-with-ai (9 ✓), tiny-experiments (8 ✓), stoic-virtues (7 ✓), superforecasting (7 ✓). Total open contradictions: **8** (unchanged). Total near-duplicate cases: Cases 1, 2 (17 confirmed), 3 — all pending owner approval.
