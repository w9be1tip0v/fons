---
title: "Self-Evolving Agent Harnesses via Gated Semantic Quality-Diversity"
source: "https://arxiv.org/html/2607.13683v1"
author: "Xiaotian Luo, Fengxingyu Wang, Chuanrui Hu, Dizhan Xue, Yafeng Deng"
published: "2026-07-15"
created: 2026-07-16
description: "Framework that separates LLM patch proposals from deterministic measurement and significance testing; a gated quality-diversity archive keyed on pathology yields +9 to +15.5pp sealed-test gains that transfer."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/agent
  - keyword/evaluation
  - keyword/reasoning
---

# Self-Evolving Agent Harnesses via Gated Semantic Quality-Diversity

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.13683v1)
- published:: 2026-07-15
- updated:: 2026-07-15
- arxiv_id:: 2607.13683v1
- pdf:: https://arxiv.org/pdf/2607.13683v1
- categories:: cs.CL

## Abstract / Summary
An LLM agent’s real-task performance is shaped as much by its harness (prompts, injected knowledge, runtime control, configuration) as by frozen weights. Self-generated feedback is noisy, so this work separates proposing changes from crediting them: a language model diagnoses failures and proposes patches, while sampling, measurement, and significance testing stay in deterministic code. Patches populate a gated categorical quality-diversity archive (GSME) keyed on (WHERE x WHY) pathology rather than tasks, reducing overfitting. Across seven domains with a frozen open-weight model, train-selected harness gains of +9 to +15.5pp on sealed tests retained 86–147% of training gain. What transfers is the diagnose-and-credit loop, not any specific harness.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.13683v1)
- [PDF](https://arxiv.org/pdf/2607.13683v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/agent #keyword/evaluation #keyword/reasoning
