---
title: "Diffusion Policies for Short-Horizon Planning in Robot Crowd Navigation"
source: "https://arxiv.org/html/2608.27158v1"
author: "Wendong Li, Jochen Garcke"
published: "2026-08-27"
created: 2026-08-31
description: "Robot crowd navigation requires safe and efficient decision-making under dense, dynamic, and multimodal human--robot interactions. Existing reinforcement-learning methods typically output a single reactive action at each timestep, which limits their ability to represent diverse short-term avoidance strategies. We propose Planning Diffusion Policy Optimization (PDPO), an offline-to-online reinforcement-learning frame…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/multimodal
  - keyword/diffusion
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
---

# Diffusion Policies for Short-Horizon Planning in Robot Crowd Navigation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27158v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27158v1
- pdf:: https://arxiv.org/pdf/2608.27158v1
- categories:: cs.LG

## Abstract / Summary
Robot crowd navigation requires safe and efficient decision-making under dense, dynamic, and multimodal human--robot interactions. Existing reinforcement-learning methods typically output a single reactive action at each timestep, which limits their ability to represent diverse short-term avoidance strategies. We propose Planning Diffusion Policy Optimization (PDPO), an offline-to-online reinforcement-learning framework that uses a diffusion policy to generate short-horizon action chunks for crowd navigation. PDPO is first pretrained on collision-avoidance demonstrations and then fine-tuned online with PPO by treating the denoising process as an internal decision process. During execution, the policy generates a five-step action chunk and applies it in a receding-horizon manner. Furthermore, we observe an evaluation artifact in common crowd-navigation benchmarks: without explicit boundary constraints, learned agents may leave the valid domain and bypass dense crowds. To address this, we introduce a setting in which boundary violations are treated as collisions. Experiments show that PDPO obtains an improved success rate over strong baselines, and ablations demonstrate that action chunks are especially important for the modified bounded benchmark.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27158v1)
- [PDF](https://arxiv.org/pdf/2608.27158v1)
- [Towards Generalizable Safety in Crowd Navigation via Conformal Uncertainty Handling](https://arxiv.org/abs/2508.05634) (2025, citations: 11)
- [Diffusion Policy Policy Optimization](https://arxiv.org/abs/2409.00588) (2024, citations: 286)
- [Learning Crowd Behaviors in Navigation with Attention-based Spatial-Temporal Graphs](https://arxiv.org/abs/2401.06226) (2024, citations: 8)
- [Diffusion policy: Visuomotor policy learning via action diffusion](https://arxiv.org/abs/2303.04137) (2023, citations: 4015)
- [Enhanced Spatial Attention Graph for Motion Planning in Crowded, Partially Observable Environments](https://www.semanticscholar.org/paper/f2f2491acff96205b78014c51bafcb704c94dd24) (2022, citations: 17)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/multimodal #keyword/diffusion #keyword/evaluation #keyword/benchmark #keyword/agents
