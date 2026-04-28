# KnItLM: Weaving Knowledge into Instruction-Tuned LLMs via Continual Pre-Training and Merging

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2uctT30vTS](https://openreview.net/forum?id=2uctT30vTS)

## Relevance

**LLM score:** 1/3 — The paper focuses on knowledge ingestion and model merging, mentioning cost avoidance of instruction fine-tuning but not making efficiency or data movement a central contribution.
**Keyword hits:** `low-rank, lora`

## TLDR
(none provided)

## Abstract
RAG has become the de facto method for incorporating new, corpus-specific knowledge into an instruction following LLM (Instruct LLM). Although RAG-based prompting improves factual grounding, it fails when retrieval is incorrect or incomplete, leading to hallucinations. Finetuning methods such as RAFT and PA-RAG enhance RAG by ingesting new knowledge into the parameters of the model,  but require generating massive amount of synthetic QA that covers the entire corpus. Continued Pre-Training (CPT) on the text corpus avoids the need for comprehensive synthetic data generation but breaks the instruction following capabilities of an Instruct LLM, necessitating instruction fine-tuning (IFT) post CPT. However, IFT is costly and may be infeasible due to the unavailability of an instruction tuning corpus. In this work, we propose KnItLM - KNowledge IngesTion via LoRA Merging. Instead of doing CPT on the Instruct LLM, KnItLM performs CPT with Low-Rank Adapters (LoRA) on its corresponding base LLM  to infuse new knowledge. These knowledge-infused LoRA weights are then merged with the Instruct LLM, imparting new knowledge without impacting their instruction following capabilities. KnItLM avoids expensive instruction fine-tuning and relies on model merging to infuse the new knowledge into the Instruct LLM without destroying its instruction following capabilities. Empirical results show that KnItLM significantly improves the performance of RAG by taking accuracy from $54.17$% to $79.26$% for retrieval failure cases. In addition, the proposed method achieves superior performance to existing approaches while requiring substantially less training data.

## Keywords
Knowledge Ingestion, RAG, Lora Transfer
