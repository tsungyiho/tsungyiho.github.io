---
layout: page
permalink: /publications/
title: Publications
description: Publication retrieved from DBLP. Full publications is available at Google Scholar.
icon: <i class="fa-solid fa-book"></i>
nav: true
order: 3
---
<!-- _pages/publications.md -->
<div class="publications">

Retrieved from <a href="https://dblp.org/pid/63/4181.html">DBLP</a>. Full publications is available at <a href="https://scholar.google.com/citations?user=TRDUYkAAAAAJ&hl=en">Google Scholar</a>.

<h2 class="pub_title">Journals</h2>
<div class="journal">
{% bibliography -f papers -q @article[journal!=CoRR]* %}
</div>

<h2 class="pub_title">Conferences</h2>
<div class="conference">
{% bibliography -f papers -q @inproceedings %}
</div>

<h2 class="pub_title">Books</h2>
<div class="book">
{% bibliography -f papers -q @book* %}
</div>

</div>
