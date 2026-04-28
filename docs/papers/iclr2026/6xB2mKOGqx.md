# Routing-Deconstructed LoRA in Federated Fine-Tuning

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=6xB2mKOGqx](https://openreview.net/forum?id=6xB2mKOGqx)

## Relevance

**LLM score:** 1/3 — Paper focuses on federated LoRA with a secondary mention of reducing communication cost via alternating freezing, but the main contribution is handling heterogeneity in FL, not energy-efficient training, data movement, sparsity, quantization, or other Sutro Group priorities.
**Keyword hits:** `lora`

## TLDR
(none provided)

## Abstract
The integration of Large Language Models (LLMs) with Federated Learning (FL) offers a promising approach to privacy-preserving Parameter-Efficient Fine-Tuning (PEFT). However, resource and data heterogeneity in FL cause differences in local knowledge distribution across clients. As a representative PEFT approach, LoRA still faces three key challenges in such settings: aggregation noise, knowledge contamination, and aggregation distortion. To address these issues, we propose Routing-Deconstructed LoRA (RD-LoRA). Building on an alternating freezing strategy to mitigate aggregation noise and concurrently reduces communication cost, RD-LoRA further introduces two novel components. For knowledge contamination, we design a Server-Client Routing Deconstructor (SCRD) that separates shared semantics from local biases, retaining fine-grained knowledge with semantic consistency. To address aggregation distortion, we propose a Poly-Consensus Aggregation (PCA) mechanism that uses adaptive weighted averaging to align global LoRA parameters with heterogeneous client distributions, thus correcting the global update direction. Extensive experiments demonstrate that RD-LoRA is effective and robust in both homogeneous and heterogeneous settings.

## Keywords
LLMs, Parameter-Efficient Fine-Tuning, Federated Learning, LoRA, Resource Heterogeneous
