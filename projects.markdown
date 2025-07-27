---
layout: page
title: Proxectos
lang: gl
permalink: /proxectos/
---

Velaquí algunhas referencias de proxectos de investigación nos que participo ou participei nos últimos anos.

<div class="card-pannel">
{%- for project in site.projects reversed -%}
  {%- include project.html -%}
{%- endfor -%}
</div>

<br/>
Tamén dirixín as teses de doutoramento:

<div class="card-pannel">
{%- for thesis in site.thesis reversed -%}
  {%- include thesis.html -%}
{%- endfor -%}
</div>
