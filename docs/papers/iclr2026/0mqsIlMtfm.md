# PTQTP: Post-Training Quantization to Trit-Planes for Large Language Models

**Venue:** iclr2026 (Withdraw)
**Authors:** He Xiao, RUNMING YANG, Qingyao Yang, Wendong XU, Zhen Li, Yupeng Su, Zhengwu Liu, Hongxia Yang, Ngai Wong
**OpenReview:** [https://openreview.net/forum?id=0mqsIlMtfm](https://openreview.net/forum?id=0mqsIlMtfm)

## Relevance

**LLM score:** 1/3 — The paper focuses on post-training quantization for efficient inference, not on energy-efficient training, which is the primary scope of the Sutro Group.
**Keyword hits:** `quantization, 1-bit`

## TLDR
(none provided)

## Abstract
Post-training quantization (PTQ) of large language models (LLMs) to extremely low bit-widths remains challenging due to the fundamental trade-off between computational efficiency and model expressiveness. While existing ultra-low-bit PTQ methods rely on binary approximations or complex compensation mechanisms, they suffer from either limited representational capacity or computational overhead that undermines their efficiency gains. We introduce **PTQ** to**T**rit-**P**lanes (PTQTP), the first ternary-weight PTQ framework that decomposes weight matrices into structured ternary \(\{-1, 0, 1\}\) trit-planes using 2×1.58-bit representation. PTQTP achieves multiplication-free inference, identical to 1-bit quantization, while maintaining superior expressiveness through its novel structured decomposition. Our approach provides: (1) a theoretically grounded progressive approximation algorithm ensuring global weight consistency; (2) model-agnostic deployment across diverse modern LLMs without architectural modifications; and (3) uniform ternary operations that eliminate the need for mixed-precision or compensation schemes. Comprehensive experiments across LLaMA3.x and Qwen3 model families (0.6B-70B parameters) demonstrate that PTQTP significantly outperforms existing low-bit PTQ methods, achieving 82.4\% mathematical reasoning retention versus 0\% for competing approaches. PTQTP approaches and sometimes surpasses 1.58-bit quantization-aware training performance while requiring only single-hour quantization compared to 10-14 GPU days for training-based methods. These results establish PTQTP as a practical solution for efficient LLM deployment in resource-constrained environments.

## Keywords
Large language model, post-training quantization, ternary
