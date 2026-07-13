---
title: "Deceptive Grounding: Entity Attribution Failure in Clinical Retrieval-Augmented Generation"
source: "https://arxiv.org/html/2607.09349v1"
author: "Cedric Caruzzo, Donggeun Yoo, Tae Soo Kim"
published: "2026-07-10"
created: 2026-07-14
description: "Defines deceptive grounding in clinical RAG: factually grounded claims attributed to the wrong entity, invisible to standard faithfulness/hallucination checks."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/retrieval
  - keyword/safety
  - keyword/evaluation
  - keyword/research-paper
---

# Deceptive Grounding: Entity Attribution Failure in Clinical Retrieval-Augmented Generation

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.09349v1)
- published:: 2026-07-10
- updated:: 2026-07-10
- arxiv_id:: 2607.09349v1
- pdf:: https://arxiv.org/pdf/2607.09349v1
- categories:: cs.CL, cs.AI, cs.LG

## Abstract / Summary
Retrieval-augmented generation evaluation checks whether model claims are factually grounded in retrieved documents. It does not check whether retrieved evidence is attributed to the correct entity. A clinical RAG response can pass every automated check (zero hallucinations, near-perfect faithfulness, real citations) while presenting drug Y's clinical evidence as evidence about queried drug X. We term this deceptive grounding (DG): a failure invisible to faithfulness, hallucination, and citation checks because every claim is sourced from a real document, about the wrong entity. Using a controlled factorial benchmark across 13 models, we find DG rates spanning 8-87% at peak adversarial conditions. Medical and biomedical fine-tuned models reach up to 86.7%; domain specialization amplifies the failure rather than mitigating it. A controlled ablation identifies the mechanism: removing entity-specific clinical evidence from retrieved documents eliminates entity-attribution failure entirely, shifting all failures to confabulation. Production measurement across 740 drug-disease pairs finds 7.8% overall DG in a deployed RAG system, rising to 13.6% for recently approved drugs. Entity-attribution verification detects DG at 97.0% precision and 98.7% DG recall; no existing framework implements it.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.09349)
- [PDF](https://arxiv.org/pdf/2607.09349v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/retrieval #keyword/safety #keyword/evaluation #keyword/research-paper
