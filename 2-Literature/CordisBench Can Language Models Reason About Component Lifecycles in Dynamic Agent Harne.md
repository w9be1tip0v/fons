---
title: "CordisBench: Can Language Models Reason About Component Lifecycles in Dynamic Agent Harnesses?"
source: "https://arxiv.org/html/2609.01600v1"
author: "Damien Sileo, Dimitri Kachler"
published: "2026-09-01"
created: 2026-09-03
description: "Dynamic agent harnesses let language models change the software that shapes their own execution. This flexibility brings a new reasoning burden: a local plugin change can propagate through dependencies and cleanup. We introduce CordisBench, a 1,200-question benchmark of this lifecycle reasoning. It combines a controlled formal setting with programs executed against Cordis, a runtime that manages component dependenci…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/agents
  - keyword/machine-learning
---

# CordisBench: Can Language Models Reason About Component Lifecycles in Dynamic Agent Harnesses?

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.01600v1)
- published:: 2026-09-01
- updated:: 2026-09-01
- arxiv_id:: 2609.01600v1
- pdf:: https://arxiv.org/pdf/2609.01600v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Dynamic agent harnesses let language models change the software that shapes their own execution. This flexibility brings a new reasoning burden: a local plugin change can propagate through dependencies and cleanup. We introduce CordisBench, a 1,200-question benchmark of this lifecycle reasoning. It combines a controlled formal setting with programs executed against Cordis, a runtime that manages component dependencies and cleanup, and asks models to identify affected components, predict state after a specified teardown order, determine which conditions hold under all or some orders, and choose reconfigurations that succeed when executed. Across these tasks, we evaluate three efficiency-oriented models at low reasoning effort with 2, 4, 8, 16, 24, or 32 relevant interactions, using deterministic task-specific scoring. Models usually handle small systems well but grow less reliable as more interactions become relevant, especially when predicting final state and when reasoning across teardown orders. Additional inference effort recovers marked gains for some models. The cost is nontrivial: on our 16-interaction subset, GPT-5.6 Luna uses nearly 3,000 reasoning tokens per question at medium effort. For these controlled instances, that cost is avoidable: an independent finite reference semantics agrees with Cordis execution on every observation and action outcome used for scoring across all 528 executable questions.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.01600v1)
- [PDF](https://arxiv.org/pdf/2609.01600v1)
- [A Programming Paradigm for Spatiotemporal Composability](https://arxiv.org/abs/2608.25512) (2026, citations: 6)
- [Evo-Bench: Can Language Models Improve Agent Harness?](https://arxiv.org/abs/2608.09096) (2026, citations: 2)
- [Hierarchical Self-Improvement: A Framework for Task-Specific Evolvable Agent Harnesses](https://arxiv.org/abs/2608.08466) (2026, citations: 2)
- [Rethinking the Evaluation of Harness Evolution for Agents](https://arxiv.org/abs/2607.12227) (2026, citations: 16)
- [ScratchLens: Lens-Parametric Behavioral Equivalence for Scratch Programs](https://arxiv.org/abs/2606.15817) (2026, citations: 6)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/agents #keyword/machine-learning
