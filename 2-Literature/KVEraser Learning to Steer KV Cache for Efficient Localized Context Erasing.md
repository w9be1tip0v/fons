---
title: "KVEraser: Learning to Steer KV Cache for Efficient Localized Context Erasing"
source: "https://arxiv.org/html/2606.17034v1"
author: "Mufei Li, Shikun Liu, Dongqi Fu, Haoyu Wang, Yinglong Xia, Hong Li, Hong Yan, Pan Li"
published: "2026-06-15"
created: 2026-06-17
description: "Post-hoc context erasing over the KV cache is challenging because a local edit has a global consequence: once a span has been processed, its influence propagates into the cached states of all subsequent tokens. This issue arises naturally in long-context LLM applications, where stale retrieved facts, incorrect tool observations, retracted user preferences, or harmful prompt injections may be identified only after pr…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/machine-learning
---

# KVEraser: Learning to Steer KV Cache for Efficient Localized Context Erasing

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.17034v1)
- published:: 2026-06-15
- updated:: 2026-06-15
- arxiv_id:: 2606.17034v1
- pdf:: https://arxiv.org/pdf/2606.17034v1
- categories:: cs.CL, cs.LG

## Abstract / Summary
Post-hoc context erasing over the KV cache is challenging because a local edit has a global consequence: once a span has been processed, its influence propagates into the cached states of all subsequent tokens. This issue arises naturally in long-context LLM applications, where stale retrieved facts, incorrect tool observations, retracted user preferences, or harmful prompt injections may be identified only after prefill. Exact erasing must then recompute all tokens after the deleted span, making its computational cost depend on suffix length rather than erased-span length. We introduce KVEraser, a learned KV-cache editing method for efficient localized context erasing. Given a processed context and a span to remove, KVEraser replaces only the KV states of the erased interval with learned steering states while reusing the remaining cache unchanged. To learn a transferable erasing mechanism, we build a two-stage training pipeline: generic span-neighbor pre-training teaches the eraser to suppress the influence of the erased span, while task-specific fine-tuning adapts this capability to downstream scenarios. Experiments show that KVEraser nearly matches full recomputation in post-erasure performance on in-domain tasks across 1K--32K context lengths, while its latency increases by only 24% compared with a 17.6x increase for full recomputation. KVEraser also generalizes to unseen long-document QA tasks with harmful factual distractors, achieving the best performance among approximate baselines with a 3--4x speedup over full recomputation.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.17034v1)
- [PDF](https://arxiv.org/pdf/2606.17034v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/machine-learning
