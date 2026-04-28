# DBLP: Noise Bridge Consistency Distillation For Efficient And Reliable Adversarial Purification

**Venue:** iclr2026 (Withdraw)
**Authors:** Chihan Huang, Belal Alsinglawi, Islam Al-Qudah
**OpenReview:** [https://openreview.net/forum?id=60RXHBGag4](https://openreview.net/forum?id=60RXHBGag4)

## Relevance

**LLM score:** 1/3 — Mentions fast inference via distillation, but the main contribution is adversarial purification not energy-efficient training or Sutro Group priorities like sparsity, quantization, or local learning.
**Keyword hits:** `distillation, lora`

## TLDR
(none provided)

## Abstract
Recent advances in deep neural networks (DNNs) have led to remarkable success across a wide range of tasks. However, their susceptibility to adversarial perturbations remains a critical vulnerability. Existing diffusion-based adversarial purification methods often require intensive iterative denoising, severely limiting their practical deployment. In this paper, we propose Diffusion Bridge Distillation for Purification (DBLP), a novel and efficient diffusion-based framework for adversarial purification. Central to our approach is a new objective, noise bridge distillation, which constructs a principled alignment between the adversarial noise distribution and the clean data distribution within a latent consistency model (LCM). To further enhance semantic fidelity, we introduce adaptive semantic enhancement, which fuses multi-scale pyramid edge maps as conditioning input to guide the purification process. Extensive experiments across multiple datasets demonstrate that DBLP achieves state-of-the-art (SOTA) robust accuracy, superior image quality, and around 0.2s inference time, marking a significant step toward real-time adversarial purification.

## Keywords
adversarial defense, latent consistency model, purification, lora
