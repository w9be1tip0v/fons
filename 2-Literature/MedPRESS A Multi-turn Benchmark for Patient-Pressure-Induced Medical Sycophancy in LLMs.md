---
title: "MedPRESS: A Multi-turn Benchmark for Patient-Pressure-Induced Medical Sycophancy in LLMs"
source: "https://arxiv.org/html/2608.02520v1"
author: "Saman Sarker Joy, Niloy Farhan"
published: "2026-08-03"
created: 2026-08-05
description: "Large language models (LLMs) are increasingly used for health-related advice. Existing research measures their safety with static questions rather than pressured patient-facing conversations. We introduce MedPRESS, a multi-turn benchmark for measuring patient-pressure-induced sycophancy in LLMs. MedPRESS contains 600 medically grounded five-turn dialogues across three scenario families: medication and treatment dema…"
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
---

# MedPRESS: A Multi-turn Benchmark for Patient-Pressure-Induced Medical Sycophancy in LLMs

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.02520v1)
- published:: 2026-08-03
- updated:: 2026-08-03
- arxiv_id:: 2608.02520v1
- pdf:: https://arxiv.org/pdf/2608.02520v1
- categories:: cs.CL

## Abstract / Summary
Large language models (LLMs) are increasingly used for health-related advice. Existing research measures their safety with static questions rather than pressured patient-facing conversations. We introduce MedPRESS, a multi-turn benchmark for measuring patient-pressure-induced sycophancy in LLMs. MedPRESS contains 600 medically grounded five-turn dialogues across three scenario families: medication and treatment demand, personal health self-care, and symptom triage and care resistance. Each dialogue begins with a health query and escalates through personal experience, social proof, external evidence claims, and direct adversarial challenge. We evaluate 20 LLMs across general, medical-domain, lightweight, large, open-weight, and proprietary families using structured judging and safety-focused metrics. Results show that models frequently shift toward unsafe agreement under repeated patient pressure, with substantial variation across model families, model scale, and prompt type. Anti-sycophancy prompting improves robustness for several models, but does not eliminate unsafe agreement. MedPRESS highlights a critical gap in medical LLM evaluation: safe medical knowledge is not enough unless models can maintain it under conversational pressure.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.02520v1)
- [PDF](https://arxiv.org/pdf/2608.02520v1)
- [DeepSeek-V4: Towards Highly Efficient Million-Token Context Intelligence](https://arxiv.org/abs/2606.19348) (2026, citations: 472)
- [Public use of a generalist LLM chatbot for health queries](https://www.nature.com/articles/s44360-026-00117-x.pdf) (2026, citations: 15)
- [SycoEval-EM: Sycophancy Evaluation of Large Language Models in Simulated Clinical Encounters for Emergency Care](https://arxiv.org/abs/2601.16529) (2026, citations: 7)
- [Holistic evaluation of large language models for medical tasks with MedHELM](https://pmc.ncbi.nlm.nih.gov/articles/PMC13267972/) (2026, citations: 56)
- [gpt-oss-120b&gpt-oss-20b Model Card](https://arxiv.org/abs/2508.10925) (2025, citations: 1112)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/safety
