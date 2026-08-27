---
title: "Chained Recursive Language Models for Multi-Iteration Reasoning"
source: "https://arxiv.org/html/2608.05124v1"
author: "Purbesh Mitra, Sennur Ulukus"
published: "2026-08-05"
created: 2026-08-07
description: "Long context reasoning in large language models (LLMs) is usually constrained by the fact that a single inference trajectory has to simultaneously explore the context, store intermediate state, verify evidence, and produce the final answer. This becomes particularly difficult in tasks that require extraction, counting, ordering, or multi-hop reasoning, where an early mistake can propagate until the final response. I…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/reasoning
  - keyword/machine-learning
---

# Chained Recursive Language Models for Multi-Iteration Reasoning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.05124v1)
- published:: 2026-08-05
- updated:: 2026-08-05
- arxiv_id:: 2608.05124v1
- pdf:: https://arxiv.org/pdf/2608.05124v1
- categories:: cs.CL, cs.AI, cs.IT, cs.LG, eess.SP

## Abstract / Summary
Long context reasoning in large language models (LLMs) is usually constrained by the fact that a single inference trajectory has to simultaneously explore the context, store intermediate state, verify evidence, and produce the final answer. This becomes particularly difficult in tasks that require extraction, counting, ordering, or multi-hop reasoning, where an early mistake can propagate until the final response. In this work, we propose Chained Recursive Language Models (Chained RLM), an inference-time architecture, in which the same underlying model is called repeatedly as a sequence of fresh reasoning roots. Each root receives the original problem and context, but does not inherit the full conversational history. Instead, it receives a compact plain-text summary, a plain-text blackboard, and some durable task-specific artifacts written by predecessor roots. The motivation is to manage the context by chopping into partial tasks rather than one large inference response; in each staged computation, intermediate artifacts can be inspected, corrected, and extended by a later fresh inference by the same model. We describe the system model, handoff mechanism, artifact workspace, and evaluation protocol for this system. We study when fresh-context artifact continuation gives a measurable gain in accuracy over direct LLM answering even with recursive tool-calling.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.05124v1)
- [PDF](https://arxiv.org/pdf/2608.05124v1)
- [Recursive Language Models](https://arxiv.org/abs/2512.24601) (2025, citations: 65)
- [Oolong: Evaluating Long Context Reasoning and Aggregation Capabilities](https://arxiv.org/abs/2511.02817) (2025, citations: 25)
- [MOTIF: Modular Thinking via Reinforcement Fine-tuning in LLMs](https://arxiv.org/abs/2507.02851) (2025, citations: 4)
- [Agentic Large Language Models, a survey](https://arxiv.org/abs/2503.23037) (2025, citations: 159)
- [LongBench v2: Towards Deeper Understanding and Reasoning on Realistic Long-context Multitasks](https://arxiv.org/abs/2412.15204) (2024, citations: 330)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/reasoning #keyword/machine-learning
