---
title: "When Models Edit Too Much: On the Fidelity of Minimal Code Edits"
source: "https://arxiv.org/html/2609.04061v1"
author: "Tongyao Zhu, Wei Hern Lim, Min-Yen Kan"
published: "2026-09-03"
created: 2026-09-05
description: "Large language models (LLMs) are increasingly used to edit existing code, but correctness alone is not enough: useful repairs should also be minimal, reviewable, and faithful to the original implementation. We study over-editing, the tendency of a model to rewrite code beyond what is required to fix a bug. We construct an evaluation framework from 400 BigCodeBench problems by injecting controlled AST-level corruptio…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/reasoning
  - keyword/machine-learning
---

# When Models Edit Too Much: On the Fidelity of Minimal Code Edits

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.04061v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.04061v1
- pdf:: https://arxiv.org/pdf/2609.04061v1
- categories:: cs.SE, cs.AI, cs.CL

## Abstract / Summary
Large language models (LLMs) are increasingly used to edit existing code, but correctness alone is not enough: useful repairs should also be minimal, reviewable, and faithful to the original implementation. We study over-editing, the tendency of a model to rewrite code beyond what is required to fix a bug. We construct an evaluation framework from 400 BigCodeBench problems by injecting controlled AST-level corruptions into reference solutions, giving each repair task a known minimal patch. Across frontier LLMs, over-editing is widespread even among strong models like GPT-5.5: high Pass@1 can coexist with unnecessarily large edits and added cognitive complexity. A preservation instruction substantially reduces this behavior, lowering average excess Levenshtein distance from 0.195 to 0.131, reducing added cognitive complexity by 26.6%, and increasing Pass@1 by 2.3 points. However, these gains do not simply follow from a larger reasoning budget or larger models. We next ask whether minimal editing can be learned directly during post-training. We observe that supervised fine-tuning overfits to seen corruption patterns, whereas reinforcement learning gives the best out-of-domain edit-fidelity and performance-retention trade-off. These results position edit fidelity as a distinct axis of code-repair quality and show that it can be measured and learned.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.04061v1)
- [PDF](https://arxiv.org/pdf/2609.04061v1)
- [QiMeng-PRepair: Precise Code Repair via Edit-Aware Reward Optimization](https://arxiv.org/abs/2604.05963) (2026, citations: 2)
- [Edit, But Verify: An Empirical Audit of Instructed Code-Editing Benchmarks](https://arxiv.org/abs/2604.05100) (2026, citations: 1)
- [PAFT: Preservation Aware Fine-Tuning for Minimal-Edit Program Repair](https://arxiv.org/abs/2604.03113) (2026, citations: 2)
- [EDIT-Bench: Evaluating LLM Abilities to Perform Real-World Instructed Code Edits](https://arxiv.org/abs/2511.04486) (2025, citations: 15)
- [SWE-Perf: Can Language Models Optimize Code Performance on Real-World Repositories?](https://arxiv.org/abs/2507.12415) (2025, citations: 34)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/reasoning #keyword/machine-learning
