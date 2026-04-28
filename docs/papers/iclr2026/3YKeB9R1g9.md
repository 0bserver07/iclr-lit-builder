# Scaling with Collapse: Efficient and Predictable Training of LLM Families

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3YKeB9R1g9](https://openreview.net/forum?id=3YKeB9R1g9)

## Relevance

**LLM score:** 3/3 — Directly advances compute-efficient training and scaling laws, a named Sutro priority, by showing loss curve collapse enables predictable, efficient LLM training and hyperparameter tuning, reducing energy and compute waste.
**Keyword hits:** `efficient training, compute-efficient, adamw`

## TLDR
(none provided)

## Abstract
Effective LLM training relies on *consistency*, meaning that key quantities—such as final losses and optimal hyperparameters—scale predictably across model sizes. Qiu et al. (2025) recently showed that this consistency extends beyond scalars: whole training loss curves can *collapse* onto a universal trajectory after a simple normalization. What remains unclear is whether this phenomenon holds for LLM families trained under *practical scaling recipes*, where width, depth, learning rate, batch size, and weight decay are scaled jointly. We show that it does: loss curves collapse across scales precisely when optimization hyperparameters are set optimally for the given data budget, in accordance with recent empirical scaling laws. Collapse thus emerges as a signature of compute-efficient training. We demonstrate two applications at scale: (1) deviation-from-collapse provides a sensitive, early diagnostic of training pathologies, and (2) the predictability of collapsed curves enables early stopping in large-scale hyperparameter tuning. Finally, we train a competitive LLM family, *Celerity*, using these insights, highlighting collapse as an effective tool for developing efficient LLMs.

## Keywords
Training loss curve collapse, Compute-efficient LLM pre-training, Tokens-per-parameter (TPP), AdamW EMA timescale, Learning-rate schedules, Scale-stable dynamics (μP), Early stopping for hyperparameter tuning
