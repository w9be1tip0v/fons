---
title: "RedEvoAgent: Automatic Red-Teaming Agent with Experience-Driven Skill Evolution"
source: "https://arxiv.org/html/2608.27439v1"
author: "Junjie Zhang, Hui Liu, Kecheng Chen, Xianbo Mo, Changsheng Chen, Haoliang Li"
published: "2026-08-27"
created: 2026-08-30
description: "LLM-based agents are increasingly deployed in product-level execution harnesses, where jailbreaks can trigger harmful tool use and persistent state changes, creating greater risks than unsafe text generation alone. Existing automatic red-teaming methods often rely on fixed attacks, while recent agentic attackers coordinate multiple jailbreak tools and show stronger potential through trajectory-based retrieval. Howev…"
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
  - keyword/agents
  - keyword/safety
---

# RedEvoAgent: Automatic Red-Teaming Agent with Experience-Driven Skill Evolution

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27439v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27439v1
- pdf:: https://arxiv.org/pdf/2608.27439v1
- categories:: cs.CR, cs.AI

## Abstract / Summary
LLM-based agents are increasingly deployed in product-level execution harnesses, where jailbreaks can trigger harmful tool use and persistent state changes, creating greater risks than unsafe text generation alone. Existing automatic red-teaming methods often rely on fixed attacks, while recent agentic attackers coordinate multiple jailbreak tools and show stronger potential through trajectory-based retrieval. However, such retrieval can reuse misleading experiences due to retrieval bias and unclear tool credit, and full trajectories add context overhead while reducing interpretability. We propose RedEvoAgent, a black-box red-teaming agent that distills cross-case attack trajectories into a concise, human-readable attack skill. The attack skill adaptively evolves through tool-effectiveness profiling and Deciding-Tool Attribution for skill updates, and a validation ratchet that retains only updates improving validation performance. Experiments on multiple benchmarks, target models, and target execution harnesses show that RedEvoAgent outperforms fixed and agentic baselines, improves tool efficiency, and transfers across attacker models and target execution harnesses.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27439v1)
- [PDF](https://arxiv.org/pdf/2608.27439v1)
- [SkillOpt-Lite: Better and Faster Agent Self-evolution via One Line of Vibe](https://arxiv.org/abs/2607.03451) (2026, citations: 9)
- [JailbreakOPT: Tool-Assisted Iterative Jailbreak Prompt Optimization](https://arxiv.org/abs/2606.11425) (2026, citations: 1)
- [Evolving Skill-Structured Attack Memory Enhances LLM Jailbreaking](https://arxiv.org/abs/2605.29237) (2026, citations: 2)
- [SkillOpt: Executive Strategy for Self-Evolving Agent Skills](https://arxiv.org/abs/2605.23904) (2026, citations: 55)
- [DeepSeek-V4: Towards Highly Efficient Million-Token Context Intelligence](https://arxiv.org/abs/2606.19348) (2026, citations: 661)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/safety
