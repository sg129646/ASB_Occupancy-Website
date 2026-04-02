---
layout: page
title: project updates
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
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

<hr>

<h2>Project Photos</h2>

<div class="row row-cols-1 row-cols-md-3 g-4">
  <div class="col">
    <img src="/assets/img/project-photo-1.jpg" alt="Project photo 1" class="img-fluid rounded shadow-sm">
  </div>
  <div class="col">
    <img src="/assets/img/project-photo-2.jpg" alt="Project photo 2" class="img-fluid rounded shadow-sm">
  </div>
  <div class="col">
    <img src="/assets/img/project-photo-3.jpg" alt="Project photo 3" class="img-fluid rounded shadow-sm">
  </div>
</div>
