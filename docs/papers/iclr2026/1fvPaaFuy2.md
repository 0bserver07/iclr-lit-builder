# Entropy-Select: Training-Free Local Entropy Token Compression for Video LLMs

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1fvPaaFuy2](https://openreview.net/forum?id=1fvPaaFuy2)

## Relevance

**LLM score:** 1/3 — Tangential: the paper proposes token compression for inference efficiency in video LLMs, which touches on sparsity and data movement reduction, but is unrelated to training efficiency, the core focus of the Sutro Group.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Video Language Models (VLMs) emit visual tokens that grow linearly with video length while attention scales quadratically, making inference sensitive to token count and latency variance. In practice, an effective token compressor should be training-free to plug into strong off-the-shelf VLMs, architecture-agnostic to avoid model-specific hooks, and deliver selection runtime that is predictable regardless of the target retention—properties that many prior methods lack. We introduce EntropySelect, a training-free, architecture-agnostic framework that ranks tokens by local neighborhood entropy, an information-theoretic measure of unpredictability relative to nearby tokens. We compute temperature-scaled similarity distributions within fixed spatial windows to obtain normalized entropy, fuse it with gradient-based structural saliency, enforce coverage via grid quotas, and allocate per-frame budgets by saliency. Because windows/grids are fixed and selection reduces to a single global sort, EntropySelect runs in O(N log N) with latency effectively decoupled from the retention ratio. Across MVBench, ActivityNet-QA, VideoMME, and EgoSchema, EntropySelect matches or exceeds the uncompressed baseline at moderate retention and degrades gracefully under aggressive compression, yielding predictable latency and plug-and-play deployment without any model modification or internal-state access. Notably, we observe “enhancement under compression” on several benchmarks—for example, 35% and 50% retention surpass the full-token baseline on benchmarks such as MVBench and EgoSchema—suggesting that removing low-entropy redundancy can improve downstream accuracy.These results establish local entropy as a principled criterion for video token selection and a practical tool for scalable VLM inference. Code will be released upon acceptance.

## Keywords
Video-language models, Vision-language models, Token selection, Entropy-guided pruning, Training-free, Video understanding
