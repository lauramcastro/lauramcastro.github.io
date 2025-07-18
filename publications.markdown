---
layout: page
title: Publicacións
lang: gl
permalink: /publicacions/
---

{%- assign articles = site.articles -%}
{%- assign grouped_by_year = articles | group_by_exp: "post","post.date | date: '%Y' " -%}

{%- for year_item in grouped_by_year reversed -%}
<span style="display: block; ">
  <h2>{{ year_item.name }}</h2>
  {%- for article in year_item.items reversed -%}
    {%- include article.html -%}    
  {%- endfor -%}
{%- endfor -%}
