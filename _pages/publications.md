---
title: Xiaojun Chang's publications
layout: default
excerpt: Xiaojun Chang's publications
permalink: /publications
---
# SELECTED PUBLICATIONS

[DBLP](https://dblp.org/pers/c/Chang:Xiaojun.html)  [Google Scholar](https://scholar.google.com/citations?hl=en&user=8suupocAAAAJ)

## CONFERENCE PAPERS

{% for publication in site.data.conference_papers %}

{% include publications.html %}

{% endfor %}

<p>&nbsp;</p>

## JOURNAL PAPERS

{% for publication in site.data.journal_papers %}

{% include publications.html %}

{% endfor %}

<p>&nbsp;</p>

{% assign numOfJournals = loopindex %}

## PREPRINTS

{% for publication in site.data.reports %}

{% include publications.html %}

{% endfor %}

