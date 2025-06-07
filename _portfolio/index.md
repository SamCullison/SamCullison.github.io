---
title: "My Projects"
layout: default
permalink: /portfolio/
---

<section id="projects" class="projects-grid container">
  <h2>My Projects</h2>
  <div class="grid">
    {% for project in site.portfolio %}
    <article class="project-card">
      <a href="{{ project.url | relative_url }}">
        <img src="{{ project.image }}" alt="{{ project.title }}">
        <h3>{{ project.title }}</h3>
        <p>{{ project.excerpt }}</p>
      </a>
    </article>
    {% endfor %}
  </div>
</section>
