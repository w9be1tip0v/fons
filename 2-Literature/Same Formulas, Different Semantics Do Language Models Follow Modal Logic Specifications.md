---
title: "Same Formulas, Different Semantics: Do Language Models Follow Modal Logic Specifications?"
source: "https://arxiv.org/html/2608.05097v1"
author: "Réemi Andrieu, Damien Sileo"
published: "2026-08-05"
created: 2026-08-07
description: "Reasoning about necessity and possibility depends on assumptions about accessibility between worlds and about which objects exist at each one. The same inference may therefore hold under one modal system and fail under another. Evaluating language models on such problems requires testing whether their judgments follow the stated semantics rather than a familiar logic. We construct paired modal problems with identica…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/reasoning
  - keyword/machine-learning
---

# Same Formulas, Different Semantics: Do Language Models Follow Modal Logic Specifications?

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.05097v1)
- published:: 2026-08-05
- updated:: 2026-08-05
- arxiv_id:: 2608.05097v1
- pdf:: https://arxiv.org/pdf/2608.05097v1
- categories:: cs.CL

## Abstract / Summary
Reasoning about necessity and possibility depends on assumptions about accessibility between worlds and about which objects exist at each one. The same inference may therefore hold under one modal system and fail under another. Evaluating language models on such problems requires testing whether their judgments follow the stated semantics rather than a familiar logic. We construct paired modal problems with identical premises and conjecture but different frame or domain conditions; automated reasoning verifies opposite labels. A balanced core prevents the semantic condition alone from revealing the answer. On this core, four of five recent models perform below the condition-only baseline under direct prompting. Yet enabling reasoning mode raises DeepSeek V4 Flash from 4.4% to 88.1% on unchanged prompts. Following stipulated modal semantics thus depends strongly on inference mode as well as model identity. When frame conditions are omitted, models often agree but fit different familiar logics best. We release the formulas, oracle artifacts, countermodels, and responses.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.05097v1)
- [PDF](https://arxiv.org/pdf/2608.05097v1)
- [SpaceNLI: Evaluating the Consistency of Predicting Inferences In Space](https://arxiv.org/abs/2307.02269) (2023, citations: 5)
- [MindGames: Targeting Theory of Mind in Large Language Models with Dynamic Epistemic Modal Logic](https://arxiv.org/abs/2305.03353) (2023, citations: 41)
- [Solving Quantified Modal Logic Problems by Translation to Classical Logics](https://arxiv.org/abs/2212.09570) (2022, citations: 8)
- [ProofWriter: Generating Implications, Proofs, and Abductive Statements over Natural Language](https://arxiv.org/abs/2012.13048) (2020, citations: 472)
- [Extensional Higher-Order Paramodulation in Leo-III](https://arxiv.org/abs/1907.11501) (2019, citations: 31)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/reasoning #keyword/machine-learning
