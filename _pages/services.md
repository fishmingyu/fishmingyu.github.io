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
        <h3>{{ service.title }}</h3>
      </div>
      <p class="service-description">{{ service.description }}</p>
      <div class="service-details">
        <p>Contact me to discuss how I can help with your {{ service.title | downcase }} needs.</p>
      </div>
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
  gap: 2rem;
  margin-top: 2rem;
}

.service-card {
  background-color: var(--global-card-bg-color);
  border: 1px solid var(--global-divider-color);
  border-radius: 8px;
  padding: 2rem;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.service-card:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.service-header {
  display: flex;
  align-items: center;
  gap: 1rem;
  margin-bottom: 1rem;
}

.service-header i {
  font-size: 2rem;
  color: var(--global-theme-color);
  min-width: 2rem;
}

.service-header h3 {
  margin: 0;
  color: var(--global-text-color);
  font-size: 1.5rem;
}

.service-description {
  font-size: 1.1rem;
  color: var(--global-text-color);
  margin-bottom: 1rem;
  line-height: 1.6;
}

.service-details {
  font-size: 0.9rem;
  color: var(--global-text-color-light);
  font-style: italic;
}

@media (max-width: 768px) {
  .service-card {
    padding: 1.5rem;
  }
  
  .service-header {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }
  
  .service-header i {
    font-size: 1.5rem;
  }
}
</style>