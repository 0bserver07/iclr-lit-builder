# Mutual Information Preserving Neural Network Pruning

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6nxI3aELvc](https://openreview.net/forum?id=6nxI3aELvc)

## Relevance

**LLM score:** 3/3 — Proposes a sparsity method (pruning) to reduce neural network resource requirements, directly aligned with the Sutro Group's sparsity priority.
**Keyword hits:** `lottery ticket, pruning`

## TLDR
(none provided)

## Abstract
Pruning has emerged as one of the primary approaches used to limit the resource requirements of large neural networks (NNs). Since the proposal of the lottery ticket hypothesis, researchers have focused either on pruning at initialization or after training. However, recent theoretical findings have shown that the sample efficiency of robust pruned models is proportional to the mutual information (MI) between the pruning masks and the model's training datasets, \textit{whether at initialization or after training}. In this paper, we introduce Mutual Information Preserving Pruning (MIPP),  a structured activation-based pruning technique applicable before or after training.  The core principle of MIPP is to select nodes in a way that conserves MI shared between the activations of adjacent layers, and consequently between the data and masks. Approaching the pruning problem in this manner means we can prove that there exists a function that can map the pruned upstream layer's activations to the downstream layer's, implying re-trainability. We demonstrate that MIPP consistently outperforms baselines, regardless of whether pruning is performed before or after training.

## Keywords
Pruning, Mutual Information, Deep Learning
