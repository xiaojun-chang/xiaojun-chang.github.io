---
title: Prof Xiaojun Chang@UTS
layout: default
excerpt: Home page of Xiaojun Chang's website
permalink: /
---

| <a href="mailto:cxj273#gmail.com" target="_blank" style="text-align:center; display:block"><i class="fa fa-envelope ai-3x"></i></a> | <a href="{{ site.google_scholar_url }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-google ai-3x"></i></a> | <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-linkedin ai-3x"></i></a> | <a href="https://profiles.uts.edu.au/XiaoJun.Chang" target="_blank" style="text-align:center; display:block"><i class="fa fa-graduation-cap ai-3x"></i></a> |

<img class="profile-picture" src="{{site.url}}{{site.baseurl}}/images/profile-picture/profile_picture.jpg" />

Greetings! Dr Xiaojun Chang is a Professor at the Australian Artificial Intelligence Institute, Faculty of Engineering and Information Technology, University of Technology Sydney. He serves as the Director of [The ReLER Lab](http://reler.net/){:target="_blank"}, originally founded by [Prof. Yi Yang](http://www.cs.cmu.edu/~yiyang/){:target="_blank"}. Additionally, he is an Honorary Professor at the School of Computing Technologies, RMIT University, Australia. Prior to joining UTS, Dr Chang was an Associate Professor at the School of Computing Technologies, RMIT University, Australia. He has also worked as a Postdoctoral Research Fellow at the School of Computer Science, Carnegie Mellon University, and as a Lecturer and Senior Lecturer in the Faculty of Information Technology, Monash University, Australia. Dr Chang's research focuses on exploring multiple signals (visual, acoustic, textual) for automatic content analysis in unconstrained or surveillance videos. His team has won numerous prizes from international grand challenges, competing against teams from MIT, University of Maryland, Facebook AI Research (FAIR), and Baidu VIS. Their goal is to advance visual understanding using deep learning. Notably, Dr Chang won first place in the TrecVID 2019 - Activity Extended Video (ActEV) challenge, hosted by the National Institute of Standards and Technology in the US.

Dr Chang has also been involved in developing deep learning models that automatically annotate disease labels from multi-source patient data, such as data from medical records in Intensive Care Units (ICUs). This project has had a significant impact on healthcare and management in the ICU at the Royal Brisbane and Women's Hospital. Automated diagnosis code annotation can greatly enhance the quality and management of healthcare for both patients and caregivers. More recently, Dr Chang collaborated with researchers from the Australian Alliance for Artificial Intelligence in Healthcare to develop an automatic report generation system for critically ill COVID-19 patients using deep learning techniques and the US public COVID-19 CT scan dataset. The system has achieved state-of-the-art performance on report generation and can generate reports that are very close to doctor-written reports. This work has received extensive media coverage from major news outlets.

Dr Chang earned his Ph.D. degree from the Centre for Artificial Intelligence and the Faculty of Engineering and Information Technology at the University of Technology Sydney, under the supervision of [Prof. Yi Yang](http://www.cs.cmu.edu/~yiyang/){:target="_blank"}. During his doctoral studies, he was mentored by Prof. [Feiping Nie](http://www.escience.cn/people/fpnie/){:target="_blank"} and [Yaoliang Yu](https://cs.uwaterloo.ca/~y328yu/){:target="_blank"}. His research during this period focused mainly on developing machine learning algorithms and applying them to multimedia analysis and computer vision. Dr Chang also holds master's and bachelor's degrees from the School of Information Science and Technology and the School of Physics, both from Northwest University. During this time, his research interests were in the areas of FPGA and VLSI.

## Research Interests

Dr Chang's research interests revolve around developing structured machine learning models for computer vision and multimedia tasks. His work primarily centers on exploring the information contained within videos and advancing artificial intelligence systems. His recent research topics include:

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
