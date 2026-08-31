---
title: "Stranger, Fan, or Peer? A Systematic Study on the Role of Interlocutor in Persona-Based Dialogue Generation"
source: "https://arxiv.org/html/2608.28467v1"
author: "Daniela Occhipinti, Malvina Nissim, Marco Guerini"
published: "2026-08-28"
created: 2026-09-01
description: "Persona-based dialogue systems are usually conditioned on speaker biography, but dialogues involve at least two participants, and who has access to whose biography can vary across training, inference, and evaluation. Prior work often neglected these aspects, obscuring mechanisms that only appear when biography visibility is toggled separately across training, inference, and evaluation, a three-stage factorisation th…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/machine-learning
---

# Stranger, Fan, or Peer? A Systematic Study on the Role of Interlocutor in Persona-Based Dialogue Generation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.28467v1)
- published:: 2026-08-28
- updated:: 2026-08-28
- arxiv_id:: 2608.28467v1
- pdf:: https://arxiv.org/pdf/2608.28467v1
- categories:: cs.CL

## Abstract / Summary
Persona-based dialogue systems are usually conditioned on speaker biography, but dialogues involve at least two participants, and who has access to whose biography can vary across training, inference, and evaluation. Prior work often neglected these aspects, obscuring mechanisms that only appear when biography visibility is toggled separately across training, inference, and evaluation, a three-stage factorisation that prior work has largely treated as a single factor. We study this factorisation on a dataset of dialogues paired with speaker's biographies, varying whether the target and interlocutor speakers see each other's biographies during training and inference, and using an LLM as a judge to perform author identification. We find that (i) training-time visibility, more than inference-time visibility, determines whether models express persona traits through dialogue or fall back on copying biographical text (a known problem/phenomenon in persona-based generation); (ii) models trained with interlocutor-biography visibility copy less target-biographical text than models trained without it, while changing visibility only at inference time has a less consistent effect; and (iii) under asymmetric disclosure, where only the interlocutor sees the target biography, target content leaks into interlocutor turns more often, and dialogues containing such traces are easier for the judge to identify, especially when interlocutor turns are visible. These results suggest that biography leakage into generated turns is an artefact of how interlocutor visibility is configured across training and inference, and separating the three stages is necessary.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.28467v1)
- [PDF](https://arxiv.org/pdf/2608.28467v1)
- [When Harry Meets Superman: The Role of The Interlocutor in Persona-Based Dialogue Generation](https://arxiv.org/abs/2505.24613) (2025, citations: 4)
- [AI can outperform humans in predicting correlations between personality items](https://www.nature.com/articles/s44271-025-00205-w.pdf) (2025, citations: 10)
- [A Survey on LLM-as-a-Judge](https://arxiv.org/abs/2411.15594) (2024, citations: 1731)
- [The Llama 3 Herd of Models](https://arxiv.org/abs/2407.21783) (2024, citations: 18152)
- [The Good, The Bad, and The Greedy: Evaluation of LLMs Should Not Ignore Non-Determinism](https://arxiv.org/abs/2407.10457) (2024, citations: 175)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/machine-learning
