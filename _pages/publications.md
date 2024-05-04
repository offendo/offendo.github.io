---
layout: page
permalink: /papers/
title: papers
description: 
nav: true
nav_order: 1
years: [2024, 2023, 2019]
---
<!-- _pages/papers.md -->
<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
