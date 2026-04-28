# EAST: Early Action Prediction Sampling Strategy with Token Masking

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3Genv8DQgf](https://openreview.net/forum?id=3Genv8DQgf)

## Relevance

**LLM score:** 2/3 — Token masking procedure cuts memory usage and accelerates training, making training efficiency a main contribution, directly relevant to energy-efficient AI training.
**Keyword hits:** `efficient training`

## TLDR
(none provided)

## Abstract
Early action prediction seeks to anticipate an action before it fully unfolds, but limited visual evidence makes this task especially challenging. We introduce EAST, a simple and efficient framework that enables a model to reason about incomplete observations. In our empirical study, we identify key components when training early action prediction models. Our key contribution is a randomized training strategy that samples a time step separating observed and unobserved video frames, enabling a single model to generalize seamlessly across all test-time observation ratios. We further show that joint learning on both observed and future (oracle) representations significantly boosts performance, even allowing an encoder-only model to excel. To improve scalability, we propose a token masking procedure that cuts memory usage in half and accelerates training by 2× with no accuracy loss. Combined with a forecasting decoder, EAST sets a new state of the art on NTU60, SSv2, and UCF101, surpassing previous best work by 10.1, 7.7, and 3.9 percentage points, respectively. We support future research by releasing efficient training implementations and pre-trained models.

## Keywords
early action prediction, token masking, video analysis, efficient training
