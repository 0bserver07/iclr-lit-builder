# A Learn-to-Optimize Approach for Coordinate-Wise Step Sizes for Quasi-Newton Methods

**Venue:** iclr2026 (Withdraw)
**Authors:** Wei Lin, Qingyu Song, Hong Xu
**OpenReview:** [https://openreview.net/forum?id=6iYVv72Pk6](https://openreview.net/forum?id=6iYVv72Pk6)

## Relevance

**LLM score:** 1/3 — The paper improves optimizer step sizes for faster convergence, indirectly reducing training time and energy, but does not directly address the group's core focus areas like data movement, sparsity, low precision, or local learning.
**Keyword hits:** `second-order`

## TLDR
(none provided)

## Abstract
Tuning step sizes is crucial for the stability and efficiency of optimization algorithms. While adaptive coordinate-wise step sizes have been shown to outperform scalar step size in first-order methods, their use in second-order methods is still under-explored and more challenging. Current approaches, including hypergradient descent and cutting plane methods, offer limited improvements or encounter difficulties in second-order contexts. To address these limitations, we first conduct a theoretical analysis within the Broyden-Fletcher-Goldfarb-Shanno (BFGS) framework, a prominent quasi-Newton method, and derive sufficient conditions for coordinate-wise step sizes that ensure convergence and stability. Building on this theoretical foundation, we introduce a novel learn-to-optimize (L2O) method that employs LSTM-based networks to learn optimal step sizes by leveraging insights from past optimization trajectories, while inherently respecting the derived theoretical guarantees. Extensive experiments demonstrate that our approach achieves substantial improvements over scalar step size methods and hypergradient descent-based method, offering up to 4$\times$ faster convergence across diverse optimization tasks.

## Keywords
Learning to Optimize, Quasi-Newton Method
