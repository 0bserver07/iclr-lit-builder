# Unveiling the Scaling Law of PINNs under Non-Euclidean Geometry

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7NS4qtPM2Q](https://openreview.net/forum?id=7NS4qtPM2Q)

## Relevance

**LLM score:** 1/3 — The paper addresses optimization scaling challenges for PINNs, which tangentially relates to training efficiency, but does not focus on energy, data movement, sparsity, quantization, local learning, or hardware-aware methods as a main contribution.
**Keyword hits:** `scaling law, muon`

## TLDR
(none provided)

## Abstract
Physics-informed neural networks (PINNs) have emerged as a powerful framework for solving partial differential equations (PDEs) by embedding physical laws into the training process. In theory, PINNs admit optimal polynomial convergence rates in approximation and generalization. However, these results rely on the unrealistic assumption of global optimization, which is intractable in practice. Consequently, scaling PINNs to large architectures remains a major challenge, as network width increases and thereby the condition number of the underlying optimization problem grows rapidly, making training increasingly difficult and creating a fundamental bottleneck.
In this work, inspired by the MUON framework, we propose a descent strategy that adapts to the geometry of the optimization landscape. The new optimization algorithm does not degrade as the network size increases. As a result, we establish—for the first time—a scaling law for PINNs that predicts how performance improves systematically with model size. Using this framework, we successfully trained a PINN with more than 1,000 neurons per layer, surpassing the previous state-of-the-art limit of 200–400. This scaling perspective bridges the gap between theoretical guarantees and practical optimization, opening the door to pushing PINNs toward machine precision at unprecedented scales.

## Keywords
PINN, Optimization
