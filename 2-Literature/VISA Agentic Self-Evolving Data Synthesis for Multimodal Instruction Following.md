---
title: "VISA: Agentic Self-Evolving Data Synthesis for Multimodal Instruction Following"
source: "https://arxiv.org/html/2608.26013v1"
author: "Min Zeng, Guanxin Tan, Libin Cen, Yawei Wen, Rui Hu, Liuyang Bian, Xiaolong Chen, Xiaoxin Chen"
published: "2026-08-26"
created: 2026-08-28
description: "Multimodal instruction-following models require training data that is accurate, diverse, verifiable, and challenging. Existing synthesis pipelines typically follow a one-pass generate-and-filter paradigm, discarding feedback from failed samples, verifier outcomes, and target-model errors. We present VISA (Visual Instruction Synthesis Agent), an agentic framework that reformulates multimodal instruction synthesis as…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
  - keyword/machine-learning
---

# VISA: Agentic Self-Evolving Data Synthesis for Multimodal Instruction Following

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.26013v1)
- published:: 2026-08-26
- updated:: 2026-08-26
- arxiv_id:: 2608.26013v1
- pdf:: https://arxiv.org/pdf/2608.26013v1
- categories:: cs.CL

## Abstract / Summary
Multimodal instruction-following models require training data that is accurate, diverse, verifiable, and challenging. Existing synthesis pipelines typically follow a one-pass generate-and-filter paradigm, discarding feedback from failed samples, verifier outcomes, and target-model errors. We present VISA (Visual Instruction Synthesis Agent), an agentic framework that reformulates multimodal instruction synthesis as a self-evolving loop. At each round, VISA analyzes an image to filter incompatible constraints and discover new verifiable ones, samples diversity- and difficulty-aware constraint sets from persistent memory, generates candidate instructions, and verifies the resulting samples with executable tools and structured large language model judges. Failed samples trigger diagnostic-guided recovery, while accepted samples are probed against the target model to estimate difficulty. The resulting verifier signals and target-model failure profiles are written back to memory, allowing subsequent rounds to adaptively expand the constraint space, reduce template repetition, and focus on unresolved model weaknesses. The same verifier contracts further provide reward signals for reinforcement learning without a separately trained reward model. Experiments on MM-IFEval show that VISA consistently improves multimodal instruction following over strong baselines, while preserving general multimodal capability across seven public benchmarks.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.26013v1)
- [PDF](https://arxiv.org/pdf/2608.26013v1)
- [Empowering Reliable Visual-Centric Instruction Following in MLLMs](https://arxiv.org/abs/2601.03198) (2026, citations: 6)
- [Reinforcement Learning with Verifiable yet Noisy Rewards under Imperfect Verifiers](https://arxiv.org/abs/2510.00915) (2025, citations: 29)
- [InternVL3.5: Advancing Open-Source Multimodal Models in Versatility, Reasoning, and Efficiency](https://arxiv.org/abs/2508.18265) (2025, citations: 1300)
- [MM-IFEngine: Towards Multimodal Instruction Following](https://arxiv.org/abs/2504.07957) (2025, citations: 44)
- [HybridFlow: A Flexible and Efficient RLHF Framework](https://arxiv.org/abs/2409.19256) (2024, citations: 2179)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/machine-learning
