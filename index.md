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
    <button class="tab-button" onclick="openTab(event, 'formacion')">Formación Académica</button>
    <button class="tab-button" onclick="openTab(event, 'experiencia')">Experiencia Profesional</button>
  </div>

  <div id="formacion" class="tab-content">
    <ul>
      <li>MBA en Alta Dirección Empresarial – Universidad Catolica de Avila, España</li>
      <li>Ingeniería Mecánica – Universidad De América, Colombia</li>
      <li>Certificación en Análisis de Datos – TripleTen</li>
      <li>Certificación en Ciberseguridad – Google (beca)</li>
    </ul>
  </div>

  <div id="experiencia" class="tab-content">
    <ul>
      <li>
        <strong>Fundador y Director – Empresa de Economía Circular</strong> <br>
        2021 - 2025, Bogotá, Colombia<br>
        Lideré operaciones, logística y alianzas estratégicas.<br>
        Implementé soluciones tecnológicas y de análisis de procesos para optimizar la cadena de suministro.<br>
        Gestioné compras y supervisé la producción, mejorando eficiencia y calidad.<br>
        Diseñé maquinaria y sistemas de control de calidad basados en datos.<br>
        <em>Logros: aumento del 20% en eficiencia de procesos y 40% en control de inventario.</em>
      </li>
      <li>
        <strong>Gerente de Producción y Operaciones</strong> <br>
        2018 – 2019, París, Francia<br>
        Preparación y control de pedidos, asegurando eficiencia y precisión.<br>
        Supervisión de personal y producción para optimizar recursos y productividad.<br>
        Operación y control de maquinaria especializada.<br>
        <em>Logros: aumento del 10% en cumplimiento de entregas y reducción del 25% en errores de empaque.</em>
      </li>
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
  text-align: justify;
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
