---
title: "Inside the Unfair Judge: A Mechanistic Interpretability Account of LLM-as-Judge Bias"
source: "https://arxiv.org/html/2607.11871v1"
author: "Zixiang Xu, Sixian Li, Huaxing Liu, Xiang Wang, Shuai Li, Zirui Song, Xiuying Chen"
published: "2026-07-13"
created: 2026-07-15
description: "Representation-level account of LLM-as-judge scoring bias: low-dimensional subspaces, causal steering, and linear projection predictors across seven judges and bias types."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/ai
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
  - keyword/research-paper
---

# Inside the Unfair Judge: A Mechanistic Interpretability Account of LLM-as-Judge Bias

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.11871v1)
- published:: 2026-07-13
- updated:: 2026-07-13
- arxiv_id:: 2607.11871v1
- pdf:: https://arxiv.org/pdf/2607.11871v1
- categories:: cs.CL

## Abstract / Summary
Existing studies of LLM-as-judge scoring bias work predominantly at the input-output level: they perturb inputs, measure score deltas, and propose prompt-level mitigations. This work argues the same biases admit a representation-level account in the judge's hidden state. Across seven judges, seven bias types, and nine benchmarks, the authors report geometry (biased inputs displace along type-specific low-dimensional subspaces), causal control (steering along the subspace shifts scoring both ways), and an operational result (linear projection anticipates judge failures on unseen benchmarks). Project page: https://xzx34.github.io/unfair-judge/

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.11871)
- [PDF](https://arxiv.org/pdf/2607.11871v1)
- [Project page](https://xzx34.github.io/unfair-judge/)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/ai #keyword/evaluation #keyword/benchmark #keyword/machine-learning #keyword/research-paper
