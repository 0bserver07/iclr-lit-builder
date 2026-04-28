# Asymmetric Proximal Policy Optimization: mini-critics boost LLM reasoning

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0vgzrcv4Dr](https://openreview.net/forum?id=0vgzrcv4Dr)

## Relevance

**LLM score:** 1/3 — The paper mentions computational efficiency of critic training as a motivation for using lightweight mini-critics, but the main contribution is algorithmic improvement in RL for LLM reasoning, not a direct advancement in energy-efficient training or the Sutro Group's core priorities.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
Reinforcement learning (RL) has become a central paradigm for post-training large language models (LLMs) to elicit stronger reasoning. Yet, most recent RL for LLMs (RL4LLM) methods avoid explicit critics, replacing them with average advantage baselines. This shift is largely pragmatic: conventional value functions are computationally expensive to train at LLM scale and often fail under sparse rewards and long reasoning horizons. We revisit this bottleneck from an architectural perspective and introduce Asymmetric Proximal Policy Optimization (**AsyPPO**), a simple and scalable framework that restores the critic’s role while remaining efficient in large-model settings. **AsyPPO** employs a set of lightweight *mini-critics*, each trained on disjoint prompt shards. This design encourages diversity while preserving calibration, reducing value-estimation bias. Beyond robust estimation, **AsyPPO** leverages inter-critic uncertainty to refine the policy update: (i) masking advantages in states where critics agree and gradients add little learning signal, and (ii) filtering high-divergence states from entropy regularization, suppressing spurious exploration. Across multiple reasoning benchmarks, **AsyPPO** consistently improves learning stability and performance over strong baselines, e.g., GRPO, achieving performance gains of $> 6$% on *Qwen3-4b-Base* and about $3$% on *Qwen3-8b-Base* and *Qwen3-14b-Base* over classic PPO. Such results highlight the importance of architectural innovations in critics for scalable, efficient algorithms.

## Keywords
Reinforcement Learning, Large Language Model, Math Reasoning
