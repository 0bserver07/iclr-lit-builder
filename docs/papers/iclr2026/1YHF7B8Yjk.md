# Generalised Flow Maps for Few-Step Generative Modelling on Riemannian Manifolds

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1YHF7B8Yjk](https://openreview.net/forum?id=1YHF7B8Yjk)

## Relevance

**LLM score:** 1/3 — The paper aims to improve inference-time efficiency (few-step sampling) rather than training efficiency, making it only tangentially relevant to the Sutro Group's focus on energy-efficient training.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
Geometric data 
and purpose-built generative models on them have become ubiquitous in high-impact deep learning application domains, ranging from protein backbone generation and computational chemistry to geospatial data. 
Current geometric generative models remain computationally expensive at inference---requiring many steps of complex numerical simulation---as they are derived from dynamical measure transport frameworks such as diffusion and flow-matching on Riemannian manifolds. In this paper, we propose Generalised Flow Maps (GFM), a new class of few-step generative models that generalises the Flow Map framework in Euclidean spaces
to arbitrary Riemannian manifolds. We instantiate GFMs with three self-distillation-based training methods: Generalised Lagrangian Flow Maps, Generalised Eulerian Flow Maps, and Generalised Progressive Flow Maps. We theoretically show that GFMs, under specific design decisions, unify and elevate existing Euclidean few-step generative models, such as consistency models, shortcut models, and meanflows, to the Riemannian setting. We benchmark GFMs against other geometric generative models on a suite of geometric datasets, including geospatial data, RNA torsion angles, and hyperbolic manifolds, and   
achieve state-of-the-art sample quality for single- and few-step evaluations, and superior or competitive log-likelihoods using the implicit probability flow.

## Keywords
generative modelling, Riemannian geometry, few-step generative modelling
