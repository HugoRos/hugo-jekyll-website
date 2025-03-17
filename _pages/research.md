---
title: "Research"
layout: gridlay
sitemap: false
permalink: /research/
date: 12-03-2025
---

<style>
img{
  border-radius: 10px;
}
.col-md-3 {
  margin-top:10px;
  margin-bottom:10px;
  padding:0px;
  display:block;
  overflow:hidden;
  text-align:center;
  display: table-cell;
  background: white;
  border-radius: 20px;
  height: auto;
}
iframe {
  margin:0;
  padding:0;
  width: 175px;
  display: inline;
  vertical-align: middle;
}
</style>

## Research

<div class="jumbotron">
<div class="col-md-12 col-sm-12">
<h4>Example Research</h4>

Example description
</div>
</div>

{% if site.data.projects %}

<div class="jumbotron">
  <h3>Participation in funded projects</h3>
  <table class="table table-dark">
  <thead>
  <tr>
    <th>Name</th>
    <th>Date (duration)</th>
    <th>Project leader</th>
    <th>Project proposal</th>
    <th>Implication</th>
  </tr> 
  </thead>
  <tbody>
    {% for project in site.data.projects %}
      <tr>
        <td>{{ project.name }}</td>
        <td> {{ project.date }} ({{ project.duration}})</td>
        <td> {{ project.leader }}</td>
        <td> {{ project.track }}</td>
        <td> {{ project.implication }}</td>
      </tr>
    {% endfor %}
  </tbody>
  </table>

   <ul>
    {% for project in site.data.projects %}
      <li>
        {{ project.name }}<br/>
        <i>{{ project.subject }}</i>
      </li>
    {% endfor %}
  </ul>

</div>
{% endif %}

{% if site.data.grants %}

<div class="jumbotron">
  <h3>Grants</h3>
  <ul>
    {% for grant in site.data.grants %}
      <li style="margin: 10px">
        {{ grant.name }} ( {{ grant.year }}, {{ grant.duration }}) - {{ grant.allocation }}<br/>
        <i>{{ grant.subject }}</i>
      </li>
    {% endfor %}
  </ul>
</div>
{% endif %}