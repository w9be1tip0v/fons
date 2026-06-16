---
title: "The Value Axis: Language Models Encode Whether They're on the Right Track"
source: "https://arxiv.org/html/2606.17056v1"
author: "Nick Jiang, Isaac Kauvar, Jack Lindsey"
published: "2026-06-15"
created: 2026-06-17
description: "We investigate whether language models internally track the value of their current trajectory, defined as the likelihood that their ongoing strategy will achieve their goals. Using synthetic, in-context reinforcement learning data, we construct a 'value' axis for Qwen3-8B. We find that activations along this axis distinguish between high vs. low verbalized confidence, rollouts without and with backtracking, and corr…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/machine-learning
---

# The Value Axis: Language Models Encode Whether They're on the Right Track

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.17056v1)
- published:: 2026-06-15
- updated:: 2026-06-15
- arxiv_id:: 2606.17056v1
- pdf:: https://arxiv.org/pdf/2606.17056v1
- categories:: cs.CL

## Abstract / Summary
We investigate whether language models internally track the value of their current trajectory, defined as the likelihood that their ongoing strategy will achieve their goals. Using synthetic, in-context reinforcement learning data, we construct a "value" axis for Qwen3-8B. We find that activations along this axis distinguish between high vs. low verbalized confidence, rollouts without and with backtracking, and correct vs. corrupted code. Steering towards high value causally suppresses self-correction and reduces explanatory verbosity, while steering towards low value induces backtracking and exploration. We demonstrate that direct preference optimization (DPO) can increase the internal value of rewarded behaviors (e.g. use a certain word), causing the model to act more confidently after exhibiting them. Finally, we apply the value axis to study in-the-wild settings. For example, we find that Qwen assigns low value to politically sensitive chat queries after post-training and that supervised fine-tuning increases internal confidence within the training domain. Our results suggest that language models linearly encode an estimate of expected goal success that modulates their confidence in pursuing a direction.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.17056v1)
- [PDF](https://arxiv.org/pdf/2606.17056v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/machine-learning
