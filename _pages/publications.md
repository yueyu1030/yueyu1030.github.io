---
layout: page
permalink: /publications/
title: Selected Publications
description: Publications by categories in reversed chronological order. Full list is available on my <a href="https://scholar.google.com/citations?hl=en&user=zQ3Jh6UAAAAJ"><b>Google Scholar</b></a>.
years: [2024, 2023, 2022, 2021, 2020, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
