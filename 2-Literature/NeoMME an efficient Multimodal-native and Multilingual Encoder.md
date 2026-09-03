---
title: "NeoMME: an efficient Multimodal-native and Multilingual Encoder"
source: "https://huggingface.co/blog/Hcompany/neomme"
author: "Hugging Face Blog"
published: "2026-09-03"
created: 2026-09-04
description: "TL;DR We introduce NeoMME , a family of 260M and 800M multilingual multimodal encoders. Unlike many generative visual language models, NeoMME does not use a separate pretrained vision tower or a causal language model. A single bidirectional Transformer processes both text tokens and raw image patches, and we train the entire model from scratch with a masked discrete-diffusion objective. We fine-tuned NeoMME for visu…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/transformer
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/diffusion
  - keyword/retrieval
  - keyword/evaluation
---

# NeoMME: an efficient Multimodal-native and Multilingual Encoder

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/Hcompany/neomme)
- published:: 2026-09-03

## Abstract / Summary
TL;DR We introduce NeoMME , a family of 260M and 800M multilingual multimodal encoders. Unlike many generative visual language models, NeoMME does not use a separate pretrained vision tower or a causal language model. A single bidirectional Transformer processes both text tokens and raw image patches, and we train the entire model from scratch with a masked discrete-diffusion objective. We fine-tuned NeoMME for visual document retrieval using ColPali's page-image approach. NeoMME -Retriever returns dense and late-interaction embeddings in one forward pass. Both model sizes lie on the ViDoRe v3 Pareto frontier for nDCG@10 and model size. At a matched 2048×2048 image input size on an NVIDIA L40S GPU, the 260M model encodes about 51 pages per second, or about twice ColModernVBERT's throughput. Hierarchical token pooling and asymmetric quantization reduce late-interaction index st… NeoMME is available in Hugging Face Transformers. We release all model checkpoints under the Apache 2.0 license. Why another multimodal encoder? Many recent visual document retrievers are adapted from pretrained generative visual language models. A separately pretrained vision encoder produces visual featur…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/transformer #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/diffusion #keyword/retrieval #keyword/evaluation
