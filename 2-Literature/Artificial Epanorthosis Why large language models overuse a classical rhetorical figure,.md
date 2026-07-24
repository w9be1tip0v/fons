---
title: "Artificial Epanorthosis: Why large language models overuse a classical rhetorical figure, and how to mitigate it"
source: "https://arxiv.org/html/2607.21498v1"
author: "Federico Boggia"
published: "2026-07-23"
created: 2026-07-25
description: "A rhetorical figure that Cicero and Quintilian catalogued two thousand years ago reappears, systematically, in the text of large language models: epanorthosis, the self-correction of the specimen «This is not a course. It is a journey of transformation». This essay argues that the overuse is a trained disposition, driven mainly by a training distribution rich in promotional prose and by preference tuning (RLHF) that…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/machine-learning
---

# Artificial Epanorthosis: Why large language models overuse a classical rhetorical figure, and how to mitigate it

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.21498v1)
- published:: 2026-07-23
- updated:: 2026-07-23
- arxiv_id:: 2607.21498v1
- pdf:: https://arxiv.org/pdf/2607.21498v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
A rhetorical figure that Cicero and Quintilian catalogued two thousand years ago reappears, systematically, in the text of large language models: epanorthosis, the self-correction of the specimen «This is not a course. It is a journey of transformation». This essay argues that the overuse is a trained disposition, driven mainly by a training distribution rich in promotional prose and by preference tuning (RLHF) that rewards confident, emphatic phrasing; the left-to-right nature of generation is an amplifier rather than the root cause. Building on evidence that models diverge from human rhetorical style, and on Fontanier's classification of epanorthosis as a figure of thought, it sets out a programme that scores the figure against genre-specific human baselines through an Epanorthosis Index (density relative to the human rate). A first measurement, on three sizes of one instruction-tuned model family, finds mis-calibration by register in both directions: the models overshoot in oratory (about twofold, near threefold in Italian, concentrated in the larger tiers) and undershoot in informal question-and-answer writing, while matching humans in argument, journalism, and encyclopedic prose. Three constructive contributions follow: a survey of mitigation techniques centred on lightweight LoRA adapters; a demonstration, in Italian, that a one-line instruction cuts the figure by half to nearly three-quarters and that a supervised-fine-tuning adapter removes it almost entirely, with a scaling coefficient that dials the reduction back onto the human rate; and the argument that the target is calibration to the human rate for each genre, not elimination. It closes on the stakes: the real risk is that we begin to write like the machines.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.21498v1)
- [PDF](https://arxiv.org/pdf/2607.21498v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/machine-learning
