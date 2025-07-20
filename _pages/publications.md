---
layout: page
permalink: //..//https://scholar.google.com/citations?user=oWJY3CEAAAAJ&hl
permalink: /publications/
title: Publications
years: [2025, 2024, 2023]
nav: true
nav_order: 1
---
For a complete list of my publications, view my [Google Scholar Page](https://scholar.google.com/citations?user=oWJY3CEAAAAJ&hl)
<!-- _pages/publications.md -->


<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
