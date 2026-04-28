# Boomerang Distillation Enables Zero-Shot Model Size Interpolation

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4ZU8v4s3IR](https://openreview.net/forum?id=4ZU8v4s3IR)

## Relevance

**LLM score:** 2/3 — The paper's main contribution is a distillation method that reduces training cost by interpolating model sizes, directly making efficiency a primary contribution.
**Keyword hits:** `knowledge distillation, distillation, pruning`

## TLDR
(none provided)

## Abstract
Large language models (LLMs) are typically deployed under diverse memory and compute constraints. Existing approaches build model families by training each size independently, which is prohibitively expensive and provides only coarse-grained size options. In this work, we identify a novel phenomenon that we call boomerang distillation: starting from a large base model (the teacher), one first distills down to a small student and then progressively reconstructs intermediate-sized models by re-incorporating blocks of teacher layers into the student without any additional training. This process produces zero-shot interpolated models of many intermediate sizes whose performance scales smoothly between the student and teacher, often matching or surpassing pretrained or distilled models of the same size. We further analyze when this type of interpolation succeeds, showing that alignment between teacher and student through pruning and distillation is essential. Boomerang distillation thus provides a simple and efficient way to generate fine-grained model families, dramatically reducing training cost while enabling flexible adaptation across deployment environments.

## Keywords
knowledge distillation, pretraining, adaptive compute, model interpolation
