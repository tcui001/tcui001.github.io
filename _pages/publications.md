---
layout: page
permalink: /publications/
title: publications
description: 
yearsj: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2011]
yearsb: [2019]
yearsc: [2018]
yearsp: [2024, 2023, 2022, 2021, 2020, 2019, 2018]
yearso: [2019, 2011]
nav: true
---
[preprints](#pre), [journal articles](#journal), [book chapters](#book), [conference articles](#conf), and [other works](#other) in reversed chronological order. 

### preprints {#pre}

<div class="publications">

{% for y in page.yearsp %}
  {% bibliography -f papers -q @techreport[year={{y}}]* %}
{% endfor %}

</div>

### journal articles {#journal}

<div class="publications">

{% for y in page.yearsj %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @article[year={{y}}]* %}
{% endfor %}

</div>

### book chapters {#book}

<div class="publications">

{% for y in page.yearsb %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @incollection[year={{y}}]* %}
{% endfor %}

</div>

### conference articles {#conf}

<div class="publications">

{% for y in page.yearsc %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @inproceedings[year={{y}}]* %}
{% endfor %}

</div>

### other works {#other}

<div class="publications">

{% for y in page.yearsp %}
  {% bibliography -f papers -q @misc[year={{y}}]* %}
{% endfor %}

</div>