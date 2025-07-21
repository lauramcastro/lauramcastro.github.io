---
layout: page
title: Teaching
lang: en
permalink: /en/docencia/
---

I coordinate and teach these courses:
<div style="columns: 2 200px;">
<div class="card">
  <img src="/assets/software-architecture.png" alt="Software Architecture" style="width: 100%">
  <div class="card__text" style="text-size: small;">
    <br/>
    <h1>Software Architecture</h1>
    <p>Compulsory subject for 3rd-year students of the Degree in Computer Engineering at University of A Coruña with a concentration on Software Engineering. Elective subject for 4th-year students of the same degree with a concentration on Computer Science.</p>
    <br/><br/>
    <p><button><a href="https://www.udc.es/en/cufie/GD/consulta-guias-docentes/" style="color: white;">Teaching guide</a></button></p>
  </div>
</div>
<div class="card">
  <img src="/assets/software-testing.jpg" alt="Software Testing" style="width: 100%">
  <div class="card__text" style="text-size: small;">
    <br/>
    <h1>Software Validation and Verification</h1>
    <p>Compulsory subject for 4th-year students of the Degree in Computer Engineering at University of A Coruña with a concentration on Software Engineering. Elective subject for 4th-year students of the same degree with a concentration on Computer Science.</p>
    <p><button><a href="https://www.udc.es/en/cufie/GD/consulta-guias-docentes/" style="color: white;">Teaching guide</a></button></p>
  </div>
</div>
</div>
<br/>

If you're a student and are on the look for a supervisor for your degree, masters or PhD project, and you'd like to work with BEAM technologies (Erlang, Elixir, Gleam...), or in test automation, or distributed systems, <a href="mailto:lcastro@udc.gal">get in touch</a>.

Do so too if you're interested in transversal aspects of technology, such as social networks, software societal impact, or free software!

These are some examples of student projects I've supervised:

{%- assign students = site.students -%}
{%- assign grouped_by_year = students | group_by_exp: "post","post.date | date: '%Y' " -%}

{%- for year_item in grouped_by_year reversed -%}
<span style="display: block; ">
  <h2>{{ year_item.name }}</h2>
  {%- for student in year_item.items reversed -%}
    {%- include student.html -%}
  {%- endfor -%}
{%- endfor -%}