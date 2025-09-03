---
layout: page
title: Publications
lang: en
permalink: /en/publicacions/
---

I conduct multidisciplinary research.

Lately, I'm involved in research on **software engineering teaching/learning processes** (with special focus on **software architecture**), but previously I've worked on **software testing** (automated, model, and property-based testing), applied to software in general, but also to **distributed, concurrent, functional systems** in particular, more specifically in the context of the **[BEAM][beam]{:target="_blank"}**. 

I'm also very interested in the analysis of the **societal impact of technology** from a **feminist** perspective. 

If you happen to be interested in these or related areas, I am always open to collaboration!

Here are some of my latest publications (<span style="background-color: whitesmoke;">grey background</span> highlights journal articles; <span style="background-color: lavenderblush;">pink background</span> is used in other cases). If you cannot access the manuscripts using the provided links, do not hesitate to <a href="mailto:lcastro@udc.gal">contact me</a> and ask me for a copy.

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

[beam]: https://www.erlang.org/blog/a-brief-beam-primer