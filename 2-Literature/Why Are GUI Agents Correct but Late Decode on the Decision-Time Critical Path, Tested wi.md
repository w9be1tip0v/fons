---
title: "Why Are GUI Agents Correct but Late? Decode on the Decision-Time Critical Path, Tested with Pre-Compiled Policy Trees"
source: "https://arxiv.org/html/2607.28399v1"
author: "Zihan Dong, Rui Qian, Qishi Zhan, Dongshen Peng, Kaixin Li, Yu Li"
published: "2026-07-30"
created: 2026-08-02
description: "Computer-use agents often fail on transient GUI events because they produce the correct action only after the relevant window has already closed. We identify the main cause as expensive autoregressive decoding on the decision-time critical path. We propose Adaptive Anticipatory Policy Trees (AAPT), which eliminates this delay without modifying the underlying model. During idle screen periods, the same frozen multimo…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/nlp
  - keyword/multimodal
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
---

# Why Are GUI Agents Correct but Late? Decode on the Decision-Time Critical Path, Tested with Pre-Compiled Policy Trees

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.28399v1)
- published:: 2026-07-30
- updated:: 2026-07-30
- arxiv_id:: 2607.28399v1
- pdf:: https://arxiv.org/pdf/2607.28399v1
- categories:: cs.LG

## Abstract / Summary
Computer-use agents often fail on transient GUI events because they produce the correct action only after the relevant window has already closed. We identify the main cause as expensive autoregressive decoding on the decision-time critical path. We propose Adaptive Anticipatory Policy Trees (AAPT), which eliminates this delay without modifying the underlying model. During idle screen periods, the same frozen multimodal model constructs a bounded conditional policy tree with observable guards, pre-authorized actions, and branch-specific deadlines. The tree is sized to cover the model's own decoding latency. When an event occurs, a lightweight observer matches change-gated frames to a prepared branch and immediately executes the corresponding action without generating new text. In paired trials with pre-registered endpoints and exact McNemar tests, AAPT improves the success rate from 0.50 to 0.79 within a contested decision window ($p=1.8\times10^{-3}$), while producing no incorrect actions. Both open-loop and predict-and-replan baselines achieve zero success because they still decode during execution. A preparation-time sweep shows that the gain emerges where the latency-based tree-sizing rule predicts, and ablations reveal three key requirements: fast observer decoding, valid tree planning, and accurate branch routing. A pre-registered oracle probe rejects our initial hypothesis and instead points to branch routing as the causal bottleneck. We further reproduce the effect on an independent general-purpose multimodal model over 126 paired trials ($p=4.9\times10^{-13}$). On an external benchmark, AAPT matches the overall performance of a reactive baseline, although the two methods exhibit complementary strengths. Together, these results suggest that AAPT performs best wh…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.28399v1)
- [PDF](https://arxiv.org/pdf/2607.28399v1)
- [SKILL.nb: Selective Formalization and Gated Execution for Durable Agent Workflows](https://arxiv.org/abs/2606.08049) (2026, citations: 1)
- [Benchmarking and Improving GUI Agents in High-Dynamic Environments](https://arxiv.org/abs/2604.25380) (2026, citations: 1)
- [AgenticCache: Cache-Driven Asynchronous Planning for Embodied AI Agents](https://arxiv.org/abs/2604.24039) (2026, citations: 1)
- [Anticipatory Planning for Multimodal AI Agents](https://arxiv.org/abs/2603.16777) (2026, citations: 4)
- [DynaWeb: Model-Based Reinforcement Learning of Web Agents](https://arxiv.org/abs/2601.22149) (2026, citations: 10)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/nlp #keyword/multimodal #keyword/evaluation #keyword/benchmark #keyword/agents
