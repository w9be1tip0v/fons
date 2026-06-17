---
title: "Variable-Width Transformers"
source: "https://arxiv.org/html/2606.18246v1"
author: "Zhaofeng Wu, Oliver Sieberling, Shawn Tan, Rameswar Panda, Yury Polyanskiy, Yoon Kim"
published: "2026-06-16"
created: 2026-06-18
description: "Scaling model size, specifically depth and width, has driven significant progress in transformer-based language models. However, most architectures maintain a constant width across all layers, allocating a fixed parameter and computation budget evenly despite different layers potentially playing distinct computational roles. In this work, we empirically investigate nonuniform capacity allocation across network depth…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/transformer
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
---

# Variable-Width Transformers

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.18246v1)
- published:: 2026-06-16
- updated:: 2026-06-16
- arxiv_id:: 2606.18246v1
- pdf:: https://arxiv.org/pdf/2606.18246v1
- categories:: cs.CL

## Abstract / Summary
Scaling model size, specifically depth and width, has driven significant progress in transformer-based language models. However, most architectures maintain a constant width across all layers, allocating a fixed parameter and computation budget evenly despite different layers potentially playing distinct computational roles. In this work, we empirically investigate nonuniform capacity allocation across network depth by proposing a $\times$-shaped > <former consistently outperforms parameter-matched uniform baselines on language modeling loss. By reducing the average layer width, this architecture also requires fewer overall FLOPs (22% reduction under fitted loss-matched scaling curves) and smaller KV cache memory and I/O cost (15% reduction). In analysis, we show that this bottleneck structure results in qualitatively different representations in residual streams. Overall, our results demonstrate that nonuniform width allocation can result in more resource-optimal scaling of language models.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.18246v1)
- [PDF](https://arxiv.org/pdf/2606.18246v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/transformer #keyword/language-model #keyword/nlp #keyword/retrieval
