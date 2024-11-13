---
layout: default
---
<link rel="stylesheet" href="/assets/css/style.css">

<header class="main-header>
  <div class="content-container">
    <div class="header-content">
      <img src="/assets/images/422765839_695656782722177_1716881690510392068_n.jpg" alt="Profile Picture" class="profile-pic">
      <div class="intro-text">
        <h1>Baptiste Lardinoit</h1>
        <p>Welcome to my robotics projects portfolio! Here, you'll find various images, videos, and descriptions showcasing the robotics projects I've worked on. From 3D modeling to autonomous navigation, I’m excited to share my work with you.</p>
      </div>
    </div>
  </div>
</header>

<div class="content-container">

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
</div>


