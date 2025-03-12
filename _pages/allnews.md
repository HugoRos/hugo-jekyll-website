---
title: "News"
layout: textlay
sitemap: false
permalink: /allnews.html
date: 12-03-2025
---

## News

<div class="jumbotron">
{% for article in site.data.news %}
<b>{{ article.date }}</b>

{{ article.headline }}
{% endfor %}

</div>
