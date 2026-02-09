---
title: "Teaching"
layout: gridlay
sitemap: false
permalink: /teaching/
date: 09-02-2026
---

## Teaching activities
All my actual teaching activities (and most of my previous activities) are focused on computer science, programming and/or image processing.
<div class="jumbotron col-md-12">
<h4>Actual teachings</h4>

In the Computer science department of IUT Saint-Dié.
<table class="table table-dark">
  <thead>
  <tr>
    <th>Year</th>
    <th>Course</th>
    <th>Degree</th>
    <th>Program</th>
    <th style="text-align: right">Total hours</th>
  </tr> 
  </thead>
  <tbody>
    {% for course in site.data.teachings %}
        {% if course.status contains "actual" and course.school contains "Dié" %}
            <tr>
                <td>{{ course.year }}</td>
                <td>{{ course.name }}</td>
                <td>{{ course.degree }}</td>
                <td>{{ course.program }}</td>
                <td style="text-align: right">{{ course.hours }}</td>
            </tr>
        {% endif %}  
    {% endfor %}
  </tbody>
</table>

In the Computer science department of IUT Nancy-Charlemagne.
<table class="table table-dark">
  <!-- <thead>
  <tr>
    <th>Year</th>
    <th>Course</th>
    <th>Degree</th>
    <th>Program</th>
    <th>Total hours</th>
  </tr> 
  </thead> -->
  <tbody>
    {% for course in site.data.teachings %}
        {% if course.school contains "Charlemagne" %}
            <tr>
                <td>{{ course.year }}</td>
                <td>{{ course.name }}</td>
                <td>{{ course.degree }}</td>
                <td>{{ course.program }}</td>
                <td style="text-align: right">{{ course.hours }}</td>
            </tr>
        {% endif %}  
    {% endfor %}
  </tbody>
</table>
</div>

In the Computer science department of Faculté de Sciences et Technologies (Université de Lorraine).
<table class="table table-dark">
  <!-- <thead>
  <tr>
    <th>Year</th>
    <th>Course</th>
    <th>Degree</th>
    <th>Program</th>
    <th>Total hours</th>
  </tr> 
  </thead> -->
  <tbody>
    {% for course in site.data.teachings %}
        {% if course.school contains "FST" %}
            <tr>
                <td>{{ course.year }}</td>
                <td>{{ course.name }}</td>
                <td>{{ course.degree }}</td>
                <td>{{ course.program }}</td>
                <td style="text-align: right">{{ course.hours }}</td>
            </tr>
        {% endif %}  
    {% endfor %}
  </tbody>
</table>
</div>

<div class="jumbotron col-sm-12">
<h4>Previous teachings</h4>
The below listing is non-exhaustive and has for sole purpose to show the main courses and their diversities that I dispensed in my previous teaching experiences.<br/>

In the Computer science department of IUT Saint-Dié.
<table class="table table-dark">
  <thead>
  <tr>
    <th>Year</th>
    <th>Course</th>
    <th>Degree</th>
    <th>Program</th>
    <th style="text-align: right">Total hours</th>
  </tr> 
  </thead>
  <tbody>
    {% for course in site.data.teachings %}
        {% if course.status contains "previous" and course.school contains "Saint-Dié" %}
            <tr>
                <td>{{ course.year }}</td>
                <td>{{ course.name }}</td>
                <td>{{ course.degree }}</td>
                <td>{{ course.program }}</td>
                <td style="text-align: right">{{ course.hours }}</td>
            </tr>
        {% endif %}  
    {% endfor %}
  </tbody>
</table>

In the Master Program 3D and Artificial intelligence of ISIMA, Clermont-Ferrand.
<table class="table table-dark">
  <thead>
  <tr>
    <th>Year</th>
    <th>Course</th>
    <th>Degree</th>
    <th>Program</th>
    <th style="text-align: right">Total hours</th>
  </tr> 
  </thead>
  <tbody>
    {% for course in site.data.teachings %}
        {% if course.school contains "isima" %}
            <tr>
                <td>{{ course.year }}</td>
                <td>{{ course.name }}</td>
                <td>{{ course.degree }}</td>
                <td>{{ course.program }}</td>
                <td style="text-align: right">{{ course.hours }}</td>
            </tr>
        {% endif %}  
    {% endfor %}
  </tbody>
</table>

In the department <i>Métiers du Multimédia et de l'Internet</i> (MMI) of IUT Clermont-Auvergne (Puy-en-Velay).
<table class="table table-dark">
  <thead>
  <tr>
    <th>Year</th>
    <th>Course</th>
    <th>Degree</th>
    <th>Program</th>
    <th style="text-align: right">Total hours</th>
  </tr> 
  </thead>
  <tbody>
    {% for course in site.data.teachings %}
        {% if course.school contains "Le Puy" %}
            <tr>
                <td>{{ course.year }}</td>
                <td>{{ course.name }}</td>
                <td>{{ course.degree }}</td>
                <td>{{ course.program }}</td>
                <td style="text-align: right">{{ course.hours }}</td>
            </tr>
        {% endif %}  
    {% endfor %}
  </tbody>
</table>

During my PhD, i gave teachings at INSA Lyon in both the Preparatory Level departement and Bio-informatics departement.
<table class="table table-dark">
  <thead>
  <tr>
    <th>Year</th>
    <th>Course</th>
    <th>Degree</th>
    <th>Program</th>
    <th style="text-align: right">Total hours</th>
  </tr> 
  </thead>
  <tbody>
    {% for course in site.data.teachings %}
        {% if course.school contains "INSA" %}
            <tr>
                <td>{{ course.year }}</td>
                <td>{{ course.name }}</td>
                <td>{{ course.degree }}</td>
                <td>{{ course.program }}</td>
                <td style="text-align: right">{{ course.hours }}</td>
            </tr>
        {% endif %}  
    {% endfor %}
  </tbody>
</table>
</div>