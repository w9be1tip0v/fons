---
title: "Cross-Tokenizer On-Policy Distillation via Byte-Prefix Marginalization"
source: "https://arxiv.org/html/2607.22334v1"
author: "Hao Wang, Kun Yuan, Wenlin Zhong, Minglei Zhang, Han Xiao, Ming Sun, Honggang Qi"
published: "2026-07-24"
created: 2026-07-28
description: "Open-weight language models from different families exhibit complementary capabilities, motivating their consolidation into a compact student through on-policy distillation (OPD). However, full-vocabulary OPD typically assumes a shared tokenizer, while existing cross-tokenizer methods may discard teacher probability mass or assign it to student tokens with unrelated content. We introduce Byte-Prefix Marginalization…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
---

# Cross-Tokenizer On-Policy Distillation via Byte-Prefix Marginalization

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.22334v1)
- published:: 2026-07-24
- updated:: 2026-07-24
- arxiv_id:: 2607.22334v1
- pdf:: https://arxiv.org/pdf/2607.22334v1
- categories:: cs.LG, cs.AI, cs.CL

## Abstract / Summary
Open-weight language models from different families exhibit complementary capabilities, motivating their consolidation into a compact student through on-policy distillation (OPD). However, full-vocabulary OPD typically assumes a shared tokenizer, while existing cross-tokenizer methods may discard teacher probability mass or assign it to student tokens with unrelated content. We introduce Byte-Prefix Marginalization (BPM), which re-expresses the teacher's next-token distribution over the student vocabulary in a shared byte space. Specifically, BPM assigns each teacher token's probability to the longest student token whose byte representation is a prefix of the teacher token's bytes, aggregates mass mapped to the same student token, and places otherwise unmatched mass in an explicit residual category. This produces a vocabulary-complete, byte-aligned, and mass-preserving target for dense OPD. The target exactly recovers the teacher-induced byte-prefix marginal when the relevant prefix does not span multiple teacher tokens (a condition satisfied at more than 99% of training positions) and uses a mass-preserving, chain-factorized lower bound otherwise. Across Qwen3-32B, GLM-Z1-9B-0414, and MiniMax-M2.7 as teachers, BPM consistently outperforms current cross-tokenizer methods on six mathematics and programming benchmarks, improving six-benchmark avg@8 by 3.7-6.6 points over the strongest baselines.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.22334v1)
- [PDF](https://arxiv.org/pdf/2607.22334v1)
- [KAT-Coder-V2.5 Technical Report](https://arxiv.org/abs/2607.05471) (2026, citations: 1)
- [The MiniMax-M2 Series: Mini Activations Unleashing Max Real-World Intelligence](https://arxiv.org/abs/2605.26494) (2026, citations: 13)
- [SimCT: Recovering Lost Supervision for Cross-Tokenizer On-Policy Distillation](https://arxiv.org/abs/2605.07711) (2026, citations: 4)
- [DeepSeek-V4: Towards Highly Efficient Million-Token Context Intelligence](https://arxiv.org/abs/2606.19348) (2026, citations: 393)
- [Rethinking On-Policy Distillation of Large Language Models: Phenomenology, Mechanism, and Recipe](https://arxiv.org/abs/2604.13016) (2026, citations: 123)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/machine-learning
