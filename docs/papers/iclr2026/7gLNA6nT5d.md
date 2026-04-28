# N-Gram Induction Heads for In-Context RL: Improving Stability and Reducing Data Needs

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7gLNA6nT5d](https://openreview.net/forum?id=7gLNA6nT5d)

## Relevance

**LLM score:** 1/3 — The paper's main contribution is improving in-context RL with n-gram induction heads, tangentially mentioning data reduction and training stability which could indirectly affect efficiency; not primarily focused on Sutro Group's core topics like energy-efficient training, data movement, sparsity, etc.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
In-context learning allows models like transformers to adapt to new tasks from a few examples without updating their weights, a desirable trait for reinforcement learning (RL). However, existing in-context RL methods, such as Algorithm Distillation (AD), demand large, carefully curated datasets and can be unstable and costly to train due to the transient nature of in-context learning abilities. In this work, we integrated the n-gram induction heads into transformers for in-context RL. By incorporating these n-gram attention patterns, we considerably reduced the amount of data required for generalization and eased the training process by making models less sensitive to hyperparameters. Our approach matches, and in some cases surpasses, the performance of AD in both grid-world and pixel-based environments, suggesting that n-gram induction heads could improve the efficiency of in-context RL.

## Keywords
reinforcement learning, in-context reinforcement learning
