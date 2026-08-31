---
title: "NL2AGBench: Benchmarking LLM Auto-Formalization for AlphaGeometry"
source: "https://arxiv.org/html/2608.28481v1"
author: "Samuel Xiao, Judy Song, Rory Hu, Ziliang Zong"
published: "2026-08-28"
created: 2026-09-01
description: "Recent advances in large language models (LLMs) have demonstrated strong capabilities in natural language understanding and mathematical reasoning. However, their ability to translate informal mathematical problems into formal representations remains underexplored. This limitation is particularly important for neuro-symbolic geometry systems such as AlphaGeometry, whose theorem-proving engine requires inputs in a sp…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/machine-learning
---

# NL2AGBench: Benchmarking LLM Auto-Formalization for AlphaGeometry

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.28481v1)
- published:: 2026-08-28
- updated:: 2026-08-28
- arxiv_id:: 2608.28481v1
- pdf:: https://arxiv.org/pdf/2608.28481v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Recent advances in large language models (LLMs) have demonstrated strong capabilities in natural language understanding and mathematical reasoning. However, their ability to translate informal mathematical problems into formal representations remains underexplored. This limitation is particularly important for neuro-symbolic geometry systems such as AlphaGeometry, whose theorem-proving engine requires inputs in a specialized domain-specific language (DSL). Although AlphaGeometry achieves near-IMO gold-medalist performance, manually converting natural-language problems into its formal syntax remains a significant usability bottleneck. To address this challenge, we introduce the Natural Language to AlphaGeometry Benchmark (NL2AGBench), which evaluates LLMs in translating English geometry problems into AlphaGeometry-compatible formal representations. NL2AGBench uses execution-based verification within AlphaGeometry to assess translation quality rather than relying solely on textual similarity. We evaluate ten state-of-the-art open- and closed-source LLMs across multiple parameter scales and analyze executable translation accuracy, syntactic correctness, and error characteristics. Our experiments reveal a substantial performance gap between closed- and open-source models: leading closed-source models achieve executable translation rates above 80%, while even the largest open-source models struggle to consistently preserve geometric constraints and produce valid formalizations. We introduce an error taxonomy distinguishing syntax and logic errors and investigate mitigation strategies, including few-shot prompting, fine-tuning, and human-guided hinting, which yield measurable improvements across multiple model families.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.28481v1)
- [PDF](https://arxiv.org/pdf/2608.28481v1)
- [OlympiadBench: A Challenging Benchmark for Promoting AGI with Olympiad-Level Bilingual Multimodal Scientific Problems](https://arxiv.org/abs/2402.14008) (2024, citations: 1279)
- [DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models](https://arxiv.org/abs/2402.03300) (2024, citations: 8464)
- [Solving olympiad geometry without human demonstrations](https://www.nature.com/articles/s41586-023-06747-5.pdf) (2024, citations: 853)
- [LeanDojo: Theorem Proving with Retrieval-Augmented Language Models](https://arxiv.org/abs/2306.15626) (2023, citations: 563)
- [Draft, Sketch, and Prove: Guiding Formal Theorem Provers with Informal Proofs](https://arxiv.org/abs/2210.12283) (2022, citations: 350)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/machine-learning
