---
title: "DataOrchestra: Learning to Orchestrate Per-Example Curation of Pretraining Data"
source: "https://arxiv.org/html/2607.24717v1"
author: "Zhen Huang, Yikun Wang, Shijie Xia, Pengfei Liu"
published: "2026-07-27"
created: 2026-07-29
description: "Pretraining data processing is critical to the downstream performance of Large Language Models (LLMs). However, many existing approaches define a fixed processing strategy at the corpus or domain level and apply it uniformly to many examples, without adapting to the needs of each example. We propose DataOrchestra, a framework that unifies different processing operations and orchestrates an example-specific pipeline…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
---

# DataOrchestra: Learning to Orchestrate Per-Example Curation of Pretraining Data

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.24717v1)
- published:: 2026-07-27
- updated:: 2026-07-27
- arxiv_id:: 2607.24717v1
- pdf:: https://arxiv.org/pdf/2607.24717v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Pretraining data processing is critical to the downstream performance of Large Language Models (LLMs). However, many existing approaches define a fixed processing strategy at the corpus or domain level and apply it uniformly to many examples, without adapting to the needs of each example. We propose DataOrchestra, a framework that unifies different processing operations and orchestrates an example-specific pipeline for each example. Given a chunk of pretraining data, an orchestrator decides whether to drop, untouch, or clean it. For a chunk to be cleaned, it selects one or more downstream operations, ranging from programmatic editing to different forms of LLM-based rewriting. For each rewriting step, it further generates a concrete instruction, which is executed by the corresponding downstream tool model. We pretrain models from 0.5B to 7B from scratch on web data processed by DataOrchestra and observe stable average gains over individual data-processing methods across 11 benchmarks. DataOrchestra is also effective for math continued pretraining and outperforms stronger processing baselines, while reducing processing compute by skipping unnecessary downstream operations.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.24717v1)
- [PDF](https://arxiv.org/pdf/2607.24717v1)
- [A Bitter Lesson for Data Filtering](https://arxiv.org/abs/2605.19407) (2026, citations: 3)
- [How Can We Synthesize High-Quality Pretraining Data? A Systematic Study of Prompt Design, Generator Model, and Source Data](https://arxiv.org/abs/2604.13977) (2026, citations: 2)
- [Data Darwinism Part II: DataEvolve - AI can Autonomously Evolve Pretraining Data Curation](https://arxiv.org/abs/2603.14420) (2026, citations: 2)
- [Data Darwinism Part I: Unlocking the Value of Scientific Data for Pre-training](https://arxiv.org/abs/2602.07824) (2026, citations: 4)
- [RePro: Training Language Models to Faithfully Recycle the Web for Pretraining](https://arxiv.org/abs/2510.10681) (2025, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/machine-learning
