# NoLoRA: Nonlinear Low-Rank Adaptation for Parameter-Efficient Fine-Tuning

**Venue:** iclr2026 (Withdraw)
**Authors:** Yongbin Liu
**OpenReview:** [https://openreview.net/forum?id=6vIc5PdqQV](https://openreview.net/forum?id=6vIc5PdqQV)

## Relevance

**LLM score:** 1/3 — The paper focuses on improving fine-tuning expressiveness via nonlinear low-rank adaptation, mentioning parameter efficiency tangentially, but does not directly advance energy-efficient training, sparsity, low-precision, or other Sutro Group priorities.
**Keyword hits:** `low-rank, lora`

## TLDR
(none provided)

## Abstract
Low-Rank Adaptation (LoRA) has been widely adopted for parameter-efficient fine-tuning of large language models, as it enables effective adaptation while maintaining efficiency. However, existing LoRA methods are fundamentally linear in nature, relying on the multiplication of two matrices (\textit{B×A}) for parameter adaptation. This inherently linear structure constrains their expressiveness, rendering them insufficient for capturing higher-order feature interactions and complex nonlinear patterns essential for advanced tasks. Consequently, this linearity becomes a bottleneck that limits further performance improvements. To address this limitation, we propose a nonlinear extension that introduces a learnable nonlinearity and a modulation mechanism into the low-rank adapter (Nonlinear Low-Rank Adaptation, NoLoRA), enhancing adaptability across diverse tasks. Our design preserves the parameter efficiency and scalability of LoRA while significantly improving representational capacity. Comprehensive experiments on four benchmarks, including commonsense reasoning, natural language understanding, image classification, and mathematical reasoning, demonstrate that our approach achieves consistent and substantial improvements over vanilla LoRA, LoRA's variant and other Parameter-efficient fine-tuning (PEFT) methods, with negligible additional computational overhead. These findings suggest that incorporating lightweight nonlinear structures into parameter-efficient fine-tuning frameworks offers a promising direction for improving the adaptability of large models.

## Keywords
Low-Rank Adaptation, Parameter-Efficient Fine-Tuning, Nonlinear
