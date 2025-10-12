---
layout: default
title: "Carlos Ortiz — Analista de Datos"
---

<div class="profile">
  <h1>Carlos Ortiz</h1>
  <p>Ingeniero Mecánico & Analista de Datos Junior Bilingüe</p>
  <p>+5 años de experiencia en sectores industriales, empresariales y de gestión. Actualmente enfocado en análisis de datos, optimización de procesos y visualización de información para la toma de decisiones estratégicas.</p>
</div>

<hr>

<h2>Proyectos Destacados</h2>

<div class="projects">
  {% for project in site.projects %}
    <div class="project-card">
      <h3>{{ project.title }}</h3>
      <p>{{ project.description }}</p>
      <a href="{{ project.link }}" target="_blank">Ver proyecto →</a>
    </div>
  
  {% endfor %}
</div>
