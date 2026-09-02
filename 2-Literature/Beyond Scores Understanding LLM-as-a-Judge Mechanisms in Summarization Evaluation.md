---
title: "Beyond Scores: Understanding LLM-as-a-Judge Mechanisms in Summarization Evaluation"
source: "https://arxiv.org/html/2609.01604v1"
author: "Himil Vasava, Ming Jiang"
published: "2026-09-01"
created: 2026-09-03
description: "LLM-based evaluators of natural language generation (NLG) quality are widely deployed as scoring tools and as automated training signals, yet the internal procedure by which they assign a rating remains poorly understood. We investigate this procedure mechanistically through an eight-attack perturbation taxonomy across the Readability and Adequacy dimensions of NLG quality, a generation pipeline that produces paired…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/transformer
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/agents
  - keyword/machine-learning
---

# Beyond Scores: Understanding LLM-as-a-Judge Mechanisms in Summarization Evaluation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.01604v1)
- published:: 2026-09-01
- updated:: 2026-09-01
- arxiv_id:: 2609.01604v1
- pdf:: https://arxiv.org/pdf/2609.01604v1
- categories:: cs.CL, cs.LG

## Abstract / Summary
LLM-based evaluators of natural language generation (NLG) quality are widely deployed as scoring tools and as automated training signals, yet the internal procedure by which they assign a rating remains poorly understood. We investigate this procedure mechanistically through an eight-attack perturbation taxonomy across the Readability and Adequacy dimensions of NLG quality, a generation pipeline that produces paired clean and corrupt summaries with controlled error intensity and explicit token-level modification maps, and a four-experiment battery of causal tracing, logit-lens vocabulary projection, and attention-head knockout applied to Themis (Llama-3-8B) and Prometheus (Mistral-7B). Both evaluators implement a structured, coherent evaluation pipeline operating in two stages: below layer 15, attention performs local error comparison and routes the result to the final input position; above it, the MLP cascade integrates the signal and writes the rating, with the decision crystallizing in the residual stream at a sharp late layer (L = 26 on Themis, L = 25 on Prometheus). Furthermore, a base-model control at the same scale (Llama-3-8B) reproduces the routing architecture and crystallization but not the stage separation, isolating the two mechanisms that fine-tuning specifically installs, suppression of below-L15 MLP contribution at the last position and a two-layer advance of the crystallization depth, indicating that fine-tuning sculpts an existing substrate rather than building the pipeline from scratch. We release the source code and data at https://github.com/himil-v/judge-mech

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.01604v1)
- [PDF](https://arxiv.org/pdf/2609.01604v1)
- [Prometheus 2: An Open Source Language Model Specialized in Evaluating Other Language Models](https://arxiv.org/abs/2405.01535) (2024, citations: 521)
- [Are LLM-based Evaluators Confusing NLG Quality Criteria?](https://arxiv.org/abs/2402.12055) (2024, citations: 56)
- [FActScore: Fine-grained Atomic Evaluation of Factual Precision in Long Form Text Generation](https://arxiv.org/abs/2305.14251) (2023, citations: 1639)
- [G-Eval: NLG Evaluation using GPT-4 with Better Human Alignment](https://arxiv.org/abs/2303.16634) (2023, citations: 3041)
- [Interpretability in the Wild: a Circuit for Indirect Object Identification in GPT-2 small](https://arxiv.org/abs/2211.00593) (2022, citations: 1248)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/transformer #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/agents #keyword/machine-learning
