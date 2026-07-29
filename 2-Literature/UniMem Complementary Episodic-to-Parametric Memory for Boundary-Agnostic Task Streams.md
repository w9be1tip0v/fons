---
title: "UniMem: Complementary Episodic-to-Parametric Memory for Boundary-Agnostic Task Streams"
source: "https://arxiv.org/html/2607.26017v1"
author: "Siyu Xia, Chenheng Zhang, Yanting Wu, Haoxuan Li, Jiajun Chai, Xiaohan Wang, Guojun Yin, Wei Lin, Zhouchen Lin, Haifeng Zhang, Jun Wang"
published: "2026-07-28"
created: 2026-07-30
description: "Memory is essential for LLM agents to accumulate task experience and reuse task-specific execution strategies. However, real-world deployment over boundary-agnostic and evolving task streams exposes a fundamental stability-plasticity dilemma. External retrieval-based memory can rapidly absorb new evidence, but it often fails to internalize recurring execution patterns and incurs inference-time retrieval overhead. Pa…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/retrieval
  - keyword/evaluation
  - keyword/agents
  - keyword/machine-learning
---

# UniMem: Complementary Episodic-to-Parametric Memory for Boundary-Agnostic Task Streams

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.26017v1)
- published:: 2026-07-28
- updated:: 2026-07-28
- arxiv_id:: 2607.26017v1
- pdf:: https://arxiv.org/pdf/2607.26017v1
- categories:: cs.CL

## Abstract / Summary
Memory is essential for LLM agents to accumulate task experience and reuse task-specific execution strategies. However, real-world deployment over boundary-agnostic and evolving task streams exposes a fundamental stability-plasticity dilemma. External retrieval-based memory can rapidly absorb new evidence, but it often fails to internalize recurring execution patterns and incurs inference-time retrieval overhead. Parametric memory enables stable and efficient execution once learned, but typically relies on explicit task boundaries and fixed parameter budgets. Inspired by the human brain, which balances plasticity and stability through complementary episodic storage and gradual consolidation, we propose UniMem, a self-routing framework for autonomous memory management. UniMem uses learnable routing tokens as memory controllers, enabling adaptive coordination between complementary memory pathways: novel or sparse tasks are retained in an episodic buffer for retrieval-augmented execution, while recurring and reliable patterns are consolidated into expandable parametric memory. By decoupling task identification from task execution with routing tokens and parametric memory blocks, UniMem expands memory on demand without task labels during deployment or uncontrolled parameter growth. Experiments on long-horizon streaming task sequences show that UniMem consistently outperforms baselines while maintaining execution fidelity, achieving an average gain of 4.0 EM points across three backbone models.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.26017v1)
- [PDF](https://arxiv.org/pdf/2607.26017v1)
- [Rethinking Personalization in Large Language Models at the Token Level](https://arxiv.org/abs/2603.06595) (2026, citations: 1)
- [ReasonCACHE: Teaching LLMs To Reason Without Weight Updates](https://arxiv.org/abs/2602.02366) (2026, citations: 2)
- [Memory in the Age of AI Agents](https://arxiv.org/abs/2512.13564) (2025, citations: 220)
- [Language Ranker: A Lightweight Ranking framework for LLM Decoding](https://arxiv.org/abs/2510.21883) (2025, citations: 2)
- [All You Need is One: Capsule Prompt Tuning with a Single Vector](https://arxiv.org/abs/2510.16670) (2025, citations: 12)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/retrieval #keyword/evaluation #keyword/agents #keyword/machine-learning
