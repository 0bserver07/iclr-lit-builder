# BaNEL: Exploration Posteriors for Generative Modeling Using Only Negative Rewards

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=51oGbQmAr4](https://openreview.net/forum?id=51oGbQmAr4)

## Relevance

**LLM score:** 1/3 — The paper addresses efficiency in terms of reducing reward evaluations, which is tangential to Sutro Group's focus on energy-efficient training, data movement, sparsity, quantization, or hardware-aware methods.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
Today's generative models thrive with large amounts of supervised data and informative reward functions characterizing the quality of the generation. They work under the assumptions that the supervised data provides knowledge to pre-train the model, and the reward function provides dense information about how to further improve the generation quality and correctness. However, in the hardest instances of important problems, two problems arise: (1) the base generative model attains a near-zero reward signal, and (2) calls to the reward oracle are expensive. This setting poses a fundamentally different learning challenge than standard reward-based post-training. To address this, we propose BaNEL (Bayesian Negative Evidence Learning), an algorithm that post-trains the model using failed attempts only, while minimizing the number of reward evaluations (NREs). Our method is based on the idea that the problem of learning regularities underlying failures can be cast as another, in-loop generative modeling problem. We then leverage this model to assess whether new data resembles previously seen failures and steer the generation away from them. We show that our method can improve model performance without observing a single successful sample on several sparse-reward tasks, outperforming existing novelty-bonus approaches by up to several orders of magnitude in success rate, while using fewer reward evaluations.

## Keywords
reinforcement learning, learning from failure, generative modeling, large language models, sparse reward, exploration
