---
layout: page
title: project updates
permalink: /projects/
description: A collection of our project work and photos.
nav: true
nav_order: 3
display_categories: [work]
horizontal: false
---

<div class="projects">
  {% assign work_projects = site.projects | where: "category", "work" | sort: "importance" %}

  <h2 class="category">work</h2>

  {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-1 row-cols-md-2">
        {% for project in work_projects %}
          {% include projects_horizontal.liquid %}
        {% endfor %}
      </div>
    </div>
  {% else %}
    <div class="row row-cols-1 row-cols-md-3">
      {% for project in work_projects %}
        {% include projects.liquid %}
      {% endfor %}
    </div>
  {% endif %}
</div>

<hr class="my-5">

<h2 class="mb-4">Project Photos</h2>
<p class="text-muted">Snapshots from our work and development process.</p>

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
