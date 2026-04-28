# Self-Rewarding Rubric-Based Reinforcement Learning for Open-Ended Reasoning

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2x9Dat4PBO](https://openreview.net/forum?id=2x9Dat4PBO)

## Relevance

**LLM score:** 1/3 — The paper mentions faster and more resource-efficient training via a lightweight framework, but the main contribution is the RL-based self-rewarding method for reasoning, not efficiency-focused techniques like data movement, sparsity, or quantization.
**Keyword hits:** `efficient training`

## TLDR
(none provided)

## Abstract
Open-ended evaluation is essential for deploying large language models in real-world settings. In studying HealthBench, we observe that using the model itself as a grader and generating rubric-based reward signals substantially improves reasoning performance. Remarkably, the trained model also becomes a stronger grader. Motivated by this, we introduce Self-Rewarding Rubric-Based Reinforcement Learning for Open-Ended Reasoning, a lightweight framework that enables faster and more resource-efficient training while surpassing baselines. Remarkably, on Qwen3-32B, training with just the 4000-sample *HealthBench Easy* subset is sufficient to obtain a model that exceeds GPT-5 on *HealthBench Hard*. Incorporating a small amount of teacher-graded data further enhances performance for less capable models.

## Keywords
Reinforcement Learning, Large Language Models
