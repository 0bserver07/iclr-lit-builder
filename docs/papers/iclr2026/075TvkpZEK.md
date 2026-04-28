# SMARAN: Closing the Generalization Gap with Performance Driven Optimization Method

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=075TvkpZEK](https://openreview.net/forum?id=075TvkpZEK)

## Relevance

**LLM score:** 1/3 — The paper proposes an optimizer that adjusts learning rate based on performance, which could offer memory savings over Adam, but the main focus is generalization, not energy-efficient training or hardware-aware computation.
**Keyword hits:** `adam`

## TLDR
(none provided)

## Abstract
Optimization methods have evolved significantly by introducing various learning rate scheduling techniques and adaptive learning strategies. Although these methods have achieved faster convergence, they often struggle to generalize well to unseen data compared to traditional approaches such as Stochastic Gradient Descent (SGD) with momentum. Adaptive methods such as Adam store each parameter's first and second moments of gradients, which can be memory-intensive. To address these challenges, we propose a novel SMARAN optimization method that adjusts the learning rate based on the model's performance rather than the objective function's curvature. This approach is particularly effective for minimizing stochastic loss functions, standard in deep learning models. Traditional gradient-based methods may get stuck in regions where the gradient vanishes, such as plateaus or local minima. Therefore, instead of only depending on the gradient, we use the model's performance to estimate the appropriate step size. We performed extensive experiments on standard vision benchmarks, and the generalization trends observed with SMARAN demonstrate compelling distinctions relative to adaptive and non-adaptive optimizers.

## Keywords
Optimization, Gradient decent, Learning rate scheduler, Regularization
