---
title: "Partition, Prompt, Aggregate: Statistical Self-Consistency in Language Models"
source: "https://arxiv.org/html/2607.15277v1"
author: "Patrik Wolf, Thomas Kleine Buening, Andreas Krause, Celestine Mendler-Dünner"
published: "2026-07-16"
created: 2026-07-17
description: "Tests whether LLM estimates obey the law of total probability across population partitions; finds widespread self-consistency failures and a ‘macro fallacy’ where fine-grained aggregates beat direct population estimates."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/evaluation
  - keyword/reasoning
  - keyword/llm
---

# Partition, Prompt, Aggregate: Statistical Self-Consistency in Language Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15277v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15277v1
- pdf:: https://arxiv.org/pdf/2607.15277v1
- categories:: cs.CL

## Abstract / Summary
If in-context learning is conditional inference, LLM estimates should obey probabilistic identities such as the law of total probability. Using binary trees to partition populations and aggregating subpopulation prompts, the authors find widespread self-consistency violations across domains and frontier models. Persona prompting exhibits a macro fallacy: estimates reconstructed from finer subpopulations often match human references better than direct population prompts. Models hold relevant subpopulation knowledge but fail to propagate it into aggregates. Statistical self-consistency is proposed as a reference-free evaluation criterion.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15277v1)
- [PDF](https://arxiv.org/pdf/2607.15277v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/evaluation #keyword/reasoning #keyword/llm
