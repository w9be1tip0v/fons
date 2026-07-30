---
title: "SpecFirst: Behavioral Specification Elicitation as a First-Class Step in Agent-Based Program Synthesis from Scratch"
source: "https://arxiv.org/html/2607.27167v1"
author: "Yihao Chen, Shi Chang, Feng Lin, Khaled Chawa, Boyuan Chen, Shaowei Wang, Ahmed E. Hassan"
published: "2026-07-29"
created: 2026-07-31
description: "LLM-based agents excel at software engineering tasks where an existing codebase provides context, but constructing a program from scratch remains fundamentally harder. Recent benchmarks such as ProgramBench quantify this gap: given only natural-language documentation and an execute-only binary as a behavioral oracle, even frontier models solve fewer than 1% of instances. Existing frameworks conflate documentation re…"
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
---

# SpecFirst: Behavioral Specification Elicitation as a First-Class Step in Agent-Based Program Synthesis from Scratch

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.27167v1)
- published:: 2026-07-29
- updated:: 2026-07-29
- arxiv_id:: 2607.27167v1
- pdf:: https://arxiv.org/pdf/2607.27167v1
- categories:: cs.SE, cs.CL

## Abstract / Summary
LLM-based agents excel at software engineering tasks where an existing codebase provides context, but constructing a program from scratch remains fundamentally harder. Recent benchmarks such as ProgramBench quantify this gap: given only natural-language documentation and an execute-only binary as a behavioral oracle, even frontier models solve fewer than 1% of instances. Existing frameworks conflate documentation reading, behavioral exploration, and code synthesis into a single pass, causing agents to probe insufficiently, lose behavioral intent as context drifts, and propagate early misinterpretations into the final implementation. Inspired by classical requirements engineering, we argue that behavioral specification elicitation should be a first-class phase that precedes implementation. We present SpecFirst, a two-stage framework that forces the specification elicitation before code synthesis. A dedicated spec agent first probes the binary and combines observations with documentation into a structured specification. Next, a code synthesis agent then uses this specification to drive implementation. This decomposition resolves documentation ambiguities before coding begins and provides a stable behavioral reference throughout synthesis. We evaluate SpecFirst on all 200 ProgramBench instances across four models spanning two families and an order of magnitude of capability. SpecFirst consistently outperforms the single-loop baseline, improving test pass rates by 6.9%-21.3% and binary exploration coverage by 9.4%-18.5%, all statistically significant. Behavioral analysis on code synthesis further shows that a prior specification enables earlier and more sustained code construction. Our results demonstrate that an explicit requirements-engineering phase is an effective para…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.27167v1)
- [PDF](https://arxiv.org/pdf/2607.27167v1)
- [ProgramBench: Can Language Models Rebuild Programs From Scratch?](https://arxiv.org/abs/2605.03546) (2026, citations: 19)
- [Quantifying Laziness, Decoding Suboptimality, and Context Degradation in Large Language Models](https://arxiv.org/abs/2512.20662) (2025, citations: 1)
- [Solving Context Window Overflow in AI Agents](https://arxiv.org/abs/2511.22729) (2025, citations: 3)
- [Lingxi: Repository-Level Issue Resolution Framework Enhanced by Procedural Knowledge Guided Scaling](https://arxiv.org/abs/2510.11838) (2025, citations: 8)
- [Drift No More? Context Equilibria in Multi-Turn LLM Interactions](https://arxiv.org/abs/2510.07777) (2025, citations: 23)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/agents
