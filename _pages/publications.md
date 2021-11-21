---
title: Xiaojun Chang's publications
layout: default
excerpt: Xiaojun Chang's publications
permalink: /publications
---

| <a href="mailto:cxj273#gmail.com" target="_blank" style="text-align:center; display:block"><i class="fa fa-envelope ai-3x"></i></a> | <a href="{{ site.google_scholar_url }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-google ai-3x"></i></a> | <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-linkedin ai-3x"></i></a> | <a href="https://www.rmit.edu.au/contact/staff-contacts/academic-staff/c/chang---xiaojun" target="_blank" style="text-align:center; display:block"><i class="fa fa-graduation-cap ai-3x"></i></a> |

# SELECTED PUBLICATIONS

Full paper list can be found at [DBLP](https://dblp.org/pers/c/Chang:Xiaojun.html) and [Google Scholar](https://scholar.google.com/citations?hl=en&user=8suupocAAAAJ).

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


## PREPRINTS

{% for publication in site.data.reports %}

{% include publications.html %}

{% endfor %}

{% assign numOfJournals = loopindex %}



