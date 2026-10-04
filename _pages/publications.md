---
layout: page
permalink: /publications/
title: publications
description: Journal articles, conference papers and repository working papers.
nav: true
nav_order: 2
---

Publication list checked against [ORCID](https://orcid.org/0000-0003-4204-3474) on 4 October 2026. Journal citations use the issue year where available.

**\* Corresponding author.** An asterisk after my name identifies publications for which I am a corresponding author.

{% include bib_search.liquid %}

## Journal articles
<div class="publications">
{% bibliography --query @article %}
</div>

## Conference papers
<div class="publications">
{% bibliography --query @inproceedings %}
</div>

## Repository working papers
These records relate to articles listed above and are not additional journal publications.
<div class="publications">
{% bibliography --query @misc %}
</div>
