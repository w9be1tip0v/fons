---
title: "Selective State-Space Adaptation and Retrieval for Language Model Reasoning"
source: "https://arxiv.org/html/2607.19326v1"
author: "Atahan Dokme, Larry Heck"
published: "2026-07-21"
created: 2026-07-23
description: "Low-rank adaptation introduces a static learned update applied identically to every input. The update provides task-level adaptation but does not explicitly represent token-level or instance-level state variation. A family of adapters is proposed that introduces selective state-space recurrence at two complementary granularities. At the token level, \textbf{MaLoRA} (Mamba-modulated low-rank adaptation) makes the ada…"
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
  - keyword/reasoning
---

# Selective State-Space Adaptation and Retrieval for Language Model Reasoning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.19326v1)
- published:: 2026-07-21
- updated:: 2026-07-21
- arxiv_id:: 2607.19326v1
- pdf:: https://arxiv.org/pdf/2607.19326v1
- categories:: cs.CL

## Abstract / Summary
Low-rank adaptation introduces a static learned update applied identically to every input. The update provides task-level adaptation but does not explicitly represent token-level or instance-level state variation. A family of adapters is proposed that introduces selective state-space recurrence at two complementary granularities. At the token level, \textbf{MaLoRA} (Mamba-modulated low-rank adaptation) makes the adapter's scaling factor a dynamic input-dependent function with recurrent state across tokens, in contrast to the stateless modulators of prior work. At the context level, \textbf{MaRA} (Mamba Retrieval Adapter) tracks cross-segment state and selects the segments most relevant to the query, before the modulated language model generates its answer. Across three frozen backbones (Qwen-2.5-7B, Llama-3.1-8B, Gemma-2-9B) and two reasoning benchmarks (MuSiQue, 2WikiMultihopQA), the family improves reasoning accuracy on every cell of the $3{\times}2$ grid, by $+6.8$ F1 ($+10.5\%$ relative) on average and up to $+9.3$ F1 ($+18.2\%$ relative) on the hardest cell over the LoRA baseline, and the token-level gains carry to RULER QA-2 under length stress.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.19326v1)
- [PDF](https://arxiv.org/pdf/2607.19326v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/reasoning
