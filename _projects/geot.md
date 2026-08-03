---
layout: page
title: GeoT
description: A tensor-centric library for GNNs, built on efficient GPU segment reduction.
category: ml systems
importance: 4
badge: "CUDA"
tags: [cuda, sparse, gnn, kernels]
github: https://github.com/fishmingyu/GeoT
paper: https://arxiv.org/abs/2404.03019
---

Graph neural network frameworks usually reach for message-passing abstractions
that fight the tensor programming model underneath them. GeoT takes the other
route: express GNN computation in terms of **segment reduction**, and then make
that one primitive genuinely fast on the GPU.

The library provides tuned segment-reduction kernels along with the index
handling around them, so GNN operators compose with ordinary tensor code
instead of living in a parallel universe of framework-specific ops.
