# Activation-aware Probe-Query: Effective Key-Value Retrieval for Long-Context LLMs Inference

**Venue:** iclr2026 (Withdraw)
**Authors:** Qingfa Xiao, Jiachuan Wang, Haoyang LI, Cheng Deng, Jiaqi Tang, Shuangyin Li, Yongqi Zhang, Jun Wang, Lei Chen
**OpenReview:** [https://openreview.net/forum?id=5E2iFvO6bH](https://openreview.net/forum?id=5E2iFvO6bH)

## Relevance

**LLM score:** 1/3 — The paper addresses data movement and sparsity in KV cache eviction for inference, which is tangential to the Sutro Group's focus on energy-efficient training.
**Keyword hits:** `sparse, cache`

## TLDR
(none provided)

## Abstract
Recent advances in large language models (LLMs) have showcased exceptional performance in long-context tasks, while facing significant inference efficiency challenges with limited GPU memory. Existing solutions first proposed the sliding-window approach to accumulate a set of historical \textbf{key-value} (KV) pairs for reuse, then further improvements selectively retain its subsets at each step. However, due to the sparse attention distribution across a long context, it is hard to identify and recall relevant KV pairs, as the attention is distracted by massive candidate pairs. Additionally, we found it promising to select representative tokens as \pq in each sliding window to accurately represent the entire context, an approach that has been overlooked in the pursuit of effective KV cache eviction. Thus, we propose \textbf{ActQKV}, a training-free, \textbf{Act}ivation-aware approach that dynamically determines probe-\textbf{Q}uery and leverages it to retrieve the relevant \textbf{KV} pairs for inference. Specifically, ActQKV monitors a token-level indicator, Activation Bias, within each context window, enabling the proper construction of \pq for retrieval at pre-filling stage. 
To accurately recall the relevant KV pairs and minimize the irrelevant ones, we design a dynamic KV cut-off mechanism guided by information density across layers at the decoding stage. Experiments on the Long-Bench and $\infty$ Benchmarks demonstrate its state-of-the-art performance with competitive inference quality and resource efficiency. 
Our source code is available at \href{https://anonymous.4open.science/r/ActQKV-DDE1}{\textnormal{https://anonymous.4open.science/r/ActQKV-DDE1}}.

## Keywords
dense retrieval, KV retrieval, KV cache eviction, long context reasoning
