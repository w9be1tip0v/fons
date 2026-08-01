---
title: "AskChem: Claim-Centered Infrastructure for Chemistry Literature Synthesis"
source: "https://arxiv.org/html/2607.28618v1"
author: "Bing Yan, Gregory Wolfe, Stefano Martiniani, Kyunghyun Cho"
published: "2026-07-30"
created: 2026-08-02
description: "Chemistry literature synthesis often requires assembling specific findings scattered across many publications, yet existing literature-search systems primarily return ranked document lists. As a result, scientists and AI agents need to locate relevant information, verify their provenance, and assemble cross-paper answers manually. We present AskChem, a claim-centered infrastructure for cross-paper chemistry search.…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/retrieval
  - keyword/evaluation
  - keyword/agents
  - keyword/research-paper
---

# AskChem: Claim-Centered Infrastructure for Chemistry Literature Synthesis

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.28618v1)
- published:: 2026-07-30
- updated:: 2026-07-30
- arxiv_id:: 2607.28618v1
- pdf:: https://arxiv.org/pdf/2607.28618v1
- categories:: cs.CL, cs.AI, cs.IR, cs.LG

## Abstract / Summary
Chemistry literature synthesis often requires assembling specific findings scattered across many publications, yet existing literature-search systems primarily return ranked document lists. As a result, scientists and AI agents need to locate relevant information, verify their provenance, and assemble cross-paper answers manually. We present AskChem, a claim-centered infrastructure for cross-paper chemistry search. AskChem changes the unit of retrieval from the paper to the provenance-carrying claim: each paper is converted into atomic, typed claims, each grounded by a source DOI and a verbatim quote or an explicit evidence locator. Over this shared claim store, AskChem exposes complementary structures for search and synthesis: a stabilized faceted taxonomy for hierarchical retrieval and browsing, an evidence graph linking claims through relations, and an exploratory living taxonomy that situates indexed papers under scientific principles. AskChem currently indexes 2.4M claims from 147K papers and provides a web interface, as well as REST, SDK, and MCP access for AI agents. On AskChem-Bench, grounding a GPT-5.5 reader in AskChem yields 100% resolvable DOIs, compared with 88.3% without retrieval, and the highest citation density among five tested systems. AskChem is live at https://askchem.org.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.28618v1)
- [PDF](https://arxiv.org/pdf/2607.28618v1)
- [Language agents achieve superhuman synthesis of scientific knowledge](https://arxiv.org/abs/2409.13740) (2024, citations: 147)
- [Chain-of-Layer: Iteratively Prompting Large Language Models for Taxonomy Induction from Limited Examples](https://arxiv.org/abs/2402.07386) (2024, citations: 35)
- [Do Language Models Know When They’re Hallucinating References?](https://arxiv.org/abs/2305.18248) (2023, citations: 163)
- [Segment Anything](https://arxiv.org/abs/2304.02643) (2023, citations: 14823)
- [OpenAlex: A fully-open index of scholarly works, authors, venues, institutions, and concepts](https://arxiv.org/abs/2205.01833) (2022, citations: 611)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/retrieval #keyword/evaluation #keyword/agents #keyword/research-paper
