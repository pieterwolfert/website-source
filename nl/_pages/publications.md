---
layout: page
permalink: /nl/publicaties/
title: publicaties
lang: nl
lang-ref: pub-page
description: publicaties per jaar in omgekeerde chronologische volgorde (engelstalig)
years: [2022, 2021, 2020, 2019, 2018, 2015]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
