---
layout: page
permalink: /publications/
title: selected publications
description: A full list of my publications is available on <a href="https://scholar.google.com/citations?user=usl__skAAAAJ&hl=en">Google Scholar</a> 
years: [2021,2019,2018,2017,2016,2015]
nav: true
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
