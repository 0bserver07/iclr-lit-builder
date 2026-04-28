# Critical attention scaling in long-context transformers

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7SLtElfqCW](https://openreview.net/forum?id=7SLtElfqCW)

## Relevance

**LLM score:** 1/3 — The paper addresses attention scaling for long contexts but does not focus on training efficiency, data movement, sparsity, or other Sutro Group priorities; its main contribution is theoretical analysis of a phase transition in attention behavior.
**Keyword hits:** `phase transition, sparse`

## TLDR
(none provided)

## Abstract
As large language models scale to longer contexts, attention layers suffer from a fundamental pathology: attention scores collapse toward uniformity as context length $n$ increases, causing tokens to cluster excessively, a phenomenon known as rank-collapse. While $\text{\emph{attention scaling}}$ effectively addresses this deficiency by rescaling attention scores with a polylogarithmic factor $\beta_n$, theoretical justification for this approach remains lacking.

We analyze a simplified yet tractable model that magnifies the effect of attention scaling. In this model, attention exhibits a phase transition governed by the scaling factor $\beta_n$: insufficient scaling collapses all tokens to a single direction, while excessive scaling reduces attention to identity, thereby eliminating meaningful interactions between tokens.
Our main result identifies the critical scaling $\beta_n \asymp \log n$ and provides a rigorous justification for attention scaling in YaRN and Qwen, clarifying why logarithmic scaling maintains sparse, content-adaptive attention at large context lengths.

## Keywords
large language models, attention scaling, long-context length scaling, rank-collapse, phase transition, YaRN, Qwen
