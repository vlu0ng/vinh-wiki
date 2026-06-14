---
title: "Large Language Models"
date: 2026-05-18
tags: [ai, machine-learning, technology, nlp]
related: [[living-and-working-with-ai]], [[ethan-mollick]], [[jagged-frontier]], [[general-purpose-technology]], [[ai-tutoring]], [[cognitive-atrophy-and-ai]]
connections:
  - type: related
    target: ethan-mollick
  - type: example-of
    target: general-purpose-technology
  - type: applies-to
    target: ai-tutoring
  - type: related
    target: cognitive-atrophy-and-ai
---

# Large Language Models

Neural networks trained on vast text corpora to predict the next token in a sequence; the underlying technology behind ChatGPT, Claude, Gemini, and related systems.

## Key Properties

- **Scale** — trained on trillions of tokens of text; model size (parameters) has grown by roughly an order of magnitude per year since the transformer architecture emerged in 2017
- **Emergence** — capabilities arise non-linearly with scale; abilities like reasoning, code generation, and multilingual translation were not explicitly trained but emerged from scale and architecture
- **Stochastic** — outputs are probabilistic, not deterministic; the same prompt can produce different responses; there is no single "correct" answer
- **Alien cognition** — LLMs process language in fundamentally different ways than humans (via tokens and attention weights, not meaning), yet produce outputs that mimic human reasoning closely enough to pass the Turing Test
- **No persistent memory (by default)** — each conversation context is typically bounded; LLMs do not learn from interactions in real time (though fine-tuning can update a model)

## Capability Profile (as of 2024)
- Excellent: writing, summarization, code generation, idea generation, translation, question answering, structured output
- Good: complex reasoning (with chain-of-thought), simple math, research synthesis
- Weak: exact counting, precise arithmetic without tools, persistent state across sessions, factual reliability (hallucination risk)

## The Jagged Frontier
See [[jagged-frontier]] — the irregular and counterintuitive boundary between tasks LLMs handle well vs. poorly.

## Societal Implications
Mollick argues LLMs are a [[general-purpose-technology|General Purpose Technology]] that will transform cognitive work across all domains. Early productivity studies show 20–80% improvement on knowledge work tasks — far exceeding past GPT impact on physical labor.

## Related Topics
- [[living-and-working-with-ai]] — how to work with LLMs effectively
- [[jagged-frontier]] — LLM capability boundaries
