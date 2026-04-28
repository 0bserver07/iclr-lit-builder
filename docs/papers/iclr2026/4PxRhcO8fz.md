# Simple yet Effective Semi-supervised Knowledge Distillation from Vision-Language Models via Dual-Head Optimization

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4PxRhcO8fz](https://openreview.net/forum?id=4PxRhcO8fz)

## Relevance

**LLM score:** 1/3 — Mentions distillation and minimal overhead, but the main contribution is accuracy improvement in semi-supervised transfer, not energy-efficient training or the other efficiency-focused priorities.
**Keyword hits:** `knowledge distillation, distillation`

## TLDR
(none provided)

## Abstract
Semi-supervised learning (SSL) has emerged as a practical solution for addressing data scarcity challenges by leveraging unlabeled data. Recently, vision-language models (VLMs), pre-trained on massive image-text pairs, have demonstrated remarkable zero-/few-shot performance that often surpasses SSL approaches due to their exceptional generalization capabilities. This gap motivates us to question: how can we effectively harness the powerful generalization capabilities of VLMs into task-specific models? Knowledge distillation (KD) offers a natural framework for transferring VLM capabilities, but we identify that it suffers from gradient conflicts between supervised and distillation losses. To address this challenge, we propose Dual-Head Optimization (DHO), which introduces dual prediction heads for each distinct signal. We observe that DHO resolves gradient conflicts, enabling improved feature learning compared to single-head KD baselines, with practical benefits of minimal computational overhead and test-time hyperparameter tuning without retraining. Extensive experiments across 15 datasets show that DHO consistently outperforms KD baselines, often outperforming teacher models with smaller student models. DHO also achieves new state-of-the-art performance on both in-distribution ImageNet semi-supervised learning and out-of-distribution generalization across ImageNet variants. We will publicly release our code and model checkpoints to facilitate future research.

## Keywords
knowledge distillation, vision-langage model, zero/few-shot distillation, semi-supervised learning
