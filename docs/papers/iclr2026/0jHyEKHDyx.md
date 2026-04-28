# Why Low-Precision Transformer Training Fails: An Analysis on Flash Attention

**Venue:** iclr2026 (Oral)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0jHyEKHDyx](https://openreview.net/forum?id=0jHyEKHDyx)

## Relevance

**LLM score:** 3/3 — Directly addresses low-precision training instability and proposes a fix, aligning with Sutro Group's quantization and hardware-aware training priorities.
**Keyword hits:** `low-precision, low-rank`

## TLDR
(none provided)

## Abstract
The pursuit of computational efficiency has driven the adoption of low-precision formats for training transformer models. However, this progress is often hindered by notorious training instabilities. This paper provides the first mechanistic explanation for a long-standing and unresolved failure case where training with flash attention in low-precision settings leads to catastrophic loss explosions. Our in-depth analysis reveals that the failure is not a random artifact but caused by two intertwined phenomena: the emergence of similar low-rank representations within the attention mechanism and the compounding effect of biased rounding errors inherent in low-precision arithmetic. We demonstrate how these factors create a vicious cycle of error accumulation that corrupts weight updates, ultimately derailing the training dynamics. To validate our findings, we introduce a minimal modification to the flash attention that mitigates the bias in rounding errors. This simple change stabilizes the training process, confirming our analysis and offering a practical solution to this persistent problem. Code is available at https://anonymous.4open.science/r/why-low-precision-training-fails.

## Keywords
low-precision training, transformer, attention
