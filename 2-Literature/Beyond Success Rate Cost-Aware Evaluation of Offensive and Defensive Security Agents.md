---
title: "Beyond Success Rate: Cost-Aware Evaluation of Offensive and Defensive Security Agents"
source: "https://arxiv.org/html/2607.15263v1"
author: "Paul Kassianik, Blaine Nelson, Yaron Singer"
published: "2026-07-16"
created: 2026-07-19
description: "Cost-success lens for LM security agents on Cybench (offense) and Splunk BOTS (defense). Offense scales with test-time compute; defense needs disciplined tool use more than raw budget."
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/agents
  - keyword/safety
  - keyword/evaluation
  - keyword/language-model
---

# Beyond Success Rate: Cost-Aware Evaluation of Offensive and Defensive Security Agents

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.15263v1)
- published:: 2026-07-16
- updated:: 2026-07-16
- arxiv_id:: 2607.15263v1
- pdf:: https://arxiv.org/pdf/2607.15263v1
- categories:: cs.AI, cs.CR

## Abstract / Summary
Security-agent evals often report peak offensive capability under generous inference budgets. Operationally, every reasoning step, tool call, telemetry query, and enrichment spends budget. This paper evaluates LM security agents with a cost-success lens on offensive Cybench and defensive Splunk BOTS v1, comparing models at fixed cost and decomposing inference vs tool spend. Offensive CTF performance improves with test-time compute; scaled open-weight models can approach proprietary systems while staying cost-competitive. Defensive SOC investigation does not scale the same way—success hinges more on disciplined tool use, telemetry navigation, and selective enrichment than raw reasoning budget. Argues benchmarks should measure economic efficiency and operational fit alongside task success. Results site: https://evals.frontier.security

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.15263v1)
- [PDF](https://arxiv.org/pdf/2607.15263v1)
- [Interactive results](https://evals.frontier.security)
- [Cyber Defense Benchmark](https://arxiv.org/abs/2604.19533) (2026, citations: 3)
- [Before You Hand Over the Wheel](https://arxiv.org/abs/2603.06422) (2026, citations: 1)
- [ExCyTIn-Bench](https://arxiv.org/abs/2507.14201) (2025, citations: 11)
- [BountyBench](https://arxiv.org/abs/2505.15216) (2025, citations: 33)
- [Benchmarking LLMs in an Embodied Environment for Blue Team Threat Hunting](https://arxiv.org/abs/2505.11901) (2025, citations: 8)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/agents #keyword/safety #keyword/evaluation #keyword/language-model
