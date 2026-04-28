# Larger Datasets Can Be Repeated More: A Theoretical Analysis of Multi-Epoch Scaling in Linear Regression

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=0CXjpAxHUE](https://openreview.net/forum?id=0CXjpAxHUE)

## Relevance

**LLM score:** 2/3 — The paper analyzes multi-epoch training efficiency, quantifying when data reuse is effective, which directly relates to reducing fresh data requirements and potentially saving training energy.
**Keyword hits:** `scaling law`

## TLDR
(none provided)

## Abstract
Large Language Model (LLM) training often processes vast text corpora in a single pass, leaving much available data underutilized. This paper presents a theoretical analysis of how a common workaround, training for multiple epochs on the same dataset, reshapes the data scaling laws. Concretely, given a $K$-epoch training on $N$ samples, how many fresh samples would one-pass training require to match the same performance? We quantify this using the \textit{effective reuse rate} of the data, $E(K, N)$, which we define as the factor by which the dataset must grow under one-pass training to match the test loss of multi-epoch training. Our analysis precisely characterizes the scaling behavior of $E(K, N)$ for SGD in linear regression under either strong convexity or Zipf-distributed data: (1) When $K$ is small, we prove that $E(K, N) \approx K$, indicating that every new epoch yields a linear gain; (2) As $K$ increases, $E(K, N)$ plateaus at a problem-dependent value that grows with $N$ ($\Theta(\log N)$ for the strongly-convex case), implying that larger datasets can be repeated more times before the marginal benefit vanishes. These theoretical findings complement a recent empirical study by [Muennighoff et al. (2023)](https://arxiv.org/abs/2305.16264), which found that training LLMs for up to $4$ epochs results in negligible loss differences compared to using fresh data at each step, \textit{i.e.}, $E(K, N) \approx K$ for $K \le 4$ in our notation. 
    Supported by further empirical validation with LLMs, our results reveal how this behavior depends on the underlying data size and distribution, and underscore the need to explicitly model both factors in future studies of scaling laws with data reuse.

## Keywords
Deep learning theory, Multi-epoch training, Data-reuse, Optimization, Scaling law, Large language model
