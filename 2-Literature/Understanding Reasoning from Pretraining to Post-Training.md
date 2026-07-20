---
title: "Understanding Reasoning from Pretraining to Post-Training"
source: "https://arxiv.org/html/2607.16097v1"
author: "Jingyan Shen, Ang Li, Salman Rahman, Yifan Sun, Micah Goldblum, Matus Telgarsky, Pavel Izmailov"
published: "2026-07-17"
created: 2026-07-21
description: "Reinforcement learning (RL) has become central to improving large language models (LLMs) on complex reasoning tasks, yet RL post-training is largely studied in isolation from the pretraining that precedes it. As a result, two basic questions remain open: (1) how do pretraining choices (model size, data) shape the returns to RL compute, and (2) what does RL actually do to the model? These questions are difficult to s…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/reasoning
  - keyword/machine-learning
---

# Understanding Reasoning from Pretraining to Post-Training

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.16097v1)
- published:: 2026-07-17
- updated:: 2026-07-17
- arxiv_id:: 2607.16097v1
- pdf:: https://arxiv.org/pdf/2607.16097v1
- categories:: cs.LG, cs.AI, cs.CL

## Abstract / Summary
Reinforcement learning (RL) has become central to improving large language models (LLMs) on complex reasoning tasks, yet RL post-training is largely studied in isolation from the pretraining that precedes it. As a result, two basic questions remain open: (1) how do pretraining choices (model size, data) shape the returns to RL compute, and (2) what does RL actually do to the model? These questions are difficult to study in the standard LLM setting: pretraining corpora are vast and uncontrolled, making it hard to attribute behaviors to pretraining versus RL, and systematic compute sweeps across both stages are prohibitively expensive. To address these challenges, we use chess as a controlled testbed for studying reasoning across the full pretraining-to-post-training pipeline. We follow the standard LLM training pipeline by pretraining language models from 5M to 1B parameters on human chess games, supervised fine-tuning on synthetic reasoning traces, and running RL on chess puzzles with verifiable rewards. Using this framework, we find that the post-RL performance at given RL compute level is well-predicted from the pretraining loss, and slope of the RL reward curves improves approximately linearly with the pretraining tokens. Beyond scaling, we find that RL does not simply sharpen the SFT policy: on easy puzzles it amplifies correct moves the SFT policy already preferred, while on hard puzzles it surfaces correct moves that were nearly absent under SFT. We further test whether our findings transfer beyond chess by training a 1B language model on math-domain text, where the same predictive pattern emerges: longer-pretrained checkpoints reach higher post-RL performance and improve faster under RL. In sum, we provide a quantitative account of the pretraining-to-RL interfac…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.16097v1)
- [PDF](https://arxiv.org/pdf/2607.16097v1)
- [RL Excursions during Pre-Training: Re-examining Policy Optimization for LLM training](https://arxiv.org/abs/2606.04272) (2026, citations: 1)
- [Test-Time Scaling Makes Overtraining Compute-Optimal](https://arxiv.org/abs/2604.01411) (2026, citations: 1)
- [IsoCompute Playbook: Optimally Scaling Sampling Compute for LLM RL](https://arxiv.org/abs/2603.12151) (2026, citations: 1)
- [On the Interplay of Pre-Training, Mid-Training, and RL on Reasoning Language Models](https://arxiv.org/abs/2512.07783) (2025, citations: 57)
- [Reasoning with Sampling: Your Base Model is Smarter Than You Think](https://arxiv.org/abs/2510.14901) (2025, citations: 71)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/reasoning #keyword/machine-learning
