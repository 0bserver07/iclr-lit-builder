# Point-MoE: Large-Scale Multi-Dataset Training with Mixture-of-Experts for 3D Semantic Segmentation

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=35HahPHrFG](https://openreview.net/forum?id=35HahPHrFG)

## Relevance

**LLM score:** 1/3 — Uses sparse mixture-of-experts (sparsity) but primarily addresses multi-dataset 3D segmentation scaling, not training efficiency or energy as a main contribution.
**Keyword hits:** `moe`

## TLDR
(none provided)

## Abstract
While massively both scaling data and models have become central in NLP and 2D vision, their benefits for 3D point cloud understanding remain limited. 
We study the initial step of 3D point cloud scaling under a realistic regime: large-scale multi-dataset joint training for 3D semantic segmentation, with no dataset labels available at inference time. 
Point clouds arise from a wide range of sensors (e.g., depth cameras, LiDAR) and scenes (e.g., indoor, outdoor), yielding heterogeneous scanning patterns, sampling densities, and semantic biases; naively mixing such datasets degrades standard backbones. 
We introduce **Point-MoE**, a Mixture-of-Experts design that expands capacity through sparsely activated expert MLPs and a lightweight top-$k$ router, allowing tokens to select specialized experts without requiring dataset supervision. 
Trained jointly on a diverse mix of indoor and outdoor datasets and evaluated on seen datasets and in zero-shot settings, Point-MoE outperforms prior methods without using dataset labels for either training or inference.
This outlines a scalable path for 3D perception: letting the model discover structure in heterogeneous 3D data rather than imposing it via manual curation or dataset-specific heuristics.

## Keywords
3D Semantic Segmentation, Mixture of Expert, Point Cloud Understanding
