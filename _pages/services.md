---
layout: page
permalink: /services/
title: services
description: Research and technical services offered
nav: true
nav_order: 3
---

<div class="services-page">
  <div class="services-container">
    {% for service in site.data.services.services %}
    <div class="service-card">
      <div class="service-header">
        <i class="{{ service.icon }}"></i>
        <div class="service-title-section">
          <h3>{{ service.title }}</h3>
          <span class="service-date">{{ service.date }}</span>
        </div>
      </div>
      <p class="service-description">{{ service.description }}</p>
    </div>
    {% endfor %}
  </div>
</div>

<style>
.services-page {
  max-width: 800px;
  margin: 0 auto;
}

.services-container {
  display: grid;
  gap: 1rem;
  margin-top: 1rem;
}

.service-card {
  background-color: var(--global-card-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 6px;
  padding: 1.25rem;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.service-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.service-header {
  display: flex;
  align-items: flex-start;
  gap: 0.75rem;
  margin-bottom: 0.75rem;
}

.service-header i {
  font-size: 1.25rem;
  color: var(--global-theme-color);
  min-width: 1.25rem;
  margin-top: 0.125rem;
}

.service-title-section {
  flex: 1;
}

.service-header h3 {
  margin: 0 0 0.125rem 0;
  color: var(--global-text-color);
  font-size: 1.1rem;
  font-weight: 600;
}

.service-date {
  font-size: 0.8rem;
  color: var(--global-theme-color);
  font-weight: 500;
}

.service-description {
  font-size: 0.9rem;
  color: var(--global-text-color);
  margin: 0;
  line-height: 1.4;
}


@media (max-width: 768px) {
  .service-card {
    padding: 1rem;
  }
  
  .service-header {
    gap: 0.5rem;
  }
  
  .service-header i {
    font-size: 1.1rem;
    min-width: 1.1rem;
  }
  
  .service-header h3 {
    font-size: 1rem;
  }
}
</style>