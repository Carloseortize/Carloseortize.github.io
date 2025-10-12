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



<section id="about">
  <h2>Sobre mí</h2>

  <div class="tabs">
    <button class="tab-button" onclick="openTab(event, 'educacion')">Educación</button>
    <button class="tab-button" onclick="openTab(event, 'experiencia')">Experiencia</button>
  </div>

  <div id="educacion" class="tab-content">
    <ul>
      <li>MBA – Gestión Empresarial, Universidad X, 2018</li>
      <li>Ingeniería Mecánica, Universidad Y, 2015</li>
      <li>Certificaciones: Python, SQL, Power BI, Tableau, Streamlit</li>
    </ul>
  </div>

  <div id="experiencia" class="tab-content">
    <ul>
      <li>Analista de Datos Junior, Empresa Z, 2024 - Actual</li>
      <li>Ingeniero Mecánico, Empresa A, 2017 - 2023</li>
      <li>Practicante en Minería, Empresa B, 2015 - 2016</li>
    </ul>
  </div>
</section>

<script>
function openTab(evt, tabName) {
  // Ocultar todos los contenidos
  var i, tabcontent, tabbuttons;
  tabcontent = document.getElementsByClassName("tab-content");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }

  // Eliminar la clase active de todos los botones
  tabbuttons = document.getElementsByClassName("tab-button");
  for (i = 0; i < tabbuttons.length; i++) {
    tabbuttons[i].className = tabbuttons[i].className.replace(" active", "");
  }

  // Mostrar el contenido seleccionado
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.className += " active";
}

// Inicialmente, no mostrar ningún contenido
var tabcontent = document.getElementsByClassName("tab-content");
for (var i = 0; i < tabcontent.length; i++) {
  tabcontent[i].style.display = "none";
}
</script>

<style>
.tab-button {
  background-color: #007acc;
  color: white;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  margin-right: 5px;
  border-radius: 5px;
}

.tab-button:hover {
  background-color: #005fa3;
}

.tab-button.active {
  background-color: #005fa3;
}

.tab-content {
  margin-top: 15px;
  border-left: 3px solid #007acc;
  padding-left: 15px;
}
</style>





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
