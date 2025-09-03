---
layout: page
title: Divulgación
lang: gl
permalink: /divulgacion/
---

 Eis unha selección das miñas palestras técnicas máis recentes (con <span style="background-color: whitesmoke;">fondo gris</span>), e tamén de actividades de divulgación para público máis amplo (con <span style="background-color: lavenderblush;">fondo rosado</span>), das que adoro!

{%- assign activities = site.activities -%}
{%- assign grouped_by_year = activities | group_by_exp: "post","post.date | date: '%Y' " -%}

{%- for year_item in grouped_by_year reversed -%}
<span style="display: block; ">
  <h2>{{ year_item.name }}</h2>
  {%- for activity in year_item.items reversed -%}
    {%- include activity.html -%}
  {%- endfor -%}
{%- endfor -%}
