# Asynchronous Matching with Dynamic Sampling for Multimodal Dataset Distillation

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7SgSMKM2KF](https://openreview.net/forum?id=7SgSMKM2KF)

## Relevance

**LLM score:** 2/3 — The paper advances dataset distillation, a technique to reduce training data size and improve efficiency, which aligns with the Sutro Group's interest in distillation for energy-efficient training.
**Keyword hits:** `efficient training, distillation`

## TLDR
(none provided)

## Abstract
Multimodal Dataset Distillation (MDD) has emerged as a vital paradigm for enabling efficient training of vision-language models (VLMs) in the era of multimodal data proliferation. Unlike traditional dataset distillation methods that focus on single-modal tasks, MDD presents distinct challenges: (i) the effective distillation of heterogeneous multimodal knowledge, complicated by feature space misalignment and asynchronous optimization dynamics; and (ii) the lack of discrete class guidance, which hinders the distribution coverage and representativeness of synthetic data due to the vastness and continuity of the semantic space. To address these challenges, this paper proposes an Asynchronous Matching with Dynamic sampling (AMD) framework. AMD enables asynchronous trajectory matching by decoupling the selection of starting points for image and text trajectories. Additionally, a Semantics-Aware Prototype Mining module is introduced, which replaces random initialization by leveraging feature-space clustering to identify representative prototypes, enhancing the coverage and representativeness of the distilled samples. Extensive experiments demonstrate that AMD achieves superior distillation performance on Flickr30k and COCO (e.g., IR@1, IR@5, and IR@10 \textbf{gains of 4.5\%, 9.6\%, and 10.9\%}, respectively, on Flickr30k 200 pairs.) with negligible computational overhead.

## Keywords
Trajectory Matching, Dataset Distillation
