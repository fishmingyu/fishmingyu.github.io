---
layout: page
title: projects
permalink: /projects/
description: Things I build and maintain.
nav: true
nav_order: 2
display_categories: [agent infrastructure, agents for hardware, ml systems]
---

<!-- pages/projects.md -->
{%- for category in page.display_categories %}
{%- assign categorized = site.projects | where: "category", category -%}
{%- if categorized.size > 0 %}
<h2>{{ category }}</h2>
<div class="work-grid">
  {%- assign sorted = categorized | sort: "importance" -%}
  {%- for project in sorted %}
  <a class="work-card" href="{{ project.url | relative_url }}">
    <div class="work-card__head">
      <span class="work-card__name">{{ project.title }}</span>
      {%- if project.badge %}<span class="work-card__stars">{{ project.badge }}</span>{% endif %}
    </div>
    <p class="work-card__desc">{{ project.description }}</p>
    {%- if project.tags %}
    <div class="work-card__tags">
      {%- for tag in project.tags %}<span class="tag">{{ tag }}</span>{% endfor %}
    </div>
    {%- endif %}
  </a>
  {%- endfor %}
</div>
{%- endif %}
{%- endfor %}
