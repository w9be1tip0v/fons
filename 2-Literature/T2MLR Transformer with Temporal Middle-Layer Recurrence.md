---
title: "T^2MLR: Transformer with Temporal Middle-Layer Recurrence"
source: "https://arxiv.org/html/2607.15178v1"
author: "Ziyang Cai, Xingyu Zhu, Yihe Dong, Yinghui He, Sanjeev Arora"
published: "2026-07-16"
created: 2026-07-17
description: "Latent reasoning via fusing a cached middle-layer state from the previous token into an earlier layer of the current step; localized middle recurrence often beats full-layer recurrence and retrofits to pretrained models."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/reasoning
  - keyword/transformer
  - keyword/llm
---

# T^2MLR: Transformer with Temporal Middle-Layer Recurrence

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15178v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15178v1
- pdf:: https://arxiv.org/pdf/2607.15178v1
- categories:: cs.CL

## Abstract / Summary
Autoregressive decoding compresses hidden computation through token space, so intermediate reasoning states struggle to persist. T2MLR fuses a cached middle-layer representation from the previous token into an earlier layer at the current position, letting abstract intermediate computation persist with little inference overhead. On NL pretraining and multi-hop finetuning it beats matched baselines; recurrence on only ~20% of layers (middle block) often beats full-layer recurrence. Retrofitting a pretrained 1.7B Transformer with brief finetuning substantially improves math reasoning. Suggests latent reasoning can emerge from targeted middle-layer recurrence rather than looping all layers.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15178v1)
- [PDF](https://arxiv.org/pdf/2607.15178v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/reasoning #keyword/transformer #keyword/llm
