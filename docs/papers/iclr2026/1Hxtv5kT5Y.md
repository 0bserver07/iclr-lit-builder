# FastALM: Hierarchical Frame Q-Former for Effective Audio Modality Adaptation

**Venue:** iclr2026 (Withdraw)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1Hxtv5kT5Y](https://openreview.net/forum?id=1Hxtv5kT5Y)

## Relevance

**LLM score:** 1/3 — The paper focuses on efficient inference for audio-language models by compressing speech features, which is tangential to the Sutro Group's core interests in training efficiency, data movement, or low-precision techniques.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
Recent advances in large language models (LLMs) have demonstrated human-expert-level capabilities, driving significant interest in their potential for achieving artificial general intelligence (AGI). In particular, there is growing momentum in adapting LLMs to various modalities—including vision, video, and speech—through the development of multimodal LLMs (MLLMs). However, existing speech-language models (SLMs) research has largely overlooked cost-effective adaptation strategies for leveraging LLMs in the speech domain. In this paper, we propose FastSLM, a lightweight yet efficient SLM designed for effective understanding and reasoning over long-form speech. To address the challenge of aligning high-frame speech features with LLM, we introduce the hierarchical frame querying transformer (HFQ-Former), which compresses frame-level speech features while capturing both local and global context. Furthermore, we present a novel three-stage training strategy that enhances generalization across a wide range of speech-related tasks. Experimental results demonstrate that FastSLM achieves competitive performance compared to existing state-of-the-art (SOTA) models, despite operating with significantly lower FLOPs and parameter counts, while representing speech with only 1.67 tokens per second. The source code and model checkpoints are available at https://anonymous.4open.science/r/FastALM-1D6B.

## Keywords
Audio Language Model (ALM), Q-Former, Multimodal
