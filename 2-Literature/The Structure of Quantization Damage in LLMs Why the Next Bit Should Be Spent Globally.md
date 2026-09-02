---
title: "The Structure of Quantization Damage in LLMs: Why the Next Bit Should Be Spent Globally"
source: "https://arxiv.org/html/2609.01587v1"
author: "Jundong Hu, Shekar Ramachandran"
published: "2026-09-01"
created: 2026-09-03
description: "Post-training quantization (PTQ) is widely used to reduce the cost of serving large language models (LLMs), but its accuracy cost is uneven and is often tuned per model. We study where quantization damage occurs and how to allocate a small additional precision budget. Using causal mixed-precision intervention as ground truth (raise each layer to 8-bit in turn and measure the accuracy it recovers) across 9 open-weigh…"
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

# The Structure of Quantization Damage in LLMs: Why the Next Bit Should Be Spent Globally

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.01587v1)
- published:: 2026-09-01
- updated:: 2026-09-01
- arxiv_id:: 2609.01587v1
- pdf:: https://arxiv.org/pdf/2609.01587v1
- categories:: cs.LG, cs.CL

## Abstract / Summary
Post-training quantization (PTQ) is widely used to reduce the cost of serving large language models (LLMs), but its accuracy cost is uneven and is often tuned per model. We study where quantization damage occurs and how to allocate a small additional precision budget. Using causal mixed-precision intervention as ground truth (raise each layer to 8-bit in turn and measure the accuracy it recovers) across 9 open-weight models in 4 architecture families, we test 3 intuitive hypotheses: that quantization damage lives in task circuits, where the model computes, or in weight statistics. None of them predicts which layers benefit from restored precision. Recovery is instead diffuse: for 8 of 9 models, recovering 75% of the gap takes roughly half the layers; the lone exception, Qwen3-8B, is sharply concentrated. At a matched precision budget, spending it globally on finer quantization granularity beats locally repairing the most recoverable layers for all 8 group-128-compatible models (all but OpenLLaMA, whose width rules out group-128), by 21-52 points, including the concentrated Qwen3-8B. We report 2 secondary findings: the residual is budget-limited (8-bit is near-lossless in our evaluation across RTN, GPTQ, and AWQ), and the location of peak recovery correlates with architecture within a family, though not across families. Within this budget setting, global granularity is a better default than selectively protecting critical layers. More broadly, cheap signals that correlate with quantization damage do not necessarily identify where restoring precision improves accuracy; this must be tested with causal intervention.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.01587v1)
- [PDF](https://arxiv.org/pdf/2609.01587v1)
- [You Had One Job: Per-Task Quantization Using LLMs' Hidden Representations](https://arxiv.org/abs/2511.06516) (2025, citations: 4)
- [Task-Circuit Quantization: Leveraging Knowledge Localization and Interpretability for Compression](https://arxiv.org/abs/2504.07389) (2025, citations: 6)
- [Scaling laws for post-training quantized large language models](https://arxiv.org/abs/2410.12119) (2024, citations: 5)
- [DataComp-LM: In search of the next generation of training sets for language models](https://arxiv.org/abs/2406.11794) (2024, citations: 405)
- [On the Impact of Calibration Data in Post-training Quantization and Pruning](https://arxiv.org/abs/2311.09755) (2023, citations: 61)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/machine-learning
