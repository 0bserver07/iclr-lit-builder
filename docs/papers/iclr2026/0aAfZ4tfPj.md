# MARS: Mamba-driven Adaptive Reordering Scheme for Semantic Occupancy Prediction in Autonomous Driving

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0aAfZ4tfPj](https://openreview.net/forum?id=0aAfZ4tfPj)

## Relevance

**LLM score:** 1/3 — The paper focuses on a task-specific architecture for autonomous driving that reduces memory usage and computational cost via voxel pruning and reordering, which is tangential to the Sutro Group's core interests in general energy-efficient training techniques like data movement, cache-aware ML, or low-precision training.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Semantic occupancy prediction provides fundamental voxel-level scene perception for autonomous driving systems, yet the massive number of voxels poses significant computational challenges, especially for Transformer-based methods with quadratic complexity. Recently, OccMamba introduces state space models to this task, but its reliance on a handcrafted 3D-to-1D reordering scheme suffers from two critical challenges: (1) indiscriminate processing of redundant empty voxels, and (2) limited adaptivity to diverse scene layouts. To address this issue, we propose the Mamba-driven Adaptive Reordering Scheme (MARS) framework, replacing the static reordering scheme with an adaptive and dynamic design, facilitating modality-aware pruning of redundant empty voxels and scene-adaptive sequence of critical voxels. Specifically, we first introduce the Adaptive Voxel Pruning (AVP) module to tackle indiscriminate processing, which filters out redundant empty voxels and retain informative ones, thereby establishing an efficient computational foundation. Then, we present the Dynamic Voxel Reordering (DVR) module to address limited adaptivity, which dynamically identifies and sequences critical voxels for scene-level perception, ensuring flexible adaptivity to diverse scenarios. Extensive experiments and analyses on the OpenOccupancy dataset showcase the effectiveness and efficiency of our MARS framework, achieving superior semantic occupancy performance while reducing training memory by 19.6% and accelerating inference by 9.7%.

## Keywords
Semantic occupancy prediction, state space model, adaptive voxel reordering
