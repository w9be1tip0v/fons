---
title: "Rethinking Reward Supervision: Rubric-Conditioned Self-Distillation"
source: "https://arxiv.org/html/2606.19327v1"
author: "Siyi Gu, Jialin Chen, Sophia Zhou, Arman Cohan, Rex Ying"
published: "2026-06-17"
created: 2026-06-19
description: "Post-training of reasoning language models is commonly driven by supervised distillation and reinforcement learning with verifiable rewards. Distillation often relies on chain-of-thought annotations that are expensive to obtain and may themselves be noisy, incomplete, or partially incorrect; even when the final solution is correct, an imperfect rationale can interfere with learning. Reinforcement learning with verif…"
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

# Rethinking Reward Supervision: Rubric-Conditioned Self-Distillation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.19327v1)
- published:: 2026-06-17
- updated:: 2026-06-17
- arxiv_id:: 2606.19327v1
- pdf:: https://arxiv.org/pdf/2606.19327v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
Post-training of reasoning language models is commonly driven by supervised distillation and reinforcement learning with verifiable rewards. Distillation often relies on chain-of-thought annotations that are expensive to obtain and may themselves be noisy, incomplete, or partially incorrect; even when the final solution is correct, an imperfect rationale can interfere with learning. Reinforcement learning with verified rewards, on the other hand, typically compresses evaluative feedback into a scalar signal, obscuring which aspects of a response should be improved. We propose \textbf{Rubric-Conditioned Self-Distillation}, a framework that incorporates rubrics as structured, fine-grained feedback for on-policy self-distillation. Our method conditions the teacher model on criterion-level rubrics and uses it to provide token-level guidance on the student's own sampled trajectories. This design avoids treating a single reference rationale as the sole supervision target. Instead, rubrics specify what a strong response should satisfy, enabling more fine-grained credit assignment over the reasoning process than scalar reward optimization. We instantiate this framework with a two-stage pipeline that first learns to generate task-specific rubrics and then trains a rubric-guided reasoner. We evaluate on a diverse suite of science reasoning benchmarks and results show that rubric-conditioned self-distillation effectively converts rubric-level criteria into token-level guidance over the reasoning process, surpassing GRPO by 1.0 points and OPSD by 0.9 points on average.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.19327v1)
- [PDF](https://arxiv.org/pdf/2606.19327v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/machine-learning
