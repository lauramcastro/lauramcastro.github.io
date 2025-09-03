---
layout: page
title: Projects
lang: en
permalink: /en/proxectos/
---

There are references to research projects I am, or have been, involved in, in recent years:

<div class="card-pannel">
{%- for project in site.projects reversed -%}
  {%- include project.html -%}
{%- endfor -%}
</div>

<br/>
I have also supervised the following PhD thesis:

<div class="card-pannel">
{%- for thesis in site.thesis reversed -%}
  {%- include thesis.html -%}
{%- endfor -%}
</div>
