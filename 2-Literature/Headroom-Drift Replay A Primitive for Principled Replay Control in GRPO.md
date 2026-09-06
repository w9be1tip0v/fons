---
title: "Headroom-Drift Replay: A Primitive for Principled Replay Control in GRPO"
source: "https://arxiv.org/html/2609.03941v1"
author: "Hyun Bin Park, Du-Seong Chang"
published: "2026-09-03"
created: 2026-09-07
description: "RL-based post-training for reasoning models is increasingly bottlenecked by repeated fresh rollout generation, particularly in agentic settings where environment interaction dominates wall-clock cost. Replay can reduce this burden by reusing past trajectories, but existing methods typically embed it within larger training pipelines involving exploration, experience restructuring, or mixed-policy optimization. This m…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/multimodal
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/agents
  - keyword/machine-learning
---

# Headroom-Drift Replay: A Primitive for Principled Replay Control in GRPO

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.03941v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.03941v1
- pdf:: https://arxiv.org/pdf/2609.03941v1
- categories:: cs.LG, cs.AI, cs.CL

## Abstract / Summary
RL-based post-training for reasoning models is increasingly bottlenecked by repeated fresh rollout generation, particularly in agentic settings where environment interaction dominates wall-clock cost. Replay can reduce this burden by reusing past trajectories, but existing methods typically embed it within larger training pipelines involving exploration, experience restructuring, or mixed-policy optimization. This makes replay's own contribution difficult to isolate. We ask a focused question: how far can principled replay selection alone go? We introduce Headroom-Drift Replay, a group-level replay control primitive for GRPO that separates reuse into two decisions. Headroom ranks stored groups by remaining learning value, while Drift gates them by compatibility with the current policy. The fresh on-policy stream remains unchanged, and the method adds no auxiliary generation or training machinery. Across mathematical reasoning, multimodal reasoning, and Agentic Search benchmarks, this single intervention outperforms naive replay and matches or exceeds broader replay methods on Avg Mean@32. In Agentic Search, where environment interaction dominates cost, it delivers comparable quality at materially lower wall-clock time.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.03941v1)
- [PDF](https://arxiv.org/pdf/2609.03941v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/multimodal #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/agents #keyword/machine-learning
