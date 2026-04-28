# DSA: Efficient Inference For Video Generation Models via Distributed Sparse Attention

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1ZmdfDzGE1](https://openreview.net/forum?id=1ZmdfDzGE1)

## Relevance

**LLM score:** 2/3 — The paper introduces sparse attention as a core method for efficient inference, directly advancing sparsity and distributed data movement, which aligns with the group's interest in sparsity and energy-aware computation though focused on inference rather than training.
**Keyword hits:** `sparsity, sparse`

## TLDR
(none provided)

## Abstract
Diffusion Transformer models have driven the rapid advances in video generation, achieving state-of-the-art quality and flexibility. However, their attention mechanism remains a major performance bottleneck, as its dense computation scales quadratically with the sequence length. To overcome this limitation and reduce the generation latency, we propose DSA, a novel attention mechanism that integrates sparse attention with distributed inference for diffusion-based video generation. By leveraging carefully-designed parallelism strategies and scheduling, DSA significantly reduces redundant computation while preserving global context. Extensive experiments on benchmark datasets demonstrate that, when deployed on 8 GPUs, DSA achieves up to 1.43× inference speedup than the existing distributed method and 10.79× faster than single-GPU inference.

## Keywords
Distributed System, Diffusion, Inference, Sparsity
