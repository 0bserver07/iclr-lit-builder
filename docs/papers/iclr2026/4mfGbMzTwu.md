# HybridCoT: Interleaving Latent and Text Chain-of-Thought for Efficient Reasoning

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4mfGbMzTwu](https://openreview.net/forum?id=4mfGbMzTwu)

## Relevance

**LLM score:** 1/3 — The paper primarily improves inference efficiency through latent reasoning, with only incidental mentions of training efficiency, making it tangential to the Sutro Group's focus on energy-efficient training and hardware-aware methods.
**Keyword hits:** `distillation, pruning`

## TLDR
(none provided)

## Abstract
Verbalizing intermediate steps in token space has been central to eliciting reasoning in large language models (LLMs), with longer reasoning generally improving performance but incurring substantial compute and memory costs. Prior attempts to improve efficiency—such as KV-pruning or latent-space reasoning---often suffer from loss of accuracy or training inefficiency.  We propose HybridCoT, a framework that interleaves latent and text reasoning tokens in context. Our method reduces the compression errors that troubles previous latent CoT methods by keeping critical text tokens like math operations, in context, while compress semantic reasoning into the latent space. In addition, we design in-context text-to-token distillation to provide explicit supervision and iterative parallelized latent rollout methods to improve training efficiency for latent token, while shortening reasoning paths for efficiency. On challenging math reasoning benchmarks including AIME and MATH, HybridCoT achieves 94\% of the performance of finetuned text-only CoT models with 1.97× less inference compute, and surpasses efficient baselines (LightThinker and StreamLLM) by 1.36× and 1.26×, respectively.

## Keywords
Language Model, Reasoning, Latent Reasoning, Latent Chain of Thought
