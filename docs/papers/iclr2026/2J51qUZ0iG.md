# Fantastic Pretraining Optimizers and Where to Find Them

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2J51qUZ0iG](https://openreview.net/forum?id=2J51qUZ0iG)

## Relevance

**LLM score:** 3/3 — The paper directly evaluates optimizers for pretraining efficiency, a named Sutro Group priority, aiming to identify real speedups that reduce training time and thus energy consumption.
**Keyword hits:** `chinchilla, optimizer, posit, adamw, muon`

## TLDR
(none provided)

## Abstract
AdamW has long been the dominant optimizer in language model pretraining, despite numerous claims that alternative optimizers offer 1.4 to 2$\times$ speedup. We posit that two methodological shortcomings have obscured fair comparisons and hindered practical adoption: (i) unequal hyperparameter tuning and (ii) limited or misleading evaluation setups.
To address these two issues, we conduct a systematic study of ten deep learning optimizers across four model scales (0.1B–1.2B parameters) and data-to-model ratios (1--8$\times$ the Chinchilla optimum). We find that fair and informative comparisons require rigorous hyperparameter tuning and evaluations across a range of model scales and data-to-model ratios, performed at the end of training.
First, optimal hyperparameters for one optimizer may be suboptimal for another, making blind hyperparameter transfer unfair. 
Second, the actual speedup of many proposed optimizers over well-tuned baselines is lower than claimed and decreases with model size to only 1.1$\times$ for 1.2B parameter models. Thirdly, comparing intermediate checkpoints before reaching the target training budgets can be misleading, as rankings between two optimizers can flip during training due to learning rate decay.
Through our thorough investigation, we find that all the fastest optimizers such as Muon and Soap, use matrices as preconditioners --- multiplying gradients with matrices rather than entry-wise scalars. However, the speedup of matrix-based optimizers is inversely proportional to model scale, decreasing from 1.4$\times$ over AdamW for 0.1B parameter models to merely 1.1$\times$ for 1.2B parameter models.

## Keywords
optimizer, benchmarking, pretrain
