# KAN or MLP? Point Cloud Shows the Way Forward

**Venue:** iclr2026 (Withdraw)
**Authors:** Yan Shi, Qingdong He, Yijun Liu, Xiaoyu Liu, Jingyong Su
**OpenReview:** [https://openreview.net/forum?id=1x0eJ8uUx6](https://openreview.net/forum?id=1x0eJ8uUx6)

## Relevance

**LLM score:** 1/3 — The paper introduces an efficient variant of KAN to reduce parameters and computational cost, but its primary contribution is point cloud architecture, not energy-efficient training or data movement.
**Keyword hits:** `flops`

## TLDR
(none provided)

## Abstract
Multi-Layer Perceptron (MLP) have become one of the fundamental architectural component in point cloud analysis due to its effective feature learning mechanism. However, when processing complex geometric structures in point clouds, MLP' fixed activation functions struggle to efficiently capture local geometric features, while suffering from poor parameter efficiency and high model redundancy. In this paper, we propose PointKAN, which applies Kolmogorov-Arnold Network (KAN) to point cloud analysis tasks to investigate their efficacy in hierarchical feature representation. First, we introduce a Geometric Affine Module (GAM) to transform local features, improving the model's robustness to geometric variations. Next, in the Local Feature Processing (LFP), a parallel structure extracts both group-level features and global context, providing a rich representation of both fine details and overall structure. Finally, these features are combined and processed in the Global Feature Processing (GFP). By repeating these operations, the receptive field gradually expands, enabling the model to capture complete geometric information of the point cloud. To overcome the high parameter counts and computational inefficiency of standard KAN, we develop Efficient-KAN in the PointKAN-elite variant, which significantly reduces parameters while maintaining accuracy. Experimental results demonstrate that PointKAN outperforms PointMLP on benchmark datasets such as ModelNet40, ScanObjectNN, and ShapeNetPart, with particularly strong performance in Few-shot Learning task. Additionally, PointKAN achieves substantial reductions in parameter counts and computational complexity (FLOPs). This work highlights the potential of KAN-based architectures in 3D vision and opens new avenues for research in point cloud understanding.

## Keywords
Point Cloud Analysis, Kolmogorov-Arnold Networks, Efficient-KAN
