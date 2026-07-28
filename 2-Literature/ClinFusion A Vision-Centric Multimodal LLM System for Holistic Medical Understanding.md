---
title: "ClinFusion: A Vision-Centric Multimodal LLM System for Holistic Medical Understanding"
source: "https://arxiv.org/html/2607.24743v1"
author: "Hangjie Yuan, Yichen Qian, Zhiwei Tang, Xianzhe Xu, Lirong Wu, Sicheng Yang, Jinwang Wang, Pengju Wang, Zhitao Zeng, Yizeng Han, Yan Xing, Shengxuan Luo, Tao Feng, Qing Xie, Weigen Yao, Yi Yang, Zuozhu Liu, Jiasheng Tang, Shaocheng Wang, Jitao Wang, Jiahong Dong, Weihua Chen, Feng Xu, Fan Wang"
published: "2026-07-27"
created: 2026-07-29
description: "Multimodal large language models (MLLMs) hold immense potential to revolutionize clinical practice, yet deploying them in the medical domain is fundamentally a vision-centric challenge: models must absorb knowledge from heterogeneous 2D and 3D medical images, and evaluation protocols must align with radiologists' clinical practice and provide an accurate, fine-grained and factualness-driven assessment. In this paper…"
tags:
  - type/literature
  - theme/research
  - theme/learning
  - source/arxiv
  - keyword/language-model
  - keyword/nlp
  - keyword/multimodal
  - keyword/retrieval
  - keyword/evaluation
  - keyword/benchmark
  - keyword/agents
  - keyword/research-paper
---

# ClinFusion: A Vision-Centric Multimodal LLM System for Holistic Medical Understanding

## Source Metadata
- type:: paper
- source:: [arXiv](https://arxiv.org/html/2607.24743v1)
- published:: 2026-07-27
- updated:: 2026-07-27
- arxiv_id:: 2607.24743v1
- pdf:: https://arxiv.org/pdf/2607.24743v1
- categories:: cs.CV, cs.AI, cs.CL

## Abstract / Summary
Multimodal large language models (MLLMs) hold immense potential to revolutionize clinical practice, yet deploying them in the medical domain is fundamentally a vision-centric challenge: models must absorb knowledge from heterogeneous 2D and 3D medical images, and evaluation protocols must align with radiologists' clinical practice and provide an accurate, fine-grained and factualness-driven assessment. In this paper, we introduce ClinFusion, a vision-centric MLLM designed for holistic medical understanding that systematically addresses these limitations. We propose a compositional and cascaded vision encoder architecture featuring a Cascade Spatial-Aware Locality Fusion operator that unifies diverse 2D and native 3D medical image understanding within a fused encoder. We further introduce a vision-grounded evaluation framework, including MedIF-Bench for instruction-following assessment and a region-of-interest-grounded method for clinically aligned and factualness-driven report generation evaluation. We show that ClinFusion sets a new state-of-the-art across a comprehensive suite of 2D and 3D multimodal medical benchmarks---spanning visual question answering, report generation, and instruction following---as well as textual medical tasks, outperforming leading open-source medical MLLMs (\textit{e.g.}, Hulu-Med, Lingshu) on 20 out of 24 benchmarks and demonstrating multimodal capabilities better than powerful proprietary models such as GPT-5.2 and Gemini-3-Flash on 13 out of 16 benchmarks, and can be further augmented with agentic tool use for retrieval-augmented and tool-assisted clinical workflows. A blinded evaluation by board-certified radiologists confirms that ClinFusion produces the highest-ranked reports, and validates our RoI-grounded metric as achieving the str…

## Why it matters for GenAI tracking
- Captured automatically as part of the nightly generative-AI research and technical-blog watchlist.
- Review manually before promoting any idea to `3_Permanent` notes.

## Related Materials
- [arXiv abstract](https://arxiv.org/abs/2607.24743v1)
- [PDF](https://arxiv.org/pdf/2607.24743v1)

## Follow-up Questions
- question:: Should this be converted into a permanent insight note?
- question:: Are there implementation details, benchmarks, or released code worth tracking separately?

---
Tags: #type/literature #theme/research #theme/learning #source/arxiv #keyword/language-model #keyword/nlp #keyword/multimodal #keyword/retrieval #keyword/evaluation #keyword/benchmark #keyword/agents #keyword/research-paper
