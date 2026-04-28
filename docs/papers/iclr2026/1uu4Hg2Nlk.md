# Eliminating VAE for Fast and High-Resolution Generative Detail Restoration

**Venue:** iclr2026 (Poster)
**Authors:** 
**OpenReview:** [https://openreview.net/forum?id=1uu4Hg2Nlk](https://openreview.net/forum?id=1uu4Hg2Nlk)

## Relevance

**LLM score:** 1/3 — The paper's primary contribution is inference acceleration and memory reduction via VAE elimination and adversarial distillation, not training efficiency or Sutro Group's core training-centric topics.
**Keyword hits:** `model compression, distillation`

## TLDR
(none provided)

## Abstract
Diffusion models have attained remarkable breakthroughs in the real-world super-resolution (SR) task, albeit at slow inference and high demand on devices. To accelerate inference, recent works like GenDR adopt step distillation to minimize the step number to one. However, the memory boundary still restricts the maximum processing size, necessitating tile-by-tile restoration of high-resolution images. Through profiling the pipeline, we pinpoint that the variational auto-encoder (VAE) is the bottleneck of latency and memory. To completely solve the problem, we leverage pixel-(un)shuffle operations to eliminate the VAE, reversing the latent-based GenDR to pixel-space GenDR-Pix. However, upscale with 
$\times$8 pixelshuffle may induce artifacts of repeated patterns. To alleviate the distortion, we propose a multi-stage adversarial distillation to progressively remove the encoder and decoder. Specifically, we utilize generative features from the previous stage models to guide adversarial discrimination. Moreover, we propose random padding to augment generative features and avoid discriminator collapse. We also introduce a masked Fourier space loss to penalize the outliers of amplitude. To improve inference performance, we empirically integrate a padding-based self-ensemble with classifier-free guidance to improve inference scaling. Experimental results show that GenDR-Pix performs 2.8$\times$  acceleration and 60% memory-saving compared to GenDR with negligible visual degradation, surpassing other one-step diffusion SR. Against all odds, GenDR-Pix can restore 4K image in only 1 second and 6 GB.

## Keywords
Diffusion, Super-Resolution, Adversarial distillation, Model Compression
