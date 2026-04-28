# Learning a Zeroth-Order Optimizer for Fine-Tuning LLMs

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2Dn4yHYLQJ](https://openreview.net/forum?id=2Dn4yHYLQJ)

## Relevance

**LLM score:** 2/3 — The paper proposes a learned zeroth-order optimizer to reduce memory consumption during LLM fine-tuning, which directly addresses training efficiency and optimizer design, both of which are central to the Sutro Group's interests.
**Keyword hits:** `optimizer`

## TLDR
(none provided)

## Abstract
Zeroth-order optimizers have recently emerged as a practical approach for fine-tuning large language models (LLMs), significantly reducing GPU memory consumption compared to traditional first-order methods. Yet, existing zeroth-order methods rely on hand-crafted, static sampling strategies that are not adaptable to model-specific structures. To address this, we propose ZO Fine-tuner, a learning-based zeroth-order optimizer for LLMs that automatically learns efficient perturbation strategies through a compact and memory-efficient design. Crucially, our approach is motivated by the observation that only a small number of foundation models and their derivatives are widely adopted in practice. Therefore, learning the optimizer once for a given LLM and reusing it across diverse downstream tasks is both feasible and highly desirable. Accordingly, ZO Fine-tuner is designed to scale learning to learn (L2L) to the foundation-model era by supporting one-time training per LLM with minimal overhead. Experiments on 4 LLMs and 7 datasets show that ZO Fine-tuner outperforms prior zeroth-order baselines in 82.1\% of task-model combinations, thereby demonstrating strong performance and scalability for efficient LLM fine-tuning.

## Keywords
Zeroth-order Optimization, Large Language Models
