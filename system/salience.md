---
title: "Salience Digest"
date: 2026-06-07
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

**2026-06-07** — Full dream-cycle pass (nightly). 82 wiki pages analyzed (48 concepts, 15 topics, 19 people). No new wiki pages added since 2026-06-04. Vault structurally stable. Inbound-link counts re-verified via ripgrep unique-file pattern-match on `[[slug` prefix across all wiki/ files. **Stage 1:** 1 new contradiction detected (`growth-mindset` vs. `mathematics-education` on empirical confidence in growth-mindset interventions); 4 prior contradictions remain open (5 total). **Stage 2:** 1 new near-duplicate case detected (`slow-productivity-and-ai-craft` vs. `cognitive-atrophy-and-ai` — ~35% body overlap); 8 prior flagged cases remain pending owner approval (9 total). **Stage 3:** Rankings confirmed stable — `mental-models` remains #1 (18 inbound, ~350 words) and the single highest-leverage enrichment target in the vault.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `mental-models` | 18 | ~350 | **#1 enrichment priority in the vault.** Highest inbound count of any page; body remains a thin properties list + model table. Referenced by every major cluster. Lacks: latticework construction process, known failure modes (see `latticework-failure-modes`), behavioral-economics convergence, cross-domain worked examples. Two uningested Munger PDFs in `raw/articles/` are the primary source for filling this gap. |
| `health-equity` | 13 | ~400 | **3rd-most-linked page in the vault.** Body thinner than centrality warrants. One unanswered open question remains ("Is health equity achievable without global wealth redistribution?"). Inline IP-answer near-duplicate case also pending trim. |
| `jagged-frontier` | 9 | ~300 | Anchor concept for all AI pages; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`. Body is a compact definition; lacks worked domain examples, BCG study details, frontier-movement dynamics, and open questions. |
| `large-language-models` | 9 | ~250 | Foundational anchor for the AI cluster; body is a brief properties list; lacks transformer history, capability trajectory, failure mode catalog, societal framing. |
| `charlie-munger` | 10 | ~350 | Central person page for the Munger/latticework cluster (10 inbound). Body is a short biography + key contributions list — well below what centrality warrants. Would benefit from Munger's key talks, disposition formation timeline, and cross-links to `latticework-failure-modes`, `munger-disposition-formation`, `latticework-feedback-loops-outside-investing`. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. Covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share the same creation band (2026-05-18 to 2026-06-02, now 5–20 days old). Staleness does not yet differentiate meaningfully within this vault; all pages are recent. Re-run this section after the next enrichment pass.

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
When open questions were answered and extracted into dedicated concept pages, the originals were not trimmed. **7 cases (unchanged from prior run).** Owner approval required for each compression individually.

| Page | Duplicated in concept page | Estimated inline word count |
|---|---|---|
| `experimental-mindset` (open-Q on experiment theater) | `experiment-theater` | ~350 |
| `adaptive-leadership` (open-Q on psychological safety) | `adaptive-leadership-and-psychological-safety` | ~300 |
| `stoic-justice` (open-Q on systemic injustice) | `stoicism-and-systemic-injustice` + `stoic-truth-telling-and-tact` | ~450 combined |
| `the-one-thing` (open-Q on tunnel vision) | `focus-vs-orientation` | ~400 |
| `living-and-working-with-ai` (open-Q on cognitive atrophy) | `cognitive-atrophy-and-ai` | ~300 |
| `disposition-vs-knowledge` (open-Q on wisdom traditions) | `wisdom-traditions-practice-vs-doctrine` | ~350 |
| `health-equity` (open-Q on IP and health equity) | `intellectual-property-and-health-equity` | ~150 |

**Proposed for each:** Compress the inline answer to a 1–2 sentence summary + wikilink to the concept page. The concept page becomes canonical; the page retains the question header and a brief pointer.

### Case 3 · `slow-productivity-and-ai-craft` / `cognitive-atrophy-and-ai` — Mechanism section overlap *(NEW — 2026-06-07)*
`slow-productivity-and-ai-craft`'s "The Atrophy Mechanism" section directly restates the Dreyfus model argument from `cognitive-atrophy-and-ai` (practice reps → expert intuition → atrophy risk for novices). The "Where AI Actually Helps" table closely mirrors `cognitive-atrophy-and-ai`'s "Key Distinction" table. The heuristic quote ("use AI to expand the range of what you can do; avoid using AI to bypass the development of the judgment required to do it well") is reproduced verbatim. Estimated overlap: ~35% of `slow-productivity-and-ai-craft`'s body.

**Proposed:** Compress "The Atrophy Mechanism" section to a 2-sentence summary + `[[cognitive-atrophy-and-ai]]` cross-reference; collapse the duplicate table to a brief note pointing to the source page. Retain only the Newport-specific application (the three principles' differential vulnerability to AI disruption, and the slow-productivity flywheel argument). Owner approval required before trimming.

---

## Surfacing for the dashboard
_Top 10 pages by salience score (inbound edges × body depth bonus; feeds `wiki-dashboard.html` node sizing)._

Inbound-link counts re-verified via ripgrep (unique files, excluding self-references). No new pages added since 2026-06-04.

| Rank | Page | Inbound (confirmed) | Body depth | Salience notes |
|---|---|---|---|---|
| 1 | `mental-models` | 18 | ~350 words | **Highest centrality in vault** — thin body makes it the single highest-leverage enrichment target. |
| 2 | `disposition-vs-knowledge` | 17 | ~900 words | Crown jewel — 2nd-most-linked; richest body; bridges Munger, Stoicism, AI, and education clusters. Well-developed; no enrichment needed. |
| 3 | `health-equity` | 13 | ~400 words | 3rd-most-linked page; body thin relative to centrality. Primary enrichment target in the health/justice cluster. |
| 4 | `cognitive-atrophy-and-ai` | 12 | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education. |
| 5 | `mental-models-and-multidisciplinary-thinking` | 11 | ~1500 words (topic) | Well-developed topic page; centrality is high but body likely adequate. |
| 6 | `growth-mindset` | 10 | ~400 words | Bridges education, AI, and experimental-mindset clusters; newly flagged in contradiction with `mathematics-education` (new row in contradictions.md). Candidate for a nuance pass adding replication-uncertainty framing to `mathematics-education` or vice versa. |
| 7 | `charlie-munger` | 10 | ~350 words | Central person page for the Munger cluster; body unexpectedly thin for centrality level. Candidate for enrichment on next ingest pass. |
| 8 | `slow-productivity` | 9 | ~800+ words (topic) | Central productivity hub; topic page substantive. |
| 9 | `latticework-pedagogy` | 9 | ~1000 words | Well-developed; bridges Munger cluster with behavioral science. |
| 10 | `jagged-frontier` | 9 | ~300 words | Very thin body vs. high centrality — **#2 AI-cluster enrichment priority**. |
| 10 (tied) | `large-language-models` | 9 | ~250 words | Thinnest body at this centrality level — **#3 AI-cluster enrichment priority**. |

_Note: `living-and-working-with-ai` (8 inbound, topic, ~1500 words) also ranks high but is well-developed. `inversion` and `bubble-finance` at 7 inbound each sit just below the top 10 but are adequately developed._

---

## Newly surfaced this run

**1 new contradiction (Stage 1):** `growth-mindset` vs. `mathematics-education` — `growth-mindset` documents replication uncertainty and structural critique of the framework, while `mathematics-education` applies it as settled educational science without caveat. See `system/contradictions.md` row 2026-06-07.

**1 new near-duplicate case (Stage 2):** `slow-productivity-and-ai-craft` vs. `cognitive-atrophy-and-ai` — ~35% body overlap in mechanism sections and key heuristic table. Flagged as Case 3 in the near-duplicate registry above. Owner approval required before any trimming.

**Salience rankings stable (Stage 3):** Inbound-link counts re-verified via ripgrep; rankings unchanged from 2026-06-06. `mental-models` remains #1 (18 inbound by this run's unique-file count, consistent with prior counts). `charlie-munger` newly noted as thin relative to its 10-inbound centrality. Two uningested Munger PDFs remain the highest-priority ingest items.
