---
title: "Mask-Aware Policy Gradients for Diffusion Language Models"
source: "https://arxiv.org/html/2607.15200v1"
author: "Haran Raajesh, Kulin Shah, Adam Klivans, Philipp Krähenbühl"
published: "2026-07-16"
created: 2026-07-17
description: "Two-stage MDP for masked diffusion LMs (token placement + remask decisions); joint policy gradients hit 87.1% GSM8K and 53.4% MBPP (COLM 2026)."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/diffusion
  - keyword/reasoning
  - keyword/post-training
---

# Mask-Aware Policy Gradients for Diffusion Language Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15200v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15200v1
- pdf:: https://arxiv.org/pdf/2607.15200v1
- categories:: cs.CL / cs.LG (COLM 2026)

## Abstract / Summary
RL improves reasoning LLMs but is hard for Masked Diffusion Language Models because log-likelihood is intractable. Prior work models only token predictions and ignores unmask order. MDLM generation is formalized as a two-stage action MDP: which tokens to place, and which positions to remask. Policy gradient decomposes into token and masking terms; optimizing both yields SOTA math and coding results (87.1% GSM8K, 53.4% MBPP).

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15200v1)
- [PDF](https://arxiv.org/pdf/2607.15200v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/diffusion #keyword/reasoning #keyword/post-training
