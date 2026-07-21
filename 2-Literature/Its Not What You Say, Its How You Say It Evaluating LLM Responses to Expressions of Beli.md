---
title: "It's Not What You Say, It's How You Say It: Evaluating LLM Responses to Expressions of Belief"
source: "https://arxiv.org/html/2607.18232v1"
author: "Kevin Du, Clara Kümpel, Michelle Wastl, Alex Warstadt"
published: "2026-07-20"
created: 2026-07-22
description: "Users frequently express their beliefs to large language models (LLMs). In some situations, the LLM should accept these contextual beliefs as true. In others, they should stick to their prior knowledge. Notably, users' expressions of belief (EoBs) can take linguistically diverse forms - using presuppositions, evidential and certainty markers, or varied tones - each of which may have a different persuasiveness over t…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/machine-learning
---

# It's Not What You Say, It's How You Say It: Evaluating LLM Responses to Expressions of Belief

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.18232v1)
- published:: 2026-07-20
- updated:: 2026-07-20
- arxiv_id:: 2607.18232v1
- pdf:: https://arxiv.org/pdf/2607.18232v1
- categories:: cs.CL

## Abstract / Summary
Users frequently express their beliefs to large language models (LLMs). In some situations, the LLM should accept these contextual beliefs as true. In others, they should stick to their prior knowledge. Notably, users' expressions of belief (EoBs) can take linguistically diverse forms - using presuppositions, evidential and certainty markers, or varied tones - each of which may have a different persuasiveness over the LLMs. We introduce a typology to systematically evaluate how different EoBs affect whether models follow context versus prior knowledge. The typology is grounded in four linguistically motivated dimensions: form, evidentiality, epistemic stance, and tone, spanning 17 fine-grained types. By pairing these EoBs with world knowledge facts, we generate controlled EoB-query pairs that isolate the effect of linguistic variation. Using this benchmark, we evaluate 16 LLMs that differ in architecture (Llama3, Qwen3, Gemma3), scale (1B-30B parameters), and training stages (base vs instruct). We identify meaningful variations in response behavior across these axes, e.g., that bigger models and instruction models tend to be less context-following than smaller models and base models. We further identify specific EoBs that statistically significantly persuade LMs more consistently than others. Our work reveals systematic patterns in how linguistic framing affects LLM context integration, with implications for prompt engineering and model robustness.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.18232v1)
- [PDF](https://arxiv.org/pdf/2607.18232v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/machine-learning
