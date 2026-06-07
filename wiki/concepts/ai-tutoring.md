---
title: "AI Tutoring"
date: 2026-05-19
tags: [education, AI, LLMs, personalized-learning]
related: [[ai-in-education]], [[sal-khan]], [[large-language-models]], [[jagged-frontier]], [[cognitive-atrophy-and-ai]]
connections:
  - type: critiqued-by
    target: cognitive-atrophy-and-ai
---

# AI Tutoring

The use of large language models to provide personalized, interactive tutoring at scale — the closest technological
approach to Benjamin Bloom's "2 Sigma" ideal of one-on-one instruction.

## The Bloom 2 Sigma Problem

Benjamin Bloom (1984) documented that students tutored one-on-one performed 2 standard deviations above
classroom-taught peers. The catch: there aren't enough human tutors to deliver this at scale and cost. AI tutoring
is the first plausible path to solving Bloom's problem.

## Design Principles (from Khanmigo)

- **Socratic over answer-giving**: Prompt the AI to ask leading questions, not provide solutions. GPT-4's
  steerability (vs. GPT-3.5) made this feasible — earlier models would revert to giving answers no matter the prompt.
- **Role maintenance**: AI can take on consistent personas (Socratic tutor, historical figure, debate partner)
  throughout a session
- **Safety by design**: Guardrails for minors, appropriate tone, avoidance of harmful content — must be designed in
  before deployment, not added after

## Capabilities Beyond Tutoring

Modern AI tutoring systems can:
- Role-play historical and literary figures for immersive learning
- Serve as debate opponents (student argues a position; AI argues the other side)
- Act as guidance counselors and career coaches
- Generate practice assessments adapted to individual progress
- Help teachers with lesson planning, student progress analysis, and administrative tasks

## Risks and Limits

- **Cognitive atrophy**: If students use AI to *avoid* thinking rather than to *deepen* it, the tutoring
  becomes counterproductive. See [[cognitive-atrophy-and-ai]].
- **Jagged frontier failures**: AI may be excellent on some topics and quietly wrong on others; students may
  not be able to detect the errors. See [[jagged-frontier]].
- **Equity**: High-quality AI tutoring requires device access, internet connectivity, and often subscription fees —
  potentially widening rather than closing educational gaps unless deployed intentionally.

## Related Topics
- [[ai-in-education]] — Khan's full argument
- [[large-language-models]] — the underlying technology
- [[growth-mindset]] — Dweck's framework suggests AI tutoring works best when students approach it with
  a growth orientation, using failure as information
