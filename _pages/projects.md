---
layout: page
permalink: /publications/
title: Projects
description: Projects by categories in reversed chronological order. 
years: [2022,2021,2020]
nav: true
nav_order: 1
---
<!-- _pages/projects.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
