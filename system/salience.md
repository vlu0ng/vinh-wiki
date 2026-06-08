---
title: "Salience Digest"
date: 2026-06-08
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

**2026-06-08** — Full dream-cycle pass (nightly). 90 wiki pages analyzed (56 concepts, 15 topics, 19 people). Eight new pages added in the 2026-06-07 weekly pass (health-equity-without-redistribution, economic-literacy-at-scale, scanlon-optimism-limits, munger-vs-behavioral-economics, financial-stability-while-experimenting, experimental-mindset-and-privilege, ai-productivity-gains-distribution, adaptive-challenge-diagnosis). Inbound-link counts re-verified via ripgrep unique-file pattern-match on `[[slug` prefix across all wiki/ files. **Stage 1:** 2 new contradictions detected (`superforecasting` vs. `munger-vs-behavioral-economics` on whether Tetlock validates or contrasts Munger; `vibecession` vs. `scanlon-optimism-limits` on whether the sentiment gap is behavioral distortion or rational distributional perception) — 7 total open contradictions. **Stage 2:** Case 2 inline-answer pattern expands from 7 to at least 9 confirmed instances (2 new entries from `experimental-mindset`'s financial-stability and privilege open questions; likely more from other 2026-06-07 weekly-pass concept pages). **Stage 3:** Rankings shift: `disposition-vs-knowledge` overtakes `mental-models` as #1 (20 vs. 18 inbound), `health-equity` rises to 16 inbound, `slow-productivity` rises to 11. Two uningested Munger PDFs remain the highest-priority ingest items.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | 18 | ~350 | **#1 enrichment priority in the vault** (despite dropping to #2 in link count). Highest inbound count outside of `disposition-vs-knowledge`, but body is still a thin properties list + model table. Referenced by every major cluster. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence (see new `munger-vs-behavioral-economics`), cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | 16 | ~400 | **3rd-most-linked page in the vault** (rose from 13 to 16 inbound). Body remains thin relative to centrality. One unanswered open question ("Is health equity achievable without global wealth redistribution?") now partially addressed by the new `health-equity-without-redistribution` concept page — but the parent page body itself could still be enriched with social-determinants framework depth and global health financing. |
| `jagged-frontier` | 9 | ~300 | Anchor concept for all AI pages; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | 10 | ~350 | Central person page for the Munger/latticework cluster (10 inbound). Body is a short biography + key contributions list — well below what centrality warrants. New `munger-vs-behavioral-economics` page makes the need for a richer person page more visible. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share a creation band of 2026-05-18 to 2026-06-07 (1–21 days old). Staleness does not yet differentiate meaningfully within this vault; pages are recent. Re-run this section after the next enrichment pass.

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
When open questions were answered and extracted into dedicated concept pages, the originals were not trimmed. **At least 9 confirmed cases (up from 7).** Owner approval required for each compression individually.

| Page | Duplicated in concept page | Estimated inline word count |
|---|---|---|
| `experimental-mindset` (open-Q on experiment theater) | `experiment-theater` | ~350 |
| `adaptive-leadership` (open-Q on psychological safety) | `adaptive-leadership-and-psychological-safety` | ~300 |
| `stoic-justice` (open-Q on systemic injustice) | `stoicism-and-systemic-injustice` + `stoic-truth-telling-and-tact` | ~450 combined |
| `the-one-thing` (open-Q on tunnel vision) | `focus-vs-orientation` | ~400 |
| `living-and-working-with-ai` (open-Q on cognitive atrophy) | `cognitive-atrophy-and-ai` | ~300 |
| `disposition-vs-knowledge` (open-Q on wisdom traditions) | `wisdom-traditions-practice-vs-doctrine` | ~350 |
| `health-equity` (open-Q on IP and health equity) | `intellectual-property-and-health-equity` | ~150 |
| `experimental-mindset` (open-Q on financial stability) *(NEW — 2026-06-08)* | `financial-stability-while-experimenting` | ~200 |
| `experimental-mindset` (open-Q on privilege) *(NEW — 2026-06-08)* | `experimental-mindset-and-privilege` | ~150 |

**Additional probable instances** from the 2026-06-07 weekly pass (not yet verified by full read): `living-and-working-with-ai` (ai-productivity-gains-distribution), `adaptive-leadership` (adaptive-challenge-diagnosis), `mental-models-and-multidisciplinary-thinking` (munger-vs-behavioral-economics), `health-equity` (health-equity-without-redistribution), `economic-literacy` (economic-literacy-at-scale + scanlon-optimism-limits). Total probable Case 2 instances: ~14–15. Verification requires reading each source page's Open Questions section.

**Proposed for each confirmed case:** Compress the inline answer to a 1–2 sentence summary + wikilink to the concept page.

### Case 3 · `slow-productivity-and-ai-craft` / `cognitive-atrophy-and-ai` — Mechanism section overlap *(flagged 2026-06-07)*
~35% body overlap in "The Atrophy Mechanism" section, "Where AI Actually Helps" table, and core heuristic. Proposed: compress mechanism section to 2-sentence cross-reference + `[[cognitive-atrophy-and-ai]]` link; retain Newport-specific content only. Owner approval required before trimming.

---

## Surfacing for the dashboard
_Top 10+ pages by salience score (inbound edges × body depth bonus; feeds `wiki-dashboard.html` node sizing)._

Inbound-link counts re-verified via ripgrep (unique files, excluding self-references). Vault grew from 82 to 90 pages since last run.

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| **1** | `disposition-vs-knowledge` | **20** | ~900 words | **New #1 — overtook `mental-models` this run.** Crown jewel: richest body among top-10; bridges Munger, Stoicism, AI, and education clusters. 3 inbound links added via weekly-pass new concept pages (`munger-vs-behavioral-economics`, `adaptive-challenge-diagnosis`, others). Well-developed; no enrichment needed. |
| 2 | `mental-models` | 18 | ~350 words | **Highest-centrality thin page — #1 enrichment target.** Dropped to #2 by link count but body remains far below what centrality warrants. |
| 3 | `health-equity` | 16 | ~400 words | Rose from 13 to 16 inbound (new concept pages add links). Body still thin relative to centrality; primary enrichment target in the health/justice cluster. |
| 4 | `cognitive-atrophy-and-ai` | 13 | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| 5 | `mental-models-and-multidisciplinary-thinking` | 11 | ~1500 words (topic) | Well-developed topic page; new `munger-vs-behavioral-economics` concept page extends it. |
| 5 (tied) | `slow-productivity` | 11 | ~800+ words (topic) | Rose from 9 to 11. Central productivity hub; topic page substantive. |
| 7 | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; contradiction with `mathematics-education` remains open (row 2026-06-07). |
| 7 (tied) | `charlie-munger` | 10 | ~350 words | Central person page; body unexpectedly thin for centrality. Enrichment candidate. |
| 7 (tied) | `latticework-pedagogy` | 10 | ~1000 words | Well-developed; bridges Munger cluster with behavioral science. |
| 10 | `jagged-frontier` | 9 | ~300 words | Very thin body vs. high centrality — **#2 AI-cluster enrichment priority**. |
| 10 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |
| 10 (tied) | `living-and-working-with-ai` | 9 | ~1500+ words (topic) | High centrality, well-developed. |
| 10 (tied) | `experimental-mindset` | 9 | ~1200 words (topic) | High centrality, well-developed. Open questions now answered. |

_Note: `stoic-virtues` (7 inbound) and `superforecasting` (7 inbound) sit just below top-10; both adequately developed. `tiny-experiments` at 8 inbound is well-developed. New concept pages (health-equity-without-redistribution, economic-literacy-at-scale, scanlon-optimism-limits, munger-vs-behavioral-economics, financial-stability-while-experimenting, experimental-mindset-and-privilege, ai-productivity-gains-distribution, adaptive-challenge-diagnosis) all have 1–2 inbound links and will accumulate over time._

---

## Newly surfaced this run

**2 new contradictions (Stage 1):**

1. **`superforecasting` vs. `munger-vs-behavioral-economics`** — `superforecasting` positions Tetlock's fox/hedgehog finding as an empirical *validation* of Munger's latticework intuition; `munger-vs-behavioral-economics` positions Tetlock's probabilistic-updating approach as *contrasting* with Munger's confident synthesis. Both pages cite the same Tetlock research; readers encounter opposite conclusions about whether Tetlock supports or problematizes the Munger framework. See `system/contradictions.md` row 2026-06-08.

2. **`vibecession` vs. `scanlon-optimism-limits`** — `vibecession` explains the consumer sentiment gap through behavioral distortion and media amplification (implying the vibes are depressed relative to genuine conditions); `scanlon-optimism-limits` argues the gap may instead reflect accurate distributional perception by those below the median income (implying consumer sentiment is *more* informative than aggregate indicators). Distinct from the 2026-06-04 Scanlon/Stockman contradiction, which concerns indicator reliability. See `system/contradictions.md` row 2026-06-08.

**Case 2 near-duplicate pattern expands (Stage 2):** Two new confirmed instances — `experimental-mindset`'s inline answers for the financial-stability and privilege open questions remain in the parent page despite being extracted into `financial-stability-while-experimenting` and `experimental-mindset-and-privilege`. Probable total: ~14–15 instances across all new concept pages from the weekly pass. Owner approval required for each trim.

**Rankings updated (Stage 3):** `disposition-vs-knowledge` is now #1 by inbound-link count (20, up from 17). `health-equity` rises to 16 (from 13). `slow-productivity` rises to 11 (from 9). `mental-models` drops to #2 by count (18) but remains #1 enrichment priority due to its thin body. Two uningested Munger PDFs remain the vault's highest-priority ingest items.
