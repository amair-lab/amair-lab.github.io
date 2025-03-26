---
layout: page
title: Projects
permalink: /projects/
description: 
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---

<!-- Custom CSS for the projects page -->
<style>
  /* Base styles */
  .projects {
    max-width: 1200px;
    margin: 0 auto;
  }
  
  /* Category styles */
  .category {
    font-size: 2.2rem;
    font-weight: 300;
    letter-spacing: -0.5px;
    margin: 3rem 0 1.5rem;
    color: #333;
    position: relative;
    display: inline-block;
  }
  
  /* Project cards */
  .project-card {
    background: #fff;
    border-radius: 10px;
    padding: 0;
    margin-bottom: 40px;
    box-shadow: 0 1px 3px rgba(0,0,0,0.08);
    transition: all 0.2s ease;
    overflow: hidden;
  }
  
  .project-card:hover {
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transform: translateY(-2px);
  }
  
  .project-card img {
    width: 100%;
    display: block;
    border-radius: 10px;
    transition: all 0.3s ease;
  }
  
  .project-card:hover img {
    transform: scale(1.25);
  }
  
  .project-card .card-body {
    padding: 20px;
  }
  
  .project-card .card-title {
    font-size: 1.4rem;
    font-weight: 500;
    margin-bottom: 10px;
    color: #ba1db1;
  }
  
  .project-card .card-text {
    font-size: 1rem;
    color: #666;
    line-height: 1.5;
  }
  
  /* Grid adjustments */
  .projects .row {
    display: flex;
    flex-wrap: wrap;
    margin-right: -15px;
    margin-left: -15px;
  }
  
  .projects .col {
    padding: 0 15px;
    margin-bottom: 30px;
  }
  
  /* Category indicators */
  .category-indicator {
    display: inline-block;
    padding: 3px 8px;
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    border-radius: 10px;
    margin-bottom: 10px;
  }
  
  .category-indicator.work {
    background-color: rgba(59, 130, 246, 0.1);
    color: rgb(37, 99, 235);
  }
  
  .category-indicator.fun {
    background-color: rgba(16, 185, 129, 0.1);
    color: rgb(5, 150, 105);
  }
  
  /* Simple hover effects */
  .view-project {
    display: inline-block;
    margin-top: 15px;
    font-size: 0.9rem;
    color: #555;
    font-weight: 500;
    position: relative;
    transition: all 0.2s ease;
  }
  
  .view-project::after {
    content: '';
    position: absolute;
    width: 100%;
    height: 1px;
    bottom: -2px;
    left: 0;
    background-color: #555;
    transform: scaleX(0);
    transform-origin: bottom right;
    transition: transform 0.3s ease;
  }
  
  .view-project:hover {
    color: #000;
  }
  
  .view-project:hover::after {
    transform: scaleX(1);
    transform-origin: bottom left;
  }
  
  /* Image placeholder styling */
  .image-placeholder {
    background: #f5f5f5;
    height: 220px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #aaa;
    font-size: 0.9rem;
  }
</style>

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
  
  <!-- Generate custom cards for each project -->
  <div class="row">
    {% for project in sorted_projects %}
    <div class="col col-sm-12 col-md-6 col-lg-4">
      <div class="project-card">
        {% if project.img %}
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.img | relative_url }}" alt="{{ project.title }}" />
        </a>
        {% else %}
        <div class="image-placeholder">No image available</div>
        {% endif %}
        <div class="card-body">
          <span class="category-indicator {{ project.category }}">{{ project.category }}</span>
          <h3 class="card-title">{{ project.title }}</h3>
          <p class="card-text">{{ project.description }}</p>
          <a href="{{ project.url | relative_url }}" class="view-project">View Project</a>
        </div>
      </div>
    </div>
    {% endfor %}
  </div>
  {% endfor %}

{% else %}

<!-- Display projects without categories -->
{% assign sorted_projects = site.projects | sort: "importance" %}

<div class="row">
  {% for project in sorted_projects %}
  <div class="col col-sm-12 col-md-6 col-lg-4">
    <div class="project-card">
      {% if project.img %}
      <a href="{{ project.url | relative_url }}">
        <img src="{{ project.img | relative_url }}" alt="{{ project.title }}" />
      </a>
      {% else %}
      <div class="image-placeholder">No image available</div>
      {% endif %}
      <div class="card-body">
        <h3 class="card-title">{{ project.title }}</h3>
        <p class="card-text">{{ project.description }}</p>
        <a href="{{ project.url | relative_url }}" class="view-project">View Project</a>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
{% endif %}
</div>