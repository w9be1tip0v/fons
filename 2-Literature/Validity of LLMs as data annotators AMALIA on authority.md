---
title: "Validity of LLMs as data annotators: AMALIA on authority"
source: "https://arxiv.org/html/2607.08731v1"
author: "Manuel Pita"
published: "2026-07-09"
created: 2026-07-11
description: "A national language model offers a linguistic community its own instrument for measuring what its citizens say and value. Portugal's AMALIA, a publicly funded 9B-parameter model for European Portuguese, appears competitive on agreement alone: asked to code the moral foundation of authority, it agrees with trained human coders to within six F1 points of open models eight to thirteen times its size. Yet agreement is r…"
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
---

# Validity of LLMs as data annotators: AMALIA on authority

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.08731v1)
- published:: 2026-07-09
- updated:: 2026-07-09
- arxiv_id:: 2607.08731v1
- pdf:: https://arxiv.org/pdf/2607.08731v1
- categories:: cs.CL, cs.AI, cs.CY

## Abstract / Summary
A national language model offers a linguistic community its own instrument for measuring what its citizens say and value. Portugal's AMALIA, a publicly funded 9B-parameter model for European Portuguese, appears competitive on agreement alone: asked to code the moral foundation of authority, it agrees with trained human coders to within six F1 points of open models eight to thirteen times its size. Yet agreement is reliability, not validity. For theoretical constructs that must be inferred rather than read from surface features, the question is whether the model follows the construct's theory or reaches the right code by correlated shortcuts. We test this with the recovery gap: the loss in performance when a holistic prompt is decomposed into the codebook's atomic clauses and recombined by the theory's explicit rule. If calibration closes that gap, some portability should survive across models and languages; where it does not, the construct-model instrument is the likely locus of failure. We ask whether a calibrated English instrument transfers to AMALIA-9B and to European Portuguese. For one construct and one corpus, it does not. Decomposition recovers only about half of AMALIA's holistic performance, and error analysis suggests reliance on surface correlates, especially moral outrage near authority figures. An open multilingual LLM closes the gap on the same Portuguese corpus under the same instructions, pointing away from the corpus as the main explanation. AMALIA can still screen and pre-code at scale, but it cannot yet measure this construct well enough to stand alone. The study is a single counterexample, not a verdict on national models; it argues that sovereign-LLM benchmark batteries should test not only agreement with human coders, but the evidential route by…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.08731v1)
- [PDF](https://arxiv.org/pdf/2607.08731v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark
