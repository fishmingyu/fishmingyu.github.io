---
layout: page
title: Agents for RTL
description: Putting agents to work on hardware — generating Verilog, then proving it wrong.
category: agents for hardware
importance: 1
badge: "ICML '26"
tags: [rtl, verification, multi-agent, rl]
paper: https://arxiv.org/abs/2602.16953
---

Hardware design is an unusually honest setting for agents: a simulator will
tell you, without negotiation, whether the thing you generated works. Three
projects build on that feedback signal, moving from generation to verification
to learning from execution.

### MAGE — multi-agent RTL generation

A multi-agent engine for automated RTL code generation, splitting the task
across specialised agents rather than asking one model to emit a whole module
in a single shot.

Published at DAC 2025 · [paper](https://arxiv.org/abs/2412.07822) ·
[code](https://github.com/stable-lab/MAGE)

### PRO-V-R1 — trainable verification agents

Generating RTL is only half the problem; someone has to write the testbench
that catches the bugs. PRO-V-R1 is the first open-source **trainable** agentic
framework for autonomous RTL verification, reaching 57.7% functional
correctness and 34.0% on robust fault detection — competitive with proprietary
models on several benchmarks.

[paper](https://arxiv.org/abs/2506.12200) ·
[code](https://github.com/stable-lab/Pro-V)

### LLM4Cov — learning under expensive execution

Execution-aware agents learn from tool feedback, but in hardware that feedback
comes from industrial simulators: slow, costly, and non-differentiable. LLM4Cov
is an offline agent-learning framework built around that constraint —
execution-validated data curation, policy-aware agentic data synthesis, and
worst-state-prioritized sampling.

A compact **4B model** reaches a 69.2% coverage pass rate under agentic
evaluation, beating its own teacher by 5.3 points and holding its own against
models an order of magnitude larger.

To appear at ICML 2026 · [paper](https://arxiv.org/abs/2602.16953) ·
[code](https://github.com/HejiaZ2023/llm4cov_oss)
