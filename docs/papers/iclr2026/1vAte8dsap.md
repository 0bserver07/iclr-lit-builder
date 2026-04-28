# pi-Flow: Policy-Based Few-Step Generation via Imitation Distillation

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1vAte8dsap](https://openreview.net/forum?id=1vAte8dsap)

## Relevance

**LLM score:** 1/3 — The paper uses distillation to accelerate inference via few-step generation, which touches on the listed priority of distillation, but the main contribution is inference efficiency, not energy-efficient training.
**Keyword hits:** `distillation`

## TLDR
(none provided)

## Abstract
Few-step diffusion or flow-based generative models typically distill a velocity-predicting teacher into a student that predicts a shortcut towards denoised data. This format mismatch has led to complex distillation procedures that often suffer from a quality--diversity trade-off. To address this, we propose policy-based flow models ($\pi$-Flow). 
$\pi$-Flow modifies the output layer of a student flow model to predict a network-free policy at one timestep. The policy then produces dynamic flow velocities at future substeps with negligible overhead, enabling fast and accurate ODE integration without extra network evaluations.
To match the policy's ODE trajectory to the teacher's,
we introduce a novel imitation distillation approach, which matches the policy's velocity to the teacher's along the policy's trajectory using a standard $\ell_2$ flow matching loss. 
By simply mimicking the teacher's behavior, $\pi$-Flow enables stable and scalable training and avoids the quality--diversity trade-off.
On ImageNet $256\times 256$, it attains a 1-NFE FID of 2.85, outperforming previous 1-NFE models of the same DiT architecture. 
On FLUX.1-12B and Qwen-Image-20B at 4 NFEs, $\pi$-Flow achieves substantially better diversity than state-of-the-art DMD models, while maintaining teacher-level quality.

## Keywords
diffusion models, flow models, few-step generation, distillation
