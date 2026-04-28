# Stabilizing MoE Reinforcement Learning by Aligning Training and Inference Routers

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6LORvHYkV3](https://openreview.net/forum?id=6LORvHYkV3)

## Relevance

**LLM score:** 1/3 — The paper focuses on stabilizing RL training in MoE models by aligning routers, mentioning training speed only as a side benefit, not advancing energy-efficient training or Sutro Group's core efficiency priorities.
**Keyword hits:** `mixture of experts, moe`

## TLDR
(none provided)

## Abstract
Reinforcement learning (RL) has emerged as a crucial approach for enhancing the capabilities of large language models. However, in Mixture-of-Experts (MoE) models, the routing mechanism often introduces instability, even leading to catastrophic RL training collapse. We analyze the training-inference consistency of MoE models and identify a notable discrepancy in routing behaviors between the two phases. Moreover, even under identical conditions, the routing framework can yield divergent expert selections across repeated forward passes. To address this foundational inconsistency, we propose Rollout Routing Replay (R3), a method that records routing distributions from the inference engine and replays them during training. R3 significantly reduces training-inference policy KL divergence and mitigates extreme discrepancies without compromising training speed. Extensive experiments on various settings confirm that R3 succeeds in stabilizing RL training, preventing collapse and outperforming methods such as GSPO and TIS. We believe this work can offer a new solution for stabilizing RL in MoE models.

## Keywords
Mixture of Experts, Large Language Models, Reinforcement Learning
