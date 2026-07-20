---
title: "Expanding the Lexicon of Ge'ez Based African Languages: A Comparative Study of Amharic and Tigrinya"
source: "https://arxiv.org/html/2607.15209v1"
author: "Hailay Kidu Teklehaymanot, Debela Desalegn Yadeta, Wolfgang Nejdl"
published: "2026-07-16"
created: 2026-07-20
description: "Multilingual pre-trained language models (PLMs) exhibit degraded performance on low-resource, non-Latin-script languages, driven by high out-of-vocabulary (OOV) rates and excessive subword fragmentation that result from Latin-script-centric tokenizer training. We introduce VEXMLM, a vocabulary-extended variant of XLM-R targeting the two highest-resource Ge'ez-script languages, Amharic and Tigrinya, and further evalu…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/machine-learning
---

# Expanding the Lexicon of Ge'ez Based African Languages: A Comparative Study of Amharic and Tigrinya

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15209v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15209v1
- pdf:: https://arxiv.org/pdf/2607.15209v1
- categories:: cs.CL

## Abstract / Summary
Multilingual pre-trained language models (PLMs) exhibit degraded performance on low-resource, non-Latin-script languages, driven by high out-of-vocabulary (OOV) rates and excessive subword fragmentation that result from Latin-script-centric tokenizer training. We introduce VEXMLM, a vocabulary-extended variant of XLM-R targeting the two highest-resource Ge'ez-script languages, Amharic and Tigrinya, and further evaluated on 17 additional low-resource African languages (19 total). We train a language-specific SentencePiece tokenizer on curated Amharic and Tigrinya monolingual corpora, extend XLM-R's vocabulary with 30,000 Ge'ez-script subwords derived from this tokenizer, and initialize their embeddings by averaging the embeddings of their constituent subwords under XLM-R's original tokenizer. VEXMLM is trained in two stages: (1) continued masked language modeling over the extended vocabulary on the curated corpora, and (2) supervised fine-tuning on question answering (QA), named entity recognition (NER), and sentiment analysis (SA). On Amharic/Tigrinya QA, VEXMLM achieves 87.0 EM /90.0 F1, versus 66.0 EM/78.0 F1 for XLM-R and 74.0 EM/ 78.0 F1 for Glot500. On SA, VEXMLM reaches 80.0\% accuracy versus 77.0\% (XLM-R) and 46.0\% (Glot500). On NER, VEXMLM raises OOV-token entity accuracy from 81.4\% to 94.3\%, averaged over 11 of the 19 evaluated languages for which OOV analysis was possible. Our contributions are: (i) a vocabulary-extension and embedding-initialization procedure tailored to Ge'ez script; (ii) a two-stage training strategy under which vocabulary and continued-pretraining gains on Amharic/Tigrinya transfer to 17 typologically related, unaugmented African languages; and (iii) an evaluation spanning both intrinsic tokenization metrics (vocabulary coverage, fert…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15209v1)
- [PDF](https://arxiv.org/pdf/2607.15209v1)
- [Byte Latent Transformer: Patches Scale Better Than Tokens](https://arxiv.org/abs/2412.09871) (2024, citations: 147)
- [Trans-Tokenization and Cross-lingual Vocabulary Transfers: Language Adaptation of LLMs for Low-Resource NLP](https://arxiv.org/abs/2408.04303) (2024, citations: 53)
- [How Can We Effectively Expand the Vocabulary of LLMs with 0.01GB of Target Language Text?](https://arxiv.org/abs/2406.11477) (2024, citations: 27)
- [How Multilingual Are Large Language Models Fine-Tuned for Translation?](https://arxiv.org/abs/2405.20512) (2024, citations: 11)
- [Low Resource Question Answering: An Amharic Benchmarking Dataset](https://www.semanticscholar.org/paper/6b73434d9aca9f7180033784862e8c8c6eae966a) (2024, citations: 10)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/machine-learning
