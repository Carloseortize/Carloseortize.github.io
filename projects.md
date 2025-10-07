---
layout: default
title: "Proyectos"
---

<h1>Mis Proyectos Destacados</h1>
<p>Estos son algunos de los proyectos que he desarrollado, abarcando análisis de datos, optimización de procesos, visualización y marketing digital.</p>

<div style="display: flex; flex-wrap: wrap; gap: 20px;">

{% assign proyectos = site.projects | sort: 'title' %}

{% for project in proyectos %}
  <div style="flex: 1 1 300px; border: 1px solid #ccc; padding: 15px; border-radius: 8px;">
    <img src="{{ project.header.overlay_image | default: '/assets/images/default_project.jpg' }}" alt="{{ project.title }}" style="width: 100%; height: auto; border-radius: 5px;">
    <h3>{{ project.title }}</h3>
    <p>{{ project.excerpt }}</p>
    <a href="{{ project.url | relative_url }}">Ver más</a>
  </div>
{% endfor %}

</div>
