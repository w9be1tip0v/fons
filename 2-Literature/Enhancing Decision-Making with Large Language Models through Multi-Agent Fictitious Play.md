---
title: "Enhancing Decision-Making with Large Language Models through Multi-Agent Fictitious Play"
source: "https://arxiv.org/html/2606.19308v1"
author: "Leyang Shen, Yang Zhang, Xiaoyan Zhao, Chun Kai Ling, Tat-Seng Chua"
published: "2026-06-17"
created: 2026-06-19
description: "Large language model (LLM)-based multi-agent systems (MAS) have demonstrated great potential in solving tasks with execution complexity, by distributing subtasks across cooperative agents. However, this divide-and-conquer paradigm falls short on decision-making tasks that are also prevalent in the real world. These tasks require simultaneous reasoning from the stances of all involved stakeholders whose decisions are…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/evaluation
  - keyword/reasoning
  - keyword/agents
---

# Enhancing Decision-Making with Large Language Models through Multi-Agent Fictitious Play

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2606.19308v1)
- published:: 2026-06-17
- updated:: 2026-06-17
- arxiv_id:: 2606.19308v1
- pdf:: https://arxiv.org/pdf/2606.19308v1
- categories:: cs.CL, cs.MA

## Abstract / Summary
Large language model (LLM)-based multi-agent systems (MAS) have demonstrated great potential in solving tasks with execution complexity, by distributing subtasks across cooperative agents. However, this divide-and-conquer paradigm falls short on decision-making tasks that are also prevalent in the real world. These tasks require simultaneous reasoning from the stances of all involved stakeholders whose decisions are mutually dependent and thus cannot be solved in isolation. We characterize this challenge as stance entanglement, a form of decision complexity distinct from execution complexity. To address it, we propose Multi-Agent Fictitious Play (MAFP), a novel MAS paradigm that represents stakeholder stances as agents and formulates decision-making as an equilibrium-seeking process. Built on the game-theoretic principle of fictitious play, MAFP iteratively updates each agent's decision by best responding to the empirical mixture of other agents' past decisions. This enables agents to expose and address one another's weaknesses, progressively improving decision quality and robustness. We evaluate MAFP on challenging decision-making tasks that test the capability of deciding strategies for competitive scenarios prior to acting. MAFP outperforms both single-round and multi-round baselines on two complementary metrics, tournament strength and robustness, demonstrating its effectiveness in addressing stance entanglement.

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2606.19308v1)
- [PDF](https://arxiv.org/pdf/2606.19308v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/evaluation #keyword/reasoning #keyword/agents
