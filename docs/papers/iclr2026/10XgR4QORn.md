# Analyzing and Internalizing Complex Policy Documents for LLM Agents

**Venue:** iclr2026 (Withdraw)
**Authors:** Jiateng Liu, Zhenhailong Wang, Xiaojiang Huang, Yingjie Li, Xiang Li, Chenlei Guo, Xing Fan, Ruhi Sarikaya, Heng Ji
**OpenReview:** [https://openreview.net/forum?id=10XgR4QORn](https://openreview.net/forum?id=10XgR4QORn)

## Relevance

**LLM score:** 1/3 — Tangential: addresses inference efficiency via policy internalization, not energy-efficient training, data movement, sparsity, or other Sutro Group priorities.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
Large Language Model (LLM) based agentic systems rely heavily on in-context policy documents that encode diverse business rules. As business requirements expand, these documents grow substantially, creating significant computational overhead. This motivates the need for internalization methods that embed policy documents into model priors while preserving performance. While prior prompt compression research primarily targets generic prompts, we find that agentic policy documents span multiple levels of complexity and demand more intensive reasoning, presenting greater internalization challenges. We first introduce CC-Gen, an agentic benchmark generator with Controllable Complexity defined across four levels,  enabling systematic benchmarking of how well agents handle complexities and provides a framework for comprehensive evaluation of policy internalization algorithms. Our initial analysis reveals that complex policy specifications governing agent workflows may pose the most significant reasoning challenges. When supporting internalization with gold user–agent interaction trajectories containing chain-of-thought (CoT) annotations through supervised fine-tuning (SFT), we find that this baseline is highly data-intensive and its effectiveness deteriorates markedly as policy document complexity increases. To mitigate data burden and reasoning challenges, we propose Category-Aware Policy Continued Pretraining (CAP-CPT). Our automated pipeline analyzes policy documents to extract key specifications, grouping them into factual, behavioral, and conditional types. We further isolate complex conditions, which introduce high workflow complexity and drive core reasoning difficulty. This categorization guides a targeted therapy, synthesizing specialized training data for each specification type and enabling agents to internalize policy information more effectively through an autoregressive pretraining loss. Our extensive experiments demonstrate the effectiveness of the curated data and training objective. Combined with SFT, our approach improves baseline across all data scenarios. It is especially effective in data-sparse settings and under high policy complexity, yielding gains of up to 41\% and 22\% on Qwen-3-32B. Overall, we achieve up to 97.3\% prompt length reduction in our benchmark. Applied to $\tau$-Bench, our approach further improves performance and reduces input length with very limited SFT data.

## Keywords
Policy Interalization, LLM Agents
