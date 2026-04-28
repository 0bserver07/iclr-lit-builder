# Scalable Variational Bayesian Fine-Tuning of LLMs via Orthogonalized Low-Rank Adapter

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1VCu7aFQzk](https://openreview.net/forum?id=1VCu7aFQzk)

## Relevance

**LLM score:** 1/3 — The paper uses parameter-efficient fine-tuning (LoRA variant) but its main contribution is uncertainty quantification via Bayesian methods, with no direct focus on energy-efficient training, data movement, sparsity, low-precision, or other Sutro Group priorities.
**Keyword hits:** `low-rank, lora`

## TLDR
(none provided)

## Abstract
When deploying large language models (LLMs) to safety-critical applications, uncertainty quantification (UQ) is of utmost importance to self-assess the reliability of the LLM-based decisions. However, such decisions typically suffer from overconfidence, particularly after parameter-efficient fine-tuning (PEFT) for downstream domain-specific tasks with limited data.
To address these limitations,  we build on the Bayesian last layer (BLL) model, where the LLM-based ${\it deterministic}$ feature extractor is followed by random LL parameters for uncertainty reasoning. 
Since existing low-rank adapters (LoRA) for PEFT have limited expressiveness due to rank collapse, we address this with Polar-decomposed Low-rank Adapter Representation (PoLAR), an orthogonalized parameterization paired with Riemannian optimization to enable more stable and expressive adaptation.
The resulting PoLAR-VBLL is a flexible framework that nicely integrates architecture-enhanced optimization with scalable Bayesian inference to endow LLMs with well-calibrated UQ.
Our empirical results verify the effectiveness of PoLAR-VBLL in terms of generalization and uncertainty estimation on both in-distribution and out-of-distribution data for various common-sense reasoning tasks.

## Keywords
Uncertainty Quantification, Bayesian Neural Network, Bayesian last layer, Large Language Models, Parameter-Efficient Fine-Tuning, Orthogonal Parametrization
