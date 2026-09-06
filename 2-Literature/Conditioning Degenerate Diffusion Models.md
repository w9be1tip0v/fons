---
title: "Conditioning Degenerate Diffusion Models"
source: "https://arxiv.org/html/2609.04090v1"
author: "Uğur Aydın, Tamer Başar"
published: "2026-09-03"
created: 2026-09-07
description: "Current conditioned generative models heavily rely on score functions for guidance during training. When the generative model is a diffusion process with a singular diffusion coefficient and the underlying (conditional) densities either do not exist or are not smooth, we use causal optimal transport to define \emph{approximate} loss functions that identify a minimum-entropy control for guidance under minimal assumpt…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/diffusion
  - keyword/machine-learning
---

# Conditioning Degenerate Diffusion Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.04090v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.04090v1
- pdf:: https://arxiv.org/pdf/2609.04090v1
- categories:: cs.LG

## Abstract / Summary
Current conditioned generative models heavily rely on score functions for guidance during training. When the generative model is a diffusion process with a singular diffusion coefficient and the underlying (conditional) densities either do not exist or are not smooth, we use causal optimal transport to define \emph{approximate} loss functions that identify a minimum-entropy control for guidance under minimal assumptions. Our approach relies on causal optimal transport and its characterization through the predictable representation property of (conditioned) diffusion processes whose associated martingale problem is well posed, à la Üstünel.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.04090v1)
- [PDF](https://arxiv.org/pdf/2609.04090v1)
- [Conditioning Diffusions Using Malliavin Calculus](https://arxiv.org/abs/2504.03461) (2025, citations: 17)
- [Malliavin Calculus for Score-based Diffusion Models](https://arxiv.org/abs/2503.16917) (2025, citations: 10)
- [Underdamped Diffusion Bridges with Applications to Sampling](https://arxiv.org/abs/2503.01006) (2025, citations: 35)
- [Adjoint Matching: Fine-tuning Flow and Diffusion Generative Models with Memoryless Stochastic Optimal Control](https://arxiv.org/abs/2409.08861) (2024, citations: 220)
- [Conditioning non-linear and infinite-dimensional diffusion processes](https://arxiv.org/abs/2402.01434) (2024, citations: 20)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/diffusion #keyword/machine-learning
