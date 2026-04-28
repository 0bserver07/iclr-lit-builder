# Slimming the Giant: Efficient Structured Pruning for Adapter-Tuned SAM

**Venue:** iclr2026 (Withdraw)
**Authors:** Xin Luo, chunjiang wang, Zihang Jiang, S Kevin Zhou
**OpenReview:** [https://openreview.net/forum?id=5Rgn6x9jGn](https://openreview.net/forum?id=5Rgn6x9jGn)

## Relevance

**LLM score:** 1/3 — Paper uses structured pruning for inference-time compression and latency gains, not for improving training efficiency, data movement during training, or other Sutro Group training-centric priorities.
**Keyword hits:** `model compression, pruning`

## TLDR
(none provided)

## Abstract
Foundation models with parameter-efficient adapters enable strong segmentation but remain hard to deploy due to scale and cost. We propose Adapter-aware Structured Sparsification (ASSP), a structured pruning framework for adapter-tuned SAM. ASSP begins with a concise dependency analysis of backbone–adapter couplings and derives unified slicing rules for heads, channels, and kernels. It then scores structures via a Projected-Gradient Residual criterion that aligns upstream and downstream gradient subspaces, and restores accuracy with a dual-stream compensation scheme that alternates supervision on both data sources. The procedure runs in two stages: prune and recover adapters, then freeze adapters and prune and recover the backbone. Built on SAM-Med2D, ASSP uses only 20k images (0.4% of SA-Med2D-20M) yet reduces encoder parameters by over 75% and compute to about one quarter, while Dice typically stays within two points of the baseline. Under the same calibration budget it outperforms a transferred SlimSAM baseline and yields consistent latency and throughput gains on H20 GPUs. Although evaluated on medical data, the dependency modeling, PGR scoring, and dual-stream compensation are task-agnostic and broadly applicable to adapter-tuned models.

## Keywords
Structured Pruning, Model Compression, Vision Foundation Models
