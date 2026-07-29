---
title: "Instruction-Tuned Models Locally Reuse Human Syntax More Than Humans Do"
source: "https://arxiv.org/html/2607.26015v1"
author: "Zandi Eberstadt"
published: "2026-07-28"
created: 2026-07-30
description: "Syntactic convergence (the tendency of speakers to adapt in language towards the grammatical profiles of their interlocutors) is a well-documented feature of human dialogue widely considered to operate below conscious awareness. Whether large language models exhibit analogous syntactic convergence toward human users relative to human baselines and across a broad range of syntactic constructions remains an open quest…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
---

# Instruction-Tuned Models Locally Reuse Human Syntax More Than Humans Do

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.26015v1)
- published:: 2026-07-28
- updated:: 2026-07-28
- arxiv_id:: 2607.26015v1
- pdf:: https://arxiv.org/pdf/2607.26015v1
- categories:: cs.CL

## Abstract / Summary
Syntactic convergence (the tendency of speakers to adapt in language towards the grammatical profiles of their interlocutors) is a well-documented feature of human dialogue widely considered to operate below conscious awareness. Whether large language models exhibit analogous syntactic convergence toward human users relative to human baselines and across a broad range of syntactic constructions remains an open question. Using substitution-paradigm data in which model generations replace one speaker's turns in pre-existing human dialogues, this study measures turn-adjacent reuse of context-free grammar (CFG) rules across sixteen open-weight Llama and Gemma models (1B-70B, pretrained and instruction-tuned) at 1,901 matched positions per model. Every model showed greater CFG-rule overlap with the preceding human turn than with a sampled unrelated human prime, and in every model this actual-versus-random difference was larger for lower-frequency rules. Each instruction-tuned model also showed greater natural-output overlap with the actual prime than the human response it replaced, and all eight matched architecture pairs exhibited greater actual-prime overlap after instruction tuning. However, relative to pretrained variants, instruction-tuned outputs overlapped more with unrelated primes, showed a smaller actual-versus-random increment, and had lower conditional rule-reuse odds once target rule-set size was held constant. In exploratory analyses, each model exhibited greater mean lexical and semantic similarity to the preceding turn than the matched human responses did. Instruction-tuned models additionally produced responses with greater mean semantic similarity than their pretrained counterparts in all eight architecture pairs, whereas the lexical similarity results wer…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.26015v1)
- [PDF](https://arxiv.org/pdf/2607.26015v1)
- [Characterizing the spiral: potential mechanisms in AI-associated delusions](https://www.nature.com/articles/s44277-026-00065-0.pdf) (2026, citations: 2)
- [Accommodation Goes Both Ways: Studying Linguistic Convergence Between Humans and Language Models](https://arxiv.org/abs/2605.29278) (2026, citations: 1)
- [Who Accommodates Whom? Bidirectional Linguistic Accommodation and Progressive Interpersonal Convergence in Human–AI Conversations](https://www.mdpi.com/2076-328X/16/5/720/pdf?version=1778157894) (2026, citations: 3)
- [Artificial Intelligence and the Psychology of Human Connection](https://doi.org/10.1177/17456916251404394) (2026, citations: 21)
- [Can Large Language Models Simulate Spoken Human Conversations?](https://www.semanticscholar.org/paper/43ebb3f400f3b0087fab234fdbd0630788f35cbb) (2025, citations: 13)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp
