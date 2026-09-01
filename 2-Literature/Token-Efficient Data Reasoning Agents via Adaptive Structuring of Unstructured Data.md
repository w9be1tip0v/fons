---
title: "Token-Efficient Data Reasoning Agents via Adaptive Structuring of Unstructured Data"
source: "https://arxiv.org/html/2608.31082v1"
author: "Milad Rezaei Hajidehi, Qitong Wang, Stratos Idreos"
published: "2026-08-31"
created: 2026-09-02
description: "Valuable data remains embedded in unstructured sources: web pages, reports, contracts, filings, earnings calls, and PDFs. The big bet in enterprise AI is deploying LLM agents that reason over this data to answer complex questions for every knowledge worker. Agents can do this today, but at prohibitive cost. Each question repeatedly opens large documents to recover scattered evidence, consuming up to a million tokens…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/agents
---

# Token-Efficient Data Reasoning Agents via Adaptive Structuring of Unstructured Data

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.31082v1)
- published:: 2026-08-31
- updated:: 2026-08-31
- arxiv_id:: 2608.31082v1
- pdf:: https://arxiv.org/pdf/2608.31082v1
- categories:: cs.AI, cs.CL, cs.DB

## Abstract / Summary
Valuable data remains embedded in unstructured sources: web pages, reports, contracts, filings, earnings calls, and PDFs. The big bet in enterprise AI is deploying LLM agents that reason over this data to answer complex questions for every knowledge worker. Agents can do this today, but at prohibitive cost. Each question repeatedly opens large documents to recover scattered evidence, consuming up to a million tokens. However, if the data were already structured, the same question would reduce to a cheap database lookup. For example, on FanOutQA benchmark, reasoning over an ideal pre-structured store is 28X cheaper, and the gap grows to orders of magnitude as questions fan out over more documents. Yet structuring everything in advance is not viable: documents hold vastly more possible structure than any workload will use, and the useful structure and documents are unknown until queries arrive. We propose agentic data cracking, a method that structures unstructured data adaptively and speculatively as a byproduct of reasoning itself. Structuring is adaptive because observed queries decide when it happens and what matters, and speculative because it goes beyond the current question. Whenever the agent opens a document to answer, a cracking sub-agent forks from the already-loaded context at marginal cost and extracts grounded structure likely to serve related future queries. Over time, an increasing share of queries is fully covered by structured data and answered without opening a document, keeping agentic accuracy at close to RAG cost. On FanOutQA, extended with merely one related question per test question, cracking cuts cost by 53% while preserving accuracy. Agentic data cracking is a first step toward next-generation data infrastructure for agentic reasoning over unst…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.31082v1)
- [PDF](https://arxiv.org/pdf/2608.31082v1)
- [OfficeQA Pro: An Enterprise Benchmark for End-to-End Grounded Reasoning](https://arxiv.org/abs/2603.08655) (2026, citations: 23)
- [Deep Research is the New Analytics System: Towards Building the Runtime for AI-Driven Analytics](https://arxiv.org/abs/2509.02751) (2025, citations: 9)
- [A-MEM: Agentic Memory for LLM Agents](https://arxiv.org/abs/2502.12110) (2025, citations: 938)
- [CacheBlend: Fast Large Language Model Serving for RAG with Cached Knowledge Fusion](https://arxiv.org/abs/2405.16444) (2024, citations: 241)
- [SGLang: Efficient Execution of Structured Language Model Programs](https://arxiv.org/abs/2312.07104) (2023, citations: 1310)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/agents
