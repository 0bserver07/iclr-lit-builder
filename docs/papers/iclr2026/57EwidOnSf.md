# VideoMind: A Chain-of-LoRA Agent for Temporal-Grounded Video Reasoning

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=57EwidOnSf](https://openreview.net/forum?id=57EwidOnSf)

## Relevance

**LLM score:** 1/3 — The Chain-of-LoRA mechanism for efficient role switching is a minor inference efficiency aspect, but the paper's main contribution is video reasoning agent architecture, not training efficiency or the group's core topics.
**Keyword hits:** `lora`

## TLDR
(none provided)

## Abstract
Videos, with their unique temporal dimension, demand precise grounded understanding, where answers are directly linked to visual, interpretable evidence. Despite significant breakthroughs in text-based reasoning with large language models, multi-modal reasoning - especially for videos - remains limited. In this work, we fill this gap by introducing VideoMind, a novel video-language agent for temporal-grounded video reasoning. Our method involves two key innovations: (1) We identify four essential capabilities for grounded video reasoning and propose a role-based agentic workflow, comprising a planner to coordinate roles, a grounder for temporal event localization, a verifier to assess event candidates, and an answerer for question answering. (2) To efficiently integrate these roles during inference, we propose a novel Chain-of-LoRA mechanism, where a unified base model with multiple LoRA adapters is leveraged to enable seamless role switching, balancing efficiency and flexibility. Extensive experiments on 15 benchmarks across Grounded VideoQA, Video Temporal Grounding, and General VideoQA tasks demonstrate the effectiveness of the proposed scheme in advancing video agent, test-time scaling, and long-form video reasoning. Code, models, datasets, and demos are available at https://videomind.github.io/.

## Keywords
Multi-modal Agent, Video Understanding, Video Temporal Grounding
