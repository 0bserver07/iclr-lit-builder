# Data-Efficient Training by Evolved Sampling

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=35yxQ6CuVT](https://openreview.net/forum?id=35yxQ6CuVT)

## Relevance

**LLM score:** 2/3 — The paper's main contribution is dynamic data selection for training acceleration, a form of training efficiency, but it does not directly address the Sutro Group's specific named priorities such as data movement, sparsity, quantization, or biologically-plausible learning.
**Keyword hits:** `efficient training, data-efficient, pruning`

## TLDR
(none provided)

## Abstract
Data selection is designed to accelerate learning with preserved performance. To achieve this, a fundamental thought is to identify informative data samples with significant contributions to the training. In this work, we propose **Evolved Sampling** (**ES**), a simple yet effective framework for *dynamic* sampling along the training process. This method conducts *batch* level data selection based on the dynamics of losses and augmented *loss differences*, which enables flexible *frequency tuning*, and hence significantly reduces the back propagation time with maintained model performance. Due to its conciseness, ES is also readily extensible to incorporate *set* level data selection (to form ES with pruning, **ESWP**) for further accelerations. As a plug-and-play framework, ES(WP) consistently achieves lossless training accelerations across various pre-training and post-training tasks, saving up to nearly 45\% wall-clock time. Our results motivate further investigations on the data efficiency aspect of modern large-scale machine learning.

## Keywords
dynamic data selection, data-efficiency, training acceleration, frequency analysis
