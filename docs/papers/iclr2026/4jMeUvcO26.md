# Surrogate Modeling of 3D Rayleigh-Bénard Convection with Equivariant Autoencoders

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=4jMeUvcO26](https://openreview.net/forum?id=4jMeUvcO26)

## Relevance

**LLM score:** 1/3 — The paper focuses on sample and parameter efficiency for surrogate modeling, tangential to the Sutro Group's core focus on energy-efficient training techniques like data movement, sparsity, or hardware-aware kernels.
**Keyword hits:** `kernel`

## TLDR
(none provided)

## Abstract
The use of machine learning for modeling, understanding, and controlling large-scale physics systems is quickly gaining in popularity, with examples ranging from electromagnetism over nuclear fusion reactors and magneto-hydrodynamics to fluid mechanics and climate modeling. These systems — governed by partial differential equations — present unique challenges regarding the large number of degrees of freedom and the complex dynamics over many scales both in space and time, and additional measures to improve accuracy and sample efficiency are highly desirable. We present an end-to-end equivariant surrogate model consisting of an equivariant convolutional autoencoder and an equivariant convolutional LSTM using $G$-steerable kernels. As a case study, we consider the three-dimensional Rayleigh-Bénard convection, which describes the buoyancy-driven fluid flow between a heated bottom and a cooled top plate. While the system is E(2)-equivariant in the horizontal plane, the boundary conditions break the translational equivariance in the vertical direction. Our architecture leverages vertically stacked layers of $D_4$-steerable kernels, with additional partial kernel sharing in the vertical direction for further efficiency improvement. We demonstrate significant gains in sample and parameter efficiency, as well as a better scaling to more complex dynamics.

## Keywords
surrogate modeling, fluid mechanics, geometric deep learning, autoencoder, time series prediction, dimensionality reduction, steerable convolutions
