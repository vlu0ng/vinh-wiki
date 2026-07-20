---
title: "Salience Digest"
date: 2026-07-20
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

**2026-07-20** — Full dream-cycle pass (nightly). 91 wiki pages; vault unchanged since 2026-06-14 weekly pass (content); 2026-07-19 weekly system pass added 16 bidirectional connection edges and 2 related: field expansions. **Stage 1:** 0 new contradictions; 8 total open contradictions confirmed. Pages scanned this run: 8 pages across AI/cognition cluster (cognitive-atrophy-and-ai, mapping-the-jagged-frontier, general-purpose-technology, ai-in-education, ai-productivity-gains-distribution) and art/aesthetics cluster (compulsive-collecting, ethics-of-private-beauty) plus mental-models concept page. Notable examinations: (1) AI/cognition cluster — cognitive-atrophy-and-ai, mapping-the-jagged-frontier, general-purpose-technology, ai-in-education, and ai-productivity-gains-distribution are internally consistent. mapping-the-jagged-frontier operationalizes cognitive-atrophy-and-ai's "threshold shifts with expertise" heuristic without contradiction; both agree that novices should preserve unaided practice while senior practitioners can delegate more aggressively. ai-productivity-gains-distribution (capital-concentration risk, historical wage precedents, counter-mechanism of freelancer amplification) does not create new tension with living-and-working-with-ai's augmentation framing — they address different analytical layers (macro distribution vs. individual workflow). (2) Art/aesthetics cluster — compulsive-collecting and ethics-of-private-beauty are tightly paired and mutually consistent; both use the Breitwieser case to illustrate the same core tension between private aesthetic devotion and public stewardship duty; no internal contradiction. (3) mental-models — consistent with all Munger/latticework cluster pages; the latticework metaphor is applied coherently across mental-models, latticework-pedagogy, disposition-building-practices, and superforecasting. Total open contradictions: **8** (unchanged). **Stage 2:** 0 new near-duplicate cases. Vault stable at 91 pages. No new raw files (still 2 Munger PDFs in raw/articles/). Cases 1, 2 (17 instances), and 3 carry forward unchanged. **Stage 3:** 0 count corrections. All 17 tracked inbound-link counts confirmed stable vs. 2026-07-19 via exact-string anchored ripgrep. No rank changes.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | **18** | ~350 | **#1 enrichment target in the vault** by thin-body/high-centrality metric. Referenced by every major cluster (Munger, Stoicism, AI, education, forecasting, adaptive leadership, productivity). Body remains a thin properties list + model table. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence (see `munger-vs-behavioral-economics`), cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | **17** | ~400 | **3rd-most-linked page in the vault**. Body remains thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| `jagged-frontier` | **10** | ~300 | Anchor concept for the AI cluster; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`, `ai-productivity-gains-distribution`, `general-purpose-technology`, `ethan-mollick`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | **11** *(10 exact + 1 piped in latticework-feedback-loops-outside-investing.md)* | ~350 | Central person page for the Munger/latticework cluster. Body is a short biography + key contributions list — well below what centrality warrants. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`, `munger-vs-behavioral-economics`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share a creation band of 2026-05-18 to 2026-06-14 (34–60 days old as of 2026-07-18). Staleness does not yet differentiate meaningfully within this vault; pages are recent. Re-run this section after the next enrichment pass.

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

