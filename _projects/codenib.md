---
layout: page
title: CodeNib
description: A multi-view data system for serving repository context to coding agents.
category: agent infrastructure
importance: 1
badge: "★ 66"
tags: [python, indexing, retrieval, mcp]
github: https://github.com/sysevol-ai/CodeNib
website: https://codenib.ai
paper: https://arxiv.org/abs/2607.25431
---

Coding agents repeatedly search, navigate, and retain context from repositories
that keep changing underneath them. In practice that context comes from
disconnected pieces — a lexical index here, a language server there, a
task-local scratchpad that dies with the session. The result is repeated
discovery work and lifecycle costs nobody measures.

CodeNib compiles a repository into **lexical, dense, and structural views**
keyed per commit, maps every output back to repository-relative source ranges,
and repairs those views incrementally as edits land instead of rebuilding from
scratch. One runtime then serves ranked search, symbol navigation, and bounded
context to agents over MCP and LSP-shaped APIs.

Across 100 repository snapshots:

- graph and vector updates are **8.7× and 25.4× faster** than independent rebuilds that produce matching output
- static navigation requests that match live-server locations see a **4.7× median latency improvement**
- context selection policies cut trajectory tokens by **50–87%** versus grep/read baselines

The project also ships a local Wiki UI, an Ask view, and a dependency map so a
human can inspect exactly what the agent would have been served.

```bash
pip install codenib
codenib wiki /path/to/repository
```

Developer preview, Apache 2.0. Built under [SysEvol](https://github.com/sysevol-ai).
