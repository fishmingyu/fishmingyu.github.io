---
layout: about
title: about
permalink: /

# Hero
role: Ph.D. Candidate
org: UC San Diego CSE
org_url: https://cse.ucsd.edu/
advisor: Jishen Zhao
advisor_url: https://cseweb.ucsd.edu/~jzhao/
tagline: >
  I build infrastructure for LLM agents — systems where agents are
  first-class computational entities rather than an application layer
  bolted onto a chat API.

profile:
  align: right
  image: image.png
  image_circular: false
  address: >
    San Diego, California

news: true
selected_papers: true
social: true
---

I am a fifth-year Ph.D. candidate at UC San Diego, advised by
[Prof. Jishen Zhao](https://cseweb.ucsd.edu/~jzhao/), and since June 2026 a
**Deep Learning Compiler Intern** at NVIDIA.
Before UCSD I received my B.E. from the Department of Electronic Engineering at
Tsinghua University.

My work sits between machine learning and computer systems, and the through-line
is that I keep treating model-shaped problems as systems problems. What an agent
needs is rarely a bigger prompt — it is a memory hierarchy, an index that
survives edits, and a serving layer with measurable lifecycle costs. That
premise drives most of what I build now:
[repository context serving](https://codenib.ai),
[memory protocols for multi-agent systems](https://arxiv.org/abs/2603.10062),
and [benchmarks that measure software as it evolves](https://arxiv.org/abs/2603.13428)
rather than one patch at a time. A parallel thread puts agents to work on
hardware, [generating](https://arxiv.org/abs/2412.07822) and
[verifying](https://arxiv.org/abs/2602.16953) RTL.

The same lens started in sparse computation — [dgSPARSE](https://dgsparse.github.io/),
[CogDL](https://cogdl.ai/), GPU sparse linear algebra — and now extends to
[compiler-agent co-design for frontier GPU kernels](https://arxiv.org/abs/2608.12629)
and [sparse attention](https://arxiv.org/abs/2602.05191) for long-context inference.

<ul class="focus-list">
  <li><b>Agent infrastructure</b> — repository context serving, incremental indexes, retrieval that respects code structure</li>
  <li><b>Agent memory</b> — multi-agent memory hierarchies, consistency, long-horizon retention</li>
  <li><b>Evaluation</b> — benchmarks for continuous software evolution, not one-shot patches</li>
  <li><b>Agents for hardware</b> — RTL generation and verification, learning from execution feedback</li>
  <li><b>ML systems</b> — compiler-agent co-design, evolving GPU kernels, sparse attention</li>
</ul>

I also maintain [SysEvol](https://github.com/sysevol-ai), an open-source effort
around AI-driven system evolution.

## current work

<div class="work-grid">
  <a class="work-card" href="{{ '/projects/cake/' | relative_url }}">
    <div class="work-card__head">
      <span class="work-card__name">CAKE</span>
      <span class="work-card__stars">arXiv '26</span>
    </div>
    <p class="work-card__desc">A compiler-agent co-design where agents evolve frontier GPU kernels through a typed, hardware-explicit schedule IR.</p>
    <div class="work-card__tags">
      <span class="tag">arXiv 2608.12629</span>
      <span class="tag">compiler-agent</span>
      <span class="tag">gpu kernels</span>
    </div>
  </a>
  <a class="work-card" href="https://codenib.ai">
    <div class="work-card__head">
      <span class="work-card__name">CodeNib</span>
      <span class="work-card__stars">★ 66</span>
    </div>
    <p class="work-card__desc">A multi-view data system that serves repository context to coding agents — lexical, dense, and structural views that update incrementally instead of rebuilding.</p>
    <div class="work-card__tags">
      <span class="tag">arXiv 2607.25431</span>
      <span class="tag">python</span>
      <span class="tag">apache-2.0</span>
    </div>
  </a>
</div>

Everything else — agent evaluation, RTL agents, the sparse computation work —
is on the [projects]({{ '/projects/' | relative_url }}) page.

Feel free to reach out if any of this overlaps with what you are working on.
