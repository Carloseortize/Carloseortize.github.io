---
layout: default
title: "Proyectos"
---
<h1>Proyectos</h1>

<ul>
  {% for project in site.projects %}
    <li>
      <a href="{{ project.url | relative_url }}">{{ project.title }}</a><br>
      {{ project.excerpt }}
    </li>
  {% endfor %}
</ul>
