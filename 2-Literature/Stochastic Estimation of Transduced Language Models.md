---
title: "Stochastic Estimation of Transduced Language Models"
source: "https://arxiv.org/html/2608.27428v1"
author: "Vésteinn Snæbjarnarson, Samuel Kiegeland, Manuel de Prada Corral, Ryan Cotterell, Tim Vieira"
published: "2026-08-27"
created: 2026-08-29
description: "Transduced language models (TLMs) compose a pretrained \emph{source} language model with a functional finite-state transducer to induce a language model over \emph{target} strings. Computing the probability of a target prefix under a TLM amounts to summing the source-model probabilities of all source strings that the transducer maps to target strings beginning with that prefix. This set can be exponentially large or…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
---

# Stochastic Estimation of Transduced Language Models

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.27428v1)
- published:: 2026-08-27
- updated:: 2026-08-27
- arxiv_id:: 2608.27428v1
- pdf:: https://arxiv.org/pdf/2608.27428v1
- categories:: cs.CL

## Abstract / Summary
Transduced language models (TLMs) compose a pretrained \emph{source} language model with a functional finite-state transducer to induce a language model over \emph{target} strings. Computing the probability of a target prefix under a TLM amounts to summing the source-model probabilities of all source strings that the transducer maps to target strings beginning with that prefix. This set can be exponentially large or infinite. Prior work uses a computational shortcut based on source prefix probabilities, then approximates the resulting sum with threshold-pruned beam summing. This produces a lower bound with unknown error. Instead, we resample source prefixes without replacement and reweight each selected prefix by the inverse of its inclusion probability. We show that applying this correction recursively gives an unbiased estimator of the target prefix probability and lets us estimate the mass lost by threshold pruning. Our beam-summing algorithm extends the retained source prefixes and samples which prefixes to keep, reducing their number as more probability mass is added to the running estimate. This can save computation and guarantees that the run halts with probability one. We evaluate the method on encyclopedic text and DNA against sequential Monte Carlo baselines that resample with replacement. It achieves a better compute--variance tradeoff on text and lower error at the same maximum number of particles on DNA. On a DNA-to-amino-acid transduction, it reduces runtime by several orders of magnitude relative to threshold-pruned beam summing and makes estimating prefix probabilities for long target strings feasible. Replacing threshold pruning with unbiased sampling in a published reading-time analysis substantially lowers the estimated corpus surprisal but leaves th…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.27428v1)
- [PDF](https://arxiv.org/pdf/2608.27428v1)
- [On the Proper Treatment of Units in Surprisal Theory](https://arxiv.org/abs/2604.28147) (2026, citations: 2)
- [Transducing Language Models](https://arxiv.org/abs/2603.05193) (2026, citations: 3)
- [From Language Models over Tokens to Language Models over Characters](https://arxiv.org/abs/2412.03719) (2024, citations: 33)
- [Probabilistic Inference in Language Models via Twisted Sequential Monte Carlo](https://arxiv.org/abs/2404.17546) (2024, citations: 77)
- [Expanding horizons of cross-linguistic research on reading: The Multilingual Eye-movement Corpus (MECO)](https://link.springer.com/content/pdf/10.3758/s13428-021-01772-6.pdf) (2022, citations: 148)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation
