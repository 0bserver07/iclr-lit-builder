# TiTok: Transfer Token-level Knowledge via Contrastive Excess to Transplant LoRA

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0B5K9pIdSK](https://openreview.net/forum?id=0B5K9pIdSK)

## Relevance

**LLM score:** 1/3 — The paper reduces overhead by avoiding a discriminator, but its main focus is knowledge transfer for LoRA transplantation, not core energy-efficient training priorities like data movement, sparsity, or low precision.
**Keyword hits:** `knowledge distillation, distillation, lora`

## TLDR
(none provided)

## Abstract
Large Language Models (LLMs) are widely applied in real world scenarios, but fine-tuning them comes with significant computational and storage costs. Parameter-Efficient Fine-Tuning (PEFT) methods such as LoRA mitigate these costs, but the adapted parameters are dependent on the base model and cannot be transferred across different backbones. One way to address this issue is through knowledge distillation, but its effectiveness inherently depends on training data. Recent work such as TransLoRA avoids this by generating synthetic data, but this adds complexity because it requires training an additional discriminator model. In this paper, we propose TiTok, a new framework that enables effective LoRA Transplantation through Token-level knowledge transfer. Specifically, TiTok captures task-relevant information through a token-wise contrastive excess between a source model with and without LoRA. This excess highlights informative tokens and enables selective filtering of synthetic data, all without additional models or overhead. Through experiments on three benchmarks across multiple transfer settings, our experiments show that TiTok is consistently effective, achieving average performance gains of +4–8% compared to baselines overall.

## Keywords
Large Language Models, Knowledge Transfer, PEFT
