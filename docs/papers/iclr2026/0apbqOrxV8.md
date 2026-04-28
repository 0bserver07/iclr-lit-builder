# Energy Efficient Language Models through Dynamic Sparsity

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0apbqOrxV8](https://openreview.net/forum?id=0apbqOrxV8)

## Relevance

**LLM score:** 1/3 — Paper focuses on inference efficiency through activation sparsity and quantization for deployment, not training, making it tangential to the group's explicit focus on energy-efficient training.
**Keyword hits:** `energy efficient, quantized, sparsity, sparse, cache`

## TLDR
(none provided)

## Abstract
Transformer models, despite their impressive performance, often face practical limitations due to their high computational requirements driven largely by the memory-bound KV-cache. State-space Models (SSMs) attempt to address this issue with linear attention, easing memory pressure and improving compute and memory efficiency. However, their efficiency is instead limited by dense linear layers with inherently low arithmetic intensity, again leading to a memory-bound landscape, posing challenges for deployment on hardware-constrained edge devices where these models might otherwise excel. In this work, we present a technique to induce high activation sparsity in quantized SSMs with minimal performance degradation, both for smaller-scale models suitable for edge-deployment and larger billion scale models. We nullify activations within a trainable threshold ($\pm \Delta$), which preserves outliers that are crucial for high performance. With only 1/4 of the effective MAC (Multiply-Accumulate) operations of a dense model, our sparse MatMul-free models maintain competitive performance compared to the dense base model. As GPUs offer limited support for unstructured sparsity during inference, we target a neuromorphic hardware platform that efficiently supports this dynamic and unstructured activation sparsity on a silicon level. Based on previous deployment results of a dense model, our sparsified models can increase throughput by 37$\times$ while decreasing power consumption by 16$\times$ compared to an edge GPU-based deployment of a comparable transformer-based LLM. Compared to a baseline dense model on the same hardware, we show improvements of 5.4$\times$ in both metrics, paving the way for future explorations of highly efficient language models leveraging dynamic activation sparsity.

## Keywords
State-space models, large language models, activation sparsity, unstructured sparsity, neuromorphic hardware, event-driven computation, low-power inference
