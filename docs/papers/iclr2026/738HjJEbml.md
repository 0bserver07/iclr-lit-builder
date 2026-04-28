# QueryStream: Advancing Streaming Video Understanding with Query-Aware Pruning and Proactive Response

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=738HjJEbml](https://openreview.net/forum?id=738HjJEbml)

## Relevance

**LLM score:** 1/3 — The paper focuses on inference-time token pruning for streaming video, not training efficiency, thus tangential to Sutro Group's training-centric priorities.
**Keyword hits:** `pruning`

## TLDR
(none provided)

## Abstract
The increasing demand for real-time interaction in online video scenarios necessitates a new class of efficient streaming video understanding models. However, existing approaches often rely on a flawed, query-agnostic ``change-is-important'' principle, which conflates visual dynamics with semantic relevance, leading to computational waste and interaction errors. To address this, we propose QueryStream, a novel framework that instills query-awareness into the core of video processing and response scheduling. QueryStream features two synergistic components: (1) Query-Aware Differential Pruning (QDP), a policy that filters the token stream by jointly assessing semantic relevance to the query and temporal novelty against a dynamically smoothed history, and (2) Relevance-Triggered Active Response (RTAR), a dual-gated mechanism that schedules responses based on both high query relevance and significant information density. As a lightweight, training-free module, QueryStream establishes a new state-of-the-art on benchmarks like StreamingBench and OVO-Bench, matching or exceeding the performance of full-token baselines while pruning over 70\% of visual tokens. Notably, our pruning mechanism generalizes to offline tasks, where it functions as an effective context-denoising module to improve accuracy on long-form videos. This work not only reveals the vast semantic redundancy in video streams relative to user intent but also establishes a promising, intent-driven direction for truly efficient and robust online video understanding.

## Keywords
Streaming Video Understanding, Query-Aware Pruning, Proactive Response
