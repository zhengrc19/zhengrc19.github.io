---
layout: page
permalink: /publications/
title: Publications
description: My publications in reversed chronological order. You could also visit my <a href='https://scholar.google.com/citations?user=gwUGHwsAAAAJ'>Google Scholar</a> page.
years: [2023, 2019]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

(* denotes equal contribution)

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
