---
title: "What, Where, and How: Disentangling the Roles of Task, Language, and Model in Code Model Representations"
source: "https://arxiv.org/html/2607.21491v1"
author: "Piotr Wilam"
published: "2026-07-23"
created: 2026-07-25
description: "Do independently trained language models come to represent the same thing in the same way? We answer for code, extending a recently introduced concept-circuit extraction method to a 2x2 design -- Python and Rust crossed with Qwen2.5-Coder-7B and DeepSeek-Coder-V1-6.7B -- and measuring a complete inventory of grammatical concepts (58 Python, 57 Rust) identically in all four cells: the smallest design that separates w…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
---

# What, Where, and How: Disentangling the Roles of Task, Language, and Model in Code Model Representations

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.21491v1)
- published:: 2026-07-23
- updated:: 2026-07-23
- arxiv_id:: 2607.21491v1
- pdf:: https://arxiv.org/pdf/2607.21491v1
- categories:: cs.CL, cs.LG

## Abstract / Summary
Do independently trained language models come to represent the same thing in the same way? We answer for code, extending a recently introduced concept-circuit extraction method to a 2x2 design -- Python and Rust crossed with Qwen2.5-Coder-7B and DeepSeek-Coder-V1-6.7B -- and measuring a complete inventory of grammatical concepts (58 Python, 57 Rust) identically in all four cells: the smallest design that separates what depends on the task, the language, and the model. The answer splits into three parts. What earns dedicated circuitry is set by the task: the models agree on which concepts receive circuits (Spearman $ρ$ = 0.638 for Python, 0.673 for Rust, both p < $10^{-7}$). Where those circuits sit is set by the model: Qwen processes concepts in a late band (~L17-19), DeepSeek at L6-7, for both languages. How circuits grow across layers is also set by the model: Qwen gives its atomic concepts an early spike that DeepSeek does not. "Are circuits universal?" thus has no single answer: yes for What, no for Where and How -- universality is a property of representational content, not of computational organisation. None of this structure was fixed in advance. The agreement could have landed anywhere between independence and identity; it lands at $ρ\approx 0.65$. Rust constructs receive 2-3x more concept-specific circuitry than their Python equivalents, in both models. Both models share neurons between the languages (6/7 and 7/7 paired constructs), DeepSeek 1.94x more than Qwen -- a direction no prior result predicts. And Qwen binds nine keywords of Rust's type-and-trait machinery into one tight neuron cluster (Jaccard 0.535 vs null 0.112, p < 0.001), a semantic dimension invisible in surface syntax. Ablation and linear probes confirm the circuits are functional. All claims a…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.21491v1)
- [PDF](https://arxiv.org/pdf/2607.21491v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp
