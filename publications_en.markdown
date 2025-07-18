---
layout: page
title: Publications
lang: en
permalink: /en/publicacions/
---

<div style="font-size: small; text-align: right">
More references: 
<a href="https://orcid.org/0000-0002-3028-1523" class="articles" rel="external nofollow noopener" target="_blank">ORCID</a>
<a href="https://dialnet.unirioja.es/servlet/autor?codigo=2608289" class="articles" rel="external nofollow noopener" target="_blank">DialNET</a>
</div>
{%- assign articles = site.articles -%}
{%- assign grouped_by_year = articles | group_by_exp: "post","post.date | date: '%Y' " -%}

{%- for year_item in grouped_by_year reversed -%}
<span style="display: block; ">
  <h2>{{ year_item.name }}</h2>
  {%- for article in year_item.items reversed -%}
    {%- include article.html -%}
  {%- endfor -%}
{%- endfor -%}