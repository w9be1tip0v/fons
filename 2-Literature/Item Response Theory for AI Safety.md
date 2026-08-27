---
title: "Item Response Theory for AI Safety"
source: "https://arxiv.org/html/2608.05086v1"
author: "Joshua Fonseca Rivera, Neil Shah, David Demitri Africa, Konstantinos Voudouris"
published: "2026-08-05"
created: 2026-08-07
description: "Language models differ in how safely they behave and these differences are measured by safety benchmarks. But aggregated benchmark scores are hard to trust and interpret, because benchmarks duplicate one another, correlate heavily, and models may sandbag when they detect evaluation. To address these issues, we draw on Item Response Theory (IRT), a statistical toolkit for measuring these latents from performance on i…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/safety
---

# Item Response Theory for AI Safety

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.05086v1)
- published:: 2026-08-05
- updated:: 2026-08-05
- arxiv_id:: 2608.05086v1
- pdf:: https://arxiv.org/pdf/2608.05086v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
Language models differ in how safely they behave and these differences are measured by safety benchmarks. But aggregated benchmark scores are hard to trust and interpret, because benchmarks duplicate one another, correlate heavily, and models may sandbag when they detect evaluation. To address these issues, we draw on Item Response Theory (IRT), a statistical toolkit for measuring these latents from performance on items with inferred psychometric properties. We fit IRT models to eight safety benchmarks across 192 language models, the largest psychometric analysis of LLM safety evaluations to date, and contribute three results. First, we find that three interpretable factors of refusal strictness, truthfulness, and contextual harm explain most of the variance between models across benchmarks. Second, psychometrically selected items recover full benchmark scores with lower error than random subsets of the same size, and roughly ten adaptively chosen items suffice for several individual benchmarks, cutting evaluation cost by 97-99%. Third, IRT supports audits of individual models, showing that it can be used to detect naive sandbagging and changes of model behind APIs. Overall, we show IRT is a ready-made toolkit for reading, reducing, and auditing safety benchmarks, which we recommend frontier labs and evaluators adopt.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.05086v1)
- [PDF](https://arxiv.org/pdf/2608.05086v1)
- [Adversarial Humanities Benchmark: Results on Stylistic Robustness in Frontier Model Safety](https://arxiv.org/abs/2604.18487) (2026, citations: 2)
- [Capabilities Ain't All You Need: Measuring Propensities in AI](https://arxiv.org/abs/2602.18182) (2026, citations: 5)
- [Measuring What AI Systems Might Do: Towards A Measurement Science in AI](https://arxiv.org/abs/2603.00063) (2026, citations: 2)
- [High-stakes psychomotor ability assessment: a military selection case study of practice effects in airplane tracking tasks](https://link.springer.com/content/pdf/10.1186/s41235-025-00672-z.pdf) (2025, citations: 1)
- [Model Equality Testing: Which Model Is This API Serving?](https://arxiv.org/abs/2410.20247) (2024, citations: 44)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/safety
