---
title: "Cultural Awareness is Represented but Not Decoded: Tracing Mythological Knowledge across 18 Open-Source LLMs"
source: "https://arxiv.org/html/2608.02486v1"
author: "Iaroslav Chelombitko, Ekaterina Chelombitko, Mika Hämäläinen"
published: "2026-08-03"
created: 2026-08-05
description: "Open-source LLMs reliably name Zeus, Jupiter, and Thor, but recover their counterparts in less-represented traditions like Finnish, Slavic, Egyptian, or Chinese mythology far less consistently. We ask where inside the model this cultural default is produced. On a parallel cross-cultural substrate of Thompson-motif entities, we instrument 18 open-source LLMs from 8 architecture families with linear probing, logit len…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
---

# Cultural Awareness is Represented but Not Decoded: Tracing Mythological Knowledge across 18 Open-Source LLMs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.02486v1)
- published:: 2026-08-03
- updated:: 2026-08-03
- arxiv_id:: 2608.02486v1
- pdf:: https://arxiv.org/pdf/2608.02486v1
- categories:: cs.CL, cs.CY, cs.LG

## Abstract / Summary
Open-source LLMs reliably name Zeus, Jupiter, and Thor, but recover their counterparts in less-represented traditions like Finnish, Slavic, Egyptian, or Chinese mythology far less consistently. We ask where inside the model this cultural default is produced. On a parallel cross-cultural substrate of Thompson-motif entities, we instrument 18 open-source LLMs from 8 architecture families with linear probing, logit lens, activation patching, and output extraction. The residual stream cleanly distinguishes cultures, well above a name-string baseline, yet the decoder collapses culturally-specific tokens onto dominant-tradition ones. The failure is at readout, not at representation. Asking the same question in the target culture's native language versus English produces failures that cluster within language but decouple across language: the decoder is gated on prompt language. We release a per-entity (probe, output) decomposition framework, a citation-anchored cross-cultural ground truth, a within- versus cross-mode correlation test for language-conditioned readout, and per-entity predictions for all 18 models.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.02486v1)
- [PDF](https://arxiv.org/pdf/2608.02486v1)
- [Compressed code: the hidden effects of quantization and distillation on programming tokens](https://arxiv.org/abs/2601.02563) (2026, citations: 2)
- [How Does Quantization Affect Multilingual LLMs?](https://arxiv.org/abs/2407.03211) (2024, citations: 49)
- [Towards Measuring and Modeling “Culture” in LLMs: A Survey](https://arxiv.org/abs/2403.15412) (2024, citations: 208)
- [Do Llamas Work in English? On the Latent Language of Multilingual Transformers](https://arxiv.org/abs/2402.10588) (2024, citations: 313)
- [The Geometry of Truth: Emergent Linear Structure in Large Language Model Representations of True/False Datasets](https://arxiv.org/abs/2310.06824) (2023, citations: 641)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp
