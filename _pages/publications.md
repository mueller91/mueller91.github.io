---
layout: page
permalink: /publications/
title: publications
description: Selected publications. Find all on Google Scholar <a href="https://scholar.google.de/citations?user=itIWDO8AAAAJ">(click here)</a>.
years: [2019, 2020, 2021]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
