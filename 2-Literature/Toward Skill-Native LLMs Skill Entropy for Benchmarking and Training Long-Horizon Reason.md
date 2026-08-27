---
title: "Toward Skill-Native LLMs: Skill Entropy for Benchmarking and Training Long-Horizon Reasoning"
source: "https://arxiv.org/html/2608.05139v1"
author: "Yinghui He, Ling Yang, Jiarui Liu, Yongjin Yang, Lechen Zhang, Yingcheng Wu, Zhenfei Yin, Mengdi Wang, Sanjeev Arora"
published: "2026-08-05"
created: 2026-08-07
description: "Long-horizon reasoning in recent LLMs demands that the model switch between distinct skills inside a reasoning chain, such as first doing a math derivation, then using the result to plan a schedule. We call such problems cross-skill long-horizon tasks: multi-step tasks whose steps require different reasoning skills and depend on earlier outputs. Existing benchmarks often evaluate individual skills, lacking a princip…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/safety
  - keyword/machine-learning
---

# Toward Skill-Native LLMs: Skill Entropy for Benchmarking and Training Long-Horizon Reasoning

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.05139v1)
- published:: 2026-08-05
- updated:: 2026-08-05
- arxiv_id:: 2608.05139v1
- pdf:: https://arxiv.org/pdf/2608.05139v1
- categories:: cs.CL, cs.LG

## Abstract / Summary
Long-horizon reasoning in recent LLMs demands that the model switch between distinct skills inside a reasoning chain, such as first doing a math derivation, then using the result to plan a schedule. We call such problems cross-skill long-horizon tasks: multi-step tasks whose steps require different reasoning skills and depend on earlier outputs. Existing benchmarks often evaluate individual skills, lacking a principled way to measure how well a model switches between skills. We address this gap from both the evaluation and training sides. We introduce Skill Entropy, a measure of the difficulty of switching from one skill to another. We then propose Skill^2-Bench, a benchmark of cross-skill long-horizon tasks built over 558 skills across 9 verifiable and open-ended domains. Each task is assigned a task-level skill-entropy score and grouped into three difficulty levels. Evaluating 8 frontier and 4 open-source models on Skill^2-Bench reveals a skill-switching gap: accuracy decreases on higher-entropy tasks. We then turn skill entropy from a benchmark scale into a training signal. We propose Skill-Entropy RL, an RL framework where the model predicts not only the answer at each step but also the skill used to produce it. The reward combines step-level correctness with a skill-entropy reward that measures the alignment between the model-predicted skill sequence and the gold skill sequence. On Qwen3-4B-Instruct and Qwen3-1.7B, Skill-Entropy RL improves the Skill^2-Bench score from 34.4% to 68.4% and from 14.6% to 40.1%, respectively, outperforming competitive baselines. The same pipeline can be applied to off-the-shelf training data such as OpenR1-Math, indicating that skill entropy is a reusable training signal. Code available at: https://github.com/Gen-Verse/Skill-Entropy-RL

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.05139v1)
- [PDF](https://arxiv.org/pdf/2608.05139v1)
- [Transferability for General Reasoning: An Automated Curriculum for Multi-Domain RLVR](https://arxiv.org/abs/2606.25178) (2026, citations: 1)
- [SkillLearnBench: Benchmarking Continual Learning Methods for Agent Skill Generation on Real-World Tasks](https://arxiv.org/abs/2604.20087) (2026, citations: 21)
- [STaD: Scaffolded Task Design for Identifying Compositional Skill Gaps in LLMs](https://arxiv.org/abs/2604.18177) (2026, citations: 1)
- [Self-Distillation Zero: Self-Revision Turns Binary Rewards into Dense Supervision](https://arxiv.org/abs/2604.12002) (2026, citations: 36)
- [SkillRouter: Skill Routing for LLM Agents at Scale](https://arxiv.org/abs/2603.22455) (2026, citations: 33)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/safety #keyword/machine-learning
