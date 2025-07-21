---
layout: page
title: Docencia
lang: gl
permalink: /docencia/
---

Coordino e imparto aulas das materias:
<div style="columns: 2 200px; column-gap: 20px; row-gap: 20px;">
<div class="card">
  <div class="card__text" style="text-size: small;">
    <br/>
    <h1>Arquitectura do Software</h1>
    <p>Materia obrigatoria para o estudantado do 3º curso do Grao en Enxeñaría Informática da Universidade da Coruña, na mención en Enxeñaría do Software (segundo cuadrimestre). Materia optativa para o estudantado da mención en Computación (primeiro cuadrimestre).</p>
    <p><button><a href="https://www.udc.es/gl/cufie/GD/consulta-guias-docentes/" style="color: white;">Guía docente</a></button></p>
  </div>
</div>
<div class="card">
  <div class="card__text" style="text-size: small;">
    <br/>
    <h1>Validación e Verificación do Software</h1>
    <p>Materia obrigatoria do 4º curso do Grao en Enxeñaría Informática da Universidade da Coruña, na mención en Enxeñaría do Software (1º cuadrimestre). Optativa na mención en Computación (2º cuadrimestre).</p>
    <p><button><a href="https://www.udc.es/gl/cufie/GD/consulta-guias-docentes/" style="color: white;">Guía docente</a></button></p>
  </div>
</div>
</div>

Se es estudante e buscas alguén que supervise o teu TFG, TFM ou proxecto de tese de doutoramento, e che apetece traballar con tecnoloxías da BEAM (Erlang, Elixir, Gleam...), ou en automatización de probas, ou con sistemas distribuídos, <a href="mailto:lcastro@udc.gal">contacta comigo</a>.

Faino tamén se tes interese en aspectos transversais da tecnoloxía, como as redes sociais, o impacto do software na sociedade, ou o software libre!

<div id="student-projects">Velaquí algúns exemplos de proxectos do estudantado que supervisei:</div>

{%- assign students = site.students -%}
{%- assign grouped_by_year = students | group_by_exp: "post","post.date | date: '%Y' " -%}

{%- for year_item in grouped_by_year reversed -%}
<span style="display: block; ">
  <h3>{{ year_item.name }}</h3>
  {%- for student in year_item.items reversed -%}
    {%- include student.html -%}
  {%- endfor -%}
{%- endfor -%}