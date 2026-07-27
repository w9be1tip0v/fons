---
title: "Biomedical Machine Translation for Low-Resource Arabic-Script Languages via Cross-Lingual Transfer and LoRA Adapter Merging"
source: "https://arxiv.org/html/2607.22300v1"
author: "Abdullah Alabdullah, Arash Eslamighayour, Sarp Harbalioglu, Lifeng Han"
published: "2026-07-24"
created: 2026-07-28
description: "We present a systematic study of healthcare-domain cross-lingual transfer to address the scarcity of biomedical NMT resources for Arabic-script languages. We use Arabic and Persian as higher-resource pivots to improve translation for \textbf{four severely low-resource} targets: Dari (Afghan Persian, a standardised variety of Persian), Pashto, Sorani Kurdish (Central Kurdish, a major standardized variety of Kurdish),…"
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

# Biomedical Machine Translation for Low-Resource Arabic-Script Languages via Cross-Lingual Transfer and LoRA Adapter Merging

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.22300v1)
- published:: 2026-07-24
- updated:: 2026-07-24
- arxiv_id:: 2607.22300v1
- pdf:: https://arxiv.org/pdf/2607.22300v1
- categories:: cs.CL

## Abstract / Summary
We present a systematic study of healthcare-domain cross-lingual transfer to address the scarcity of biomedical NMT resources for Arabic-script languages. We use Arabic and Persian as higher-resource pivots to improve translation for \textbf{four severely low-resource} targets: Dari (Afghan Persian, a standardised variety of Persian), Pashto, Sorani Kurdish (Central Kurdish, a major standardized variety of Kurdish), and Urdu (closely related to Hindi). Using LoRA fine-tuning on small decoder-only LLMs, we train \textit{domain-specific pivot adapters} and evaluate \textbf{three transfer strategies}: few-shot in-context learning, minimal supervised adaptation, and, to the best of our knowledge, for the first time in this setting, zero-data LoRA adapter merging. Supervised adaptation with just 500 sentences achieves near pivot-language quality for Dari (CHrF++ 41.01) and meaningful gains for Urdu (28.88), while adapter merging reaches within 3.5 CHrF++ of supervised adaptation for Dari at zero additional cost. Pashto and Sorani Kurdish remain insufficient for high-stakes clinical deployment exposing the limits of cross-lingual transfer when structural distance from the pivots is too great. LoRA adapter merging works surprisingly well for closely related languages, even without target-language biomedical data.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.22300v1)
- [PDF](https://arxiv.org/pdf/2607.22300v1)
- [Cross-Lingual Empirical Evaluation of Large Language Models for Arabic Medical Tasks](https://arxiv.org/abs/2602.05374) (2026, citations: 1)
- [Advancing Dialectal Arabic to Modern Standard Arabic Machine Translation](https://arxiv.org/abs/2507.20301) (2025, citations: 7)
- [The Unreasonable Effectiveness of Model Merging for Cross-Lingual Transfer in LLMs](https://arxiv.org/abs/2505.18356) (2025, citations: 7)
- [Pivot Language for Low-Resource Machine Translation](https://arxiv.org/abs/2505.14553) (2025, citations: 3)
- [Esposito: An English-Persian Scientific Parallel Corpus for Machine Translation](https://www.semanticscholar.org/paper/316e826d28c70894420f0120d9296f963c4413c3) (2024, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/machine-learning
