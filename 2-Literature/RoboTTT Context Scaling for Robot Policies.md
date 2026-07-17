---
title: "RoboTTT: Context Scaling for Robot Policies"
source: "https://arxiv.org/html/2607.15275v1"
author: "Yunfan Jiang, Yevgen Chebotar, Ruijie Zheng, Fengyuan Hu, Yunhao Ge, Jimmy Wu, Tianyuan Dai, Scott Reed, Li Fei-Fei, Yuke Zhu, Linxi \"Jim\" Fan"
published: "2026-07-16"
created: 2026-07-17
description: "Test-time training robot policies scale visuomotor context to 8K timesteps without growing inference latency; +87% over single-step baselines and first full five-minute multi-stage assembly completion."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/agent
  - keyword/foundation-model
  - keyword/machine-learning
---

# RoboTTT: Context Scaling for Robot Policies

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15275v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15275v1
- pdf:: https://arxiv.org/pdf/2607.15275v1
- categories:: cs.AI / robotics

## Abstract / Summary
Robot foundation models usually use single-step or short-history context. RoboTTT (Test-Time-Training Robot Policies) scales visuomotor context to 8K timesteps (~three orders of magnitude beyond SOTA) without growing inference latency, enabling one-shot in-context imitation from human video, on-the-fly improvement, perturbation robustness, and stronger long-horizon multi-stage tasks. Integrates test-time training into VLA-style policies via fast weights updated by gradient descent at train and inference. Real-robot results: +87% overall vs single-step baseline; fully completes a five-minute ten-stage assembly no baseline finishes; 8K-context pretraining beats 1K by 62%. Context length proposed as a new scaling axis for robot foundation models. Site: https://research.nvidia.com/labs/gear/robottt/

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15275v1)
- [PDF](https://arxiv.org/pdf/2607.15275v1)
- [Project](https://research.nvidia.com/labs/gear/robottt/)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/agent #keyword/foundation-model #keyword/machine-learning
