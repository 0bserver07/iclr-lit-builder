# Spectral-Aware Sparse Communication and Entropy-Balanced Tasking in Multi-Agent Systems

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4br3ZhwhIG](https://openreview.net/forum?id=4br3ZhwhIG)

## Relevance

**LLM score:** 1/3 — The paper addresses communication sparsification and energy reduction in multi-agent coordination, not training efficiency of a single model; the efficiency angle is tangential to the group's focus on training-centric methods.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
Multi-agent systems (MAS) face scalability constraints stemming from dense messaging—raising bandwidth and energy—and from imbalanced tasking that produces bottlenecks, especially under non-stationary, LLM-driven workloads. We introduce a unified framework that prunes redundant links using an information-theoretic priority and enforces connectivity via a spectral $\lambda_2$ guard, and balances workload with an entropy-regularized assignment under capacity constraints; an MDP allocator adapts thresholds and repairs to system drift. We prove that the $\lambda_2$-guarded repair preserves connectivity and, under standard spectral envelope assumptions, the sparsified graph approximates dense-graph dynamics; we analyze discrete-time stability via Jury/Nyquist bounds. Across GSM8K, MMLU, and SMACv2, the method improves over a dense complete-graph baseline by +6.12\%/+5.59\%/+4.76\%, reduces active links by 28\%, and shows the strongest robustness under 30\% edge drops -- all while keeping per-iteration communication proportional to the number of active edges. These results indicate a practical route to communication-efficient, entropy-balanced coordination for LLM-augmented MAS and cooperative control.

## Keywords
Multi-Agent Systems, Reinforcement Learning, LLM Agents, Spectral Sparsification, Algebraic Connectivity, Mutual Information, Entropy-Regularized Assignment, Graph Laplacian
