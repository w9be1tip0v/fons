---
title: "A Factorial Study of Synthetic Data Generation for Low-Resource Machine Translation using Grammar Books"
source: "https://arxiv.org/html/2607.22376v1"
author: "Varun Ghat Ravikumar, Sina Ahmadi, Lena Jäger, Rico Sennrich"
published: "2026-07-24"
created: 2026-07-28
description: "Most endangered languages lack the parallel data required for machine translation, despite the existence of descriptive grammar books. We introduce a pipeline that uses large language models to extract grammatical rules, example sentences, and lexicons from grammar books and generate synthetic parallel corpora for fine-tuning-rather than feeding grammar content into prompts at inference time, as in prior work. Valid…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/agents
  - keyword/machine-learning
---

# A Factorial Study of Synthetic Data Generation for Low-Resource Machine Translation using Grammar Books

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.22376v1)
- published:: 2026-07-24
- updated:: 2026-07-24
- arxiv_id:: 2607.22376v1
- pdf:: https://arxiv.org/pdf/2607.22376v1
- categories:: cs.CL

## Abstract / Summary
Most endangered languages lack the parallel data required for machine translation, despite the existence of descriptive grammar books. We introduce a pipeline that uses large language models to extract grammatical rules, example sentences, and lexicons from grammar books and generate synthetic parallel corpora for fine-tuning-rather than feeding grammar content into prompts at inference time, as in prior work. Validated on three typologically diverse low-resource languages-Kalamang (Papuan), Tuatschin (Romance), and Mandan (Siouan)-we show that fine-tuning on synthetic data improves over seed-data baselines in 75% of configurations for Kalamang and 59% for Tuatschin, with best-case ChrF++ gains of +8.8, +5.3, and +3.3 respectively. Through a systematic factorial study across 96 configurations varying target part-of-speech, retrieval granularity, and sample volume, we identify which factor combinations drive gains and where they break down. Our results demonstrate that static linguistic documentation can be repurposed for machine translation fine-tuning, offering a practical path towards translation tools for severely under-resourced languages.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.22376v1)
- [PDF](https://arxiv.org/pdf/2607.22376v1)
- [Read it in Two Steps: Translating Extremely Low-Resource Languages with Code-Augmented Grammar Books](https://arxiv.org/abs/2506.01796) (2025, citations: 11)
- [Scaling Low-Resource MT via Synthetic Data Generation with LLMs](https://arxiv.org/abs/2505.14423) (2025, citations: 13)
- [Compositional Translation: A Novel LLM-based Approach for Low-resource Machine Translation](https://arxiv.org/abs/2503.04554) (2025, citations: 16)
- [Can LLMs Help Create Grammar?: Automating Grammar Creation for Endangered Languages with In-Context Learning](https://arxiv.org/abs/2412.10960) (2024, citations: 11)
- [Back to School: Translation Using Grammar Books](https://arxiv.org/abs/2410.15263) (2024, citations: 19)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/agents #keyword/machine-learning
