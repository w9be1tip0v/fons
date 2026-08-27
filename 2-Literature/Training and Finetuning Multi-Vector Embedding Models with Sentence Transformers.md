---
title: "Training and Finetuning Multi-Vector Embedding Models with Sentence Transformers"
source: "https://huggingface.co/blog/train-multi-vector-encoder"
author: "Hugging Face Blog"
published: "2026-08-26"
created: 2026-08-28
description: "Finetuning multi-vector models involves several components: the model itself, datasets, loss functions, training arguments, evaluators, and the trainer class. I'll have a look at each of these components, accompanied by practical examples of how they can be used for finetuning strong multi-vector models. Lastly, in the Evaluation section, I'll show you that my finetuned multi-vector-encoder/mLateOn-medical model, tr…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/transformer
  - keyword/retrieval
  - keyword/evaluation
  - keyword/machine-learning
---

# Training and Finetuning Multi-Vector Embedding Models with Sentence Transformers

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/train-multi-vector-encoder)
- published:: 2026-08-26

## Abstract / Summary
Finetuning multi-vector models involves several components: the model itself, datasets, loss functions, training arguments, evaluators, and the trainer class. I'll have a look at each of these components, accompanied by practical examples of how they can be used for finetuning strong multi-vector models. Lastly, in the Evaluation section, I'll show you that my finetuned multi-vector-encoder/mLateOn-medical model, trained in 14.5 hours on a single RTX 3090 alongside this blogpost, easily outperforms every general-purpose retrieval model I could find on my medical retrieval evaluation: dense, sparse, lexical, and multi-vector alike. If you're interested in finetuning dense embedding models, sparse embedding models, or rerankers instead, then consider reading through my prior Training and Finetuning Embedding Models , Training and Finetuning Sparse Embedding Models , and Training and Finetuning Reranker Models blogposts. This blogpost is about training multi-vector models. If you want to learn how to use them, from loading and encoding to indexing in vector databases, see the companion Multi-Vector (Late Interaction) Embedding Models with Sentence Transformers blogpost. Table of Cont…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/transformer #keyword/retrieval #keyword/evaluation #keyword/machine-learning
