---
title: "Hindcast: Replaying Prediction Markets to Evaluate LLM Forecasters"
source: "https://arxiv.org/html/2607.14051v1"
author: "Xiao Ye, Jacob Dineen, Evan Zhu, Shijie Lu, Kevin Song, Ben Zhou"
published: "2026-07-15"
created: 2026-07-16
description: "Hindcast closes leakage in LLM forecasting evals by replaying resolved Polymarket markets against a frozen pre-cutoff Reddit snapshot, grading models as if they stood before the outcome existed in retrieval or training data."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/evaluation
  - keyword/reasoning
  - keyword/llm
---

# Hindcast: Replaying Prediction Markets to Evaluate LLM Forecasters

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.14051v1)
- published:: 2026-07-15
- updated:: 2026-07-15
- arxiv_id:: 2607.14051v1
- pdf:: https://arxiv.org/pdf/2607.14051v1
- categories:: cs.CL

## Abstract / Summary
Forecasters are evaluated by backtesting, which replays resolved questions and grades the probability the system would have assigned before the outcome was known. For LLMs, two channels leak the answer: retrieval of post-event reports, and training data that already contains the outcome. Hindcast closes both leaks by grading a model as if it stood at a chosen past date t0, replaying resolved Polymarket markets against a frozen public Reddit snapshot and scoring forecasts against both ground truth and the market price at t0. Once the leak is closed, retrieval still helps most models only where Reddit discussed the event beforehand; where the archive carried only speculation, retrieval hurts.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.14051v1)
- [PDF](https://arxiv.org/pdf/2607.14051v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/evaluation #keyword/reasoning #keyword/llm
