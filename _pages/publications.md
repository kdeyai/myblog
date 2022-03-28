---
layout: page
permalink: /publications/
title: publications
description: I don't have any publication yet as soon as I have one I will update it .
years:
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
