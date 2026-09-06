---
title: "SurgeGen: A Hybrid Generative Diffusion Framework for Storm Surge Scenario Synthesis"
source: "https://arxiv.org/html/2609.03382v1"
author: "Shunan Zheng, John J. Hasenbein"
published: "2026-09-03"
created: 2026-09-07
description: "Predicting storm surge induced by landfalling tropical cyclones is crucial for flood mitigation and coastal risk management. Traditionally, physics-based numerical models simulate storm surge by solving the Navier--Stokes equations using numerical methods, but these simulations are computationally expensive. Generative models are promising for storm surge emulation because they can generate diverse realizations rath…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/diffusion
  - keyword/retrieval
  - keyword/machine-learning
  - keyword/research-paper
---

# SurgeGen: A Hybrid Generative Diffusion Framework for Storm Surge Scenario Synthesis

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.03382v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.03382v1
- pdf:: https://arxiv.org/pdf/2609.03382v1
- categories:: math.DS, cs.LG

## Abstract / Summary
Predicting storm surge induced by landfalling tropical cyclones is crucial for flood mitigation and coastal risk management. Traditionally, physics-based numerical models simulate storm surge by solving the Navier--Stokes equations using numerical methods, but these simulations are computationally expensive. Generative models are promising for storm surge emulation because they can generate diverse realizations rather than producing a single deterministic prediction. However, their use for storm surge emulation remains largely unexplored. In this paper, we leverage diffusion models for storm surge surrogate modeling, combining a baseline prediction stage with conditional generation to provide a more interpretable modeling framework. We develop SurgeGen, a two-stage generative framework for generating storm surge scenarios conditioned on hypothetical storms with parameters defined in a continuous space. First, a baseline model produces a coarse estimate of the storm surge height. This estimate then conditions a diffusion model, which generates refined storm surge scenarios that better capture spatial patterns and variability. We demonstrate that our approach can generate realistic and diverse storm surge scenarios under conditions both within and outside the training distribution.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.03382v1)
- [PDF](https://arxiv.org/pdf/2609.03382v1)
- [Latent Diffusion and Spatiotemporal Transformers Generate Large Ensemble Climate Simulations](https://doi.org/10.1109/tai.2025.3621121) (2026, citations: 3)
- [Flo: A data-driven limited-area storm surge model](https://arxiv.org/abs/2601.02090) (2026, citations: 2)
- [Value of considering extreme weather resilience in grid capacity expansion planning](https://www.semanticscholar.org/paper/a0a657732a8819d36f538345c3bac8e44fdd0e32) (2025, citations: 19)
- [Flood Scenario Generation Using the Norta Model](https://www.semanticscholar.org/paper/fcad7d2bf6aed2c0705806982e4f36d7d73bebc0) (2024, citations: 2)
- [Probabilistic weather forecasting with machine learning](https://doi.org/10.1038/s41586-024-08252-9) (2024, citations: 736)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/diffusion #keyword/retrieval #keyword/machine-learning #keyword/research-paper
