---
layout: page
title: Proxectos
lang: gl
permalink: /proxectos/
---

Velaquí algunhas referencias de proxectos de investigación nos que participei:

<div class="card-pannel">
{%- for project in site.projects reversed -%}
  {%- include project.html -%}
{%- endfor -%}
</div>
