# TSDINO: Teacher–Student Self-Distillation Framework for Robust Pre-training of Time-Series Foundation Models

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1ndthBqbyK](https://openreview.net/forum?id=1ndthBqbyK)

## Relevance

**LLM score:** 1/3 — The paper uses self-distillation for pre-training but does not focus on energy efficiency or data movement, sparsity, quantization, or other Sutro Group priorities.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
Building time-series foundation models (TSFM) poses challenges in terms of learning stability due to limited data availability and heterogeneous temporal dynamics across various time-series datasets. We propose TSDINO, a teacher-student framework for robust pre-training of TSFM based on the principle of self-distillation with no labels. TSDINO offers a model-agnostic approach that combines two complementary objectives: (i) feature preservation under augmentations and (ii) masked patch prediction. A meta-architecture comprising teacher-student networks and projection heads enables adaptation to various models. We evaluate TSDINO on classification and forecasting tasks using diverse publicly available benchmarking datasets. TSDINO consistently achieves competitive zero-shot performance over gradient-based pre-training.

## Keywords
time series, self-distillation, time-series foundation models
