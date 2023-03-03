---
layout: page
permalink: /publications/
title: Publications
description: A collection of relevant research and non-peer reviewed work.
years: [2023, 2022, 2021, 2020, 2019, 2018]
nav: true
order: 3
group_by: abbr
---
<!-- Pubs -->
<h2>Research Papers</h2>
<div class="publications">
  {%- for y in "2022" %}
    <h5 class="year">{{y}}</h5>
    {% bibliography -f papers -q @*[year = {{y}}]* %}
  {% endfor %}
</div>

<div class="publications">
  {%- for y in "2019" %}
    <h5 class="year">{{y}}</h5>
    {% bibliography -f papers -q @*[year = {{y}}]* %}
  {% endfor %}
</div>

<!-- <h2>Theses / Student Projects</h2>
<div class="publications">
  {%- for y in "2021" %}
    <h5 class="year">{{y}}</h5>
    {% bibliography -f studentprojects -q @*[year = {{y}}]* %}
  {% endfor %}
  {%- for y in "2020" %}
    <h5 class="year">{{y}}</h5>
    {% bibliography -f studentprojects -q @*[year = {{y}}]* %}
  {% endfor %}
</div> -->