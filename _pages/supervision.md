---
title: "Home"
layout: gridlay
sitemap: false
permalink: /supervision/
date: "12-03-2025"
---

{% if site.data.people %}

<h2>Students and Mentoring</h2>

<div class="jumbotron">
  <h3>PhD Thesis</h3>
  <ul>
    {% for student in site.data.people %}
    {% if student.degree == "PhD Thesis" %}
      <li>
        {{ student.name }}, {{ student.location }} ({{ student.degree }}) [{{ student.year }}, {{ student.duration }}]. {{ student.supervision }}.
        <br/>
        <p><i> {{ student.subject }} </i></p>
      </li>
    {% endif %}
    {% endfor %}
  </ul>
</div>

<div class="jumbotron">
  <h3>Post-doc</h3>
  <ul>
    {% for student in site.data.people %}
    {% if student.degree contains "Post-doc" %}
      <li>
        {{ student.name }}, {{ student.location }} ({{ student.degree }}) [{{ student.year }}, {{ student.duration }}]. {{ student.supervision }}.
        <br/>
        <p><i> {{ student.subject }} </i></p>
      </li>
    {% endif %}
    {% endfor %}
  </ul>
</div>

<div class="jumbotron">
  <h3>Internships and student projects</h3>
  <ul>
    {% for student in site.data.people %}
    {% if student.degree contains "internship" or student.degree contains "project"%}
      <li>
        {{ student.name }}, {{ student.location }} ({{ student.degree }}) [{{ student.year }}, {{ student.duration }}]. {{ student.supervision }}.
        <br/>
        <p><i> {{ student.subject }} </i></p>
      </li>
    {% endif %}
    {% endfor %}
  </ul>
</div>
{% endif %}