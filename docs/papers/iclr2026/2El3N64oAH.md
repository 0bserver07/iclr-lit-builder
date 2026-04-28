# Matrix-Free Least Squares Solvers: Values, Gradients, and What to Do With Them

**Venue:** iclr2026 (Reject)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=2El3N64oAH](https://openreview.net/forum?id=2El3N64oAH)

## Relevance

**LLM score:** 2/3 — The paper makes sparsity (enforcing weight sparsity on a 50M parameter model) a main contribution, directly aligning with Sutro Group's sparsity priority.
**Keyword hits:** `sparsity`

## TLDR
(none provided)

## Abstract
This paper argues that the method of least squares has significant unfulfilled potential in modern machine learning, far beyond merely being a tool for fitting linear models. To release its potential, we derive custom gradients that transform the solver into a differentiable operator, like a neural network layer, enabling many diverse applications. Empirically, we demonstrate: (i) scalability by enforcing weight sparsity on a 50 million parameter model; (ii) imposing conservativeness constraints in score-based generative models; and (iii) hyperparameter tuning of Gaussian processes based on predictive performance. By doing this, our work represents the next iteration in developing differentiable linear-algebra tools and making them widely accessible to machine learning practitioners.

## Keywords
Automatic differentiation, Numerical Linear Algebra, Constrained Optimization, Implicit Differentiation, Gaussian Process
