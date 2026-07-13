---
title: "Autoregressive latent diffusion for 3D molecule generation"
source: "https://arxiv.org/html/2607.09277v1"
author: "Federico Ottomano, Gaopeng Ren, Yingzhen Li, Kim E. Jelfs, Alex M. Ganose"
published: "2026-07-10"
created: 2026-07-14
description: "KRONOS is a latent autoregressive diffusion model for variable-length 3D molecule generation, supporting unconditional and fragment-conditioned design in one architecture."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/diffusion
  - keyword/machine-learning
  - keyword/research-paper
---

# Autoregressive latent diffusion for 3D molecule generation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.09277v1)
- published:: 2026-07-10
- updated:: 2026-07-10
- arxiv_id:: 2607.09277v1
- pdf:: https://arxiv.org/pdf/2607.09277v1
- categories:: cs.LG

## Abstract / Summary
Three-dimensional (3D) molecule generation has been dominated by diffusion models, which achieve strong generation quality but typically require the molecular size to be specified a priori. Recent autoregressive approaches have substantially narrowed the performance gap while naturally supporting variable-length generation and conditioning on partial molecular context. However, balancing unconditional and context-conditioned generation remains challenging. We introduce KRONOS, a latent autoregressive diffusion framework that generates molecules in the latent space of a pre-trained autoencoder, jointly modeling molecular graph topology and geometry, while retaining the flexibility of autoregressive generation. We further introduce a mixed training strategy inspired by Fill-in-the Middle (FIM) paradigm, enabling both unconditional and fragment-conditioned molecular generation within a single left-to-right autoregressive model. Experiments on QM9 and GEOM-Drugs demonstrate that KRONOS achieves leading unconditional generation performance among autoregressive methods, while remaining competitive with diffusion models. Moreover, fragment-conditioned generation is achieved with negligible impact on unconditional generation performance, demonstrating that both generation paradigms can be supported within a single architecture.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.09277)
- [PDF](https://arxiv.org/pdf/2607.09277v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/diffusion #keyword/machine-learning #keyword/research-paper
