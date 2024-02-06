---
layout: softwares
permalink: /softwares/
title: softwares
description: softwares
years: [2024, 2023, 2018, 2011]
nav: true
nav_order: 4
---
<!-- _pages/publications.md -->

<!-- <p>An up-to-date list is available on <a href="https://scholar.google.com/citations?user=qNk6tgcAAAAJ" target="_blank" rel="noopener noreferrer">Google Scholar</a>.</p> -->

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>