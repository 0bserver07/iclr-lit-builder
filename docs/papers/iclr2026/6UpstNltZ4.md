# A Recovery Guarantee for Sparse Neural Networks

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6UpstNltZ4](https://openreview.net/forum?id=6UpstNltZ4)

## Relevance

**LLM score:** 3/3 — The paper provides a sparse recovery guarantee for neural networks using iterative hard thresholding, directly advancing sparsity, a core interest of the Sutro Group for energy-efficient training.
**Keyword hits:** `pruning, sparse`

## TLDR
(none provided)

## Abstract
We prove the first guarantees of sparse recovery for ReLU neural networks, where the sparse network weights constitute the signal to be recovered. Specifically, we study structural properties of the sparse network weights for two-layer, scalar-output networks under which a simple iterative hard thresholding algorithm recovers these weights exactly, using memory that grows linearly in the number of nonzero weights. We validate this theoretical result with simple experiments on recovery of sparse planted MLPs, MNIST classification, and implicit neural representations. Experimentally, we find performance that is competitive with, and often exceeds, a high-performing but memory-inefficient baseline based on iterative magnitude pruning.

## Keywords
compressed sensing, neural networks, model pruning, sparse weight recovery
