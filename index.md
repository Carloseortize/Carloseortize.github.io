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

<style>
.tabs { display: flex; justify-content: center; gap: 10px; margin-bottom: 1rem; }
.tab-link { background-color:#007acc;color:white;border:none;padding:10px 18px;cursor:pointer;border-radius:6px;font-weight:bold;transition:0.3s;}
.tab-link:hover { background-color:#005fa3; }
.tab-link.active { background-color:#005fa3; }
.tab-content { background:#fefefe;padding:20px;border-radius:10px;box-shadow:0 4px 12px rgba(0,0,0,0.08);text-align: justify; }
</style>

<script>
function openTab(evt, tabName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tab-content");
  for (i = 0; i < tabcontent.length; i++) { tabcontent[i].style.display = "none"; }
  tablinks = document.getElementsByClassName("tab-link");
  for (i = 0; i < tablinks.length; i++) { tablinks[i].classList.remove("active"); }
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.classList.add("active");
}
</script>

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
