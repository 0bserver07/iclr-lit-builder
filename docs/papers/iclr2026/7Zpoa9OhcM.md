# MoE-PHDS: One MoE checkpoint for flexible runtime sparsity

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7Zpoa9OhcM](https://openreview.net/forum?id=7Zpoa9OhcM)

## Relevance

**LLM score:** 3/3 — Directly addresses sparsity and training efficiency by enabling a single MoE checkpoint to serve multiple sparsity levels, reducing the need to train multiple models.
**Keyword hits:** `mixture of experts, sparsity, sparse, moe`

## TLDR
(none provided)

## Abstract
Sparse Mixtures of Experts (MoEs) are typically trained to operate at a fixed sparsity level, e.g. $k$ in a top-$k$ gating function. This global sparsity level determines an operating point on the accuracy/latency curve; currently, meeting multiple efficiency targets means training and maintaining multiple models. This practice complicates serving, increases training and maintenance costs, and limits flexibility in meeting diverse latency, efficiency, and energy requirements. We show that pretrained MoEs are more robust to runtime sparsity shifts than commonly assumed, and introduce MoE-PHDS ({\bf P}ost {\bf H}oc {\bf D}eclared {\bf S}parsity), a lightweight SFT method that turns a single checkpoint into a global sparsity control surface. PHDS mixes training across sparsity levels and anchors with a short curriculum at high sparsity, requiring no architectural changes. The result is predictable accuracy/latency tradeoffs from one model: practitioners can ``dial $k$'' at inference time without swapping checkpoints, changing architecture, or relying on token-level heuristics. Experiments on OLMoE-1B-7B-0125, Qwen1.5-MoE-A2.7B, and proprietary models fit on multiple operating points show that PHDS matches or exceeds well-specified oracle models, improves cross-sparsity agreement by up to 22\% vs. well-specified oracle models, and enables simplified, flexible runtime MoE deployment by making global sparsity a first-class serving primitive.

## Keywords
Mixture of Experts (MoE), model misspecification, model adaptability
