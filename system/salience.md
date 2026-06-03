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

**2026-06-03** — Full dream-cycle pass (nightly). 69 wiki pages analyzed (48 concepts, 15 topics, 19 people). No new pages have been added since the 2026-06-02 run. Inbound-edge counts, body-depth estimates, and staleness values are unchanged. One new contradiction was detected (Stage 1): `stoic-virtues` vs. `wisdom-traditions-practice-vs-doctrine` on whether Stoic practice constitutes or merely produces a disposition. No new near-duplicates detected (Stage 2). Salience rankings carry forward from the prior run.

---

## Under-developed but central
_Pages with many inbound edges but a thin body — highest enrichment leverage._

| Page | Est. inbound links | Est. body (words) | Why it matters |
|---|---|---|---|
| `jagged-frontier` | 7 | ~300 | Anchor concept for all AI pages; referenced by `ai-tutoring`, `cognitive-atrophy-and-ai`, `living-and-working-with-ai`, `mapping-the-jagged-frontier`, `ai-tutoring-and-human-motivation`, `ai-in-education`, `large-language-models`. Body is a compact definition; lacks worked examples, domain breakdown, and open questions. **Top enrichment priority in the vault.** |
| `large-language-models` | 6 | ~250 | Foundational anchor for the AI cluster; referenced by nearly every AI-related page. Body is a brief properties list; lacks transformer history, capability trajectory, societal framing, and failure modes. |
| `mental-models` | 7 | ~350 | Most-linked concept page overall; referenced by `stoic-justice`, `stoic-virtues`, `disposition-vs-knowledge`, `latticework-pedagogy`, `latticework-failure-modes`, `focus-vs-orientation`, `the-one-thing`. Model table is useful but the page lacks depth on how the latticework is built, known failure modes, and the relationship to behavioral economics. |
| `focusing-question` | 4 | ~250 | Referenced by `the-one-thing`, `focus-vs-orientation`, `experiment-theater`, and `experimental-mindset`. The page covers the mechanics well but has no open questions, no failure modes, and no worked cross-domain examples. |
| `adaptive-vs-technical-challenges` | 3 | ~400 | Referenced by `adaptive-leadership` and `adaptive-leadership-and-psychological-safety`; core Heifetz diagnostic tool. Body is adequate but lacks the "mixed challenge" worked examples and the diagnostic failure modes that would make it independently useful. |

---

## Stale high-value
_Central pages not touched in a while — candidates to revisit._

All pages share the same creation band (2026-05-18 to 2026-05-20, now ~14–16 days old). Staleness does not yet differentiate within this vault. Re-run this section after the next enrichment pass.

**Exception — uningested raw articles (aging gap):** Two PDF files in `raw/articles/` remain uningested:
- `raw/articles/charlie munger - mental models Part 1.pdf`
- `raw/articles/charlie munger mental Models Part 2.pdf`

These are high-probability transcripts of Munger's 1994 USC "Elementary Worldly Wisdom" talk or related primary writings — the foundational source for the latticework framework. Pages `mental-models`, `latticework-pedagogy`, `munger-disposition-formation`, and `mental-models-and-multidisciplinary-thinking` have been built from *Poor Charlie's Almanack* (epub) and secondary references; these PDFs may contain primary material not yet captured. Both have been in the ingest queue since 2026-06-02 at high priority.

---

## Near-duplicate flags (Stage 2)
_Unchanged from 2026-06-02 run. No new near-duplicates detected. Owner approval required before any merge or trim._

### Case 1 · `ai-tutoring` / `ai-tutoring-and-human-motivation` — Overlapping opening sections
Both pages open with an independent Bloom's 2 Sigma exposition and a description of Khanmigo's Socratic design. `ai-tutoring-and-human-motivation`'s first section ("The Bloomian Promise…") covers Infinite Patience, Perfect Adaptability, Socratic Inquiry, and Low-Stakes Failure — substantially repeating `ai-tutoring`'s Design Principles section before diverging into the relational/motivation analysis. Estimated overlap: ~25% of `ai-tutoring-and-human-motivation`'s body.

