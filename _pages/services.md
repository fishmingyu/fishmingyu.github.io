---
layout: page
permalink: /services/
title: services
description: Reviewing and program-committee service.
nav: true
nav_order: 3
---

<div class="svc-list">
  {% for service in site.data.services.services %}
  <div class="svc-row">
    <div class="svc-row__date">{{ service.date }}</div>
    <div>
      <div class="svc-row__title">{{ service.title }}</div>
      <p class="svc-row__desc">{{ service.description }}</p>
    </div>
  </div>
  {% endfor %}
</div>
