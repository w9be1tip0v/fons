---
title: "DreamReasoner-8B: Block-Size Curriculum Learning for Diffusion Reasoning Models"
source: "https://arxiv.org/html/2606.19257v1"
author: "Zirui Wu, Lin Zheng, Jiacheng Ye, Shansan Gong, Xueliang Zhao, Yansong Feng, Wei Bi, Lingpeng Kong"
published: "2026-06-17"
created: 2026-06-19
description: "Block diffusion language models accelerate decoding through parallel block-wise denoising, yet whether they can be reliably scaled for long chain-of-thought (CoT) reasoning remains unresolved. To this end, we develop DreamReasoner-8B, an open-source block diffusion reasoning model, and conduct a systematic study of how training and inference block sizes affect long-CoT reasoning. Our analysis reveals a stark perform…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/diffusion
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/machine-learning
---

# DreamReasoner-8B: Block-Size Curriculum Learning for Diffusion Reasoning Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.19257v1)
- published:: 2026-06-17
- updated:: 2026-06-17
- arxiv_id:: 2606.19257v1
- pdf:: https://arxiv.org/pdf/2606.19257v1
- categories:: cs.CL

## Abstract / Summary
Block diffusion language models accelerate decoding through parallel block-wise denoising, yet whether they can be reliably scaled for long chain-of-thought (CoT) reasoning remains unresolved. To this end, we develop DreamReasoner-8B, an open-source block diffusion reasoning model, and conduct a systematic study of how training and inference block sizes affect long-CoT reasoning. Our analysis reveals a stark performance disparity: training with large block sizes yields remarkably poor reasoning, whereas small block sizes preserve effective reasoning. To bridge this granularity gap, we propose block-size curriculum learning, which gradually transitions training from fine-grained to coarse-grained block sizes, thereby overcoming this limitation and enabling strong reasoning performance that generalizes across diverse inference block sizes. On mathematical and code reasoning benchmarks, DreamReasoner-8B achieves results competitive with leading open autoregressive models such as Qwen3-8B. This work establishes a practical foundation for efficient, reasoning-capable diffusion language models. We release our model at https://github.com/DreamLM/DreamReasoner.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.19257v1)
- [PDF](https://arxiv.org/pdf/2606.19257v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/diffusion #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/machine-learning