**Proposed:** Trim `ai-tutoring-and-human-motivation`'s opening to a 2-sentence cross-reference to `ai-tutoring`, then pick up with the relational-gap analysis. The concept page carries the deeper treatment; the opener should signal the dependency, not re-explain it.

### Case 2 · Structural pattern: 6 topic pages contain inline answers that duplicate extracted concept pages
When open questions were answered and extracted into dedicated concept pages, the originals were not trimmed. This produces near-duplicate content at every affected topic page:

| Topic page | Duplicated in concept page | Estimated inline word count |
|---|---|---|
| `experimental-mindset` (open-Q on experiment theater) | `experiment-theater` | ~350 |
| `adaptive-leadership` (open-Q on psychological safety) | `adaptive-leadership-and-psychological-safety` | ~300 |
| `stoic-justice` (open-Q on systemic injustice) | `stoicism-and-systemic-injustice` + `stoic-truth-telling-and-tact` | ~450 combined |
| `the-one-thing` (open-Q on tunnel vision) | `focus-vs-orientation` | ~400 |
| `living-and-working-with-ai` (open-Q on cognitive atrophy) | `cognitive-atrophy-and-ai` | ~300 |
| `disposition-vs-knowledge` (open-Q on wisdom traditions) | `wisdom-traditions-practice-vs-doctrine` | ~350 |

**Proposed for each:** Compress the inline answer to a 1–2 sentence summary + wikilink to the concept page. The concept page becomes canonical; the topic page retains the question header and a brief pointer. **Owner must approve each compression individually.**

---

## Surfacing for the dashboard
_Top 10 pages by salience score (inbound edges × body depth bonus; feeds `wiki-dashboard.html` node sizing)._

| Rank | Page | Inbound est. | Body depth | Salience notes |
|---|---|---|---|---|
| 1 | `disposition-vs-knowledge` | 10+ | ~900 words | Crown jewel — most-linked concept, richest body; bridges Munger, Stoicism, AI, and education clusters |
| 2 | `mental-models` | 7+ | ~350 words | Highest centrality; body underweight relative to link count — prime enrichment target |
| 3 | `cognitive-atrophy-and-ai` | 6 | ~800 words | Dense, well-developed; bridges AI cluster with productivity and education |
| 4 | `large-language-models` | 6 | ~250 words | Very high centrality, very thin — 2nd-highest enrichment leverage |
| 5 | `jagged-frontier` | 7 | ~300 words | Highest enrichment leverage of all: link count rivals `mental-models` but body is barely a definition |
| 6 | `growth-mindset` | 6 | ~400 words | Bridges education, AI, and experimental-mindset clusters |
| 7 | `latticework-pedagogy` | 5+ | ~700 words | Dense and well-developed; core of the Munger/wisdom cluster |
| 8 | `health-equity` | 5+ | unknown | Anchor for TB + illness cluster; need body-depth check |
| 9 | `romanticization-of-illness` | 4–5 | ~600 words | Well-developed; central to the illness narrative cluster |
| 10 | `slow-productivity` | 4–5 | unknown | Anchor for productivity cluster; need body-depth check |

_Note: `jagged-frontier` ranks #5 on raw link count but is effectively the **top enrichment priority** given the gap between centrality (7 inbound) and body depth (~300 words). `mental-models` is the same profile at rank 2._

---

## Newly surfaced this run

**New contradiction (Stage 1):** `stoic-virtues` vs. `wisdom-traditions-practice-vs-doctrine`

`stoic-virtues` states that Stoic virtue is "not a feeling or **disposition** but a practice"; `wisdom-traditions-practice-vs-doctrine` frames Stoic exercises as the primary example of building stable *dispositional* character. These two pages use the same concept with opposite valences. The tension is philosophically real (strict Stoic action-theory vs. Aristotelian hexis/habituation reading) and deserves owner attention before new Stoicism-related content is added. See `system/contradictions.md` row dated 2026-06-03 for the full entry.
