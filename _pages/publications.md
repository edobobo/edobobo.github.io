---
layout: page
permalink: /publications/
title: publications
description: 
years: [2025, 2024, 2023, 2022, 2021, 2020]
nav: true
---

<div class="container" style="margin-top:32px;">
{% for y in page.years %}
  <h2 class="section-title">{{ y }}</h2>
  <div class="pub-year reveal">
    {% bibliography -f papers -q @*[year={{y}}]* %}
  </div>
{% endfor %}
</div>
