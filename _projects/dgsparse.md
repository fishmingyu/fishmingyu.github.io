---
layout: page
title: dgSPARSE
description: Open-source sparse kernels and GNN operators for the GPU.
category: ml systems
importance: 6
badge: "open source"
tags: [cuda, spmm, sddmm, library]
github: https://github.com/dgSPARSE/dgSPARSE-Library
website: https://dgsparse.github.io/
---

dgSPARSE is a collection of GPU sparse kernels aimed at graph learning
workloads — SpMM, SDDMM, and the GNN operators built on top of them, shipped as
a drop-in library rather than a research artifact.

My contributions here span several papers: online locality and reduction
parallelism for [SDDMM](https://ieeexplore.ieee.org/abstract/document/9643711)
(ICCD '21), heuristic adaptability to input dynamics for
[SpMM](https://dl.acm.org/doi/10.1145/3489517.3530508) (DAC '22), and the
computation-graph analysis behind
[dgNN](https://proceedings.mlsys.org/paper/2022/file/9a1158154dfa42caddbd0694a4e9bdc8-Paper.pdf)
(MLSys '22).
