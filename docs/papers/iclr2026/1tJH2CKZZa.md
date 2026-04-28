# Think Twice, Act Once: Token-Aware Compression and Action Reuse for Efficient Inference in Vision-Language-Action Models

**Venue:** iclr2026 (Withdraw)
**Authors:** Xudong Tan, Yaoxin Yang, Peng Ye, Jialin Zheng, Bizhe Bai, Xinyi Wang, Jia Hao, Tao Chen
**OpenReview:** [https://openreview.net/forum?id=1tJH2CKZZa](https://openreview.net/forum?id=1tJH2CKZZa)

## Relevance

**LLM score:** 1/3 — Addresses inference efficiency via token pruning and action reuse, not training efficiency or any Sutro Group training-focused priority.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
Vision-Language-Action (VLA) models have emerged as a powerful paradigm for robot control through natural language instructions. However, their high inference cost—stemming from large-scale token computation and autoregressive decoding—poses significant challenges for real-time deployment and edge applications. While prior work has primarily focused on efficient architectural optimization, we take a different and innovative perspective by identifying a dual form of redundancy in VLA models: (i) high similarity across consecutive action steps, and (ii) substantial redundancy in visual tokens.
Motivated by these observations, we propose FlashVLA, the first training-free and plug-and-play acceleration framework that enables action reuse in VLA models. Specifically, FlashVLA improves inference efficiency through a token-aware action reuse mechanism that avoids redundant decoding across stable action steps, and an information-guided visual token selection strategy that prunes low-contribution tokens.
Extensive experiments on the LIBERO benchmark show that FlashVLA reduces FLOPs by 55.7% and latency by 36.0%, with only a 0.7% drop in task success rate. These results demonstrate the effectiveness of FlashVLA in enabling lightweight, low-latency VLA inference without retraining.

## Keywords
Vision-Language-Action Models, Model Acceleration
