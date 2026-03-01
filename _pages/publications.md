---
layout: page
permalink: /publications/
title: publications
description: Selected publications. Find all on Google Scholar <a href="https://scholar.google.de/citations?user=itIWDO8AAAAJ">(click here)</a>.
years: [2026, 2025, 2024, 2023, 2022, 2021, 2020, 2019]
nav: true
nav_order: 2
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
