---
title: "ContextPilot: Teaching Agents for Proactive Context Management via Fine-grained RL"
source: "https://arxiv.org/html/2608.28476v1"
author: "Zhuoshi Pan, Qizhi Pei, Junru Lu, Honglin Lin, H. Vicky Zhao, Di Yin, Xing Sun"
published: "2026-08-28"
created: 2026-09-01
description: "Long-horizon agentic tasks require large language models (LLMs) to iteratively retrieve, integrate, and maintain dispersed information across multi-turn interactions, but preserving all interaction histories leads to a continuously growing working context. Recent proactive context management methods allow models to edit their own working context with specialized tools, yet they still face three key limitations: (1)…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/agents
---

# ContextPilot: Teaching Agents for Proactive Context Management via Fine-grained RL

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.28476v1)
- published:: 2026-08-28
- updated:: 2026-08-28
- arxiv_id:: 2608.28476v1
- pdf:: https://arxiv.org/pdf/2608.28476v1
- categories:: cs.CL

## Abstract / Summary
Long-horizon agentic tasks require large language models (LLMs) to iteratively retrieve, integrate, and maintain dispersed information across multi-turn interactions, but preserving all interaction histories leads to a continuously growing working context. Recent proactive context management methods allow models to edit their own working context with specialized tools, yet they still face three key limitations: (1) a limited toolset restricted to search, deletion, and summarization, with no support for global planning, long-term memory, and adaptive compression; (2) inefficient exploration that treats context management actions uniformly despite their heterogeneous impacts on final outcomes; and (3) coarse-grained credit assignment that assigns the final trajectory-level reward to all intermediate context editing actions during RL. To bridge these gaps, we introduce ContextPilot, a proactive context management framework for long-horizon agentic reasoning. Our approach systematically augments the toolset with planning, long-term memory, and soft context offloading tools. We further propose an RL method tailored for context management, which uses context and entropy variation to identify critical editing decisions for branch sampling and estimates action-level advantages from all branched trajectories that pass through the corresponding context editing action. Experiments on long-context QA and deep search tasks show that ContextPilot achieves stronger performance with a more compact working context, consistently outperforming existing baselines across various base models and benchmarks. Code is available at https://github.com/Tencent/ContextPilot.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.28476v1)
- [PDF](https://arxiv.org/pdf/2608.28476v1)
- [From Plan to Action: How Well Do Agents Follow the Plan?](https://arxiv.org/abs/2604.12147) (2026, citations: 6)
- [OpenSeeker: Democratizing Frontier Search Agents by Fully Open-Sourcing Training Data](https://arxiv.org/abs/2603.15594) (2026, citations: 25)
- [The Pensieve Paradigm: Stateful Language Models Mastering Their Own Context](https://arxiv.org/abs/2602.12108) (2026, citations: 6)
- [U-Fold: Dynamic Intent-Aware Context Folding for User-Centric Agents](https://arxiv.org/abs/2601.18285) (2026, citations: 6)
- [Structured Episodic Event Memory](https://arxiv.org/abs/2601.06411) (2026, citations: 3)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/agents
