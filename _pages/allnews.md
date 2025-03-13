---
title: "News"
layout: textlay
sitemap: false
permalink: /allnews.html
date: 13-03-2025
---

## News

<div class="jumbotron">
{% for article in site.data.news %}
<h5>{{ article.date }}</h5>

<i>{{ article.headline }}</i>

<p class="text-justify">{{ article.body }}</p>
{% endfor %}

</div>
