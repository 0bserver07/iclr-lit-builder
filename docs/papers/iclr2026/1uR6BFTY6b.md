# DoRAN: Stabilizing Weight-Decomposed Low-Rank Adaptation via Noise Injection and Auxiliary Networks

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1uR6BFTY6b](https://openreview.net/forum?id=1uR6BFTY6b)

## Relevance

**LLM score:** 1/3 — Focuses on parameter-efficient fine-tuning stabilization and sample efficiency, tangentially related to efficiency but not directly advancing energy-efficient training, data movement, sparsity, low-precision, or other named Sutro Group priorities.
**Keyword hits:** `mixture of experts, low-rank, lora`

## TLDR
(none provided)

## Abstract
Parameter-efficient fine-tuning (PEFT) methods have become the standard paradigm for adapting large-scale models. Among these techniques, Weight-Decomposed Low-Rank Adaptation (DoRA) has been shown to improve both the learning capacity and training stability of the vanilla Low-Rank Adaptation (LoRA) method by explicitly decomposing pre-trained weights into magnitude and directional components. In this work, we propose **DoRAN**, a new variant of DoRA designed to further stabilize training and boost the sample efficiency of DoRA. Our approach includes two key stages: (i) injecting noise into the denominator of DoRA’s weight decomposition, which serves as an adaptive regularizer to mitigate instabilities; and (ii) replacing static low-rank matrices with auxiliary networks that generate them dynamically, enabling parameter coupling across layers and yielding better sample efficiency in both theory and practice. Comprehensive experiments on vision and language benchmarks show that DoRAN consistently outperforms LoRA, DoRA, and other PEFT baselines. These results underscore the effectiveness of combining stabilization through noise-based regularization with network-based parameter generation, offering a promising direction for robust and efficient fine-tuning of foundation models.

## Keywords
low-rank adaptation, weight decomposition, self-attention, mixture of experts
