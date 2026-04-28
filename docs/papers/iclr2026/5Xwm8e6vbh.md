# Are EEG Foundation Models Worth It? Comparative Evaluation with Traditional Decoders in Diverse BCI Tasks

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=5Xwm8e6vbh](https://openreview.net/forum?id=5Xwm8e6vbh)

## Relevance

**LLM score:** 1/3 — Mentions scaling laws tangentially but primarily benchmarks EEG foundation models, not advancing Sutro Group's core energy-efficient training, sparsity, low-precision, or data movement priorities.
**Keyword hits:** `scaling law`

## TLDR
(none provided)

## Abstract
Foundation models have recently emerged as a promising approach for learning generalizable EEG representations for brain–computer interfaces (BCIs). Yet, their true advantages over traditional methods—particularly classical non-neural approaches—remain unclear. In this work, we present a comprehensive benchmark of state-of-the-art EEG foundation models, evaluated across diverse datasets, decoding tasks, and six evaluation protocols, with rigorous statistical testing. We introduce spatiotemporal EEGFormer (ST-EEGFormer), a simple yet effective Vision Transformer (ViT)-based baseline, pre-trained solely with masked autoencoding (MAE) on over 8M EEG segments. Our results show that while fine-tuned foundation models perform well in data-rich, population-level settings, they often fail to significantly outperform compact neural networks or even classical non-neural decoders in data-scarce scenarios. Furthermore, linear probing remains consistently weak, and performance varies greatly across downstream tasks, with no clear scaling law observed among neural network decoders. These findings expose a substantial gap between pre-training and downstream fine-tuning, often diminishing the benefits of complex pre-training tasks. We further identify hidden architectural factors that affect performance and emphasize the need for transparent, statistically rigorous evaluation. Overall, this study calls for community-wide efforts to construct large-scale EEG datasets and for fair, reproducible benchmarks to advance EEG foundation models.

## Keywords
Foundation Model, Brain–Computer Interface, EEG, Benchmark
