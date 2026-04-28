# A Separable Self-attention Inspired by the State Space Model for Computer Vision

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1KUMxnrhnH](https://openreview.net/forum?id=1KUMxnrhnH)

## Relevance

**LLM score:** 1/3 — The paper proposes an efficient separable self-attention with linear complexity, but its main contribution is architectural design for vision, not explicitly focusing on energy-efficient training, data movement, sparsity, or other Sutro Group priorities.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
Separable self-attention is an early attention mechanism with linear complexity. When parameters and FLOPs are comparable, lightweight networks built upon separable self-attention and its variants underperform the recent Vision Mamba (ViM). By analyzing the strengths and weaknesses of separable self-attention, we distill four design principles and, inspired by the State Space Model (SSM) serving as the core of ViM, propose a novel separable self-attention termed Vision Mamba Inspired Separable self-Attention (VMI-SA). Notably, VMI-SA does not incorporate any SSM blocks, and its attention computation process differs from all existing attention mechanisms to the best of our knowledge. We introduce proof-of-concept networks, VMINet and VMIFormer, enabling fair comparisons with ViMs through deliberate control of parameters, FLOPs, and encoder numbers. Compared to state-of-the-art Transformers, CNNs, and ViMs, VMINet and VMIFormer achieve competitive results in image classification and high-resolution dense prediction tasks.

## Keywords
Separable Self-attention, State Space Models, Vision Mamba
