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
