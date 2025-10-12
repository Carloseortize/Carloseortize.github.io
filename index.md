---
layout: default
title: "Proyectos de Análisis de Datos"
---

<header class="profile">
  <h1>Carlos Ortiz</h1>
  <p>Ingeniero Mecánico & Analista de Datos Junior Bilingüe</p>
  <p>+5 años de experiencia en sectores industriales y empresariales. Enfocado en análisis de datos, optimización de procesos y visualización para la toma de decisiones estratégicas.</p>
</header>

<section>
  <h2>Proyectos</h2>
  <div class="projects">
    {% for project in site.projects %}
      <div class="project-card">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        <a href="{{ project.link }}" target="_blank">Ver proyecto</a>
      </div>
    {% endfor %}
  </div>
</section>

<footer>
  <p>© 2025 Carlos Ortiz — Desarrollado con GitHub Pages</p>
</footer>
