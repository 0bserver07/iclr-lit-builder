# Conceptrol: Concept Control of Zero-shot Personalized Image Generation

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6hudf7aLUL](https://openreview.net/forum?id=6hudf7aLUL)

## Relevance

**LLM score:** 1/3 — Mentions no computational overhead but primarily focuses on personalized image generation control, not energy-efficient training or Sutro Group priorities.
**Keyword hits:** `lora`

## TLDR
(none provided)

## Abstract
Personalized image generation with text-to-image diffusion models generates unseen images based on reference image content. Zero-shot adapter methods such as IP-Adapter and OminiControl are especially interesting because they do not require test-time fine-tuning.  However, they struggle to balance preserving personalized content and adherence to the text prompt. We identify a critical design flaw resulting in this performance gap: current adapters inadequately integrate reference images with the textual descriptions. The generated images, therefore, tend to replicate the reference or misunderstand the personalized target. Yet the base text-to-image has strong conceptual understanding capabilities that can be leveraged. We propose Conceptrol, a simple yet effective framework that enhances zero-shot adapters without adding computational overhead. Conceptrol constrains the attention of visual specification with a textual concept mask that improves subject-driven generation capabilities. It achieves as much as 89\% improvement on personalization benchmarks over the vanilla IP-Adapter and can even outperform fine-tuning approaches such as Dreambooth LoRA.

## Keywords
text-to-image generation, diffusion model, subject-driven generation
