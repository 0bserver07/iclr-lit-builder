# Pruning with Occam's Razor

**Venue:** iclr2026 (Desk Reject)
**Authors:** B.N. Kausik
**OpenReview:** [https://openreview.net/forum?id=0LKnVeXBGK](https://openreview.net/forum?id=0LKnVeXBGK)

## Relevance

**LLM score:** 3/3 — The paper directly advances energy-efficient training by integrating pruning with gradient descent to reduce model size and compute, aligning with sparsity and training efficiency priorities.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Deep learning neural network models must be large enough to adapt to their problem domain, while small enough to avoid overfitting training data during gradient descent.  To balance these competing demands, over-provisioned deep learning models such as transformers are trained for a single epoch on large data sets, and hence inefficient with both computing resources and training data.  In response to these inefficiencies, we derive a provably good algorithm that can combine any training and pruning methods to simultaneously optimize efficiency and accuracy,  identifying conditions that resist overfitting and reduce model size while outperforming the underlying training algorithm. We then use the algorithm to combine gradient descent with magnitude pruning into "Occam Gradient Descent." With respect to loss, compute and model size  (a) on image classification benchmarks, linear and convolutional neural networks trained with Occam Gradient Descent outperform traditional gradient descent with or without post-train pruning; (b) on a range of tabular data classification tasks, neural networks trained with Occam Gradient Descent outperform traditional gradient descent, as well as Random Forests; (c) on natural language transformers, Occam Gradient Descent outperforms traditional gradient descent.

## Keywords
Learning theory, occam's razor, pruning, gradient descent
