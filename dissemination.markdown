---
layout: page
title: Divulgación
lang: gl
permalink: /divulgacion/
---

Ademáis das palestras técnicas que imparto, tamén adoro de facer divulgación para público máis amplo. Eis unha selección de ambas categorías.

{%- assign activities = site.activities -%}
{%- assign grouped_by_year = activities | group_by_exp: "post","post.date | date: '%Y' " -%}

{%- for year_item in grouped_by_year reversed -%}
<span style="display: block; ">
  <h2>{{ year_item.name }}</h2>
  {%- for activity in year_item.items reversed -%}
    {%- include activity.html -%}
  {%- endfor -%}
{%- endfor -%}
