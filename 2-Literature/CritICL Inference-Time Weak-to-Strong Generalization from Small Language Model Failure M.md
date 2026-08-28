---
title: "CritICL: Inference-Time Weak-to-Strong Generalization from Small Language Model Failure Modes"
source: "https://arxiv.org/html/2608.27455v1"
author: "Yufan Wu, Yinghui He, Zhengyi Hu, Lang Wei, Ruichen Li, Qifan Yang, Ting Zhu"
published: "2026-08-27"
created: 2026-08-29
description: "Recent advances in inference-time scaling have significantly improved the reasoning performance of large language models (LLMs). However, these methods typically rely on repeated generation or external verification. To address this limitation, we introduce CritICL, a novel inference-time framework that improves reasoning while maintaining high efficiency. Our key insight is that LLM failure modes exhibit structured…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/reasoning
  - keyword/machine-learning
---

# CritICL: Inference-Time Weak-to-Strong Generalization from Small Language Model Failure Modes

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27455v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27455v1
- pdf:: https://arxiv.org/pdf/2608.27455v1
- categories:: cs.CL

## Abstract / Summary
Recent advances in inference-time scaling have significantly improved the reasoning performance of large language models (LLMs). However, these methods typically rely on repeated generation or external verification. To address this limitation, we introduce CritICL, a novel inference-time framework that improves reasoning while maintaining high efficiency. Our key insight is that LLM failure modes exhibit structured patterns across model scales within the same family. Instead of treating failures as undesirable outputs, CritICL leverages them as a source of guidance. Specifically, we utilize failure modes derived from weaker models and incorporate them into inference through critique-based in-context examples. We propose two variants: CritICL-dynamic, which adaptively predicts input-specific failure modes and retrieves critiques, and CritICL-static, which uses a global failure mode profile to provide stable guidance. Experimental results show that CritICL consistently outperforms standard in-context learning and achieves performance competitive with or superior to test-time scaling methods, while requiring significantly fewer generations and lower token cost. Code available at: https://github.com/umwyf/CRITICL

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27455v1)
- [PDF](https://arxiv.org/pdf/2608.27455v1)
- [W2S-AlignTree: Weak-to-Strong Inference-Time Alignment for Large Language Models via Monte Carlo Tree Search](https://arxiv.org/abs/2511.11518) (2025, citations: 5)
- [Skill-Targeted Adaptive Training](https://arxiv.org/abs/2510.10023) (2025, citations: 4)
- [AdaptMI: Adaptive Skill-based In-context Math Instruction for Small Language Models](https://arxiv.org/abs/2505.00147) (2025, citations: 5)
- [ReasonIR: Training Retrievers for Reasoning Tasks](https://arxiv.org/abs/2504.20595) (2025, citations: 79)
- [Self-Evolving Critique Abilities in Large Language Models](https://arxiv.org/abs/2501.05727) (2025, citations: 9)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/reasoning #keyword/machine-learning
