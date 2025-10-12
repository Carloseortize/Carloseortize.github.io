---
layout: default
title: "Carlos Ortiz — Analista de Datos"
---
<section id="about" class="tabs-section">
  <h2>Sobre mí</h2>

  <div class="tabs">
    <button class="tab-link active" onclick="openTab(event, 'Education')">Educación</button>
    <button class="tab-link" onclick="openTab(event, 'Experience')">Experiencia</button>
  </div>

  <div id="Education" class="tab-content" style="display: block;">
    <ul>
      <li><strong>MBA – Gestión Empresarial</strong>, Universidad X, 2018</li>
      <li><strong>Ingeniería Mecánica</strong>, Universidad Y, 2015</li>
      <li><strong>Certificaciones</strong>: Python, SQL, Power BI, Tableau, Streamlit</li>
    </ul>
  </div>

  <div id="Experience" class="tab-content">
    <ul>
      <li><strong>Analista de Datos Junior</strong>, Empresa Z, 2024 - Actual</li>
      <li><strong>Ingeniero Mecánico</strong>, Empresa A, 2017 - 2023</li>
      <li><strong>Practicante en Minería</strong>, Empresa B, 2015 - 2016</li>
    </ul>
  </div>
</section>

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
      <p class="project-description">{{ project.description | markdownify }}</p>
      <a href="{{ project.link }}" target="_blank">Ver proyecto →</a>
    </div>
    <p> </p>
    <p> </p>
  <p> </p>
  {% endfor %}
</div>
