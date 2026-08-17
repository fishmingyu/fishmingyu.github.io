---
layout: page
title: CAKE
description: Compiler-agent co-design for evolving frontier GPU kernels.
category: ml systems
importance: 1
badge: "arXiv '26"
tags: [agents, compilers, gpu, kernels]
paper: https://arxiv.org/abs/2608.12629
---

GPU kernel agents typically see the compiler as a black box: they submit code
and receive errors, correctness results, and timings. That interface hides the
hardware scheduling structure an agent needs to diagnose and improve a kernel.

**CAKE** co-designs the agent and compiler around CAKE IR, a typed,
hardware-explicit schedule representation. It exposes warp roles, memory
movement, synchronization, and pipelines while giving agents verification,
cost modeling, and localized diagnostics. The surrounding harness evolves as
well, turning recurring failures into verifier rules, IR primitives, model
calibrations, and reusable optimization tactics.

Reported results include:

- a best Flash-KMeans candidate reaching **1.144×** the tuned FlashML baseline on B200
- agent-generated Kimi Delta Attention achieving a **2.05× geometric-mean speedup** over official FlashKDA
- dispatcher-backed KNN and KMeans improving performance by **1.42×–2.12×** across more than 400 shapes

CAKE targets NVIDIA GPUs from Ampere through Blackwell and separates
single-shape kernel evolution from library-level generalization and dispatch.

[Read the paper on arXiv](https://arxiv.org/abs/2608.12629).
