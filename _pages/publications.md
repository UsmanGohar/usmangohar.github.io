---
permalink: /publications/
nav: true
layout: forward
target: https://scholar.google.com/citations?user=oWJY3CEAAAAJ&hl
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
