# RS-MoE: Collaborative Compression for Mixture-of-Experts LLMs based on Low-Rank and Sparse Approximation

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5SQbPbCU6P](https://openreview.net/forum?id=5SQbPbCU6P)

## Relevance

**LLM score:** 1/3 — The paper addresses post-training compression using low-rank and sparse approximation, not directly training efficiency or the Sutro Group's named training-focused priorities.
**Keyword hits:** `model compression, low-rank, sparse, moe`

## TLDR
(none provided)

## Abstract
Mixture-of-Experts (MoE) based Large Language Models (LLMs), despite their computational efficiency, face significant storage and memory challenges, which hinder their deployment on edge devices. 
However, existing methods primarily focus on compressing at the expert level, resulting in the loss of specialized knowledge. 
To address these challenges, we propose a novel framework termed RS-MoE, which compresses MoE models by collaboratively decomposing the weights of each expert into low-rank and sparse components. 
Through a preliminary investigation of the relationship between activations and weights, we identified two key observations: (i) a small fraction of weight dimensions, identifiable by high activation peaks, are critical and can be treated as a sparse component, and (ii) the remaining weights, after removing these high-importance dimensions, exhibit an inherent low-rank structure.
Building on this, we developed a comprehensive importance score based on activation peaks to apply a tailored policy: high-importance dimensions are sparsely preserved, while the remaining dimensions are approximated using a low-rank representation.
Additionally, ridge regression and mutual information techniques are incorporated to further minimize errors.
We performed a comprehensive evaluation of RS-MoE on several MoE LLMs, including DeepSeekMoE-16B-Base, Mixtral-8x7B, and Qwen3-30B-A3B.
The results demonstrate that our approach consistently outperforms existing monolithic sparse or low-rank methods across a variety of downstream tasks, highlighting its superior effectiveness and generalizability.

## Keywords
Mixture-of-Experts, Model Compression, Low-Rank Approximation, Mutual Information, Ridge Regression
