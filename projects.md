---
layout: default
title: "Proyectos"
---
<h1>Proyectos</h1>

<ul>
  {% for project in site.projects %}
    <li>
      <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
      <p>{{ project.excerpt }}</p>
    </li>
  {% endfor %}
</ul>
