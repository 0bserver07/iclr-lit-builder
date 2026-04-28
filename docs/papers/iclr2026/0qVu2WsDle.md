# Toward Bit-Efficient Dataset Condensation: A General Framework

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0qVu2WsDle](https://openreview.net/forum?id=0qVu2WsDle)

## Relevance

**LLM score:** 3/3 — The paper introduces a low-precision quantization method for dataset condensation, directly reducing memory, bandwidth, and improving hardware utilization, aligning closely with Sutro Group priorities in low-precision, data movement, and efficient training.
**Keyword hits:** `efficient training, low-precision`

## TLDR
(none provided)

## Abstract
Dataset condensation aims to distill a large-scale dataset into a compact set of synthetic samples for efficient training. Existing methods primarily focus on reducing the number of samples but generally assume full-precision representations. While effective, this assumption limits their applicability in resource-constrained scenarios due to several major drawbacks:
(1) \textit{Transmission bottlenecks}—full-precision datasets consume excessive bandwidth and introduce latency during network transfer, especially in cloud–edge collaborative learning;
(2) \textit{Memory overhead}—storing and processing full-precision data rapidly exhausts GPU memory or RAM, restricting batch sizes; and
(3) \textit{Hardware underutilization}—modern accelerators are optimized for low-precision operations, yet full-precision data prevents full efficiency gains in training and inference.
To address these challenges, we propose a novel approach that fine-tunes distilled full-precision datasets into compact low-bit representations, substantially reducing memory usage with minimal computational overhead. Central to our method is a differentiable bit-conscious optimization framework. This framework allows more synthetic samples to be stored within the same memory budget, thereby improving downstream performance.
Beyond the algorithmic contribution, we provide theoretical analysis that characterizes (1) the trade-off between compression error and generalization error under memory constraints, and (2) the extent to which Fisher information is preserved under bit compression. Extensive experiments on multiple benchmarks against state-of-the-art baselines validate both the effectiveness and efficiency of our method.

## Keywords
Dataset Condensation
