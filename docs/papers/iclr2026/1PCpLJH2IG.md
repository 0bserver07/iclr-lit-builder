# Curriculum-Guided Layer Scaling for Language Model Pretraining

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1PCpLJH2IG](https://openreview.net/forum?id=1PCpLJH2IG)

## Relevance

**LLM score:** 2/3 — The paper's primary contribution is a compute-efficient pretraining method that reduces resource consumption, making training efficiency a central focus.
**Keyword hits:** `compute-efficient`

## TLDR
(none provided)

## Abstract
As the cost of pretraining large language models grows, there is continued interest in strategies to improve learning efficiency during this core training stage. Motivated by cognitive development, where humans gradually build knowledge as their brains mature, we propose Curriculum-Guided Layer Scaling (CGLS), a framework for compute-efficient pretraining that synchronizes increasing data difficulty with model growth through progressive layer stacking (i.e. gradually adding layers during training). At the 100M parameter scale, using a curriculum transitioning from synthetic short stories to general web data, CGLS outperforms baseline methods on the question-answering benchmarks PIQA and ARC. Pretraining at the 1.2B scale, we stratify the DataComp-LM corpus with a DistilBERT-based classifier and progress from general text to highly technical or specialized content. Our results show that progressively increasing model depth alongside sample difficulty leads to better generalization and zero-shot performance on various downstream benchmarks. Altogether, our findings demonstrate that CGLS unlocks the potential of progressive stacking, offering a simple yet effective strategy for improving generalization on knowledge-intensive and reasoning tasks.

## Keywords
large language models, pretraining, curriculum learning, scaling
