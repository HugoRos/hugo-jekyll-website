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
  <h4>Main research interests and topics</h4>
  <ul>
    <li>Image analysis and processing applied to biomedical data.</li>
    <li>Feature extraction and segmentation of region of interest.</li>
    <li>Discrete objects analysis.</li>
    <li>Imaging acquisition systems from pre-clininal (microscopy, phase contrast imaging) to clinical (MRI, Scanner).</li>
  </ul>
  </div>
</div>

#### Some selected research activities
<div class="jumbotron">
<h5>Extraction and reconstruction of mouse hepatic vascular network.</h5>
<p class="text-justify">From phase contrast images, we were able to create the proof of concept about extraction of mouse hepatic vascular network [Work presented at the NEUBIAS conference in 2018].
All methodologies employed (see figure below) allowed us to assess the feasability of a complete pipeline from data acquisition, to analysis of them and finally, high level information extraction.</p>

<center>
  <img src="{{ site.url }}{{ site.baseurl }}/images/neubias.png" alt="extraction pipeline of vascular network." width="100%">
</center>

<p class="text-justify">
This topic consists of my <b>main research activity</b> and since i joined LORIA lab (ADAGIO team) i am even more convinced that 
we need to focus our effort on the nature of studied discrete objects (example below of the graph representation of a vascular network), refine them and make good use of the information bring by their <b>geometrical properties</b>. </p>

<center>
  <img src="{{ site.url }}{{ site.baseurl }}/images/SquelGraphVascNetwork.png" alt="graph representation of a vascular network." width="100%">
</center>
<p class="text-justify">
Two work axis are now clearly my priority: first, improve the accuracy of the segmentation methods and tools, second, develop methodologies to tackle the discontinuities problem always present in this kind of network application.
</p>
</div>

<div class="jumbotron">
<h5>Mixed reality impact in a clinical context (2016-2020)</h5>

<p class="text-justify">
In the scope of athe AVACM project (CNRS PEPS INSIS), we were interested in measuring the impact of mixed reality in a medical context application.
This project was designed to bring a specific type of mixed reality equipment (Microsoft HoloLens) towards patient to assess its acceptability and benefit in a clinical context.
</p>

<p class="text-justify">
This study was performed over 30 patients and showed that this kind of technology can be used in a medical context and present a good acceptability among the patient sample who participate. Moreover, a learning by the gesture can be performed and there improve the knowledge acquired 
by the patient [Barret-Grimault et al. (2019), Rositi et al. (2021), Appadoo et al. (2023)].
</p>
<center>
  <img src="{{ site.url }}{{ site.baseurl }}/images/avacm.jpg" alt="Illustration of a workshop using mixed reality in a clinical context." width="100%">
</center>
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