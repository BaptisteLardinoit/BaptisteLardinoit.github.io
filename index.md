---
layout: default
---
<link rel="stylesheet" href="/assets/css/style.css">

# Welcome to My Robotics Projects

Here you'll find images and videos of my different projects.

## Projects 
<div class="project-grid">

{% for project in site.projects %}
  <div class="project-card">
    <a href="{{ project.url | relative_url }}">
      <div class="image-container">
        <img src="{{ project.image }}" alt="{{ project.title }}">
        <div class="overlay">
          <h3>{{ project.title }}</h3>
          <p>{{ project.description }}</p>
        </div>
      </div>
    </a>
  </div>
{% endfor %}


</div>
