# Shadow loss: Memory-linear deep metric learning with anchor projection

**Venue:** iclr2026 (Withdraw)
**Authors:** Alif Elham Khan, Mohammad Junayed Hasan, Humayra Anjum, Nabeel Mohammed
**OpenReview:** [https://openreview.net/forum?id=3fx0Kz6Zfl](https://openreview.net/forum?id=3fx0Kz6Zfl)

## Relevance

**LLM score:** 3/3 — The paper directly advances energy-efficient training by reducing memory buffer from O(S*D) to O(S) in metric learning, addressing data movement and enabling training on memory-constrained hardware.
**Keyword hits:** `efficient training`

## TLDR
(none provided)

## Abstract
Deep metric learning objectives (e.g., triplet loss) require storing and comparing high-dimensional embeddings, making the per-batch loss buffer scale as $O(S\cdot D)$ and limiting training on memory-constrained hardware. We propose Shadow Loss, a proxy-free, parameter-free objective that measures similarity via scalar projections onto the anchor direction, reducing the loss-specific buffer from $O(S\cdot D)$ to $O(S)$ while preserving the triplet structure. We analyze gradients, provide a Lipschitz continuity bound, and show that Shadow Loss penalizes trivial collapse for stable optimization. Across fine-grained retrieval (CUB-200, CARS196), large-scale product retrieval (Stanford Online Products, In-Shop Clothes), and standard/medical benchmarks (CIFAR-10/100, Tiny-ImageNet, HAM-10K, ODIR-5K), Shadow Loss consistently outperforms recent objectives (Triplet, Soft-Margin Triplet, Angular Triplet, SoftTriple, Multi-Similarity). It also converges in $\approx 1.5\text{-}2\times$ fewer epochs under identical backbones and mining. Furthermore, it improves representation separability as measured by higher silhouette scores. The design is architecture-agnostic and vectorized for efficient implementation. By decoupling discriminative power from embedding dimensionality and reusing batch dot-products, Shadow Loss enables memory-linear training and faster convergence, making deep metric learning practical on both edge and large-scale systems.

## Keywords
Deep Metric Learning, Proxy-free Loss, Shadow Loss, Anchor Projection, Siamese Networks, Triplet Objectives, Contrastive Objectives, Memory-efficient Training, Large-scale Image Retrieval, Fine-grained Retrieval, Lipschitz Analysis, Architecture-agnostic Objective
