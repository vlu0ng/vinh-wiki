---
title: "Contradictions Registry"
date: 2026-06-02
tags: [system, registry]
---

# Contradictions Registry

Tracks conflicting claims detected across `wiki/` pages by the `vinh-wiki-dream-cycle` skill. Contradictions are **surfaced, never silently resolved** — the user decides how to reconcile. The `status` column provides idempotency: rows marked `resolved` or `accepted` are not re-flagged.

`status` values: `open` (newly detected) · `accepted` (a genuine tension worth keeping — both views stand) · `resolved` (user reconciled the pages) · `dismissed` (false positive).

## Entries

| Date | Page A | Page B | Nature of conflict | Status |
|---|---|---|---|---|
| 2026-06-02 | `cognitive-atrophy-and-ai` | `slow-productivity-and-ai-craft` | `cognitive-atrophy-and-ai` states "for experts: aggressive AI augmentation is safer — the underlying expert intuition is already built and can catch AI errors." `slow-productivity-and-ai-craft` states "AI assistance that produces quality outputs without developing the practitioner's skill stalls the flywheel: the work looks good but the artist hasn't grown" — implying even senior practitioners need ongoing productive struggle. Conflict: does expertise exempt a practitioner from ongoing atrophy risk, or must even experts guard against craft stagnation? | open |
| 2026-06-02 | `ai-in-education` | `ai-tutoring-and-human-motivation` | The open-question answer in `ai-in-education` says "AI can emulate relational scaffolding (patience, personalized framing) and lower social pressure for low-stakes failure, supporting a growth-mindset." `ai-tutoring-and-human-motivation` says "students eventually detect this simulation, which can lead to a flattening of motivation over time." Conflict: does AI tutoring's relational emulation work, or does its eventual detection by students undermine the motivational goal? | open |
| 2026-06-03 | `stoic-virtues` | `wisdom-traditions-practice-vs-doctrine` | `stoic-virtues` states "Virtue, in the Stoic sense, is not a feeling or disposition but a practice — something you do, not something you have." `wisdom-traditions-practice-vs-doctrine` uses Stoic morning exercises as the primary example of "dispositional development," explicitly framing Stoic practice as a vehicle for building stable dispositions. `disposition-vs-knowledge` reinforces the dispositional reading by citing Epictetus's practice emphasis as evidence that practice builds behavioral character. Conflict: is Stoic virtue (a) categorically not a disposition — an ongoing enactment with no stable "state" to acquire — or (b) a practice that progressively builds a stable dispositional orientation? The first reading is the strict Stoic philosophical position; the second is the modern behavioral/Aristotelian reading used by the other two pages. | open |
| 2026-06-04 | `vibecession` + `economic-literacy` | `bubble-finance` + `crony-capitalism-and-monetary-deformation` | `vibecession` and `economic-literacy` (Scanlon) use "hard indicators" (GDP, unemployment, corporate earnings) as a reliable baseline measuring genuine economic health: "Hard indicators… are technically healthy." The vibecession is precisely the gap between this real performance and depressed consumer sentiment. `bubble-finance` (Stockman) explicitly states those same indicators are distorted: "Real-economy weakness — financial gains mask stagnant productivity, wages, and productive investment" — headline GDP and corporate earnings partly reflect asset-price reflation and suppressed interest rates, not genuine productive output. Conflict: if Stockman is correct, Scanlon's "technically healthy" premise is suspect — the gap the vibecession describes is not between good real performance and bad sentiment, but between artificially inflated headline numbers and a lived reality that consumer sentiment may already be tracking accurately. The two authors are using the same data to reach opposite conclusions about what it means. | open |
