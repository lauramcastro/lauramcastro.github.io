---
layout: page
title: Projects
lang: en
permalink: /en/proxectos/
---

There are references to research projects I've been involved in:

<div class="card-pannel">
{%- for project in site.projects reversed -%}
  {%- include project.html -%}
{%- endfor -%}
</div>