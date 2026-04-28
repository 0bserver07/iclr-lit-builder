# AnyDepth: Depth Estimation Made Easy

**Venue:** iclr2026 (Withdraw)
**Authors:** Zeyu Ren, Zeyu Zhang, Wukai Li, Hao Tang
**OpenReview:** [https://openreview.net/forum?id=1aIDxrT6P4](https://openreview.net/forum?id=1aIDxrT6P4)

## Relevance

**LLM score:** 1/3 — The paper proposes a lightweight decoder and data filtering for depth estimation, touching on efficiency but not directly addressing Sutro Group's core topics like data movement, sparsity, or energy-efficient training.
**Keyword hits:** `efficient training`

## TLDR
(none provided)

## Abstract
Recent monocular depth estimation models have achieved impressive performance. However, they typically rely on traditional encoders, complex decoders, and large training sets, which collectively limit their efficiency and generalization. In this work, we pursue a complementary approach: building a lightweight and efficient training framework without sacrificing accuracy. First, we apply DINOv3 to zero-shot monocular depth estimation for the first time. Secondly, we design a lightweight decoder SDT to reduce the number of parameters and computational cost while maintaining performance. Third, inspired by data-centric learning, we first analyze the characteristics that a high-quality sample should possess and then propose a filtering strategy based on these characteristics to filter out low-quality samples, thereby reducing dataset size while improving model training quality. Experiments on multiple benchmarks demonstrate that, despite using fewer parameters and data, our method achieves comparable or even higher accuracy than similar methods at larger scale. Our work emphasizes the integration of visual backbone performance, decoder efficiency, and data quality to explore more efficient and simple zero-shot monocular depth estimation pipelines.

## Keywords
Zero-shot monocular depth estimation, Data-Centric Learning, Lightweight Decoder, Computer Vision
