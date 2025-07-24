---
layout: page
title: Publicacións
lang: gl
permalink: /publicacions/
---

Fago investigación multidisciplinar.

A maioría do meu traballo ocorre no contexto da [BEAM][beam]{:target="_blank"}. Traballei en validación de software (automatización de probas, probas baseadas en modelos, probas baseadas en propiedades) en xeral, pero tamén especificamente de sistemas distribuídos, concorrentes e funcionais. Recentemente, estou participando en investigacións relacionadas coa docencia e a aprendizaxe na enxeñaría do software (con especial interese na arquitectura do software).

Alén diso, estou moi interesada na análise do impacto da tecnoloxía desde unha perspectiva feminista. 

Se che interesa algunha destas áreas, sempre estou disposta a colaborar!

Estas son algunhas das miñas publicacións recentes (os artigos en revista aparecen con <span style="background-color: whitesmoke;">fondo gris</span>, o resto de contribucións con <span style="background-color: lavenderblush;">fondo rosado</span>). Se non podes acceder aos orixinais mediante as ligazóns que se achegan, non dubides en <a href="mailto:lcastro@udc.gal">contactares comigo</a> para pedir unha copia.

<div style="font-size: small; text-align: right">
Máis referencias:
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