---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2023, 2021, 2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h4 class="year">{{y}}</h4>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
