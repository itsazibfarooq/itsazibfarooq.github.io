---
layout: page
title: Projects
permalink: /projects/
description: Selected research and engineering projects.
nav: true
nav_order: 2
---

<!-- pages/projects.md -->
<div class="projects">
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
</div>
