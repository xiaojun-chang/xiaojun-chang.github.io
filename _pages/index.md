---
title: Xiaojun Chang@RMIT University
layout: default
excerpt: Home page of Xiaojun Chang's website
permalink: /
---

| <a href="mailto:cxj273@gmail.com" target="_blank" style="text-align:center; display:block"><i class="fa fa-envelope ai-3x"></i></a> | <a href="{{ site.google_scholar_url }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-google ai-3x"></i></a> | <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-linkedin ai-3x"></i></a> | <a href="https://research.monash.edu/en/persons/xiaojun-chang" target="_blank" style="text-align:center; display:block"><i class="fa fa-graduation-cap ai-3x"></i></a> |

<img class="profile-picture" src="{{site.url}}{{site.baseurl}}/images/profile-picture/profile_picture.jpg" />

Greetings! Dr Xiaojun Chang is a [Senior Lecturer](https://en.wikipedia.org/wiki/Senior_lecturer){:target="_blank"} at Vision & Lanugage Group, Department of Data Science and AI, Faculty of Information Technology, Monash University Clayton Campus, Australia. Dr Chang is an ARC Discovery Early Career Researcher Award (DECRA) Fellow between 2019-2021 (awarded in 2018).

Greetings! Dr Xiaojun Chang is an Associate Professor in School of Computing Technologies, RMIT University, Australia. He is an ARC Discovery Early Career Researcher Award (DECRA) Fellow between 2019-2021 (awarded in 2018).

Before joining RMIT, he was a Senior Lecturer in Vision & Lanugage Group, Department of Data Science and AI, Faculty of Information Technology, Monash University from December 2018 and July 2021. He was a Postdoc Research Associate in School of Computer Science, Carnegie Mellon University, working with [Prof. Alex Hauptmann](http://www.cs.cmu.edu/~alex/){:target="_blank"}. He has focused his research on exploring multiple signals (visual, acoustic, textual) for automatic content analysis in unconstrained or surveillence videos. His team has won multiple prizes from international grand challenges which hosted competitive teams from MIT, University of Maryland, Facebook AI Research (FAIR) and Baidu VIS, and aim to advance visual understanding using deep learning. For example, he won the first place in the TrecVID 2019 - Activity Extended Video (ActEV) challenge, which was held by National Institute of Standards and Technology, US.

Dr Chang also has been working on developing deep learning models to automatically annotate the disease labels from multi-source patient data (eg data from medical record) in Intensive Care Units (ICUs). The successful outcome of this project has greatly benefited health care and management in ICU of Royal Brisbane and Women&#39;s Hospital, considering that the automated diagnosis code annotation can significantly improve the quality and management of health care for both patients and caregivers. The outcome has been published in IEEE Transactions on Knowledge and Data Engineering in December 2016. Recently, he has successfully developed an automatic report generation system for critically ill COVID-19 patients using deep learning techniques with US public COVID-19 CT scan dataset. He collaborated with researchers from Australian Alliance for Artificial Intelligence in Healthcare on this project. The system achieves state-of-the-art performance on report generation and can generate reports very close to doctor handwritten report.

He received the Ph.D. degree in Centre for Artificial Intelligence & Faculty of Engineering and Information Technology, University of Technology Sydney, under the supervision of [Prof. Yi Yang](http://www.cs.cmu.edu/~yiyang/){:target="_blank"}. During his PhD study, he was sequentially mentored by Prof. [Feiping Nie](http://www.escience.cn/people/fpnie/){:target="_blank"} and [Yaoliang Yu](https://cs.uwaterloo.ca/~y328yu/){:target="_blank"}. His research focus in this period was mainly on developing machine learning algorithms and apply them to multimedia analysis and computer vision. He received his master and bachelor degrees from School of Information Science and Technology and School of Physics, both from Northwest University. In this period, his research interests were FPGA and VLSI.

## Research Interests

His general research interest is to develop structured machine learning models for computer vision and multimedia tasks. He mainly investigates how to explore the information contained in videos and develop the advanced artificial intelligence systems. Recently, he focuses on the following topics, include:

- Video Analysis, including event detection, object detection, segmentation.

- Multi-Agent Reinforcement Learning.

- Vision-Language Grounding, including vision-language navigation, vision-and-dialog navigation, and medical report generation.

- Automated Machine Learning (AutoML).


## News

<table>
{% for article in site.data.news %}
<tr>
{% include news.html %}
</tr>
{% endfor %}
</table>
