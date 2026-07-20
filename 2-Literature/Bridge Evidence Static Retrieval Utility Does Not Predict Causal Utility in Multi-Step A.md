---
title: "Bridge Evidence: Static Retrieval Utility Does Not Predict Causal Utility in Multi-Step Agentic Search"
source: "https://arxiv.org/html/2607.15253v1"
author: "Debayan Mukhopadhyay, Utshab Kumar Ghosh, Shubham Chatterjee"
published: "2026-07-16"
created: 2026-07-20
description: "Retrieval systems are trained and evaluated on a static idea of usefulness: hand a document and a question to a reader model, see whether the answer improves, and score the document accordingly. The idea holds up when a document is read on its own. It breaks when a language model works as a search agent, issuing several queries and reasoning across turns, because a document can matter for what it lets the agent do n…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/retrieval
  - keyword/evaluation
  - keyword/reasoning
  - keyword/agents
---

# Bridge Evidence: Static Retrieval Utility Does Not Predict Causal Utility in Multi-Step Agentic Search

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15253v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15253v1
- pdf:: https://arxiv.org/pdf/2607.15253v1
- categories:: cs.IR, cs.CL

## Abstract / Summary
Retrieval systems are trained and evaluated on a static idea of usefulness: hand a document and a question to a reader model, see whether the answer improves, and score the document accordingly. The idea holds up when a document is read on its own. It breaks when a language model works as a search agent, issuing several queries and reasoning across turns, because a document can matter for what it lets the agent do next rather than for what it says about the current question. We measure that gap rather than argue it. Using a ReAct style agent over HotpotQA, we replay 1000 development questions and, for every document the agent read, delete it and re-run the rest of the trajectory from that point. Comparing the original run against its counterfactual gives a Counterfactual Trajectory Utility (CTU) score from three deltas: final answer quality, next query retrieval quality, and turn count. Crossing CTU against Static RAG Utility (SRU) over 23,322 document observations, the two are close to statistically independent (Spearman rho = -0.026). Roughly a third of the documents the agent reads are causally load bearing while looking useless to a static reader; we call these bridge documents. The pattern survives when the reader based axis is swapped for a BM25 and cross encoder proxy, giving a bridge cell of 27.2% on an evenly spread axis. A second experiment pins down the mechanism. Using the Observable Entity Relevance (OER) measure from prior work, entities that discriminate relevant from non-relevant candidates appear in the agent's next query 4.02 times more often than entities found only in non-relevant documents (6.1% vs 1.5%, n = 227,139). A bridge document earns its keep by handing the agent a discriminative entity that redirects the search. Static relevance and causal…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15253v1)
- [PDF](https://arxiv.org/pdf/2607.15253v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/retrieval #keyword/evaluation #keyword/reasoning #keyword/agents
