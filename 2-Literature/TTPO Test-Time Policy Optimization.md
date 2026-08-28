---
title: "TTPO: Test-Time Policy Optimization"
source: "https://arxiv.org/html/2608.27448v1"
author: "Aozhe Wang, Zhengxi Lu, Jianze Wang, Shangke Lv, Ying Liu, Weiming Lu, Jun Xiao, Yueting Zhuang, Hua Yang, Qianglong Chen, Yongliang Shen"
published: "2026-08-27"
created: 2026-08-29
description: "Recent prominent post-training methods, such as Reinforcement Learning (RL) and On-Policy Self-Distillation (OPSD), have driven rapid progress in mathematical reasoning for large language models, yet their reliance on ground-truth labels precludes test-time training (TTT). Replacing ground truth with majority-vote pseudo-labels is a natural alternative, yet it is fragile: an incorrect vote corrupts the teacher and m…"
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
  - keyword/machine-learning
---

# TTPO: Test-Time Policy Optimization

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27448v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27448v1
- pdf:: https://arxiv.org/pdf/2608.27448v1
- categories:: cs.CL

## Abstract / Summary
Recent prominent post-training methods, such as Reinforcement Learning (RL) and On-Policy Self-Distillation (OPSD), have driven rapid progress in mathematical reasoning for large language models, yet their reliance on ground-truth labels precludes test-time training (TTT). Replacing ground truth with majority-vote pseudo-labels is a natural alternative, yet it is fragile: an incorrect vote corrupts the teacher and misleads every token. We observe that this failure mode is asymmetric: rollouts that disagree with the pseudo-label are typically wrong regardless of whether the vote itself is correct. Building on this observation, we propose Test-Time Policy Optimization (TTPO), an asymmetric objective that distills agreeing rollouts via OPSD and penalizes disagreeing rollouts with Grouped RL. Token-level selection further refines both branches: distillation down-weights already-converged positions, while RL penalizes only confident errors. Both updates remain well-grounded even under frequent pseudo-label errors, and majority-vote routing yields tighter self-supervision as the model improves. Without any labels, TTPO matches label-supervised OPSD on five competition-level benchmarks, raises Qwen3-1.7B from 38.0% to 45.2% in TTT, yields +25.2% to +36.4% without thinking, and shows strong cross-task generalization.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27448v1)
- [PDF](https://arxiv.org/pdf/2608.27448v1)
- [On-Policy Self-Distillation without Any Supervision](https://arxiv.org/abs/2608.06296) (2026, citations: 1)
- [Hi-TTRL: Regulating Consensus with Hints for Test-Time Reinforcement Learning](https://arxiv.org/abs/2608.03545) (2026, citations: 1)
- [Distill Where You Fail: Recovering Learning Signals of Negative RL-Groups from Adaptive Teacher Guidance](https://arxiv.org/abs/2608.00782) (2026, citations: 2)
- [Consensus as Privileged Context for Label-Free Self-Distillation](https://arxiv.org/abs/2607.13643) (2026, citations: 1)
- [Finding the Evidence: Discovering Decision-Supporting Tokens for On-Policy Reasoning Distillation](https://arxiv.org/abs/2606.22830) (2026, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/machine-learning
