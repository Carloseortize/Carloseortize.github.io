---
layout: default
title: "Carlos Ortiz — Analista de Datos"
---

<div class="profile">
  <h1>De la ingeniería al análisis de datos</h1>
  <p>
    Después de varios años trabajando como Ingeniero Mecánico y liderando proyectos en eficiencia operativa, mantenimiento y mejora de procesos,
    decidí dar un giro hacia el mundo del análisis de datos. Mi experiencia técnica y visión estratégica se transformaron en una pasión por descubrir
    patrones, optimizar decisiones y crear soluciones basadas en datos.
  </p>
  <p>
    A continuación encontrarás una selección de proyectos que reflejan mi evolución en este nuevo camino, combinando lógica, curiosidad y creatividad
    para generar valor a través del análisis de la información.
  </p>
</div>

<hr>

<section id="about">
  <h2>Sobre mí</h2>

  <div class="tabs">
    <button class="tab-button" onclick="toggleTab(event, 'formacion')">Formación Académica</button>
    <button class="tab-button" onclick="toggleTab(event, 'experiencia')">Experiencia Profesional</button>
    <button class="tab-button" onclick="toggleTab(event, 'habilidades')">Habilidades</button>
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

  <div id="habilidades" class="tab-content">
    <p>
      Especializado en Ciberseguridad y Análisis de Datos, domino herramientas como
      <strong>Python, SQL, Pandas, Numpy, Tableau, Power BI, Streamlit, Jupyter Notebook, Git/GitHub</strong> y
      <strong>Excel avanzado</strong>.
      He aplicado técnicas de <em>machine learning</em> (regresión, clasificación y clustering), análisis estadístico
      y visualización de datos para generar <em>insights</em> accionables que impulsan la toma de decisiones.
    </p>
  </div>
</section>

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
  {% endfor %}
</div>

<script>
function toggleTab(evt, tabName) {
  var i, tabcontent, tabbuttons;
  tabcontent = document.getElementsByClassName("tab-content");
  tabbuttons = document.getElementsByClassName("tab-button");

  var currentTab = document.getElementById(tabName);

  // Si ya está abierto, cerrarlo
  if (currentTab.style.display === "block") {
    currentTab.style.display = "none";
    evt.currentTarget.className = evt.currentTarget.className.replace(" active", "");
    return;
  }

  // Ocultar todos los contenidos
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }

  // Quitar clase activa de los botones
  for (i = 0; i < tabbuttons.length; i++) {
    tabbuttons[i].className = tabbuttons[i].className.replace(" active", "");
  }

  // Mostrar el contenido actual
  currentTab.style.display = "block";
  evt.currentTarget.className += " active";
}

// Ocultar todo al inicio
var tabcontent = document.getElementsByClassName("tab-content");
for (var i = 0; i < tabcontent.length; i++) {
  tabcontent[i].style.display = "none";
}
</script>

<style>
.profile p {
  text-align: justify;
}

.tabs {
  margin-bottom: 10px;
}

.tab-button {
  background-color: #007acc;
  color: white;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  margin-right: 5px;
  border-radius: 5px;
  transition: background-color 0.2s;
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

.project-card {
  border: 1px solid #ddd;
  padding: 15px;
  border-radius: 8px;
  margin-bottom: 20px;
  text-align: justify;
}

.project-card a {
  color: #007acc;
  text-decoration: none;
  font-weight: bold;
}

.project-card a:hover {
  text-decoration: underline;
}
</style>
