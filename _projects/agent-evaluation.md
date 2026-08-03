---
layout: page
title: Agent Evaluation
description: Benchmarks for what agents actually have to do — evolve software and remember things.
category: agent infrastructure
importance: 3
badge: "ICML '26"
tags: [benchmarks, memory, evaluation]
paper: https://arxiv.org/abs/2603.13428
website: https://ama-bench.github.io
---

Two benchmarks built around the same complaint: the standard evaluations
measure a setting agents are not deployed in.

### SWE-Milestone — continuous software evolution

Real software is maintained, not written once. SWE-Milestone uses a pipeline
called **DeepCommit** to reconstruct development milestones from commit logs,
turning them into streams of milestone-level tasks that require sustained
system integrity rather than isolated patches.

Evaluating 12 frontier models across 4 agent frameworks, overall performance
drops from **>80% on isolated tasks to 38.03% in the continuous setting** —
exposing error propagation and technical-debt accumulation that per-task
benchmarks cannot see. To appear at ICML 2026.

### AMA-Bench — long-horizon agent memory

Memory benchmarks are mostly about dialogue. AMA-Bench instead measures
retention across realistic agent–environment interaction: states, actions,
observations, tool outputs. It shows current memory systems fail to preserve
causal relationships and objective facts, leaning too hard on
similarity-based retrieval.

The accompanying **AMA-Agent** uses causality-graph construction and
tool-augmented retrieval to reach 57.22% accuracy, beating the strongest
baseline by 11.16 points.
