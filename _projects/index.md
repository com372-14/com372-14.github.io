---
layout: default
title: Projects
slug: projects
---

<h2 class="section-title">Building Blocks of the Web</h2>

<ul class="posts">
  <li><h3><a href="/lesson_files/final-project-info.pdf">Final Project</a></h3></li>
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