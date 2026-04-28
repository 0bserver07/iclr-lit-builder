# LoRA-DA: Data-Aware Initialization for Low-Rank Adaptation via Asymptotic Analysis

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4nNqVpC3td](https://openreview.net/forum?id=4nNqVpC3td)

## Relevance

**LLM score:** 1/3 — The paper improves LoRA initialization to potentially reduce training steps, indirectly enhancing training efficiency, but efficiency is not the main contribution or explicitly addressed.
**Keyword hits:** `low-rank, lora`

## TLDR
(none provided)

## Abstract
With the widespread adoption of LLMs, LoRA has become a dominant method for PEFT, and its initialization methods have attracted increasing attention. However, existing methods have notable limitations: 
many methods do not incorporate target-domain data, while gradient-based methods exploit data only at a shallow level by relying on one-step gradient decomposition, 
which remains unsatisfactory due to the weak empirical performance of the one-step fine-tuning model that serves as their basis, as well as the fact that these methods either lack a rigorous theoretical foundation or depend heavily on restrictive isotropic assumptions.
In this paper, we establish a theoretical framework for data-aware LoRA initialization based on asymptotic analysis. Starting from a general optimization objective that minimizes the expectation of the parameter discrepancy between the fine-tuned and target models, we derive an optimization problem with two components: a bias term, which is related to the parameter distance between the fine-tuned and target models, and is approximated using a Fisher–gradient formulation to preserve anisotropy; and a variance term, which accounts for the uncertainty introduced by sampling stochasticity through the Fisher information.
By solving this problem, we obtain an optimal initialization strategy for LoRA.
Building on this theoretical framework, we develop an efficient algorithm, LoRA-DA, which estimates the terms in the optimization problem from a small set of target domain samples and obtains the optimal LoRA initialization. Empirical results across multiple benchmarks demonstrate that LoRA-DA consistently improves final accuracy over existing initialization methods. Additional studies show faster, more stable convergence, robustness across ranks, and only a small initialization overhead for LoRA-DA.
The source code will be released upon publication.

## Keywords
LoRA, Asymptotic Analysis, Initialization, Fisher information
