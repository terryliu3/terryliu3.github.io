---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

  <p>See also my <a href="https://scholar.google.com/citations?user=IUnFMnAAAAAJ">Google Scholar</a> profile.</p>

  <h2>conference papers</h2>
  {% bibliography -f papers -q @inproceedings %}

  <h2>preprints</h2>
  {% bibliography -f papers -q @*[preprint=true]* %}

</div>
