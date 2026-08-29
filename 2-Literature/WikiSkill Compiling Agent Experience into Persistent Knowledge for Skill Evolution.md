---
title: "WikiSkill: Compiling Agent Experience into Persistent Knowledge for Skill Evolution"
source: "https://arxiv.org/html/2608.27454v1"
author: "Liyan Tang, Cyrus Rashtchian, Chun-Sung Ferng, Andrew Tomkins, Da-Cheng Juan, Tu Vu"
published: "2026-08-27"
created: 2026-08-30
description: "Agent skills package specialized knowledge and workflows into reusable resources that extend AI agent capabilities. Recent work automatically discovers such skills from agent experience, which enables agents to progressively adapt through interaction. However, the insights that guide skill development typically remain scattered across optimization histories, limiting their systematic reuse across iterations. We intr…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
---

# WikiSkill: Compiling Agent Experience into Persistent Knowledge for Skill Evolution

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27454v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27454v1
- pdf:: https://arxiv.org/pdf/2608.27454v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
Agent skills package specialized knowledge and workflows into reusable resources that extend AI agent capabilities. Recent work automatically discovers such skills from agent experience, which enables agents to progressively adapt through interaction. However, the insights that guide skill development typically remain scattered across optimization histories, limiting their systematic reuse across iterations. We introduce WikiSkill, a framework that co-evolves agent skills with a persistent knowledge base (wiki). At a high level, WikiSkill separates raw execution experience, accumulated knowledge, and executable skills, while continuously consolidating experience into the wiki, which subsequent skill updates can build on. Across diverse benchmarks and models, WikiSkill consistently outperforms state-of-the-art skill-evolution methods and improves over no-skill baselines in most model-benchmark settings. We find that skill evolution complements model scaling: larger models generally benefit more from evolved skills, while smaller models with skills can outperform substantially larger models without them. We also find that evolved skills transfer effectively across models and model families, and skills evolved by other models can outperform self-evolved skills. Finally, our ablation studies confirm that persistent knowledge accumulation in the wiki is critical for effective skill evolution. These results demonstrate the benefits of systematically accumulating and refining agent experience for developing reusable and transferable skills.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27454v1)
- [PDF](https://arxiv.org/pdf/2608.27454v1)
- [Gemma 4 Technical Report](https://arxiv.org/abs/2607.02770) (2026, citations: 50)
- [HarnessX: A Composable, Adaptive, and Evolvable Agent Harness Foundry](https://arxiv.org/abs/2606.14249) (2026, citations: 18)
- [Self-Harness: Harnesses That Improve Themselves](https://arxiv.org/abs/2606.09498) (2026, citations: 29)
- [SkillGrad: Optimizing Agent Skills Like Gradient Descent](https://arxiv.org/abs/2605.27760) (2026, citations: 14)
- [SkillOpt: Executive Strategy for Self-Evolving Agent Skills](https://arxiv.org/abs/2605.23904) (2026, citations: 55)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/evaluation #keyword/benchmark #keyword/agents
