---
layout: default
title: "Carlos Ortiz — Analista de Datos"
---

<div class="profile">
  <h1>De la ingeniería al análisis de datos</h1>
  <p>Después de varios años trabajando como Ingeniero Mecánico y liderando proyectos en eficiencia operativa, mantenimiento y mejora de procesos, decidí dar un giro hacia el mundo del análisis de datos.
Mi experiencia técnica y visión estratégica se transformaron en una pasión por descubrir patrones, optimizar decisiones y crear soluciones basadas en datos.</p>
  <p>A continuación encontrarás una selección de proyectos que reflejan mi evolución en este nuevo camino, combinando lógica, curiosidad y creatividad para generar valor a través del análisis de la información.</p>
</div>

<hr>

<h2>Proyectos Destacados</h2>

<div class="projects">
  {% for project in site.projects %}
    <div class="project-card">
      <h3>{{ project.title }}</h3>
      <p>{{ project.description | markdownify }}</p>
      <a href="{{ project.link }}" target="_blank">Ver proyecto →</a>
    </div>
    <p> </p>
    <p> </p>
  <p> </p>
  {% endfor %}
</div>
