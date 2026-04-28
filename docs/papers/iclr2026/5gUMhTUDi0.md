# Sampling Complexity of TD and PPO in RKHS

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5gUMhTUDi0](https://openreview.net/forum?id=5gUMhTUDi0)

## Relevance

**LLM score:** 1/3 — The paper discusses sample efficiency but its main contribution is theoretical convergence analysis, not directly addressing energy-efficient training, data movement, sparsity, quantization, or local learning.
**Keyword hits:** `kernel`

## TLDR
(none provided)

## Abstract
We revisit Proximal Policy Optimization (PPO) from a function-space perspective. 
Our analysis decouples policy evaluation and improvement in a reproducing kernel Hilbert space (RKHS): 
(i)  A kernelized temporal-difference (TD) critic performs efficient RKHS-gradient updates using only one-step state–action transition samples.
(ii) a KL-regularized, natural-gradient policy step exponentiates the evaluated action-value, recovering a PPO/TRPO-style proximal update in continuous state-action spaces. 
We provide non-asymptotic, instance-adaptive guarantees whose rates depend on RKHS entropy, unifying tabular, linear, Sobolev, Gaussian, and Neural Tangent Kernel (NTK) regimes, and we derive a sampling rule for the proximal update that ensures the optimal $k^{-1/2}$  convergence rate for stochastic optimization.
Empirically, the theory-aligned schedule improves stability and sample efficiency on common control tasks (e.g., CartPole, Acrobot), while our TD-based critic attains favorable throughput versus a GAE baseline. 
Altogether, our results place PPO on a firmer theoretical footing beyond finite-dimensional assumptions and clarify when RKHS-proximal updates with kernel-TD critics yield global policy improvement with practical efficiency.

## Keywords
Kernel method, Kernel gradient descent, PPO, Temporal difference
