---
title: "Test-Time Training for Modality Order Consistency in Vision-Language Models"
source: "https://arxiv.org/html/2607.20351v1"
author: "Aditi Gupta, Yossi Gandelsman"
published: "2026-07-22"
created: 2026-07-24
description: "We find that vision-language models are sensitive to a specific semantically irrelevant change: the order in which the image and question are presented. Across three models and three benchmarks, image first prompting consistently outperforms question-first prompting, revealing a repeatable modality order failure. We use this gap to design an order-consistent test-time training method. Our method substantially closes…"
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
  - keyword/safety
  - keyword/machine-learning
---

# Test-Time Training for Modality Order Consistency in Vision-Language Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.20351v1)
- published:: 2026-07-22
- updated:: 2026-07-22
- arxiv_id:: 2607.20351v1
- pdf:: https://arxiv.org/pdf/2607.20351v1
- categories:: cs.CV, cs.CL

## Abstract / Summary
We find that vision-language models are sensitive to a specific semantically irrelevant change: the order in which the image and question are presented. Across three models and three benchmarks, image first prompting consistently outperforms question-first prompting, revealing a repeatable modality order failure. We use this gap to design an order-consistent test-time training method. Our method substantially closes the modality-order gap across all evaluated settings. Surprisingly, it also yields consistent improvements in the stronger image-first branch over the baseline, hence bootstrapping both orderings toward mutual consistency. Activation patching localizes the ordering failure to a narrow mid-network region where representations diverge sharply between prompt orders. We find that the test-time training method repairs this misalignment across layers. Together, our results identify modality-order sensitivity as a circuit-level failure in VLMs and demonstrate that simple, asymmetric test-time adaptation can effectively mitigate it and even improve performance over the baseline.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.20351v1)
- [PDF](https://arxiv.org/pdf/2607.20351v1)
- [Qwen3-VL Technical Report](https://arxiv.org/abs/2511.21631) (2025, citations: 1689)
- [Flip-Flop Consistency: Unsupervised Training for Robustness to Prompt Perturbations in LLMs](https://arxiv.org/abs/2510.14242) (2025, citations: 2)
- [Test-Time Consistency in Vision Language Models](https://arxiv.org/abs/2506.22395) (2025, citations: 4)
- [Same Task, Different Circuits: Disentangling Modality-Specific Mechanisms in VLMs](https://arxiv.org/abs/2506.09047) (2025, citations: 30)
- [Words or Vision: Do Vision-Language Models Have Blind Faith in Text?](https://arxiv.org/abs/2503.02199) (2025, citations: 74)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/evaluation #keyword/benchmark #keyword/safety #keyword/machine-learning
