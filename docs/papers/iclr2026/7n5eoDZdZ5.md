# FLoRA-NA: Nearly Accurate Aggregation for Federated Low-Rank Adaptation

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7n5eoDZdZ5](https://openreview.net/forum?id=7n5eoDZdZ5)

## Relevance

**LLM score:** 1/3 — The paper addresses communication efficiency in federated learning, tangentially relevant to data movement, but its main focus is aggregation accuracy for LoRA, not core Sutro Group priorities like energy-efficient training, sparsity, or hardware-aware methods.
**Keyword hits:** `low-rank, lora`

## TLDR
(none provided)

## Abstract
With the rapid emergence of foundation models and the increasing need for fine-tuning across distributed environments, Federated Low-Rank Adaptation (FedLoRA) has recently gained significant attention. Despite its potential, current FedLoRA methods face notable challenges due to inexact updates. Existing approaches have attempted to mitigate this issue, but they often introduce a \emph{local-global generalization gap} and incur \emph{substantial communication overhead}, limiting their scalability and effectiveness.  
To address these limitations, we propose \textbf{F}ederated \textbf{Lo}w-\textbf{R}ank \textbf{A}ggregation with \textbf{N}early \textbf{A}ccurate Estimation (FLoRA-NA). FLoRA-NA leverages the local LoRA matrices on the server to estimate the aggregated matrices $\hat{A}$ and $\hat{B}$, which are then distributed to clients for local updates. This surrogated aggregated matrices minimizes the divergence between ideal $\bar{W} = \sum^{U}_{u=1}B_u A_u$ and practical updates $\hat{W} = \hat{B}\hat{A}$ without adding communication cost beyond vanilla FedLoRA. By doing so, FLoRA-NA achieves communication efficiency and bridges the gap between local personalization and global generalization, addressing a key limitation of prior personalized FedLoRA approaches.
We conduct extensive evaluations across diverse tasks, including natural language understanding, mathematical reasoning, and code-solving ability using various foundation models. Experimental results consistently demonstrate that FLoRA-NA achieves state-of-the-art performance while maintaining low communication overhead.

## Keywords
Federated Learning, Low-rank Adaptation, Data heterogeneity, language models
