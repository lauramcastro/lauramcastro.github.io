---
layout: page
title: Dissemination
lang: en
permalink: /en/divulgacion/
---

Alongside technical speaking, I enjoy getting involved in dissemination activities for wider audiences. This is a selection of both.

{%- assign activities = site.activities -%}
{%- assign grouped_by_year = activities | group_by_exp: "post","post.date | date: '%Y' " -%}

{%- for year_item in grouped_by_year reversed -%}
<span style="display: block; ">
  <h2>{{ year_item.name }}</h2>
  {%- for activity in year_item.items reversed -%}
    {%- include activity.html -%}
  {%- endfor -%}
{%- endfor -%}
