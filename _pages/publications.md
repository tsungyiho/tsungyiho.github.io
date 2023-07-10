---
layout: page
permalink: /publications/
title: publications
description: 
years: [2023, 2022, 2021, 2020, 2019]
patentyears: [2022]
nav: true
order: 5
---
<!-- _pages/publications.md -->
<div class="publications">

More information on the publications is available at <a href="https://scholar.google.com/citations?user=TRDUYkAAAAAJ&hl=en">Google Scholar</a>.

<h3 class="pub_title">referred journals</h3>
{% bibliography -f papers -q @article[journal!=CoRR]* %}

<h3 class="pub_title">referred conferences</h3>
{% bibliography -f papers -q @inproceedings %}

<h3 class="pub_title">books</h3>
{% bibliography -f papers -q @book* %}
</div>
