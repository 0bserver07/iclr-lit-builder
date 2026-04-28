# Dynamic Rank Adjustment for Accurate and Efficient Neural Network Training

**Venue:** iclr2026 (Withdraw)
**Authors:** Hyuntak Shin, Aecheon Jung, Sungeun Hong, Sunwoo Lee
**OpenReview:** [https://openreview.net/forum?id=54BPFBsT2p](https://openreview.net/forum?id=54BPFBsT2p)

## Relevance

**LLM score:** 3/3 — Directly advances energy-efficient training by reducing computational cost through low-rank training with dynamic rank adjustments, aligning with data movement and efficiency priorities.
**Keyword hits:** `low-rank`

## TLDR
(none provided)

## Abstract
Low-rank training is a primary strategy for efficient deep learning, but it presents a fundamental challenge. It reduces computational cost, yet it permanently caps a model’s representational capacity and accelerates the rank collapse that diminishes its expressive power during training. We address this with dynamic-rank training, a framework built on the intuition that a model can temporarily escape its low-rank constraints to restore its full learning potential. Our approach strategically interleaves full-rank epochs within a low-rank schedule, with the timing of these restorative phases aligned with the learning rate’s noise regimes to maximize their effect. This enables the model to regain expressive power at critical stages of training by restoring the effective rank of its weights. Our extensive evaluations across various computer vision and natural language processing benchmarks show this method achieves the accuracy of full-rank models while retaining the computational advantages of low-rank training.

## Keywords
Low-rank training, Rank adjustment, model reparameterization
