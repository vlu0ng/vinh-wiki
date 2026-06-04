---
title: "Salience Digest"
date: 2026-06-03
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

**2026-06-04** — Full dream-cycle pass (nightly). 82 wiki pages analyzed (48 concepts, 15 topics, 19 people). No new wiki pages have been added since the 2026-06-03 run. This pass completed a **full vault-wide inbound-link scan** for the first time since the vault reached its current size; prior estimates were based on partial scans and are now significantly revised upward. One new contradiction was detected (Stage 1): `vibecession`/`economic-literacy` vs. `bubble-finance`/`crony-capitalism-and-monetary-deformation` on whether headline economic indicators are reliable baselines or themselves distorted by bubble finance. One new near-duplicate case detected (Stage 2): `health-equity` inline IP-answer duplicated by `intellectual-property-and-health-equity` (7th case of the structural pattern). `health-equity` newly elevated to 3rd-most-linked page in the vault (13 inbound). Two new ingest-queue entries added.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | 19 | ~350 | **#1 enrichment priority in the vault.** Highest inbound count of any page (full scan revision: 7+ → 19); body remains a thin properties list + model table. Referenced by every major cluster. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence, cross-domain worked examples. |
| `health-equity` | 13 | ~400 | **Newly elevated priority.** Full scan revealed 13 inbound links (vs. 5+ estimated), making it the 3rd-most-linked page in the vault. Body is thinner than this centrality warrants. One unanswered open question remains ("Is health equity achievable without global wealth redistribution?"). Inline IP-answer near-duplicate case also pending trim. |
| `jagged-frontier` | 9 | ~300 | Anchor concept for all AI pages; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; tied with `jagged-frontier` at 9 inbound (revised up from 6). Body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. The page covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share the same creation band (2026-05-18 to 2026-06-02, now 2–17 days old). Staleness does not yet differentiate meaningfully within this vault; all pages are recent. Re-run this section after the next enrichment pass.

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
When open questions were answered and extracted into dedicated concept pages, the originals were not trimmed. **Updated this run: 7 cases identified (6 prior + 1 new).** Owner approval required for each compression individually.

| Page | Duplicated in concept page | Estimated inline word count |
|---|---|---|
| `experimental-mindset` (open-Q on experiment theater) | `experiment-theater` | ~350 |
| `adaptive-leadership` (open-Q on psychological safety) | `adaptive-leadership-and-psychological-safety` | ~300 |
| `stoic-justice` (open-Q on systemic injustice) | `stoicism-and-systemic-injustice` + `stoic-truth-telling-and-tact` | ~450 combined |
| `the-one-thing` (open-Q on tunnel vision) | `focus-vs-orientation` | ~400 |
| `living-and-working-with-ai` (open-Q on cognitive atrophy) | `cognitive-atrophy-and-ai` | ~300 |
| `disposition-vs-knowledge` (open-Q on wisdom traditions) | `wisdom-traditions-practice-vs-doctrine` | ~350 |
| `health-equity` (open-Q on IP and health equity) ← **new** | `intellectual-property-and-health-equity` | ~150 |

**Proposed for each:** Compress the inline answer to a 1–2 sentence summary + wikilink to the concept page. The concept page becomes canonical; the page retains the question header and a brief pointer.

---

## Surfacing for the dashboard
_Top 10 pages by salience score (inbound edges × body depth bonus; feeds `wiki-dashboard.html` node sizing)._

**Revised inbound-link counts** from full vault scan (2026-06-04). Prior estimates were significantly understated.

| Rank | Page | Inbound (revised) | Body depth | Salience notes |
|---|---|---|---|---|
| 1 | `mental-models` | 19 | ~350 words | **Highest centrality in vault** — revised up from 7+. Thin body makes it the single highest-leverage enrichment target. |
| 2 | `disposition-vs-knowledge` | 17 | ~900 words | Crown jewel — most-linked concept after `mental-models`; richest body; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. |
| 3 | `health-equity` | 13 | ~400 words | **Newly elevated** — 3rd-most-linked page; body thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| 4 | `cognitive-atrophy-and-ai` | 12 | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| 5 | `mental-models-and-multidisciplinary-thinking` | 11 | ~1500 words (topic) | Well-developed topic page; centrality is high but body likely adequate. |
| 6 | `slow-productivity` | 10 | ~800+ words (topic) | Central productivity hub; topic page likely substantive. |
| 7 | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; could be enriched with replications debate and structural-support nuance. |
| 8 | `charlie-munger` | 10 | unknown | Central person page; check body depth. |
| 9 | `jagged-frontier` | 9 | ~300 words | Very thin body vs. high centrality — **#2 enrichment priority** behind `mental-models`. |
| 10 | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level; effectively tied with `jagged-frontier` as a top AI-cluster enrichment target. |

_Note: `tuberculosis-and-global-health` (9 inbound, topic page, ~1000+ words) also sits at rank 9–10 but is well-developed. The thin-body targets — `jagged-frontier` and `large-language-models` — are the higher-leverage enrichment bets._

---

## Newly surfaced this run

**New contradiction (Stage 1):** `vibecession` + `economic-literacy` vs. `bubble-finance` + `crony-capitalism-and-monetary-deformation`

Scanlon's vibecession framework rests on the premise that hard economic indicators (GDP, unemployment, corporate earnings) are "technically healthy" — the gap between this real performance and depressed consumer sentiment is the vibecession. Stockman's bubble finance framework explicitly states those same indicators are distorted: "financial gains mask stagnant productivity, wages, and productive investment" — headline GDP and corporate earnings partly reflect asset-price reflation and Fed-suppressed interest rates, not genuine productive output. If Stockman is correct, the vibecession gap is not between good real performance and bad sentiment, but between artificially inflated headline numbers and a lived reality that consumer sentiment may already be accurately detecting. `economic-literacy`'s own open questions section flags the adjacent tension: "Scanlon's framing is optimistic (economies trend toward okay-ness). How does that hold up against structural inequality and climate risk?" See `system/contradictions.md` row dated 2026-06-04 for the full entry.

**New near-duplicate case (Stage 2):** `health-equity` — the inline answer to the IP open question in `health-equity`'s `## Open Questions` section (~150 words) duplicates content now in `intellectual-property-and-health-equity`. This is the 7th case of the structural inline-answer pattern first identified on 2026-06-02. Added to Stage 2 table above.

**Inbound-link count revision (Stage 3):** First full vault-wide scan completed on this run. Prior estimates were based on partial scans; revised counts are substantially higher for the most-linked pages: `mental-models` (7+ → 19), `disposition-vs-knowledge` (10+ → 17), `health-equity` (5+ → 13), `cognitive-atrophy-and-ai` (6 → 12), `large-language-models` (6 → 9), `jagged-frontier` (7 → 9). Salience rankings above reflect these corrections. `mental-models` is now unambiguously the #1 enrichment priority in the vault.
