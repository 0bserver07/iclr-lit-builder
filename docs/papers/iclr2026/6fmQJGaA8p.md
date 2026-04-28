# Beyond Benchmarks: Understanding Mixture-of-Experts Models through Internal Mechanisms

**Venue:** iclr2026 (Withdraw)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6fmQJGaA8p](https://openreview.net/forum?id=6fmQJGaA8p)

## Relevance

**LLM score:** 1/3 — Paper analyzes sparsity and expert utilization in MoE models, tangential to energy-efficient training but not its main contribution.
**Keyword hits:** `moe`

## TLDR
(none provided)

## Abstract
Mixture-of-Experts (MoE) architectures have emerged as a promising direction, offering efficiency and scalability by activating only a subset of parameters during inference. However, current research remains largely performance-centric, with limited understanding of its internal mechanisms, thereby constraining broader progress. In this work, we use an internal metric to investigate the mechanisms of MoE architecture by explicitly incorporating routing mechanisms and analyzing expert-level behaviors. Through systematic analyses of a wide range of publicly available MoE models, we uncover several findings: (1) neuron utilization decreases as models evolve, reflecting stronger generalization; (2) training exhibits a dynamic trajectory, where benchmark performance alone provides limited signal while MUI reveals deeper insights; (3) task completion emerges from collaborative contributions of multiple experts, with shared experts driving concentration; and (4) activation patterns at the neuron level provide a fine-grained proxy for data diversity. Together, these results demonstrate the potential of MUI as a complementary indicator to benchmark performance, offering new insights into the capacity, dynamics, and specialization of MoE models.

## Keywords
LLMs, evaluation, MoE, intepretation
