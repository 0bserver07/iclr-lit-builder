# CoKV: Optimizing LLM Inference with Game-Theoretic Adaptive KV Cache

**Venue:** iclr2026 (Withdraw)
**Authors:** Qiheng Sun, Hongwei Zhang, Haocheng Xia, Jiayao Zhang, Xiaokai Mao, Junxu Liu, Jinfei Liu, Haibo Hu, Kui Ren
**OpenReview:** [https://openreview.net/forum?id=1iuaBRErka](https://openreview.net/forum?id=1iuaBRErka)

## Relevance

**LLM score:** 1/3 — The paper addresses inference memory efficiency via KV cache optimization, which is tangential to the training-focused priorities of energy-efficient training, data movement, and hardware-aware training.
**Keyword hits:** `quantization, cache`

## TLDR
(none provided)

## Abstract
Large language models (LLMs) have achieved remarkable success in various aspects of human life. However, one of the major challenges in deploying these models is the substantial memory consumption required to store key-value pairs (KV), which imposes significant resource demands. Recent research has focused on KV cache budget allocation, with several approaches proposing head-level budget distribution by evaluating the importance of individual attention heads. These methods, however, assess the importance of heads independently, overlooking their cooperative contributions within the model, which may result in a deviation from their true impact on model performance. In light of this limitation, we propose CoKV, a novel method that models the cooperation between heads in model inference as a cooperative game. By attributing the contribution of each head within the model, CoKV can more effectively allocate the cache budget in KV cache techniques such as eviction and quantization. Extensive experiments demonstrate the effectiveness of CoKV on long-context benchmarks (e.g., LongBench, NIAH, and RULER) and mathematical reasoning benchmarks (e.g., GSM8K and MATH) across multiple model families, including Qwen, Llama, and Mistral. Code is provided in \url{https://anonymous.4open.science/r/CoKV-40AC}.

## Keywords
Game theory, Model inference, Large Language Models
