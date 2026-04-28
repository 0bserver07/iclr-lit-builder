# Textual Equilibrium Propagation for Deep Compound AI Systems

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4XsV5Qoj0j](https://openreview.net/forum?id=4XsV5Qoj0j)

## Relevance

**LLM score:** 3/3 — Proposes a local learning method inspired by biologically-plausible Equilibrium Propagation, directly aligning with Sutro Group's local learning priority.
**Keyword hits:** `equilibrium propagation, local learning`

## TLDR
(none provided)

## Abstract
Large language models (LLMs) are increasingly deployed as part of compound AI systems which coordinate multiple modules (e.g., retrievers, tools, verifiers) over long-horizon workflows. Although recent frameworks that propagate textual feedback globally (e.g., TextGrad make it feasible to optimize such pipelines, we identify two depth-scaling failure modes in long-horizon agentic workflows: 1) exploding textual gradient, where textual feedback grows exponentially with depth, leading to prohibitively long message and amplifies evaluation biases; and 2) vanishing textual gradient, where limited long-context ability causes models overemphasize recent or early feedback, while compression of lengthy feedback causes downstream messages to lose specificity gradually as they propagate many hops upstream. To mitigate these issues, we introduce Textual Equilibrium Propagation (TEP), a local learning principle inspired by Equilibrium Propagation in energy-based models. TEP includes two phases: 1) a free phase where a local LLM critics iteratively refine prompts until reaching equilibrium (no further improvements are suggested); and 2) a nudged phase which applies proximal prompt edits with bounded modification intensity, using task-level objectives that propagate via forward signaling rather than backward feedback chains. This design supports local prompt optimization followed by controlled adaptation toward global goals without the computational burden and signal degradation of global textual backpropagation. Across long-horizon QA benchmarks and multi-agent tool-use dataset, TEP consistently improves accuracy and efficiency over global propagation methods such as TextGrad, with gains that increase at greater depths, while preserving the practicality of black-box LLM components in deep compound AI system.

## Keywords
Compound AI System
