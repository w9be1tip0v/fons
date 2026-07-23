---
title: "LKValues: Aligning Large Language Models with Sri Lankan Societal Values"
source: "https://arxiv.org/html/2607.20410v1"
author: "Nethmi Muthugala, Supryadi, Surangika Ranathunga, Nisansa de Silva, Ruijie Tao, Ovindu Gunatunga, Pengyun Zhu, Shaowei Zhang, Jingting Zheng, Deyi Xiong"
published: "2026-07-22"
created: 2026-07-24
description: "Value alignment of Large Language Models (LLMs) has been shown to be culturally biased toward Western norms. This results in the mishandling of local values in multilingual societies such as Sri Lanka that have their unique cultural dynamics. Existing benchmarks overlook Sri Lankan-contextualized values in its official language Sinhala, hindering culturally sensitive evaluation and fine-tuning. To bridge this gap, w…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/safety
  - keyword/machine-learning
---

# LKValues: Aligning Large Language Models with Sri Lankan Societal Values

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.20410v1)
- published:: 2026-07-22
- updated:: 2026-07-22
- arxiv_id:: 2607.20410v1
- pdf:: https://arxiv.org/pdf/2607.20410v1
- categories:: cs.CL

## Abstract / Summary
Value alignment of Large Language Models (LLMs) has been shown to be culturally biased toward Western norms. This results in the mishandling of local values in multilingual societies such as Sri Lanka that have their unique cultural dynamics. Existing benchmarks overlook Sri Lankan-contextualized values in its official language Sinhala, hindering culturally sensitive evaluation and fine-tuning. To bridge this gap, we propose LKValues, the first survey-grounded resource suite for Sri Lankan value alignment. From a trilingual survey of 205 respondents, blending adapted global frameworks and LLM-elicited local constructs, we derive 40 majority-endorsed societal values. Using these values, we construct LKvaluesIT, a Sinhala-English news-derived instruction corpus containing 150k scenario-based instances, and LKvaluesBench, a value-sensitive evaluation benchmark of 1,000 instances. We evaluate a set of proprietary and open-weight LLMs with LKvaluesBench. We fine-tune three open-weight base models (Qwen3.5-4B-Base, Qwen3.5-9B-Base, and Aya-Expanse-8B-Base). Our experiments show that newer and larger LLMs still exhibit low-resource and cultural value-alignment gaps. LKValues fine-tuning improves Qwen-family models in English and Sinhala, reducing invalid outputs and cross-lingual disparities, though gains remain model-family dependent. These highlight LKValues efficacy in embedding Sri Lankan values, offering a replicable pipeline for low-resource, country-specific pluralist value alignment. The dataset is publicly available at https://github.com/NextME14/LKValues.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.20410v1)
- [PDF](https://arxiv.org/pdf/2607.20410v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/safety #keyword/machine-learning
