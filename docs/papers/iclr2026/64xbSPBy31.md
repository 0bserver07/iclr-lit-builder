# DistillMatch: Leveraging Knowledge Distillation from Vision Foundation Model for Multimodal Image Matching

**Venue:** iclr2026 (Withdraw)
**Authors:** Meng Yang, Fan Fan, Zizhuo Li, Ruimin Huang, Songchu Deng, Yong Ma, Jiayi Ma
**OpenReview:** [https://openreview.net/forum?id=64xbSPBy31](https://openreview.net/forum?id=64xbSPBy31)

## Relevance

**LLM score:** 1/3 — The paper uses knowledge distillation to transfer features from a vision foundation model, resulting in a lightweight student, but the main contribution is multimodal image matching performance, not training efficiency or Sutro Group priorities like energy-efficient training.
**Keyword hits:** `knowledge distillation, distillation`

## TLDR
(none provided)

## Abstract
Multimodal image matching seeks pixel-level correspondences between images of different modalities, crucial for cross-modal perception, fusion and analysis. However, the significant appearance differences between modalities make this task challenging. Due to the scarcity of high-quality annotated datasets, existing deep learning methods that extract modality-common features for matching perform poorly and lack adaptability to diverse scenarios. Vision Foundation Model (VFM), trained on large-scale data, yields generalizable and robust feature representations adapted to data and tasks of various modalities, including multimodal matching. Thus, we propose DistillMatch, a multimodal image matching method using knowledge distillation from VFM. DistillMatch employs knowledge distillation to build a lightweight student model that extracts high-level semantic features from VFM to assist matching across modalities. To retain modality-specific information, it extracts and injects modality category information into the other modality's features, which enhances the model's understanding of cross-modal correlations. Furthermore, we design V2I-GAN to boost the model's generalization by translating visible to pseudo-infrared images for data augmentation. Experiments show that DistillMatch outperforms existing algorithms on public datasets.

## Keywords
multimodal image matching, vision foundation model, knowledge distillation, modality-specific information
