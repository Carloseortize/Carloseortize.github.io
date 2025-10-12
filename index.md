---
layout: default
---

<!doctype html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="chrome=1">
    <title>Portafolio | Carlos - Ingeniero Mecánico & Analista de Datos</title>

    <link rel="stylesheet" href="stylesheets/styles.css">
    <link rel="stylesheet" href="stylesheets/pygment_trac.css">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!--[if lt IE 9]>
      <script src="//html5shiv.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
  </head>

  <body>
    <div class="wrapper">
      <!-- HEADER -->
      <header>
        <h1>Carlos Ortiz</h1>
        <p>Ingeniero Mecánico & Analista de Datos Junior Bilingüe</p>
        <p>+5 años de experiencia en sectores industriales, empresariales y de gestión. Actualmente enfocado en análisis de datos, optimización de procesos y visualización de información para la toma de decisiones estratégicas.</p>
        <p>Apasionado por la innovación, la mejora continua y el uso de datos para generar soluciones sostenibles con impacto real.</p>

        <ul>
          <li><a href="https://github.com/Carloseortize" target="_blank">GitHub</a></li>
          <li><a href="https://www.linkedin.com/in/Carloseortize/" target="_blank">LinkedIn</a></li>
          <li><a href="mailto:carlos.e.ortize@gmail.com">Correo</a></li>
        </ul>
      </header>

      <!-- SECCIÓN DE PROYECTOS -->
      <section>
        <h1>Portafolio de Proyectos</h1>
        <p>Estos son algunos de los proyectos en los que he trabajado recientemente, enfocados en análisis de datos, automatización, visualización y mejora de procesos.</p>

        <div class="projects-grid">
          {% for project in site.projects %}
            <div class="project-card">
              <h2>{{ project.title }}</h2>
              <p>{{ project.description }}</p>
              <a href="{{ project.link }}" target="_blank">Ver más →</a>
            </div>
          {% endfor %}
        </div>
      </section>

      <!-- PIE DE PÁGINA -->
      <footer>
        <p>© 2025 Carlos Ortiz — Portafolio Profesional</p>
        <p><small>Diseñado con 💡 usando HTML, CSS y Jekyll</small></p>
      </footer>
    </div>

    <script src="javascripts/scale.fix.js"></script>
  </body>
</html>
