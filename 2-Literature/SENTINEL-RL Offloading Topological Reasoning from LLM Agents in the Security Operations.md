---
title: "SENTINEL-RL: Offloading Topological Reasoning from LLM Agents in the Security Operations Center"
source: "https://arxiv.org/html/2609.04159v1"
author: "Uday Vallabhaneni, Cassie L. Cagwin, David J. Wild"
published: "2026-09-03"
created: 2026-09-06
description: "Large language model (LLM) agents are increasingly proposed as autonomous SOC analysts, but two limitations make them unreliable at enterprise scale: a finite context window cannot hold a multi-thousand-host authentication graph, and free-form generation offers no guarantee that a recommended containment action is consistent with the topology it operates on. We present Sentinel-RL, an agentic-SOC architecture that d…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/transformer
  - keyword/language-model
  - keyword/nlp
  - keyword/reasoning
  - keyword/agents
  - keyword/machine-learning
---

# SENTINEL-RL: Offloading Topological Reasoning from LLM Agents in the Security Operations Center

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2609.04159v1)
- published:: 2026-09-03
- updated:: 2026-09-03
- arxiv_id:: 2609.04159v1
- pdf:: https://arxiv.org/pdf/2609.04159v1
- categories:: cs.CR, cs.AI

## Abstract / Summary
Large language model (LLM) agents are increasingly proposed as autonomous SOC analysts, but two limitations make them unreliable at enterprise scale: a finite context window cannot hold a multi-thousand-host authentication graph, and free-form generation offers no guarantee that a recommended containment action is consistent with the topology it operates on. We present Sentinel-RL, an agentic-SOC architecture that decouples topological reasoning from semantic reasoning: a heterogeneous graph attention encoder summarizes the live authentication subgraph into a fixed-dimensional state, a Proximal Policy Optimization (PPO) policy maps this state to a constrained set of investigative actions, and an LLM agent loop is restricted to consuming the policy's recommendations and producing analyst-readable narratives gated by a critic. We instantiate the system on the LANL Comprehensive, Multi-Source Cyber-Security Events dataset and the Indiana University Quartz HPC cluster, reporting four results: (i) a two-phase CREATE ingestion pattern loads a 24M-edge authentication subgraph into Neo4j in 14.2 minutes on a single 32-core node, roughly 24x faster than the canonical MERGE-based pipeline; (ii) a sliding-window alert engine reliably trips a 25-event/10-second threshold in <=2.5 s across 50 trials; (iii) PPO training over 200 iterations converges to a mean episodic return of 8.74+/-0.31, with held-out precision of 0.91 and recall of 0.87 on labeled red-team events; and (iv) the integrated containment loop completes a full detect-investigate-recommend-human-approve cycle in a median of 6.3 s. We contribute a reusable engineering pattern (the hot-node deadlock workaround), a portable HPC deployment pattern (anchor-node co-location), and an enterprise-readiness analysis covering fal…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2609.04159v1)
- [PDF](https://arxiv.org/pdf/2609.04159v1)
- [CyberGFM: Graph Foundation Models for Lateral Movement Detection in Enterprise Networks](https://arxiv.org/abs/2601.05988) (2026, citations: 2)
- [Large Language Model Integration with Reinforcement Learning to Augment Decision-Making in Autonomous Cyber Operations](https://arxiv.org/abs/2509.05311) (2025, citations: 6)
- [Designing a reliable lateral movement detector using a graph foundation model](https://arxiv.org/abs/2504.13527) (2025, citations: 3)
- [Lateral Movement Detection via Time-aware Subgraph Classification on Authentication Logs](https://arxiv.org/abs/2411.10279) (2024, citations: 3)
- [CybORG++: An Enhanced Gym for the Development of Autonomous Cyber Agents](https://arxiv.org/abs/2410.16324) (2024, citations: 15)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/transformer #keyword/language-model #keyword/nlp #keyword/reasoning #keyword/agents #keyword/machine-learning
