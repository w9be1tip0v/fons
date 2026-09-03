---
title: "EarlyEval: Cheaper Agent Evaluation via Early Outcome Prediction"
source: "https://arxiv.org/html/2609.02783v1"
author: "Yuling Shi, Zhensu Sun, Junsen Dong, Chengcheng Wan, David Lo, Xiaodong Gu"
published: "2026-09-02"
created: 2026-09-04
description: "Evaluating LLM agents is essential for guiding their development, yet it has grown prohibitively expensive: a single pass of a frontier model over an agentic benchmark can cost hundreds to thousands of dollars, a price paid repeatedly across iterative development cycles. Prior efforts, centered on benchmark distillation, reduce the number of evaluation tasks but leave the cost of executing each retained task untouch…"
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
  - keyword/agents
---

# EarlyEval: Cheaper Agent Evaluation via Early Outcome Prediction

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.02783v1)
- published:: 2026-09-02
- updated:: 2026-09-02
- arxiv_id:: 2609.02783v1
- pdf:: https://arxiv.org/pdf/2609.02783v1
- categories:: cs.CL

## Abstract / Summary
Evaluating LLM agents is essential for guiding their development, yet it has grown prohibitively expensive: a single pass of a frontier model over an agentic benchmark can cost hundreds to thousands of dollars, a price paid repeatedly across iterative development cycles. Prior efforts, centered on benchmark distillation, reduce the number of evaluation tasks but leave the cost of executing each retained task untouched. In this work, we introduce early outcome prediction, a complementary axis of efficiency that instead cuts cost within each task. Our key insight is that an agent's final outcome is often evident from its intermediate behavior well before execution completes. We instantiate this idea in EarlyEval, a lightweight framework that trains a pair of LightGBM success and failure classifiers over behavioral, textual, and reference-solution features, and halts an agent run the moment either classifier crosses a calibrated confidence threshold, adding negligible per-step overhead. Across three benchmarks, SWE-bench Verified, TerminalBench, and Toolathlon, EarlyEval can eliminate 13%-26% of agent steps and up to 44.1% input tokens and 29.4% output tokens at 89%-97% prediction accuracy, while perturbing per-agent resolve rates by only one to two percentage points on average.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.02783v1)
- [PDF](https://arxiv.org/pdf/2609.02783v1)
- [SWE-Pruner Pro: The Coder LLM Already Knows What to Prune](https://arxiv.org/abs/2607.18213) (2026, citations: 2)
- [Are Performance-Optimization Benchmarks Reliably Measuring Coding Agents?](https://arxiv.org/abs/2607.01211) (2026, citations: 1)
- [Code Is More Than Text: Uncertainty Estimation for Code Generation](https://arxiv.org/abs/2606.09577) (2026, citations: 1)
- [BAGEN: Are LLM Agents Budget-Aware?](https://arxiv.org/abs/2606.00198) (2026, citations: 6)
- [Active Testing of Large Language Models via Approximate Neyman Allocation](https://arxiv.org/abs/2605.10075) (2026, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/agents
