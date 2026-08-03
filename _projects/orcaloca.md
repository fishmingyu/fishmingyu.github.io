---
layout: page
title: OrcaLoca
description: An LLM agent framework for software issue localization.
category: agent infrastructure
importance: 2
badge: "ICML '25"
tags: [agents, swe-bench, scheduling]
github: https://github.com/fishmingyu/OrcaLoca
paper: https://arxiv.org/abs/2502.00350
---

Resolving a software issue starts with finding the code to change, and that
first step is where most agent pipelines lose accuracy. OrcaLoca treats
localization as a scheduling problem rather than a single retrieval call:

- **Priority-based scheduling** for LLM-guided actions, so the agent spends its budget on the most promising leads first
- **Action decomposition with relevance scoring**, breaking coarse search steps into ranked sub-actions
- **Distance-aware context pruning**, keeping the working set small as the search widens

The combination sets a new state of the art in function-match rate on
SWE-bench Lite, and slots in ahead of existing repair agents as a drop-in
localization stage.

Published at ICML 2025.
