---
title: "BLOOM-WILT: Logit Tilting for Behaviour Elicitation in Automated LLM Auditing"
source: "https://arxiv.org/html/2608.31105v1"
author: "Adrians Skapars, Edoardo Manino"
published: "2026-08-31"
created: 2026-09-02
description: "Users of a deployed language model routinely encounter behaviours that testing almost never surfaces, since deployment puts the model through orders of magnitude more interactions than any evaluation can simulate. Automated auditors make testing cheap to scale and flexible enough to cover almost any specified behaviour, yet their lack of optimisation pressure makes them sample-inefficient. To address this shortcomin…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/safety
  - keyword/machine-learning
---

# BLOOM-WILT: Logit Tilting for Behaviour Elicitation in Automated LLM Auditing

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.31105v1)
- published:: 2026-08-31
- updated:: 2026-08-31
- arxiv_id:: 2608.31105v1
- pdf:: https://arxiv.org/pdf/2608.31105v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
Users of a deployed language model routinely encounter behaviours that testing almost never surfaces, since deployment puts the model through orders of magnitude more interactions than any evaluation can simulate. Automated auditors make testing cheap to scale and flexible enough to cover almost any specified behaviour, yet their lack of optimisation pressure makes them sample-inefficient. To address this shortcoming, we introduce BLOOM-WILT, a full auditing pipeline that elicits natural multi-turn instances of rare behaviours, without training cost or access beyond the target's next-token distribution. On the input side, WILT's auditor model revises its conversational strategy across rounds, learning from previous scored interactions. On the output side, WILT adaptively reweights the target's decoding using the model's own distribution conditioned on an elicitation prompt, so that behaviour-relevant generations are sampled ahead of others it finds equally probable when unprompted. We evaluate WILT across 4 target models and 8 behaviours, where it beats the baseline auditor in 30 of the 32 settings and overturns the previous model safety rankings. WILT raises average behaviour presence from 51% to 100% when eliciting self-harm encouragement from Qwen3.5-4B, beating every elicitation method we port into the same pipeline at matched compute, without pushing output probability below the baseline's.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.31105v1)
- [PDF](https://arxiv.org/pdf/2608.31105v1)
- [AuditBench: Evaluating Alignment Auditing Techniques on Models with Hidden Behaviors](https://arxiv.org/abs/2602.22755) (2026, citations: 26)
- [Eliciting Behaviors in Multi-Turn Conversations](https://arxiv.org/abs/2512.23701) (2025, citations: 3)
- [Sampling-aware Adversarial Attacks Against Large Language Models](https://arxiv.org/abs/2507.04446) (2025, citations: 8)
- [Data Swarms: Optimizable Generation of Synthetic Evaluation Data](https://arxiv.org/abs/2506.00741) (2025, citations: 2)
- [Large Language Models Often Know When They Are Being Evaluated](https://arxiv.org/abs/2505.23836) (2025, citations: 94)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/safety #keyword/machine-learning
