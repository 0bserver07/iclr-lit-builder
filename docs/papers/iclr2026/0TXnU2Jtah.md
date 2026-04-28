# Modular Distillation Makes Small Models Think Like Big Ones

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0TXnU2Jtah](https://openreview.net/forum?id=0TXnU2Jtah)

## Relevance

**LLM score:** 2/3 — The paper's main contribution is a modular distillation framework that improves computing efficiency and enables smaller models to reason effectively, directly matching the Sutro Group's focus on distillation for efficiency.
**Keyword hits:** `knowledge distillation, distillation`

## TLDR
(none provided)

## Abstract
Large Language Models (LLMs) have demonstrated exceptional performance in knowledge-sensitive reasoning tasks, but their practical application is still restricted by high computing demand. To address these challenges, we propose a novel modular distillation framework that breaks down knowledge-intensive reasoning tasks into three distinct components: an Analyzer for question decomposition, a Informant for context building, and a Reasoner for step-by-step reasoning inference. Unlike previous distillation methods that focus only on matching final outputs or step-by-step reasoning, our approach introduces a structured pipeline that enables the student model to learn both the analytical and reasoning abilities of the teacher model, while also capturing the teacher’s internal knowledge to guide more accurate and informed inference. This architecture improves interpretability, efficiency, and modularity, allowing for independent optimization of subcomponents. Empirical tests on three different benchmarks—OBQA, StrategyQA, and MedQA—show that our framework outperforms monolithic baselines in accuracy and computing efficiency while achieving competitive performance with much smaller models. Our findings demonstrate that smaller language models can do reasoning more efficiently when the whole process is divided into more manageable distinct components. This modular approach offers a practical and transparent alternative to relying on extremely large, resource-intensive models.

## Keywords
Large Language Models (LLMs), Knowledge Distillation, Reasoning Distillation, Question Decomposition, Efficient Reasoning
