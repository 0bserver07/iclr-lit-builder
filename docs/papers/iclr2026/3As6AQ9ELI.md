# The Markovian Thinker

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=3As6AQ9ELI](https://openreview.net/forum?id=3As6AQ9ELI)

## Relevance

**LLM score:** 3/3 — The paper directly reduces data movement and memory footprint for reasoning models via a Markovian context deletion algorithm, achieving linear compute scaling and enabling efficient training and inference, aligning closely with the group's data movement and cache-aware priorities.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
Reasoning LLMs suffer from quadratic compute growth as their context length increases, making reinforcement learning with verifiable rewards (RLVR) and test-time scaling prohibitively expensive. Prior work has tried to lighten the computational burden by shortening reasoning traces through pruning, summarization, or multi-stage training, but these methods remain bound to quadratic costs. We introduce Delethink, a thinking algorithm that realizes the Markovian Thinking Paradigm. Instead of producing one long monolithic reasoning trace,  Delethink thinks in a sequence of chunks, the Delethink trace. Each chunk continues reasoning by referring only to a fixed number of prior tokens, which functions as a Markovian state sufficient for progressing reasoning, while deleting the rest. This preserves continuity without carrying the quadratic baggage. As a result, compute scales linearly and peak memory remains constant. In experiments, we show that Delethink can be applied directly to off-the-shelf reasoning models ranging from $1.5\textnormal{B}$ to $30\textnormal{B}$ parameters, with no loss in performance. Extended reasoning becomes possible under fixed memory and linear compute, while enabling efficient RL training on new tasks. On the DeepScaleR dataset, Delethink trains R1DistillQwen1.5B to the same benchmark performance as a standard long chain-of-thought (LongCoT) approach, where both models generate up to $24\textnormal{k}$ thinking tokens. The difference is efficiency. Delethink reasons $40\%$ faster with $70\%$ less memory footprint. By decoupling reasoning length from context length, the Markovian Thinking paradigm opens the door to next-generation reasoning LLMs that can scale to millions of tokens with linear compute and constant memory.

## Keywords
LLM Reasoning, RL for LLMs, Reasoning Models, Scalable Reasoning, Test-Time Scaling
