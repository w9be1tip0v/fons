---
title: "Groc-PO: Grounded Context Preference Optimization for Truthful Multimodal LLMs"
source: "https://arxiv.org/html/2607.13712v1"
author: "Zhixiao Zheng, Zheren Fu, Zhiyuan Yao, Chunxiao Liu, Dongming Zhang, Zhendong Mao"
published: "2026-07-15"
created: 2026-07-16
description: "Grounded Context Preference Optimization applies multi-stage preference supervision over object grounding, contextual grounding, and grounded reasoning to reduce MLLM hallucinations and cross-stage error propagation."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/multimodal
  - keyword/alignment
  - keyword/safety
---

# Groc-PO: Grounded Context Preference Optimization for Truthful Multimodal LLMs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.13712v1)
- published:: 2026-07-15
- updated:: 2026-07-15
- arxiv_id:: 2607.13712v1
- pdf:: https://arxiv.org/pdf/2607.13712v1
- categories:: cs.CL (ACM-MM 2026)

## Abstract / Summary
MLLMs still suffer from visual hallucinations, fabrication, and unfaithful reasoning. Standard DPO applies preference optimization mainly at the final-answer level, so supervision for early grounding is indirect and error can propagate from grounding drift. Groc-PO is a grounded preference framework with the Grounded Context Preference Dataset (GCPD) spanning Object Grounding, Contextual Grounding, and Grounded Reasoning. Explicit multi-stage preference supervision strengthens context-dependent reasoning and mitigates cross-stage error propagation, improving hallucination mitigation, faithful reasoning, and reliability versus standard DPO and strong baselines.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.13712v1)
- [PDF](https://arxiv.org/pdf/2607.13712v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/multimodal #keyword/alignment #keyword/safety
