---
title: "Jagged Frontier"
date: 2026-05-18
tags: [ai, capability, llm, mental-model]
related: [[living-and-working-with-ai]], [[ethan-mollick]], [[large-language-models]], [[mapping-the-jagged-frontier]]
connections:
  - type: applies-to
    target: mapping-the-jagged-frontier
---

# Jagged Frontier

A metaphor for the irregular, invisible boundary of AI capability — developed by Ethan Mollick and co-authors based on empirical research into LLM performance on professional tasks.

## Definition

Imagine a fortress wall with irregular battlements: some towers jut far out into the countryside (tasks AI handles easily), while others fold back toward the castle interior (tasks AI handles poorly). The wall represents AI capability, and its key feature is that it is **invisible** — you cannot tell from the outside which tasks are on which side.

## Key Insight

Tasks that seem equally difficult may be on opposite sides of the frontier:
- Writing a sonnet → easy for AI (inside the frontier)
- Writing an exactly 50-word poem → surprisingly hard (outside the frontier, because LLMs tokenize rather than count words)
- Generating creative ideas → easy
- Basic arithmetic without a calculator → often unreliable

The counterintuitive distribution means that **experience-based mapping is essential** — you cannot predict where the frontier falls for your specific domain without experimenting.

## Implications

1. **Individual advantage** — a worker in a specific domain who systematically experiments with AI for their tasks becomes the world's leading expert on AI in that domain, because no dataset or research team has their specific knowledge
2. **Risk of misapplication** — tasks that feel like they should be inside the frontier may be outside it; over-reliance leads to confident errors (hallucinations, miscounts, fabricated citations)
3. **Evolving boundary** — the frontier shifts with each model generation; what is outside today may be inside tomorrow, requiring continuous re-mapping

## Research Basis

Mollick and co-authors conducted studies with management consultants using AI for professional tasks. They found that AI helped most on tasks within the frontier but actively harmed performance when consultants over-relied on AI for tasks outside it — the AI's confident errors led consultants astray.

## Related Topics
- [[living-and-working-with-ai]] — the broader context of working with AI
- [[large-language-models]] — the technology whose capabilities the frontier describes
