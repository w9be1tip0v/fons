---
title: "A Sovereign, Open-Source Foundation Model for German and English"
source: "https://arxiv.org/html/2607.09424v1"
author: "The Soofi-Team"
published: "2026-07-10"
created: 2026-07-14
description: "Soofi S 30B-A3B is a German/English MoE hybrid Mamba-Transformer foundation model (3B active of 30B) pretrained on ~27T tokens with open release of weights and data accounting."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/ai
  - keyword/machine-learning
  - keyword/research-paper
---

# A Sovereign, Open-Source Foundation Model for German and English

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.09424v1)
- published:: 2026-07-10
- updated:: 2026-07-10
- arxiv_id:: 2607.09424v1
- pdf:: https://arxiv.org/pdf/2607.09424v1
- categories:: cs.CL, cs.AI, cs.LG

## Abstract / Summary
We present Soofi S 30B-A3B, a sovereign, open-source Mixture-of-Experts (MoE) hybrid Mamba Transformer foundation model for German and English. Its hybrid design activates only 3B of 30B parameters per token and keeps the inference cache near-constant as context grows, giving it a decisive throughput advantage over dense models for long-context, high-concurrency deployment. Pretrained on roughly 27 trillion tokens with deliberately up-weighted German, Soofi S matches dense 14 to 27B models on aggregate English and German benchmarks while achieving the best code aggregates in both languages among 17 open base models, and outperforms every European sovereign baseline in our comparison, including ones far larger in active parameters. Among fully open models, Soofi S obtains the highest English and German evaluation scores, ahead of Olmo 3 32B and Apertus 70B. Soofi S was built end-to-end on the German Industrial AI Cloud. Soofi S will be released under highly permissive, open-access terms: weights, selected intermediate checkpoints, full per-source data accounting, hyperparameters, and training and evaluation code.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.09424)
- [PDF](https://arxiv.org/pdf/2607.09424v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/ai #keyword/machine-learning #keyword/research-paper
