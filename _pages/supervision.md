---
title: "Home"
layout: homelay
sitemap: false
permalink: /supervision/
date: "12-03-2025"
---

{% if site.data.people %}

<div class="jumbotron">
  <h3>Students and Mentoring</h3>
  <ul>
    {% for student in site.data.people %}
      <li>
        {{ student.name }}, {{ student.location }} ({{ student.degree }}) [{{ student.year }}, {{ student.duration }}]
        <br/>
        <p><i> {{ student.subject }} </i></p>
      </li>
    {% endfor %}
  </ul>
</div>
{% endif %}