Inbound-link counts verified via exact-string and prefix ripgrep (excludes self-reference, captures piped wikilinks). Vault at 91 pages. **1 count correction this run:** experimental-mindset reverted from 10 back to **9** (the 2026-07-18 "correction" was erroneous — experimental-mindset-and-privilege.md was never excluded from the 9-count). charlie-munger confirmed at 11 (10 exact + 1 piped); jagged-frontier confirmed at 10 (9 exact + 1 piped); mental-models-and-multidisciplinary-thinking confirmed at 12 (11 exact + 1 piped-only; 2 piped-link files total, one of which also has exact link); health-equity confirmed at 17 (exact-string).

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
| 13 (tied) | `experimental-mindset` | **9** *(reverted from erroneous 10; confirmed 9 via today's exact-string grep)* | ~1200 words (topic) | High centrality, well-developed. Open questions now all answered. |
| 13 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |
| 13 (tied) | `living-and-working-with-ai` | 9 | ~1500+ words (topic) | High centrality, well-developed. |
| 15 | `tiny-experiments` | 8 | ~450 words | Adequately developed for its centrality. |
| 16 (tied) | `stoic-virtues` | 7 | ~500 words | Adequately developed; open contradiction with `wisdom-traditions-practice-vs-doctrine` remains. |
| 16 (tied) | `superforecasting` | 7 | ~900 words | Well-developed; open contradiction with `munger-vs-behavioral-economics` remains. |

_Note: `social-media-and-illness-aesthetics` (created 2026-06-14) has 1 confirmed inbound link (`romanticization-of-illness`). Will accumulate links over time. Near-duplicate alert (Case 2, #16): its creation left a ~250-word duplicate in `contemporary-romanticized-illnesses` pending owner approval for compression._

---

## Newly surfaced this run

**0 new contradictions (Stage 1):**

Eight pages scanned across AI/cognition cluster (cognitive-atrophy-and-ai, mapping-the-jagged-frontier, general-purpose-technology, ai-in-education, ai-productivity-gains-distribution) and art/aesthetics cluster (compulsive-collecting, ethics-of-private-beauty), plus mental-models concept page. No new contradiction candidates emerged.

Notable: (1) AI/cognition cluster — cognitive-atrophy-and-ai and mapping-the-jagged-frontier are consistent and complementary: mapping-the-jagged-frontier operationalizes cognitive-atrophy-and-ai's "novices should preserve unaided practice; senior practitioners can delegate more aggressively" heuristic; no contradiction. ai-productivity-gains-distribution addresses macro distributional dynamics of AI productivity gains and does not conflict with living-and-working-with-ai's individual workflow guidance. general-purpose-technology is a thin definition page; internally consistent with all AI cluster pages. ai-in-education is consistent with ai-tutoring-and-human-motivation (contradiction #2 already registered). (2) Art/aesthetics cluster — compulsive-collecting and ethics-of-private-beauty are tightly paired and consistent; the Breitwieser case is analyzed through the same philosophical lens in both pages with no contradictory claims. (3) mental-models concept page is consistent with latticework-pedagogy, disposition-building-practices, superforecasting, and charlie-munger. Total open contradictions: **8** (unchanged).

**0 new near-duplicate cases (Stage 2):**

Vault stable at 91 pages since 2026-06-14 (content); 2026-07-19 weekly system pass modified connections/related fields only. No new raw files (still 2 Munger PDFs in raw/articles/). Cases 1, 2 (17 confirmed instances), and 3 carry forward unchanged. All pending owner approval.

**0 count corrections (Stage 3):**

All 17 tracked inbound-link counts confirmed stable vs. 2026-07-19 via exact-string anchored ripgrep. The 2026-07-19 reversion of experimental-mindset to 9 (from the erroneous 10) holds: confirmed again at 9. No rank changes. Full confirmation: disposition-vs-knowledge (20 ✓), mental-models (18 ✓), health-equity (17 ✓), cognitive-atrophy-and-ai (14 ✓), mental-models-and-multidisciplinary-thinking (12 ✓ — 11 exact + 1 piped-only), charlie-munger (11 ✓ — 10 exact + 1 piped), slow-productivity (11 ✓), growth-mindset (10 ✓), jagged-frontier (10 ✓ — 9 exact + 1 piped), latticework-pedagogy (10 ✓), tuberculosis-and-global-health (10 ✓), experimental-mindset (9 ✓), large-language-models (9 ✓), living-and-working-with-ai (9 ✓), tiny-experiments (8 ✓), stoic-virtues (7 ✓), superforecasting (7 ✓).
