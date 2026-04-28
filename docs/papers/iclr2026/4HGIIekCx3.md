# DenseMixer: Improving MoE Post-Training with Precise Router Gradient

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4HGIIekCx3](https://openreview.net/forum?id=4HGIIekCx3)

## Relevance

**LLM score:** 1/3 — Mentions MoE sparsity and training efficiency indirectly, but the main contribution is a refined router gradient estimation for post-training quality, not a direct advance in energy-efficient training, data movement, or other Sutro Group priorities.
**Keyword hits:** `lora, moe`

## TLDR
(none provided)

## Abstract
Mixture-of-Experts (MoE) models are notoriously harder to train compared with dense models. Existing approaches either rely on imprecise router gradient or freeze router parameters entirely, limiting training effectiveness. We introduce DenseMixer, a novel MoE post-training technique that trades one extra forward pass on inactive experts for a more precise router gradient estimation. Our method consistently outperforms conventional methods across different MoE scales (7B, 14B, 16B, 30B), architectures (with/without shared experts), pre-training methods (from scratch/up-cycling), and post-training data types (instruction/long CoT data). It is universally applicable to any MoE using Top-K routing and can be used in a plug-and-play manner, compatible with existing training libraries and parameter-efficient methods like LoRA, introducing no changes to inference. We provide comprehensive empirical validation showing DenseMixer's effectiveness in improving MoE post-training quality while maintaining practical computational overhead.

## Keywords
MoE, Post-Training
