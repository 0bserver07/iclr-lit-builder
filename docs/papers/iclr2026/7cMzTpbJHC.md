# Temporal superposition and feature geometry of RNNs under memory demands

**Venue:** iclr2026 (Oral)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=7cMzTpbJHC](https://openreview.net/forum?id=7cMzTpbJHC)

## Relevance

**LLM score:** 1/3 — The paper studies representational geometry and sparsity in RNNs under memory constraints, tangentially touching on capacity efficiency, but its main contribution is mechanistic understanding rather than advancing energy-efficient training techniques.
**Keyword hits:** `phase transition, sparse`

## TLDR
(none provided)

## Abstract
Understanding how populations of neurons represent information is a central challenge across machine learning and neuroscience. Recent work in both fields has begun to characterize the representational geometry and functionality underlying complex distributed activity. For example, artificial neural networks trained on data with more features than neurons compress data by representing features non-orthogonally in so-called *superposition*. However, the effect of time (or memory), an additional capacity-constraining pressure, on underlying representational geometry in recurrent models is not well understood. Here, we study how memory demands affect representational geometry in recurrent neural networks (RNNs), introducing the concept of temporal superposition. We develop a theoretical framework in RNNs with linear recurrence trained on a delayed serial recall task to better understand how properties of the data, task demands, and network dimensionality lead to different representational strategies, and show that these insights generalize to nonlinear RNNs. Through this, we identify an effectively linear, dense regime and a sparse regime where RNNs utilize an interference-free space, characterized by a phase transition in the angular distribution of features and decrease in spectral radius. Finally, we analyze the interaction of spatial and temporal superposition to observe how RNNs mediate different representational tradeoffs. Overall, our work offers a mechanistic, geometric explanation of representational strategies RNNs learn, how they depend on capacity and task demands, and why.

## Keywords
RNNs, superposition, representational geometry, features, capacity, memory demands
