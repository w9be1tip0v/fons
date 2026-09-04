---
title: "Sequential Beats Joint: On the Interplay between On-Policy Distillation and RLVR"
source: "https://arxiv.org/html/2609.04108v1"
author: "Boyan Li, Bingsen Chen, Chenghao Yang, Ping Nie, Chen Zhao, Xi Ye"
published: "2026-09-03"
created: 2026-09-05
description: "Reinforcement learning with verifiable rewards (RLVR) and on-policy distillation (OPD) have emerged as two dominant methods for post-training reasoning LLMs. Prior work uses OPD's dense token-level supervision to complement the sparse RL reward, fusing the two signals within a single step: either as a \emph{weighted-additive combination} or a \emph{teacher-modulated rescaling} of the RL advantage. In this paper, we…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/machine-learning
  - keyword/research-paper
---

# Sequential Beats Joint: On the Interplay between On-Policy Distillation and RLVR

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.04108v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.04108v1
- pdf:: https://arxiv.org/pdf/2609.04108v1
- categories:: cs.CL, cs.AI, cs.LG

## Abstract / Summary
Reinforcement learning with verifiable rewards (RLVR) and on-policy distillation (OPD) have emerged as two dominant methods for post-training reasoning LLMs. Prior work uses OPD's dense token-level supervision to complement the sparse RL reward, fusing the two signals within a single step: either as a \emph{weighted-additive combination} or a \emph{teacher-modulated rescaling} of the RL advantage. In this paper, we show that a simple two-stage scheme, OPD-then-RL, consistently outperforms pure OPD, pure RLVR, and all such joint baselines across logic and math reasoning benchmarks. Beyond the empirical results, we further provide a systematic understanding of this through pass@$k$ behavior, learning dynamics, and parameter updates, yielding a consistent explanation: OPD expands the student's coverage of teacher-supported solutions and RL sharpens within that support, while jointly optimizing the two signals causes them to interfere.To provide a practical recipe, we find that the OPD validation score is the key signal for when to switch to RL, and that OPD is a better cold start for RL than SFT. Together, our results establish OPD-then-RL as a simple yet strong way to combine the two methods, turning two entangled signals into complementary stages.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.04108v1)
- [PDF](https://arxiv.org/pdf/2609.04108v1)
- [Beyond GRPO and On-Policy Distillation: An Empirical Sparse-to-Dense Reward Principle for Language-Model Post-Training](https://arxiv.org/abs/2605.12483) (2026, citations: 7)
- [GEAR: Granularity-Adaptive Advantage Reweighting for LLM Agents via Self-Distillation](https://arxiv.org/abs/2605.11853) (2026, citations: 7)
- [Rebellious Student: Reversing Teacher Signals for Reasoning Exploration with Self-Distilled RLVR](https://arxiv.org/abs/2605.10781) (2026, citations: 11)
- [Beyond SFT-to-RL: Pre-alignment via Black-Box On-Policy Distillation for Multimodal RL](https://arxiv.org/abs/2604.28123) (2026, citations: 7)
- [SFT-then-RL Outperforms Mixed-Policy Methods for LLM Reasoning](https://arxiv.org/abs/2604.23747) (2026, citations: 8)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/machine-learning #keyword/research-paper
