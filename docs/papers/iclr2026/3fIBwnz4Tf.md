# FlexTraj: Image-to-Video Generation with Flexible Point Trajectory Control

**Venue:** iclr2026 (Withdraw)
**Authors:** ZHIYUAN ZHANG, Dongdong Chen, Can Wang, Jing Liao
**OpenReview:** [https://openreview.net/forum?id=3fIBwnz4Tf](https://openreview.net/forum?id=3fIBwnz4Tf)

## Relevance

**LLM score:** 1/3 — The paper mentions efficiency in convergence and inference as a minor benefit of its sequence-concatenation scheme but focuses on point trajectory control for video generation, not on energy-efficient training or the Sutro Group's core priorities.
**Keyword hits:** `sparse`

## TLDR
(none provided)

## Abstract
We present FlexTraj, a framework for image-to-video generation with flexible point trajectory control. FlexTraj introduces a unified point-based motion representation that encodes each point with a segmentation ID, a  temporally consistent trajectory ID, and an optional color channel for appearance cues, enabling both dense and sparse trajectory control.
Instead of injecting trajectory conditions into the video generator through token concatenation or ControlNet, FlexTraj employs an efficient sequence-concatenation scheme that achieves faster convergence, stronger controllability, and more efficient inference, while maintaining robustness under unaligned conditions.
To train such a unified point trajectory-controlled video generator, FlexTraj adopts an annealing training strategy that gradually reduces reliance on complete supervision and aligned condition. Experimental results demonstrate that FlexTraj enables multi-granularity, alignment-agnostic trajectory control for video generation, supporting various applications such as motion cloning, drag-based image-to-video, motion interpolation, camera redirection, flexible action control and mesh animations.

## Keywords
Diffusion Models, Video Generation
