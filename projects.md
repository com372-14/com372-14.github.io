---
layout: default
title: Projects
slug: projects
---

<h2 class="section-title">Building Blocks of the Web</h2>

<ul class="posts">
  {% for project in site.projects %}
    <li>
    <h3><a href="{{ project.url }}">
      {{ project.title }}
    </a></h3>
    <p class="lesson-date">{{ project.duedate }}</p>
    <hr>
    </li>
  {% endfor %}
</ul>