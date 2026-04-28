# Exploring Knowledge Purification in Multi-Teacher Knowledge Distillation for LLMs

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7pvJoB4aKO](https://openreview.net/forum?id=7pvJoB4aKO)

## Relevance

**LLM score:** 2/3 — The paper proposes knowledge purification to reduce resource demands in multi-teacher distillation, directly addressing training efficiency, a key concern of the Sutro Group.
**Keyword hits:** `knowledge distillation, distillation`

## TLDR
(none provided)

## Abstract
Knowledge distillation has emerged as a pivotal technique for transferring knowledge from stronger large language models (LLMs) to smaller, more efficient models. However, traditional distillation approaches face challenges related to knowledge conflicts and high resource demands, particularly when leveraging multiple teacher models. In this paper, we introduce the concept of **Knowledge Purification**, which consolidates the rationales from multiple teacher LLMs into a single rationale, thereby mitigating conflicts and enhancing efficiency. To investigate the effectiveness of knowledge purification, we further propose five purification methods from various perspectives. Our experiments demonstrate that these methods not only improve the performance of the distilled model but also effectively alleviate knowledge conflicts. Moreover, router-based methods exhibit robust generalization capabilities, underscoring the potential of innovative purification techniques in optimizing multi-teacher distillation and facilitating the practical deployment of powerful yet lightweight models.

## Keywords
knowledge distillation, large language model, LLM routing
