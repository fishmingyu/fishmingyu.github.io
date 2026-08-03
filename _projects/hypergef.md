---
layout: page
title: HyperGef
description: Efficient kernel fusion for hypergraph neural networks on GPUs.
category: ml systems
importance: 5
badge: "MLSys '23"
tags: [cuda, fusion, hypergraph]
github: https://github.com/fishmingyu/HyperGef
paper: https://proceedings.mlsys.org/paper_files/paper/2023/hash/c0987e6b6da2428e8cd43efa74790ccb-Abstract-mlsys2023.html
---

Hypergraph neural networks run two rounds of irregular gather/scatter per
layer — vertex-to-edge, then edge-to-vertex. Executed as separate kernels, that
pattern spends most of its time moving intermediate results through memory.

HyperGef is a framework that fuses those stages, with a workload-balancing
scheme that keeps the fused kernel from stalling on skewed hyperedge degrees.

Published at MLSys 2023.
