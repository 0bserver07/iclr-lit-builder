# Enhancing LLMs for Knowledge Base Question Answering by Chain-of-Decomposition

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4vfEo07rmv](https://openreview.net/forum?id=4vfEo07rmv)

## Relevance

**LLM score:** 1/3 — Mentions efficient fine-tuning and reduced LLM calls via task decomposition, but training efficiency, data movement, or Sutro Group priorities are not the main contribution.
**Keyword hits:** `lora`

## TLDR
(none provided)

## Abstract
Large language models (LLMs) have demonstrated remarkable success across diverse domains through in-context learning or fine-tuning. However, adapting LLMs to Knowledge Base Question Answering (KBQA) remains challenging, as KBQA necessitates multi-step reasoning over large-scale structured knowledge bases. Directly prompting LLMs with entire knowledge bases incurs prohibitive computational costs, while existing methods provide limited guidance on effectively fine-tuning LLMs for such complex reasoning tasks. In this work, we propose Chain-of-Decomposition (\texttt{CoD}), a novel framework that decomposes KBQA into three modular steps: (1) an LLM-free retrieval module to extract query-relevant subgraphs from the knowledge base, (2) a parameter-free reformulation step that transforms retrieved contexts into structured reasoning paths, and (3) a lightweight LLM-based reasoning module trained to evaluate the logical validity of each path. By isolating computation-heavy retrieval and rule-based reformulation from LLM reasoning, \texttt{CoD} reduces task complexity and enables efficient fine-tuning focused solely on the final verification step. Comprehensive experiments demonstrate that Llama-2 7B, fine-tuned with the proposed \texttt{CoD} surpasses strong baselines, including GPT-4 augmented with retrieved knowledge, achieving state-of-the-art performance on WebQSP and MetaQA benchmarks.

## Keywords
LLMs, LoRA, KBQA
