---
title: "CorporateBench: Large-Scale Q&A Benchmarking with Temporal Knowledge Bases"
source: "https://arxiv.org/html/2608.27391v1"
author: "Sil Hamilton, Albert Yu Sun, Oscar J. Romero, Carl-Leander Henneking, David Mimno, Bishan Yang, Igor Labutov"
published: "2026-08-27"
created: 2026-08-30
description: "LLMs are increasingly able to answer complex questions about enterprise-scale document collections. But evaluation is hard: companies don't want to share internal communications, and synthetic datasets have been overly simple. We present CorporateBench (CB), a human-validated multi-task Q&A benchmark whose scale approaches the conditions LLMs encounter in corporate communication networks, with evaluation corpora sur…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
---

# CorporateBench: Large-Scale Q&A Benchmarking with Temporal Knowledge Bases

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27391v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27391v1
- pdf:: https://arxiv.org/pdf/2608.27391v1
- categories:: cs.AI, cs.CL, cs.IR, cs.LG

## Abstract / Summary
LLMs are increasingly able to answer complex questions about enterprise-scale document collections. But evaluation is hard: companies don't want to share internal communications, and synthetic datasets have been overly simple. We present CorporateBench (CB), a human-validated multi-task Q&A benchmark whose scale approaches the conditions LLMs encounter in corporate communication networks, with evaluation corpora surpassing 230,000 documents. CB evaluates LLMs across two dimensions (information extraction and knowledge base querying) through four synthetically generated firms ranging from 12 to 10,000 employees. Each corpus is sampled from a temporally evolving knowledge base describing a consistent world, guaranteeing cross-document logical consistency even across hundreds of thousands of documents. We evaluate five LLMs on CB, revealing increasingly poor performance as input size approaches realistic scales. CB provides LLM developers a metric for corporate communication reasoning, filling a crucial gap in the benchmarking ecosystem.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27391v1)
- [PDF](https://arxiv.org/pdf/2608.27391v1)
- [Can LLMs Help You at Work? A Sandbox for Evaluating LLM Agents in Enterprise Environments](https://arxiv.org/abs/2510.27287) (2025, citations: 13)
- [Benchmarking Deep Search over Heterogeneous Enterprise Data](https://arxiv.org/abs/2506.23139) (2025, citations: 18)
- [Enterprise Large Language Model Evaluation Benchmark](https://arxiv.org/abs/2506.20274) (2025, citations: 5)
- [Too Long, Didn't Model: Decomposing LLM Long-Context Understanding With Novels](https://arxiv.org/abs/2505.14925) (2025, citations: 10)
- [Docs2KG: A Human-LLM Collaborative Approach to Unified Knowledge Graph Construction from Heterogeneous Documents](https://dl.acm.org/doi/pdf/10.1145/3701716.3715309) (2025, citations: 9)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/evaluation #keyword/benchmark #keyword/reasoning
