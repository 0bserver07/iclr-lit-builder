# Streaming Visual Geometry Transformer

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5APgTKsnx8](https://openreview.net/forum?id=5APgTKsnx8)

## Relevance

**LLM score:** 1/3 — The paper uses distillation for training and FlashAttention for inference, which touches on efficiency tangentially, but the main contribution is streaming 3D reconstruction, not energy-efficient training or the Sutro Group's core priorities.
**Keyword hits:** `efficient training, cache`

## TLDR
(none provided)

## Abstract
Perceiving and reconstructing 3D geometry from videos is a fundamental yet challenging computer vision task. To facilitate interactive and low-latency applications, we propose a streaming visual geometry transformer that shares a similar philosophy with autoregressive large language models. We explore a simple and efficient design and employ a causal transformer architecture to process the input sequence in an online manner. We use temporal causal attention and cache the historical keys and values as implicit memory to enable efficient streaming long-term 3D reconstruction. This design can handle low-latency 3D reconstruction by incrementally integrating historical information while maintaining high-quality spatial consistency. For efficient training, we propose to distill knowledge from the dense bidirectional visual geometry grounded transformer (VGGT) to our causal model. For inference, our model supports the migration of optimized efficient attention operators (e.g., FlashAttention) from large language models. Extensive experiments on various 3D geometry perception benchmarks demonstrate that our model enhances inference speed in online scenarios while maintaining competitive performance, thereby facilitating scalable and interactive 3D vision systems.

## Keywords
3D reconstruction, geometry transformer
