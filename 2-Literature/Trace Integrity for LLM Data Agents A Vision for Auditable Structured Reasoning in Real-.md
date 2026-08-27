---
title: "Trace Integrity for LLM Data Agents: A Vision for Auditable Structured Reasoning in Real-World Systems"
source: "https://arxiv.org/html/2608.26036v1"
author: "Srimonti Dutta, Akshata Kishore Moharir"
published: "2026-08-26"
created: 2026-08-28
description: "Answer accuracy is an insufficient reliability signal for LLM data agents. In structured-data tasks, a benchmark-correct answer can be produced by an invalid trace. This paper introduces Trace Integrity, a deployment reliability criterion for evaluating whether the computation recorded behind an answer is explicit, executable, schema-valid, operator-faithful, replayable, answer-consistent, and auditable. We identify…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/benchmark
  - keyword/reasoning
  - keyword/agents
  - keyword/research-paper
---

# Trace Integrity for LLM Data Agents: A Vision for Auditable Structured Reasoning in Real-World Systems

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2608.26036v1)
- published:: 2026-08-26
- updated:: 2026-08-26
- arxiv_id:: 2608.26036v1
- pdf:: https://arxiv.org/pdf/2608.26036v1
- categories:: cs.AI, cs.CL

## Abstract / Summary
Answer accuracy is an insufficient reliability signal for LLM data agents. In structured-data tasks, a benchmark-correct answer can be produced by an invalid trace. This paper introduces Trace Integrity, a deployment reliability criterion for evaluating whether the computation recorded behind an answer is explicit, executable, schema-valid, operator-faithful, replayable, answer-consistent, and auditable. We identify the Structure Gap as the deployment failure mode that makes Trace Integrity necessary: natural-language reasoning and free-form rationales do not reliably specify the operator-level programs required by real-world systems. We operationalize Trace Integrity with execution contracts, structured artifacts that bind user intent to schema elements, operator plans, assumptions, executable queries, verification status, and final-answer linkage. We also introduce CAIT (Correct Answer / Invalid Trace) Rate, which measures how often answer-only evaluation counts computationally unsupported outputs as successes. In an empirical demonstration on BIRD Mini-Dev, Direct SQL, Operation Summary + SQL, and Contract-First SQL achieve answer accuracies of 20%, 22%, and 24%, while their Trace Integrity Pass Rates are 39%, 43%, and 40% and their CAIT Rates remain high at 55%, 59.1%, and 45.8%, showing that answer accuracy, trace validity, and silent-failure risk are distinct evaluation signals. Real-world LLM data agents should, therefore, be evaluated not only by whether their outputs match a reference answer, but by whether those outputs are backed by auditable computation.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2608.26036v1)
- [PDF](https://arxiv.org/pdf/2608.26036v1)
- [Talk to your data: Enhancing Business Intelligence and Inventory Management with LLM-Driven Semantic Parsing and Text-to-SQL for Database Querying](https://www.semanticscholar.org/paper/d8696c3bdb7a1e92182a8777c9794a9235646098) (2023, citations: 12)
- [Can LLM Already Serve as A Database Interface? A BIg Bench for Large-Scale Database Grounded Text-to-SQLs](https://arxiv.org/abs/2305.03111) (2023, citations: 1132)
- [Toolformer: Language Models Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761) (2023, citations: 5309)
- [Program of Thoughts Prompting: Disentangling Computation from Reasoning for Numerical Reasoning Tasks](https://arxiv.org/abs/2211.12588) (2022, citations: 1456)
- [ReAct: Synergizing Reasoning and Acting in Language Models](https://arxiv.org/abs/2210.03629) (2022, citations: 10608)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/benchmark #keyword/reasoning #keyword/agents #keyword/research-paper
