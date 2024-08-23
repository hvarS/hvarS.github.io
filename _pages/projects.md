---
layout: page
permalink: /projects/
title: projects
description: Some Curated Projects that I have been a part of!
years: [RL, Cloud, Databases,NLP,ML, Security, Power]
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
