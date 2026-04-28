# Training-Free Determination of Network Width via Neural Tangent Kernel

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0elvad3gEu](https://openreview.net/forum?id=0elvad3gEu)

## Relevance

**LLM score:** 1/3 — The paper addresses efficient model sizing to avoid overparameterization, which indirectly reduces training compute, but does not directly advance energy-efficient training techniques.
**Keyword hits:** `kernel`

## TLDR
(none provided)

## Abstract
Determining an appropriate size for an artificial neural network under computational constraints is a fundamental challenge. This paper introduces a practical metric, derived from Neural Tangent Kernel (NTK), for estimating the minimum necessary network width with respect to test loss -- prior to training. We provide both theoretical and empirical evidence that the smallest eigenvalue of the NTK strongly influences test loss in wide but finite-width neural networks. Based on this observation, we define an NTK-based metric computed at initialization to identify what we call cardinal width, i.e., the width of a network at which generalization performance saturates. Our experiments across multiple datasets and architectures demonstrate the effectiveness of this metric in estimating the cardinal width.

## Keywords
neural tangent kernel, kernel regression, smallest eigenvalue, generalization error
