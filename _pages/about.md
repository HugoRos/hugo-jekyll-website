---
title: "About"
layout: gridlay
sitemap: false
permalink: /about/
date: 13-03-2025
---

## About

{% for member in site.data.pi %}

<div class="jumbotron">
<div class="row">
<div class="col-sm-4">
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-8 col-xs-12">
  <h3>{{ member.name }}</h3>
  <h4><i>{{ member.info }}</i></h4>

  <h6>Teaching in the {{ member.teaching }}.</h6>
  <h6>Research activities at {{ member.research }}.</h6>
  {% if member.email %}<a href="mailto:{{ member.email }}" target="_blank"><i class="fa fa-envelope-square fa-3x"></i></a> {% endif %}
  {% if member.cv %} <a href="{{ site.url }}{{ site.baseurl }}/{{ member.cv }}" target="_blank"><i class="ai ai-cv-square ai-3x"></i></a> {% endif %}
  {% if member.scholar %} <a href="{{ member.scholar }}" target="_blank"><i class="ai ai-google-scholar-square ai-3x"></i></a> {% endif %}
  {% if member.orcid %} <a href="{{ member.orcid }}" target="_blank"><i class="ai ai-orcid-square ai-3x"></i></a> {% endif %}
  {% if member.hal %} <a href="{{ member.hal }}" target="_blank"><i class="ai ai-hal-square ai-3x"></i></a> {% endif %}
  {% if member.github %} <a href="{{ member.github }}" target="_blank"><i class="fa fa-github-square fa-3x"></i></a> {% endif %}
  {% if member.researchgate %} <a href="{{ member.researchgate }}" target="_blank"><i class="ai ai-researchgate-square ai-3x"></i></a> {% endif %}

  <ul style="overflow: hidden">
    {% for education in member.education %}
      <li>{{ education | replace: "-","&#8211;" }}</li>
    {% endfor %}
  </ul>

</div>
</div>
</div>
{% endfor %}

{% if site.data.awards %}

<div class="jumbotron">
  <h3>Awards</h3>
  <ul>
    {% for award in site.data.awards %}
      <li>{{ award.name | replace: "-","&#8211;" }}</li>
    {% endfor %}
  </ul>
</div>
{% endif %}

<div class="jumbotron">
  <h3>Editorial reviewing and expertise</h3>
  <ul>
    {% if site.data.journals %}
    <li>Reviews in peer-reviewed journals : 
      <ul>
        {% for journal in site.data.journals %}
        <li>{{ journal.name }}</li>
        {% endfor %}
      </ul>
    </li>
    {% endif %}
    <li>Participation in conference commitee</li>
    <ul>
      <li>ORASIS 2019 (program commitee)</li>
    </ul>
    <li>Reviews of project proposal</li>
    <ul>
      <li>ANR</li>
    </ul>
    <li>PhD thesis commitee</li>
    <ul>
      <li>Member of the follow-up commitee of Cassandra Céré's PhD thesis (LARIS Laboratory)<br/>
        <i>MRI and machine learning for neurology in veterinary imaging.</i>
      </li>
    </ul>
  </ul>
</div>

<div class="jumbotron">
  <h3>Scientific responsabilities</h3>
  <ul>
    <li>[2018-2023] Co-representative of team-group CAVITI in the WP4 (Multidimensional image processing) of LABEX Primes.</li>
  </ul>
</div>

<div class="jumbotron">
  <h3>Teaching responsabilities</h3>
  <ul>
    <li>[2023 - ...] Supervisor of internships in the Computer Science Departement (IUT Saint-Dié).</li>
    <li>[2022-2023] Supervisor of Web development track in BUT MMI.</li>
    <li>[2021-2023] Supervisor of several SAés in BUT MMI (IUT Clermont-Ferrand, Site du Puy-en-Velay).</li>
    <li>[2019-2022] Supervisor of the tutorship projects of Licence Métiers du Numérique.</li>
    <li>[2021-2023] Supervisor of <i>Internet of Things</i> module in the Master 2 Computer Science - 3D and Artificial Intelligence (ISIMA Clermont-Ferrand).</li>
    <li>[2017-2021] Supervisor of the tutorship projects of DUT Métiers du Multimédia et de l'Internet (MMI, IUT Clermont-Ferrand, Site du Puy-en-Velay).</li>
  </ul>
</div>

<div class="jumbotron">
  <h3>Other responsabilities</h3>
  <ul>
    <li>[2022-2023] Elected member of the teacher and university lecturer commission of IUT Clermont-Auvergne.</li>
  </ul>
</div>


<div class="jumbotron">
  <h4>Affiliations</h4>
  <div style='display:block; text-align:center; margin-left:auto; margin-right:auto;'>
  {% for funder in site.data.funders %}<a href="{{ funder.url }}" target="_blank"><img src='{{ site.url }}{{ site.baseurl }}/images/{{ funder.image }}' style='max-height: 80px; max-width: 500px; margin: 1%'/></a>{% endfor %}
  </div>
</div>
