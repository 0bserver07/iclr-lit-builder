# Mechanistic Interpretability of In-Context Learning Generalization through Structured Task Curriculum

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2Fv4GxUElU](https://openreview.net/forum?id=2Fv4GxUElU)

## Relevance

**LLM score:** 1/3 — Mentions data efficiency improvement through curriculum learning but the main contribution is mechanistic interpretability of ICL generalization, not directly advancing energy-efficient training or Sutro Group priorities.
**Keyword hits:** `data-efficient`

## TLDR
(none provided)

## Abstract
We study the generalization mechanisms of In-Context Learning (ICL) in Transformer-based language models from the perspective of mechanistic interpretability. While prior works have explored ICL either through single-task mechanistic analysis or multi-task empirical evaluation, a unified mechanistic understanding of ICL generalization has not yet been established. To address this gap, we conduct a systematic study using two structured tasks: ICL Markov Chain and ICL Regression. These tasks respectively instantiate Markovian and i.i.d. data distributions, enabling tractable analysis and principled definitions of task similarity. We investigate how knowledge acquired from a source task facilitates learning in a target task, and how this transfer depends on formal measures of similarity between the tasks. Our empirical results show that initializing from data-dependent checkpoints trained on simpler source tasks significantly improves data efficiency when training on more complex target tasks. Furthermore, we identify mathematically and mechanistically interpretable "common structures" in the Transformer QK circuits at lower layers, along with higher-layer features, that support cross-task generalization. These structures vary predictably with formal similarity metrics. Our work unifies mechanistic and generalization perspectives on ICL, offering new insights into curriculum learning phenomena and informing the design of more scalable and data-efficient ICL training pipelines.

## Keywords
Mechanistic Interpretability, In-Context Learning, Transformer, Transformer Interpretability, Generalization, Curriculum Learning
