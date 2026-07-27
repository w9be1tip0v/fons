---
title: "Skill Self-Play: Pushing the Frontier of LLM Capability with Co-Evolving Skills"
source: "https://arxiv.org/html/2607.22529v1"
author: "Siyuan Huang, Pengyu Cheng, Haotian Liu, Tao Chen, Yihao Liu, Jingwei Ni, Shijie Zhou, Ziyi Yang, Gangwei Jiang, Mengyu Zhou, Yu Cheng, Xiaoxi Jiang, Guanjun Jiang"
published: "2026-07-24"
created: 2026-07-28
description: "LLM training is shifting from manual design and annotation to interaction-driven self-evolution. However, existing self-evolutionary methods face a fundamental dilemma between task diversity and verification reliability: environment-bound methods obtain precise feedback but confine learning to narrow domains, while open-ended self-generation broadens the task space but lacks reliable verification, allowing misleadin…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/agents
  - keyword/machine-learning
---

# Skill Self-Play: Pushing the Frontier of LLM Capability with Co-Evolving Skills

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.22529v1)
- published:: 2026-07-24
- updated:: 2026-07-24
- arxiv_id:: 2607.22529v1
- pdf:: https://arxiv.org/pdf/2607.22529v1
- categories:: cs.CL

## Abstract / Summary
LLM training is shifting from manual design and annotation to interaction-driven self-evolution. However, existing self-evolutionary methods face a fundamental dilemma between task diversity and verification reliability: environment-bound methods obtain precise feedback but confine learning to narrow domains, while open-ended self-generation broadens the task space but lacks reliable verification, allowing misleading rewards to pollute the training loop. We identify agent skills as a powerful middle ground to reconcile this tension: each skill ensures deep, verifiable execution in a specific scenario, while dynamic routing across skills maintains open-ended task variety. Leveraging this insight, we introduce Skill Self-Play (Skill-SP), a co-evolutionary framework comprising a proposer, a solver, and a dynamic skill controller. Orchestrated via a reinforcement learning loop, these components co-evolve in a continuous self-play loop: the proposer generates challenging tasks conditioned on dynamically sampled skills; the solver explores candidate solutions to push its capability boundaries; and the skill controller collects execution feedback to update and expand the skill library. This interactive co-evolution effectively bridges the gap between structured verification and open-ended exploration. Empirical evaluations on tool-use and reasoning benchmarks demonstrate that Skill-SP, serving as a robust evolution engine, consistently pushes the performance ceiling of competent backbones while catalyzing striking turnarounds for initially misaligned models. Our code is available at https://github.com/Qwen-Applications/skill-self-play.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.22529v1)
- [PDF](https://arxiv.org/pdf/2607.22529v1)
- [SkillJuror: Measuring How Agent Skill Organization Changes Runtime Behavior](https://arxiv.org/abs/2606.11543) (2026, citations: 1)
- [SkillAxe: Sharpening LLM-Authored Agent Skills Through Evaluation-Guided Self-Refinement](https://arxiv.org/abs/2606.10546) (2026, citations: 3)
- [OpenSkill: Open-World Self-Evolution for LLM Agents](https://arxiv.org/abs/2606.06741) (2026, citations: 1)
- [Skill-RM: Unifying Heterogeneous Evaluation Criteria via Agent Skill](https://arxiv.org/abs/2606.03980) (2026, citations: 3)
- [SkillRevise: Improving LLM-Authored Agent Skills via Trace-Conditioned Skill Revision](https://arxiv.org/abs/2606.01139) (2026, citations: 1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/agents #keyword/machine-learning
