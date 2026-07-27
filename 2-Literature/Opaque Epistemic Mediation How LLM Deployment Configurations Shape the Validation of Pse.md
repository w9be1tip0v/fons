---
title: "Opaque Epistemic Mediation: How LLM Deployment Configurations Shape the Validation of Pseudo-Science"
source: "https://arxiv.org/html/2607.22513v1"
author: "Davide Scarso, Hugo Noronha de Almeida, Joaquim Pina"
published: "2026-07-24"
created: 2026-07-28
description: "Commercial large language models are increasingly used as knowledge references, yet their stance on contested scientific claims is neither stable nor transparent. We tested how four major LLM families (Claude, Grok, GPT, Gemini) evaluate ethnonationalist pseudo-science derived from Frank Salter's biosocial framework across four temporal snapshots (October 2025-February 2026), via both API and web interfaces. Grok's…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/safety
---

# Opaque Epistemic Mediation: How LLM Deployment Configurations Shape the Validation of Pseudo-Science

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.22513v1)
- published:: 2026-07-24
- updated:: 2026-07-24
- arxiv_id:: 2607.22513v1
- pdf:: https://arxiv.org/pdf/2607.22513v1
- categories:: cs.CY, cs.AI, cs.CL

## Abstract / Summary
Commercial large language models are increasingly used as knowledge references, yet their stance on contested scientific claims is neither stable nor transparent. We tested how four major LLM families (Claude, Grok, GPT, Gemini) evaluate ethnonationalist pseudo-science derived from Frank Salter's biosocial framework across four temporal snapshots (October 2025-February 2026), via both API and web interfaces. Grok's Fast versions (which power the default user experience on X) consistently assigned credibility scores of 70-75, two to five times higher than all other models (which scored 15-40). This pattern was absent from control prompts testing basic evolutionary consensus and refuted Lamarckian claims, where all models performed comparably. Three additional findings emerged: (1) a silent patch reversed Grok's behaviour from chaotic to stably high validation overnight, without any public documentation; (2) the same Grok model identifier produced radically divergent outputs via API (75) and web (5.5) three months later; (3) refusal to rate the pseudo-scientific claim, the most defensible response observed, appeared in two model families through different interfaces (Claude Opus 4.1 categorically via web, GPT-5.1 Chat intermittently via API) and eroded in the successor version of each. These results indicate that the epistemic stance of a commercial LLM is not a stable property of the model but a contingent effect of deployment configuration: system prompts, safety layers, interface routing, and silent updates. This remains opaque to users and researchers alike. We argue this constitutes a matter of public concern requiring new forms of epistemic accountability.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.22513v1)
- [PDF](https://arxiv.org/pdf/2607.22513v1)
- [What Kind of Reasoning (if any) is an LLM actually doing? On the Stochastic Nature and Abductive Appearance of Large Language Models](https://arxiv.org/abs/2512.10080) (2025, citations: 2)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/safety
