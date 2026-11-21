---
layout: page
title: 项目
permalink: /projects/
description: 课题组项目
nav: true
nav_order: 2
horizontal: false
---

<!-- pages/projects.md -->
<style>
  .projects > .row,
  .projects .container > .row {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
    margin-left: 0;
    margin-right: 0;
  }
  .projects .col {
    width: auto;
    max-width: none;
    min-width: 0;
  }
  .projects a {
    color: inherit;
    text-decoration: none;
  }
  .projects .card-text {
    color: var(--global-text-color-light);
  }
  .projects .card-title {
    font-size: 1.15rem;
    font-weight: 650;
    line-height: 1.35;
    margin-bottom: 0.4rem;
  }
  .projects .card-img-top {
    height: 160px;
    object-fit: contain;
    background: color-mix(in srgb, var(--global-text-color) 4%, var(--global-card-bg-color));
  }
  @media (min-width: 768px) {
    .projects > .row,
    .projects .container > .row {
      grid-template-columns: repeat(3, minmax(0, 1fr));
    }
  }
</style>
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
    {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
