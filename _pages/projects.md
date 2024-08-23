---
layout: page
permalink: /projects/
title: projects
description: Some Curated Projects that I have been a part of!
years: [Security,NLP,ML, Power Electronics, RL, Cloud, Databases]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f projects -q @*[year={{y}}]* %}
{% endfor %}

</div>
