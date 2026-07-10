---
title: "DominoTree: Conditional Tree-Structured Drafting with Domino for Speculative Decoding"
source: "https://arxiv.org/html/2607.08642v1"
author: "Saw S. Lin, Jyh-Shing Roger Jang"
published: "2026-07-09"
created: 2026-07-11
description: "Speculative decoding accelerates LLM inference by drafting several tokens and verifying them in parallel. Block-diffusion drafters such as DFlash produce a draft block in one pass but model only per-position marginals; best-first tree methods such as DDTree expand candidate trees from those marginals. The released Domino drafter adds a GRU-based causal correction that makes each draft token's distribution path-depen…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/diffusion
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
---

# DominoTree: Conditional Tree-Structured Drafting with Domino for Speculative Decoding

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.08642v1)
- published:: 2026-07-09
- updated:: 2026-07-09
- arxiv_id:: 2607.08642v1
- pdf:: https://arxiv.org/pdf/2607.08642v1
- categories:: cs.CL

## Abstract / Summary
Speculative decoding accelerates LLM inference by drafting several tokens and verifying them in parallel. Block-diffusion drafters such as DFlash produce a draft block in one pass but model only per-position marginals; best-first tree methods such as DDTree expand candidate trees from those marginals. The released Domino drafter adds a GRU-based causal correction that makes each draft token's distribution path-dependent, a structure DDTree's factorized formulation cannot represent. We introduce DominoTree, a training-free best-first draft tree scored by Domino's conditional, non-factorized correction along each root-to-node path, made practical by restricting the per-node correction to a candidate top-M. On Qwen3-4B across eight benchmarks, DominoTree reaches up to 6.6x speedup over autoregressive decoding and the highest mean accept length of any evaluated method, up to 10.7 tokens per round, at every temperature we test. DominoTree constructs its tree with a GPU-native, CUDA-graph builder that is bit-identical to a reference Python implementation, so acceptance is unchanged, while keeping per-round tree construction cheap. With this builder as default, DominoTree wins throughput over the released Domino decoder at every temperature, 9-10% overall on Qwen3-4B and up to +22% on Alpaca, and over DDTree/CaDDTree at every temperature we test. On Qwen3- 8B, DominoTree keeps the highest accepted length at every temperature and adds a decisive throughput win at T=0, +24% over DDTree; at higher temperature that edge over DDTree/CaDDTree narrows to a tie and a small loss, while its Overall aggregate wins over DFlash and Domino persist.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.08642v1)
- [PDF](https://arxiv.org/pdf/2607.08642v1)
- [JetSpec: Breaking the Scaling Ceiling of Speculative Decoding with Parallel Tree Drafting](https://arxiv.org/abs/2606.18394) (2026, citations: 3)
- [Cost-Aware Diffusion Draft Trees for Speculative Decoding](https://arxiv.org/abs/2606.01813) (2026, citations: 1)
- [Domino: Decoupling Causal Modeling from Autoregressive Drafting in Speculative Decoding](https://arxiv.org/abs/2605.29707) (2026, citations: 4)
- [Accelerating Speculative Decoding with Block Diffusion Draft Trees](https://arxiv.org/abs/2604.12989) (2026, citations: 10)
- [DFlash: Block Diffusion for Flash Speculative Decoding](https://arxiv.org/abs/2602.06036) (2026, citations: 47)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/diffusion #keyword/evaluation #keyword/benchmark #keyword/machine-learning
