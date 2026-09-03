---
title: "Dutch Books for Language Models"
source: "https://arxiv.org/html/2609.02797v1"
author: "Isaiah Andrews, Suproteem Sarkar"
published: "2026-09-02"
created: 2026-09-04
description: "People increasingly use language models to support life decisions. Many such decisions involve a probabilistic forecast: How likely is a major life event, a natural disaster, or an economic outcome? Users of language models may implicitly trust that these forecasts fall out of a coherent world model. In this paper, we evaluate the coherence of language model probabilistic forecasts through a procedure that builds on…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/machine-learning
  - keyword/research-paper
---

# Dutch Books for Language Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.02797v1)
- published:: 2026-09-02
- updated:: 2026-09-02
- arxiv_id:: 2609.02797v1
- pdf:: https://arxiv.org/pdf/2609.02797v1
- categories:: econ.GN, cs.AI, cs.CL, cs.LG

## Abstract / Summary
People increasingly use language models to support life decisions. Many such decisions involve a probabilistic forecast: How likely is a major life event, a natural disaster, or an economic outcome? Users of language models may implicitly trust that these forecasts fall out of a coherent world model. In this paper, we evaluate the coherence of language model probabilistic forecasts through a procedure that builds on a theorem due to de Finetti. We elicit forecasts from language models across events generated from stock returns data. We then use linear programs to compute the largest Dutch-book profit - the profit an arbitrageur could guarantee by betting against model-generated probabilities - which we use as a measure of incoherence. Our procedure does not require outcome labels, so we can evaluate coherence even in settings where outcomes are not observed or have not yet resolved. We find substantial evidence of incoherence in language model forecasts. Such incoherence increases when there are richer logical relationships between events, and irrelevant contextual details can increase incoherence by an order of magnitude. We conclude by discussing how alternative training strategies may improve probabilistic coherence.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.02797v1)
- [PDF](https://arxiv.org/pdf/2609.02797v1)
- [Revealed Rationality: Label-Free Evaluation and Regularization from Representation Theorems](https://arxiv.org/abs/2608.05015) (2026, citations: 1)
- [Position: It's Time to Optimize LLMs for Self-Consistency](https://arxiv.org/abs/2608.05188) (2026, citations: 2)
- [Elicitation Matters: How Prompts and Query Protocols Shape LLM Surrogates under Sparse Observations](https://arxiv.org/abs/2605.04764) (2026, citations: 1)
- [Poly-EPO: Training Exploratory Reasoning Models](https://arxiv.org/abs/2604.17654) (2026, citations: 4)
- [PolyBench: Benchmarking LLM Forecasting and Trading Capabilities on Live Prediction Market Data](https://arxiv.org/abs/2604.14199) (2026, citations: 11)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/machine-learning #keyword/research-paper
