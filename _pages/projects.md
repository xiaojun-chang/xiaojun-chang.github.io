---
title: Xiaojun Chang's Projects
layout: default
excerpt: Xiaojun Chang's projects
permalink: /projects
---

| <a href="mailto:cxj273@gmail.com" target="_blank" style="text-align:center; display:block"><i class="fa fa-envelope ai-3x"></i></a> | <a href="{{ site.google_scholar_url }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-google ai-3x"></i></a> | <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-linkedin ai-3x"></i></a> | <a href="https://research.monash.edu/en/persons/xiaojun-chang" target="_blank" style="text-align:center; display:block"><i class="fa fa-graduation-cap ai-3x"></i></a> |
  
# Projects

{% for project in site.data.projects %}

{% include projects.html %}

{% endfor %}
