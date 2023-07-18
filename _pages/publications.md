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

Recent publications I have contributed to. More information on the publications is available at <a href="https://scholar.google.com/citations?user=TRDUYkAAAAAJ&hl=en">Google Scholar</a>.

<h2 class="pub_title">Journals</h2>
{% bibliography -f papers -q @article[journal!=CoRR]* %}

<h2 class="pub_title">Conferences</h2>
{% bibliography -f papers -q @inproceedings %}

<h2 class="pub_title">Books</h2>
{% bibliography -f papers -q @book* %}
</div>
