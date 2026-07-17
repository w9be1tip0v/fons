---
title: "On-Policy Delta Distillation"
source: "https://arxiv.org/html/2607.15161v1"
author: "Byeongho Heo, Jaehui Hwang, Sangdoo Yun, Dongyoon Han"
published: "2026-07-16"
created: 2026-07-17
description: "OPD² distills the delta between a reasoning-tuned teacher and its base model rather than full teacher logits, improving on-policy distillation on math/science/code with short post-training."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/post-training
  - keyword/reasoning
  - keyword/llm
---

# On-Policy Delta Distillation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15161v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15161v1
- pdf:: https://arxiv.org/pdf/2607.15161v1
- categories:: cs.CL

## Abstract / Summary
On-policy distillation gives token-level teacher supervision without reward models, but its design is underexplored. Instead of imitating the full teacher distribution, OPD² uses a delta signal: the difference between a reasoning-tuned teacher and its pre-instruction base. That delta captures changes induced by reasoning tuning and transfers them more directly. Across math, science, and code-reasoning benchmarks, OPD² consistently beats conventional on-policy distillation with only short post-training. Code: https://github.com/naver-ai/opd2

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15161v1)
- [PDF](https://arxiv.org/pdf/2607.15161v1)
- [Code](https://github.com/naver-ai/opd2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/post-training #keyword/reasoning #keyword/llm
