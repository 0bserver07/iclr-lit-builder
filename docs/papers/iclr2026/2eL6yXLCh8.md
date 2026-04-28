# Hyden: A Hybrid Dual-Path Encoder for Monocular Geometry of High-resolution Images

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2eL6yXLCh8](https://openreview.net/forum?id=2eL6yXLCh8)

## Relevance

**LLM score:** 1/3 — The paper emphasizes inference efficiency and uses self-distillation for label generation, but the main contribution is a vision encoder architecture, not energy-efficient training or core priorities like data movement, sparsity, or hardware-aware training.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
We present a hybrid dual-path vision encoder (Hyden) for high-resolution monocular depth, point map and surface normal estimation, surpassing state-of-the-art accuracy with a fraction of the inference cost. The architecture pairs a low-resolution Vision Transformer branch for global context with a full-resolution CNN branch for fine details, fusing features via a lightweight MLP before decoding. By exploiting the linear scaling of CNNs and constraining transformer computation to a fixed resolution, the model delivers fast inference even on multi-megapixel inputs. To overcome the scarcity of high-quality high-resolution supervision, we introduce a self-distillation framework that generates pseudo-labels from existing models at both lower resolution full images and high-resolution crops—global labels preserve geometric accuracy, while local labels capture sharper details. To demonstrate the flexibility of our approach, we integrate Hyden and our self-distillation method into DepthAnything-v2 for depth estimation and MoGe2 for surface normal and metric point map prediction, achieving state-of-the-art results on high-resolution benchmarks with the lowest inference latency among competing methods.

## Keywords
3D vision, Monocular Depth Estimation, Monocular Surface Normal Estimation
