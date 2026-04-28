# FitLight: Federated Imitation Learning for Plug-and-Play Autonomous Traffic Signal Control

**Venue:** iclr2026 (Withdraw)
**Authors:** Yutong Ye, Yingbo Zhou, Xiao Du, Zhusen Liu, Hao Zhou, Li Sun, Xiang Lian, Mingsong Chen
**OpenReview:** [https://openreview.net/forum?id=0XiGLcOpLK](https://openreview.net/forum?id=0XiGLcOpLK)

## Relevance

**LLM score:** 1/3 — Mentions model pruning for resource-constrained deployment, but the main contribution is federated imitation learning for traffic signal control, not advances in energy-efficient training or hardware-aware training methods.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Although Reinforcement Learning (RL)-based Traffic Signal Control (TSC) methods have been extensively studied, their practical applications still raise some serious issues such as high learning cost and poor generalizability. This is because the ``trial-and-error'' training style makes RL agents extremely dependent on the specific traffic environment, which also requires a long convergence time. To address these issues, we propose a novel Federated Imitation Learning (FIL)-based framework for multi-intersection TSC, named FitLight, which allows RL agents to plug-and-play for any traffic environment without additional pre-training cost. Unlike existing imitation learning approaches that rely on pre-training RL agents with demonstrations, FitLight allows real-time imitation learning and seamless transition to reinforcement learning. Due to our proposed knowledge-sharing mechanism and novel hybrid pressure-based agent design, RL agents can quickly find a best control policy with only a few episodes. Moreover, for resource-constrained TSC scenarios, FitLight supports model pruning and heterogeneous model aggregation, such that RL agents can work on a micro-controller with merely 16{\it KB} RAM and 32{\it KB} ROM. Extensive experiments demonstrate that, compared to state-of-the-art methods, FitLight not only provides a superior starting point but also converges to a better final solution on both real-world and synthetic datasets, even under extreme resource limitations.

## Keywords
Autonomous System, Traffic Signal Control, Federated Imitation Learning
