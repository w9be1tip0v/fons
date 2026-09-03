---
title: "User Feedback Provides a Unique Signal that LLMs Can not Detect"
source: "https://arxiv.org/html/2609.02859v1"
author: "Shachar Don-Yehiya, Leshem Choshen, Omri Abend"
published: "2026-09-02"
created: 2026-09-04
description: "Harnessing naturally occurring feedback from user interactions offers a promising learning signal for Large Language Models (LLMs). However, recent studies suggest this feedback is inherently noisy and difficult to leverage effectively. We challenge this conception by demonstrating that user feedback is a highly actionable signal for improvement, and that its perceived ineffectiveness stems from a systematic bias in…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
---

# User Feedback Provides a Unique Signal that LLMs Can not Detect

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.02859v1)
- published:: 2026-09-02
- updated:: 2026-09-02
- arxiv_id:: 2609.02859v1
- pdf:: https://arxiv.org/pdf/2609.02859v1
- categories:: cs.CL

## Abstract / Summary
Harnessing naturally occurring feedback from user interactions offers a promising learning signal for Large Language Models (LLMs). However, recent studies suggest this feedback is inherently noisy and difficult to leverage effectively. We challenge this conception by demonstrating that user feedback is a highly actionable signal for improvement, and that its perceived ineffectiveness stems from a systematic bias in current evaluation paradigms. To isolate the usefulness of feedback, we construct synthetic data with a definitive ground truth, alongside naturalistic data to validate that our findings hold in real-world scenarios. By comparing model revisions generated with and without access to feedback across both settings, we show that feedback-informed revisions resolve targeted issues at significantly higher rates than baseline revisions. Finally, we expose the root of the evaluation bias: when a model successfully fixes an issue exclusively due to feedback, LLM judges frequently fail to identify the genuinely corrected response, systematically preferring inferior baseline outputs instead.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.02859v1)
- [PDF](https://arxiv.org/pdf/2609.02859v1)
- [Mediocrity is the key for LLM as a Judge Anchor Selection](https://arxiv.org/abs/2603.16848) (2026, citations: 4)
- [Aligning Language Models from User Interactions](https://arxiv.org/abs/2603.12273) (2026, citations: 17)
- [The Era of Real-World Human Interaction: RL from User Conversations](https://arxiv.org/abs/2509.25137) (2025, citations: 15)
- [User Feedback in Human-LLM Dialogues: A Lens to Understand Users But Noisy as a Learning Signal](https://arxiv.org/abs/2507.23158) (2025, citations: 22)
- [Self-Adapting Language Models](https://arxiv.org/abs/2506.10943) (2025, citations: 61)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation
