---
title: "Consensus as Privileged Context for Label-Free Self-Distillation (CANON)"
source: "https://arxiv.org/html/2607.13643v1"
author: "John Gkountouras, Josip Jukić, Ivan Titov"
published: "2026-07-15"
created: 2026-07-16
description: "CANON turns multi-sample majority consensus into dense token-level self-distillation supervision, improving pass@1 by up to 12 points and outperforming label-free RL at a fraction of the compute."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/reasoning
  - keyword/post-training
  - keyword/llm
---

# Consensus as Privileged Context for Label-Free Self-Distillation (CANON)

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.13643v1)
- published:: 2026-07-15
- updated:: 2026-07-15
- arxiv_id:: 2607.13643v1
- pdf:: https://arxiv.org/pdf/2607.13643v1
- categories:: cs.CL

## Abstract / Summary
Sampling multiple solutions and returning the majority answer is among the most reliable label-free ways to improve LLM reasoning accuracy, but existing methods use consensus only as a filter, preference, or scalar reward. CANON (Consensus-ANchored self-distillatiON) samples multiple solutions, extracts the majority answer, conditions a frozen snapshot of the model on a solution that reaches it, and uses that consensus-anchored teacher for dense token-level supervision on the student’s rollouts. On math and science reasoning, CANON improves pass@1 by up to 12 points, outperforming label-free RL by 6 points at about one-seventh the compute, and approaches a teacher conditioned on gold solutions. After training, models solve problems previously never solved in 32 attempts, and majority vote itself becomes more accurate.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.13643v1)
- [PDF](https://arxiv.org/pdf/2607.13643v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/reasoning #keyword/post-training #keyword/llm
