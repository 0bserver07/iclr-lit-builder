# BlindSight: Harnessing Sparsity for Efficient Vision-Language Models

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=63L0Vsvpn9](https://openreview.net/forum?id=63L0Vsvpn9)

## Relevance

**LLM score:** 1/3 — The paper leverages sparsity and a hardware-aware kernel for inference optimization, not training, making it tangential to the Sutro Group's training-focused efficiency priorities.
**Keyword hits:** `sparsity, sparse, kernel`

## TLDR
(none provided)

## Abstract
Large vision-language models (VLMs) enable joint processing of text and images. However, the inclusion of vision data significantly increases the prompt length, resulting in a longer time to first token (TTFT). This bottleneck can be mitigated by leveraging the inherent sparsity in the attention computation. Analyzing these attention patterns in VLMs when processing a series of images, we observe the absence of cross-image attention in a substantial portion of layers. Based on this, we propose BlindSight: a training-free approach to optimize multi-image VLM inference using an input-template-aware attention sparsity mask.  We utilize a dataset to derive a prompt-agnostic categorization for attention heads: Dense, Sink, Intra-Image, and Intra-Image+Sink. We further develop a Triton-based GPU kernel to leverage this sparsity. BlindSight achieves a 1.8-3.2X speedup in the attention computation (prompt length 36K-300K). We evaluate BlindSight using VLMs such Qwen2-VL, Qwen2.5-VL and Gemma 3; observing only a 0.78% accuracy degradation on average for the evaluated multi-image understanding benchmarks.

## Keywords
VLMs, Sparse Attention, Multimodal Models, Prefill Optimization
