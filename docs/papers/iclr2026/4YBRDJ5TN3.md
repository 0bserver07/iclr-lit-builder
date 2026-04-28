# Exploring Redundancy and Shared Representations for Transformer Models Optimization

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4YBRDJ5TN3](https://openreview.net/forum?id=4YBRDJ5TN3)

## Relevance

**LLM score:** 1/3 — The paper touches on efficiency via model compression but does not directly advance energy-efficient training or specific Sutro Group priorities like data movement, sparse parity, or local learning.
**Keyword hits:** `model compression, low-rank`

## TLDR
(none provided)

## Abstract
Large Language Models (LLMs) deliver state-of-the-art performance but at the cost of extreme computational and energy demands, raising the question of how much of their capacity is truly necessary. This paper explores structural and weight redundancies in Transformer-based architectures, aiming to identify inefficiencies and leverage them through targeted compression techniques.
A central focus is assessing whether different modules perform overlapping functions. Although some degree of similarity is observed in the analyzed cases, redundancy proves to be lower than expected, challenging the assumption that weight matrices can be interchanged across layers without compromising performance. Additionally, an analysis of model matrices examines whether they exhibit an inherently low-rank structure.
To further explore these aspects, three novel compression methods are introduced: MASS, which enforces weight aggregation and sharing, along with two factorization-based techniques, GlobaL Fact and ABACO. Experimental results show that while these approaches achieve model compression, their ability to maintain performance is limited, reducing their practical viability.
The findings highlight the complexity of extracting redundancy from Transformer architectures, raising questions about its extent across layers and blocks. By addressing these challenges, this paper aims to contribute to ongoing efforts to improve the efficiency of LLMs.

## Keywords
Large Language Models, Redundancy, Weight sharing, Model compression, Low-rank approximation
