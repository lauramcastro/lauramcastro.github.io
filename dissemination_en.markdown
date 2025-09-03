---
layout: page
title: Dissemination
lang: en
permalink: /en/divulgacion/
---

This is a selection my most recent technical speaking (<span style="background-color: whitesmoke;">grey background</span>) and dissemination activities for wider audiences (<span style="background-color: lavenderblush;">pink background</span>) that I enjoy so much.

{%- assign activities = site.activities -%}
{%- assign grouped_by_year = activities | group_by_exp: "post","post.date | date: '%Y' " -%}

{%- for year_item in grouped_by_year reversed -%}
<span style="display: block; ">
  <h2>{{ year_item.name }}</h2>
  {%- for activity in year_item.items reversed -%}
    {%- include activity.html -%}
  {%- endfor -%}
{%- endfor -%}
