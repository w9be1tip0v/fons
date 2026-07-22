---
title: "Prompt Design at Scale: How Format, Instruction Count, and Context Length Shape Instruction Adherence and Hallucination in Large Language Models"
source: "https://arxiv.org/html/2607.19257v1"
author: "Netanel Eliav"
published: "2026-07-21"
created: 2026-07-23
description: "Practitioners make three prompt-design decisions with almost no controlled evidence behind them: how to format instructions and context (markdown, plain text, prose, or tabular), how many simultaneous instructions a system prompt can carry before compliance degrades, and how much context a model can hold before recall and honesty degrade. We report two controlled experiments crossing all three factors on one held, c…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
---

# Prompt Design at Scale: How Format, Instruction Count, and Context Length Shape Instruction Adherence and Hallucination in Large Language Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.19257v1)
- published:: 2026-07-21
- updated:: 2026-07-21
- arxiv_id:: 2607.19257v1
- pdf:: https://arxiv.org/pdf/2607.19257v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Practitioners make three prompt-design decisions with almost no controlled evidence behind them: how to format instructions and context (markdown, plain text, prose, or tabular), how many simultaneous instructions a system prompt can carry before compliance degrades, and how much context a model can hold before recall and honesty degrade. We report two controlled experiments crossing all three factors on one held, contamination-free synthetic corpus (the "Book of Veyra," 8,780 uniquely-named entities, deterministically regenerable from a fixed seed), evaluated across five models. Experiment 1 (960 calls/model) measures instruction-following decay as rule count N grows from 10 to 160, crossed with four formats and system-prompt vs. user-turn placement. Perfect-response rate collapses to zero by N=80 for every model, format, and placement. Placement produces effects at least as large as format at N=160 in most models, but the direction is model-specific. No model shows a reliable markdown advantage; one 35B model favors plain text instead. Experiment 2 (5,520 calls/model) measures recall accuracy, false-premise sycophancy, and absent-fact fabrication across a 2k-to-512k-token context ladder in the same four formats. Recall stays near ceiling through 64-128k tokens, then degrades sharply and format-dependently: one model's accuracy spread reaches 48 points at 128k tokens. Fabrication never occurs (0/5,760 probes), and sycophancy stays negligible (<=8.3%). What rises sharply near each model's context ceiling is outright refusal to answer (0% to 79-90%), distinct from sycophancy or fabrication. Neither pre-registered format ordering holds, and token overhead (+22% to +37% over plain text) further changes which format is preferable where accuracy spread is genuine. We releas…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.19257v1)
- [PDF](https://arxiv.org/pdf/2607.19257v1)
- [When Instructions Multiply: Measuring and Estimating LLM Capabilities of Multiple Instructions Following](https://arxiv.org/abs/2509.21051) (2025, citations: 5)
- [Interaction Context Often Increases Sycophancy in LLMs](https://arxiv.org/abs/2509.12517) (2025, citations: 24)
- [Format as a Prior: Quantifying and Analyzing Bias in LLMs for Heterogeneous Data](https://arxiv.org/abs/2508.15793) (2025, citations: 3)
- [How Many Instructions Can LLMs Follow at Once?](https://arxiv.org/abs/2507.11538) (2025, citations: 15)
- [A Controllable Examination for Long-Context Language Models](https://arxiv.org/abs/2506.02921) (2025, citations: 7)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation
