# Qronos: Correcting the Past by Shaping the Future... in Post-Training Quantization

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7axclBCYul](https://openreview.net/forum?id=7axclBCYul)

## Relevance

**LLM score:** 1/3 — While quantization is a named priority, the paper focuses on post-training quantization for inference efficiency, not energy-efficient training or training-specific advancements.
**Keyword hits:** `quantization, quantized`

## TLDR
(none provided)

## Abstract
We introduce Qronos---a new post-training quantization algorithm that not only explicitly corrects errors due to both weight and activation quantization, but also corrects errors accumulated from previously quantized layers. Our iterative algorithm is based on an interpretable and disciplined optimization framework that surpasses existing data-driven approaches. At each step, Qronos alternates between error correction and diffusion via optimal update rules. Importantly, we prove that Qronos admits an equivalent formulation that significantly improves algorithmic efficiency; we use our discovery to reduce peak memory usage by 18\times on Llama3 8B, and our scaling analysis shows a speedup of up to  13.8\times for a single-layer microbenchmark. We demonstrate compatibility with existing transformation techniques such as Hadamard-based incoherence processing and weight-activation scaling equalization, among others. We evaluate Qronos using recent language models in the Llama3 and Qwen3 families; Qronos consistently outperforms previous state-of-the-art adaptive rounding methods when quantizing the weights, activations, and/or KV caches to 4 bits or fewer.

## Keywords
Post Training Quantization, Large Language Models, Foundation Models, Efficient Machine Learning
