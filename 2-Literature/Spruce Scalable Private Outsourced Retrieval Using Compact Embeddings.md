---
title: "Spruce: Scalable Private Outsourced Retrieval Using Compact Embeddings"
source: "https://arxiv.org/html/2609.03376v1"
author: "Peichun Hua, Yunming Xiao"
published: "2026-09-03"
created: 2026-09-07
description: "Retrieval-Augmented Generation (RAG) has made dense retrieval over large document collections a standard building block. Organizations increasingly outsource vector indexes to untrusted clouds, exposing proprietary corpora and user queries. Cryptographic protection is challenging because each query searches corpus-scale state, causing computation, correlated randomness, and communication to grow with the corpus. At…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/retrieval
  - keyword/evaluation
---

# Spruce: Scalable Private Outsourced Retrieval Using Compact Embeddings

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.03376v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.03376v1
- pdf:: https://arxiv.org/pdf/2609.03376v1
- categories:: cs.CR, cs.IR, cs.LG

## Abstract / Summary
Retrieval-Augmented Generation (RAG) has made dense retrieval over large document collections a standard building block. Organizations increasingly outsource vector indexes to untrusted clouds, exposing proprietary corpora and user queries. Cryptographic protection is challenging because each query searches corpus-scale state, causing computation, correlated randomness, and communication to grow with the corpus. At million-document scale, a naive secure implementation takes minutes and about 90 GB of communication per query. Even recent optimized systems require 10--22 seconds. We propose Spruce (Scalable Private Outsourced Retrieval Using Compact Embeddings), which co-designs representations with the cryptographic protocol. Spruce learns compact binary codes that preserve candidates for full-precision reranking, replacing corpus-wide embedding scoring with efficient Hamming-distance computation under two-server multi-party computation (MPC). A corpus-calibrated fixed-radius protocol avoids multi-round candidate selection while preserving retrieval quality. Spruce also provides private cluster pruning, which trades minor quality loss for substantially less computation, and a one-core owner-operated dealer that removes cloud OT preprocessing bottlenecks. Across four corpora containing 383K--5.42M documents, Spruce preserves the original search quality with median candidate sets of only 382--1,952. At 10 Gbps inter-server bandwidth, full scans take 0.21--2.97 seconds, $4.8$--$6.7\times$ faster than the closest measured prior work. Private pruning takes 0.06--1.09 seconds, achieves $13.1$--$22.9\times$ speedups, and retains $93.9\%$--$97.3\%$ of full-float NDCG. On the largest corpus, pruning and the dealer jointly improve sustained throughput by $31.5\times$ at 1 Gbps pe…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.03376v1)
- [PDF](https://arxiv.org/pdf/2609.03376v1)
- [Panther: Private Approximate Nearest Neighbor Search in the Single Server Setting](https://doi.org/10.1145/3719027.3765190) (2025, citations: 14)
- [A Survey on Deep Text Hashing: Efficient Semantic Text Retrieval with Binary Representation](https://arxiv.org/abs/2510.27232) (2025, citations: 3)
- [PIR-RAG: A System for Private Information Retrieval in Retrieval-Augmented Generation](https://arxiv.org/abs/2509.21325) (2025, citations: 6)
- [Breaking the Layer Barrier: Remodeling Private Transformer Inference with Hybrid CKKS and MPC](https://arxiv.org/abs/2508.19525) (2025, citations: 31)
- [RemoteRAG: A Privacy-Preserving LLM Cloud RAG Service](https://arxiv.org/abs/2412.12775) (2024, citations: 36)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/retrieval #keyword/evaluation
