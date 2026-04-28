# LoRA Meets Second-Order Optimization: Towards Optimal Low-Rank Updates

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3IGUspVNtk](https://openreview.net/forum?id=3IGUspVNtk)

## Relevance

**LLM score:** 2/3 — Proposes a second-order optimizer for low-rank fine-tuning that improves convergence and reduces training overhead, directly addressing training efficiency which aligns with Sutro Group's interest in optimizers for energy-efficient training.
**Keyword hits:** `second-order, low-rank, shampoo, lora`

## TLDR
(none provided)

## Abstract
Low-rank fine-tuning is widely applied for the effective adaptation of large models. Most existing methods rely on low-rank matrix factorization, whose performance is limited by the condition number of the associated Jacobi operator. Although these methods are computationally efficient, their performance still falls short compared to full fine-tuning. To address this, we propose SoLoRA, which leverages an adaptive metric to find a low-rank approximation of the full fine-tuning gradient. This low-rank approximation can be viewed as an approximation of Hessian, effectively incorporating second-order information to achieve faster convergence and higher optimization efficiency. Furthermore, the low-rank approximation in SoLoRA is computationally simple and easy to implement, achieving a close approximation to the performance of full fine-tuning with almost no additional computational overhead. We conduct fine-tuning experiments on large language models and diffusion models, and the results consistently demonstrate that SoLoRA achieves superior performance advantages over state-of-the-art low-rank fine-tuning methods.

## Keywords
Fine-tuning, Low-rank matrix weights, Shampoo, Adaptive metric
