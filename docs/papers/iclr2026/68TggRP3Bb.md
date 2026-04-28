# Scaling Law for Catastrophic Forgetting via Gradient Products

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=68TggRP3Bb](https://openreview.net/forum?id=68TggRP3Bb)

## Relevance

**LLM score:** 1/3 — The paper studies scaling laws for catastrophic forgetting, which is tangentially related to the group's interest in scaling laws but does not address energy-efficient training, data movement, sparsity, or other core priorities.
**Keyword hits:** `scaling law`

## TLDR
(none provided)

## Abstract
Catastrophic forgetting occurs when models lose performance on previously learned tasks after acquiring new ones. Although larger models are empirically observed to forget less, the theoretical origin of this effect remains unclear. In this work, we analyze forgetting in simple linear and nonlinear teacher-student models and introduce a gradient-product proxy that closely tracks forgetting. This formulation allows us to decompose the phenomenon into its main components. We show that the orthogonality of the output heads is the necessary condition underlying the $1/d$ scaling law of forgetting, where $d$ is the hidden dimension. Other factors, such as initialization, task similarity, network architecture, and activation functions, play a secondary role, modulating but not overturning the dominant scaling behavior. Our results provide a step toward a principled understanding of how model capacity mitigates forgetting and clarify the role of gradient interference in continual learning.

## Keywords
Catastrophic Forgetting
