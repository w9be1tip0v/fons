---
title: "From the Hugging Face Hub to robot hardware with Strands Agents and LeRobot"
source: "https://huggingface.co/blog/amazon/strands-lerobot-hub-to-hardware"
author: "Hugging Face Blog"
published: "2026-06-17"
created: 2026-06-18
description: "You have a robot, a folder of demonstration data on the Hugging Face Hub , and a new task you want it to learn. Today that takes five separate tools: one to record new demonstrations, another to train, a third to test in simulation, custom code to deploy on hardware, and yet another to coordinate when you have more than one robot. The pieces work on their own. They don't talk to each other. Strands Robots is an open…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/huggingface
  - keyword/agents
---

# From the Hugging Face Hub to robot hardware with Strands Agents and LeRobot

## Source Metadata
- type:: blog
- source:: [Hugging Face Blog](https://huggingface.co/blog/amazon/strands-lerobot-hub-to-hardware)
- published:: 2026-06-17

## Abstract / Summary
You have a robot, a folder of demonstration data on the Hugging Face Hub , and a new task you want it to learn. Today that takes five separate tools: one to record new demonstrations, another to train, a third to test in simulation, custom code to deploy on hardware, and yet another to coordinate when you have more than one robot. The pieces work on their own. They don't talk to each other. Strands Robots is an open source SDK from AWS ( Apache 2.0 ) that exposes robot abstractions, simulation, and the LeRobot stack as AgentTools that you compose into a single Strands agent. The integration is deliberately thin: LeRobot's own scripts handle hardware recording and calibration, and the Strands AgentTools come in for the parts an agent actually orchestrates. The simulation tool records LeRobotDatasets in the same format LeRobot writes on hardware. GR00T and LerobotLocal serve policy… This post walks you through five steps inside a single agent: build the agent over the LeRobot AgentTools, record a demonstration as a LeRobotDataset in simulation, run a policy on the same robot, deploy the same agent code to a physical SO-101 with one keyword argument change, and broadcast commands acr…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [Hugging Face Blog](https://huggingface.co/blog)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/huggingface #keyword/agents
