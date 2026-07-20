---
title: "Frontier Language Models Struggle to Copy: Text Can Be Better Viewed in 2D"
source: "https://arxiv.org/html/2607.16072v1"
author: "Haodong Wen, Yiran Zhang, Yingfa Chen, Kaifeng Lyu"
published: "2026-07-17"
created: 2026-07-21
description: "While large language models (LLMs) can solve advanced reasoning problems in seconds, we show that even frontier models fail to perform a much simpler operation: exactly copying an input string that lies well within their context windows. We attribute this failure to positional encodings in Transformer architectures, whose inductive bias favors copying through a shortcut based on matching local contexts rather than c…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/transformer
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/reasoning
  - keyword/machine-learning
---

# Frontier Language Models Struggle to Copy: Text Can Be Better Viewed in 2D

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.16072v1)
- published:: 2026-07-17
- updated:: 2026-07-17
- arxiv_id:: 2607.16072v1
- pdf:: https://arxiv.org/pdf/2607.16072v1
- categories:: cs.CL

## Abstract / Summary
While large language models (LLMs) can solve advanced reasoning problems in seconds, we show that even frontier models fail to perform a much simpler operation: exactly copying an input string that lies well within their context windows. We attribute this failure to positional encodings in Transformer architectures, whose inductive bias favors copying through a shortcut based on matching local contexts rather than carefully locating the corresponding input positions. To address this issue, we introduce 2D-RoPE, which organizes text into a 2D grid rather than a 1D sequence and assigns each token a row ID and a column ID. Under this view, copying becomes simply retrieving input tokens at a fixed column offset, which makes the task easy to learn. In synthetic copy experiments, shallow Transformers with 2D-RoPE achieve perfect copying at input lengths hundreds of times longer than those seen during training, whereas standard positional encodings fall far behind. We further show that the advantage of 2D-RoPE language models on copy tasks consistently holds in large-scale pretraining on DCLM with model sizes up to 1.4B parameters. Overall, our results suggest that viewing text in 2D can benefit language modeling, and we hope this encourages future work to further explore the potential of 2D positional encodings.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.16072v1)
- [PDF](https://arxiv.org/pdf/2607.16072v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/transformer #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/reasoning #keyword/machine-learning
