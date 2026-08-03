---
title: "Sycophancy Undermines Epistemic Vigilance in Cooperative Vision-Language Tasks"
source: "https://arxiv.org/html/2607.29585v1"
author: "Rupak Sarkar, Neha Srikanth, Saloni Gupta, Claire Bonial, Philip Resnik, Rachel Rudinger"
published: "2026-07-31"
created: 2026-08-04
description: "To maintain common ground in cooperative conversation, humans iteratively update their beliefs as conversation participants share new information; participants who are epistemically vigilant detect when new information conflicts with prior beliefs and take steps to repair these conflicts. In order for AI systems to serve as reliable partners in complex cooperative tasks, they must similarly weigh incoming informatio…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
---

# Sycophancy Undermines Epistemic Vigilance in Cooperative Vision-Language Tasks

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.29585v1)
- published:: 2026-07-31
- updated:: 2026-07-31
- arxiv_id:: 2607.29585v1
- pdf:: https://arxiv.org/pdf/2607.29585v1
- categories:: cs.CL

## Abstract / Summary
To maintain common ground in cooperative conversation, humans iteratively update their beliefs as conversation participants share new information; participants who are epistemically vigilant detect when new information conflicts with prior beliefs and take steps to repair these conflicts. In order for AI systems to serve as reliable partners in complex cooperative tasks, they must similarly weigh incoming information against their own private evidence and shared context and appropriately surface inconsistencies when they arise. To measure the epistemic vigilance of vision-language models in cooperative settings, we present an information-asymmetric, dialog-based "spot-the-difference" task. Two models are privately shown one image each, and must determine through conversation whether the images are identical or, if not, identify the difference. Models routinely fail at this: they frequently overlook key evidence in their private image in favor of agreeing with their conversational partner, even when their agreement is unwarranted. We relate these violations of epistemic vigilance to the broader behavior of sycophancy, which manifests itself in cooperative goal-oriented dialog as over-accommodation and weak evidential grounding. Our results show that model steering to reduce sycophancy with a vector learned from task-agnostic sycophancy examples can reduce epistemic vigilance-related errors, making models more faithful reporters of their evidence, and in turn, more reliable partners in information-asymmetric cooperative tasks.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.29585v1)
- [PDF](https://arxiv.org/pdf/2607.29585v1)
- [MT-PingEval: Evaluating Multi-Turn Collaboration with Private Information Games](https://arxiv.org/abs/2602.24188) (2026, citations: 4)
- [Say It My Way: Exploring Control in Conversational Visual Question Answering with Blind Users](https://arxiv.org/abs/2602.16930) (2026, citations: 2)
- [A Rational Analysis of the Effects of Sycophantic AI](https://arxiv.org/abs/2602.14270) (2026, citations: 11)
- [Safer Policy Compliance with Dynamic Epistemic Fallback](https://arxiv.org/abs/2601.23094) (2026, citations: 1)
- [Accommodation and Epistemic Vigilance: A Pragmatic Account of Why LLMs Fail to Challenge Harmful Beliefs](https://arxiv.org/abs/2601.04435) (2026, citations: 7)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal
