---
title: "Multi-Task Learning for Heterogeneous Prediction from Video Game State with Transfer Learning"
source: "https://arxiv.org/html/2607.21290v1"
author: "Jonas Peché, Aliaksei Tsishurou, Alexander Zap, Günter Wallner"
published: "2026-07-23"
created: 2026-07-27
description: "Multi-task learning (MTL) is a promising approach for prediction tasks derived from video game state data, as modern game telemetry provides multiple related supervision signals from the same structured observations. We study whether a shared model trained jointly across tasks in team-based multiplayer games can improve generalization while reducing training and inference cost compared to specialized single-task mod…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/transformer
  - keyword/nlp
  - keyword/multimodal
  - keyword/evaluation
  - keyword/machine-learning
---

# Multi-Task Learning for Heterogeneous Prediction from Video Game State with Transfer Learning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.21290v1)
- published:: 2026-07-23
- updated:: 2026-07-23
- arxiv_id:: 2607.21290v1
- pdf:: https://arxiv.org/pdf/2607.21290v1
- categories:: cs.LG, cs.AI

## Abstract / Summary
Multi-task learning (MTL) is a promising approach for prediction tasks derived from video game state data, as modern game telemetry provides multiple related supervision signals from the same structured observations. We study whether a shared model trained jointly across tasks in team-based multiplayer games can improve generalization while reducing training and inference cost compared to specialized single-task models. We adapt a multimodal architecture for endpoint prediction to a general multi-task setting that combines rasterized vision inputs, global match context, and per-unit state information through an image encoder and attention-based interaction modeling. Experiments on a large proprietary World of Tanks dataset compare single-task and multi-task training, evaluate weighting strategies for mixed losses and conflicting gradients, and test pre-training/fine-tuning under limited target-data regimes. We also examine within-game transfer across game maps under structured environment shift.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.21290v1)
- [PDF](https://arxiv.org/pdf/2607.21290v1)
- [Deep multi-task learning: a review of concepts, methods, and cross-domain applications](https://link.springer.com/content/pdf/10.1007/s41060-025-00892-y.pdf) (2025, citations: 9)
- [Bootstrap Your Own Teacher: Online Policy Distillation for Multi-Game Reinforcement Learning](https://www.semanticscholar.org/paper/edb97b420ffd6a4e0498de139594ed1fc8b79c07) (2025, citations: 1)
- [A Multimodal Architecture for Endpoint Position Prediction in Team-Based Multiplayer Games](https://arxiv.org/abs/2507.20670) (2025, citations: 1)
- [Knowledge enhanced graph contrastive learning for match outcome prediction](https://www.semanticscholar.org/paper/dc7b67e2882ae175bad3e5763c98272e94fd0f8f) (2025, citations: 4)
- [Learning general multi-agent decision model through multi-task pre-training](https://www.semanticscholar.org/paper/dfe98357f426d9bdbf8d11aa01d5b29b3b26ef61) (2025, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/transformer #keyword/nlp #keyword/multimodal #keyword/evaluation #keyword/machine-learning
