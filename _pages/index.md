---
title: Prof Xiaojun Chang@UTS
layout: default
excerpt: Home page of Xiaojun Chang's website
permalink: /
---

| <a href="mailto:cxj273#gmail.com" target="_blank" style="text-align:center; display:block"><i class="fa fa-envelope ai-3x"></i></a> | <a href="{{ site.google_scholar_url }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-google ai-3x"></i></a> | <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-linkedin ai-3x"></i></a> | <a href="https://profiles.uts.edu.au/XiaoJun.Chang" target="_blank" style="text-align:center; display:block"><i class="fa fa-graduation-cap ai-3x"></i></a> |

<img class="profile-picture" src="{{site.url}}{{site.baseurl}}/images/profile-picture/profile_picture.jpg" />

Greetings! Dr Xiaojun Chang is a Full Professor affiliated with the Australian Artificial Intelligence Institute within the Faculty of Engineering and Information Technology at the University of Technology Sydney. As the Director of [The ReLER Lab](http://reler.net/){:target="_blank"}, Prof. Chang leads cutting-edge research in the field of artificial intelligence. He also holds the position of Visiting Professor at Mohamed bin Zayed University of Artificial Intelligence (MBZUAI). Before joining UTS, Prof. Chang served as an Associate Professor at the School of Computing Technologies at RMIT University, Australia. His academic journey has encompassed a diverse range of roles, including a Postdoctoral Research Fellowship at the School of Computer Science, Carnegie Mellon University, as well as Lecturer and Senior Lecturer positions within the Faculty of Information Technology at Monash University, Australia. Prof. Chang's research is centered on three primary areas of expertise: Video Analysis, Multi-Modal Foundation Models, and Medical Foundation Models. His groundbreaking work in these domains underscores his commitment to advancing artificial intelligence and its applications. Through his pioneering work, Prof. Chang continues to play a pivotal role in advancing the field of artificial intelligence, making significant strides in the realm of automatic content analysis and deep learning.

Prof. Chang has also been involved in developing deep learning models that automatically annotate disease labels from multi-source patient data, such as data from medical records in Intensive Care Units (ICUs). This project has had a significant impact on healthcare and management in the ICU at the Royal Brisbane and Women's Hospital. Automated diagnosis code annotation can greatly enhance the quality and management of healthcare for both patients and caregivers. More recently, Prof. Chang collaborated with researchers from the Australian Alliance for Artificial Intelligence in Healthcare to develop an automatic report generation system for critically ill COVID-19 patients using deep learning techniques and the US public COVID-19 CT scan dataset. The system has achieved state-of-the-art performance on report generation and can generate reports that are very close to doctor-written reports. This work has received extensive media coverage from major news outlets.

Dr Chang earned his Ph.D. degree from the Centre for Artificial Intelligence and the Faculty of Engineering and Information Technology at the University of Technology Sydney, under the supervision of [Prof. Yi Yang](http://www.cs.cmu.edu/~yiyang/){:target="_blank"}. During his doctoral studies, he was mentored by Prof. [Feiping Nie](http://www.escience.cn/people/fpnie/){:target="_blank"} and [Yaoliang Yu](https://cs.uwaterloo.ca/~y328yu/){:target="_blank"}. His research during this period focused mainly on developing machine learning algorithms and applying them to multimedia analysis and computer vision. Dr Chang also holds master's and bachelor's degrees from the School of Information Science and Technology and the School of Physics, both from Northwest University. During this time, his research interests were in the areas of FPGA and VLSI.

## Research Interests

Dr Chang's research interests revolve around developing structured machine learning models for computer vision and multimedia tasks. His work primarily centers on exploring the information contained within videos and advancing artificial intelligence systems. His recent research topics include:

- Video Analysis, including event detection, object detection, segmentation.

- Multi-Modal Foundation Models.

- Medical Foundation Models.

- Multi-Agent Reinforcement Learning.


## News

<table>
{% for article in site.data.news %}
<tr>
{% include news.html %}
</tr>
{% endfor %}
</table>
