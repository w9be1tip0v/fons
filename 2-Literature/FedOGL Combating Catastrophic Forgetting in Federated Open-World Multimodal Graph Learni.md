---
title: "FedOGL: Combating Catastrophic Forgetting in Federated Open-World Multimodal Graph Learning"
source: "https://arxiv.org/html/2607.27665v1"
author: "Zekai Chen, Haodong Lu, Shihao Li, Weiwei Ji, Xunkai Li, Xun Wu, Yinlin Zhu, Rong-Hua Li"
published: "2026-07-30"
created: 2026-08-03
description: "Federated graph learning enables collaborative training over decentralized graph data without sharing raw graph information. As such risks evolve, clients must learn emerging classes from private multimodal graph streams, retain historical categories, and reject samples outside the known class space. In this setting, clients must learn emerging classes from private multimodal graph streams while preserving historica…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/nlp
  - keyword/multimodal
  - keyword/retrieval
  - keyword/machine-learning
---

# FedOGL: Combating Catastrophic Forgetting in Federated Open-World Multimodal Graph Learning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.27665v1)
- published:: 2026-07-30
- updated:: 2026-07-30
- arxiv_id:: 2607.27665v1
- pdf:: https://arxiv.org/pdf/2607.27665v1
- categories:: cs.LG

## Abstract / Summary
Federated graph learning enables collaborative training over decentralized graph data without sharing raw graph information. As such risks evolve, clients must learn emerging classes from private multimodal graph streams, retain historical categories, and reject samples outside the known class space. In this setting, clients must learn emerging classes from private multimodal graph streams while preserving historical categories and rejecting samples outside the current known class space. The core challenge is catastrophic forgetting, which in federated multimodal graphs is not merely a classifier-level failure: old knowledge can be erased through modality-semantic overwriting, topology-induced structural erosion, and federated memory fragmentation. To address this challenge, we propose \textbf{FedOGL}, a semantic-structural memory preservation framework. On the client side, FedOGL preserves historical decision behavior through replay and task-start distillation, while protecting graph-propagation memory via projection onto a globally shared structure basis. On the server side, FedOGL maintains and transfers compact category prototypes to facilitate cross-client knowledge sharing without exposing raw graph data. Extensive experiments demonstrate that, compared with the best-performing baselines, FedOGL reduces performance degradation caused by catastrophic forgetting by \textbf{42.67\%}, while maintaining or improving performance on downstream tasks.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.27665v1)
- [PDF](https://arxiv.org/pdf/2607.27665v1)
- [PRISM: Topology-Aware Cross-Modal Imputation for Modality-Deficient Federated Graph Learning](https://arxiv.org/abs/2606.09301) (2026, citations: 2)
- [MM-OpenFGL: A Comprehensive Benchmark for Multimodal Federated Graph Learning](https://arxiv.org/abs/2601.22416) (2026, citations: 7)
- [Modeling Inter-Intra Heterogeneity for Graph Federated Learning](https://arxiv.org/abs/2412.11402) (2024, citations: 19)
- [FedSSP: Federated Graph Learning with Spectral Knowledge and Personalized Preference](https://arxiv.org/abs/2410.20105) (2024, citations: 33)
- [OpenFGL: A Comprehensive Benchmark for Federated Graph Learning](https://arxiv.org/abs/2408.16288) (2024, citations: 21)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/nlp #keyword/multimodal #keyword/retrieval #keyword/machine-learning
