# MAGNET: Multi-granular Adaptive Gradient-guided Knowledge Distillation for Pareto-Efficient Tuning

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=465S0gvFWc](https://openreview.net/forum?id=465S0gvFWc)

## Relevance

**LLM score:** 3/3 — Directly advances energy-efficient training via knowledge distillation with gradient-guided sparsity and Pareto-efficient student architecture selection, aligning with key Sutro Group priorities.
**Keyword hits:** `knowledge distillation, distillation`

## TLDR
(none provided)

## Abstract
Despite the remarkable advances achieved by large pretrained models (LPMs), their practical utility remains significantly constrained due to prohibitive computational and memory demands. While knowledge distillation (KD) partially alleviates this challenge, existing KD techniques rely predominantly on heuristically selected student architectures, resulting in suboptimal teacher-student pairings that frequently fail to achieve Pareto-optimal trade-offs between efficiency and performance. To overcome this limitation, we introduce MAGNET, a multi-granular adaptive gradient-guided knowledge distillation framework designed to analytically derive Pareto-efficient student architectures without heuristic intervention. Specifically, MAGNET initiates a concise gradient-profiling step on a small validation set, computing mean absolute gradients to rank layers according to their saliency. Based on this gradient-informed hierarchy, MAGNET selectively inherits only the most informative blocks, forming a highly compact student model. Within each selected block, MAGNET further masks parameters exhibiting minimal gradient magnitudes and executes a unified, single-stage training procedure integrating direct supervision, logit matching, and feature alignment. Comprehensive experiments across various vision and language benchmarks demonstrate that MAGNET consistently achieves superior accuracy with significantly fewer parameters and reduced computational overhead compared to state-of-the-art (SOTA) KD approaches.

## Keywords
Large Pretrained Models, Knowledge Distillation, Gradient-Guided Distillation, Pareto Efficiency
