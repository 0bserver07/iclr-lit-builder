# DC-LLM: HARDWARE-FRIENDLY LLM WEIGHT COMPRESSION VIA DYNAMIC LINEAR COMBINATION

**Venue:** iclr2026 (Withdraw)
**Authors:** Mingzi Wang, Lancheng Zou, Shuo Yin, Zhuolun He, Bei Yu
**OpenReview:** [https://openreview.net/forum?id=3YUL5LJ3s4](https://openreview.net/forum?id=3YUL5LJ3s4)

## Relevance

**LLM score:** 1/3 — Focuses on inference weight compression and data movement, not training efficiency; mentions low-precision and hardware acceleration tangentially but does not advance energy-efficient training or Sutro Group's training-centric priorities.
**Keyword hits:** `asic`

## TLDR
(none provided)

## Abstract
The progressive scaling of large language models (LLMs) has consistently en-
hanced multimodal understanding and advanced reasoning capabilities, but has
substantially increased computational and hardware execution overhead. In this
paper, we present DC-LLM, a novel post-method that compresses only model
weights. We partition each weight tensor into fixed-size blocks and assign a sin-
gle seed to each block. The seed drives a hardware-friendly Linear Feedback
Shift Register (LFSR) generator that dynamically produces multiple basis ma-
trices. Each block is then reconstructed as a linear combination of these basis
matrices, with block-specific coefficients, which substantially reduces the amount
of stored data, increases the data-transfer efficiency between memory and com-
pute units, and consequently speeds up memory-bound inference for large lan-
guage models. Experimental results on different LLM models ranging
from 7B–70B parameters show that DC-LLM attains state-of-the-art performance
when weights are compressed to approximately 3-bit or 4-bit. We also design a
dedicated ASIC accelerator that achieves a 4× speed-up for memory-bound LLM
inference.

## Keywords
LLM, Compression
