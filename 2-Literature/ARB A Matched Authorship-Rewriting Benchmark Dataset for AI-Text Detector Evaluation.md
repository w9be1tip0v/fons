---
title: "ARB: A Matched Authorship-Rewriting Benchmark Dataset for AI-Text Detector Evaluation"
source: "https://arxiv.org/html/2607.29539v1"
author: "Gaetano Perrone, Simon Pietro Romano"
published: "2026-07-31"
created: 2026-08-04
description: "Standard AI-text detection benchmarks compare human-written text against text generated directly by large language models (LLMs). While prior work has shown that rewriting and paraphrasing can degrade detector performance, it remains unclear whether performance measured on this conventional benchmark predicts detector behavior when human-authored content is rewritten by an LLM. To address this gap, we introduce Auth…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
---

# ARB: A Matched Authorship-Rewriting Benchmark Dataset for AI-Text Detector Evaluation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.29539v1)
- published:: 2026-07-31
- updated:: 2026-07-31
- arxiv_id:: 2607.29539v1
- pdf:: https://arxiv.org/pdf/2607.29539v1
- categories:: cs.CL, cs.AI

## Abstract / Summary
Standard AI-text detection benchmarks compare human-written text against text generated directly by large language models (LLMs). While prior work has shown that rewriting and paraphrasing can degrade detector performance, it remains unclear whether performance measured on this conventional benchmark predicts detector behavior when human-authored content is rewritten by an LLM. To address this gap, we introduce Authorship-Rewriting Benchmark (ARB), built from 1,800 human source texts (600 each from XSum, WritingPrompts, and OpenWebText) and four open-weight generators (Llama-3.2-3B, Qwen2.5-7B, Mistral-7B, Gemma-2-9B). Each source item yields four matched variants: human-written (HUMAN), direct LLM generation (Free-LLM), LLM-rewritten human text (H2L), and same-generator LLM-rewritten LLM text (LLM2L). We evaluated five detectors (FastDetectGPT, Binoculars-falcon-7b, RADAR, BERT-Defense, RoBERTa-Defense) at a strict 1%-false-positive operating point (TPR@1%FPR). FastDetectGPT and Binoculars-falcon-7b detected 91.2% and 93.5\% of direct LLM text, but only 30.8% and 15.1% of human text an LLM had rewritten, a drop of 60-78 percentage points. The same detectors retained 78.3% and 83.0% recall when LLM text was rewritten by the same model, a much smaller decline of 10-13 points. RADAR followed the same pattern (66.8% to 12.2%), while BERT-Defense and RoBERTa-Defense stayed below 3% recall across all regimes. These results show that detector performance measured on the conventional human-vs-LLM benchmark does not transfer to human-authored text revised by an LLM, even though the same detectors remain largely robust to LLM-only rewriting.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.29539v1)
- [PDF](https://arxiv.org/pdf/2607.29539v1)
- ['Your AI Text is not Mine': Redefining and Evaluating AI-generated Text Detection under Realistic Assumptions](https://arxiv.org/abs/2606.04906) (2026, citations: 2)
- [Feature-Augmented Transformers for Robust AI-Text Detection Across Domains and Generators](https://arxiv.org/abs/2605.03969) (2026, citations: 2)
- [Spotlights and Blindspots: Evaluating Machine-Generated Text Detection](https://arxiv.org/abs/2604.16607) (2026, citations: 2)
- [Detecting the Machine: A Comprehensive Benchmark of AI-Generated Text Detectors Across Architectures, Domains, and Adversarial Conditions](https://arxiv.org/abs/2603.17522) (2026, citations: 2)
- [StealthRL: Reinforcement Learning Paraphrase Attacks for Multi-Detector Evasion of AI-Text Detectors](https://arxiv.org/abs/2602.08934) (2026, citations: 4)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark
