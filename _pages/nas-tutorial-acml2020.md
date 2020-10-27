---
title: ACML 2020 Tutorial - Towards Efficient Neural Architecture Search -- Challenges and Solutions
layout: default
excerpt: NAS Tutorial
permalink: /nas-tutorial-acml2020
---

| <a href="mailto:cxj273@gmail.com" target="_blank" style="text-align:center; display:block"><i class="fa fa-envelope ai-3x"></i></a> | <a href="{{ site.google_scholar_url }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-google ai-3x"></i></a> | <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-linkedin ai-3x"></i></a> | <a href="https://research.monash.edu/en/persons/xiaojun-chang" target="_blank" style="text-align:center; display:block"><i class="fa fa-graduation-cap ai-3x"></i></a> |
  
# ACML 2020 Tutorial
## Towards Efficient Neural Architecture Search -- Challenges and Solutions

### Description
Deep learning has made major breakthroughs and substantial in many fields due to its powerful automatic representation capabilities. It has been proven that neural architecture design is crucial to the feature representation of data and the final performance. To obtain a good representation, researchers have designed various complex neural architectures. However, the design of the neural architecture heavily relies on the researchers’ prior knowledge and experience. Due to the limitations of human’ inherent knowledge, it is difficult for people to jump out of their original thinking paradigm and design an optimal model. Therefore, an intuitive idea would be to reduce human intervention as much as possible and let the algorithm automatically design the neural architecture.

In recent years, a large number of algorithms related to Neural Architecture Search (NAS) have emerged. Various improvements to the NAS algorithm have been made, and the related research work is complicated and rich. A comprehensive and systematic survey on the NAS is essential. Previously related surveys have begun to classify existing work mainly based on the key components of NAS: search space, search strategy and evaluation strategy. While this classification method is more intuitive, it is difficult for readers to grasp the challenges and the landmark work involved. Therefore, in this tutorial, we provide a new perspective: beginning with an overview of the characteristics of the earliest NAS algorithms, summarizing the problems in these early NAS algorithms, and then providing solutions for subsequent related research work. In addition, we conduct a detailed and comprehensive analysis, comparison and summary of these works. Finally, we provide some possible future research directions.

### Part I -- Characteristics of early NAS
NAS usually begins with a set of predefined operation sets and uses a controller to obtain a large number of candidate neural architectures based on the search space created by these operation sets. The candidate architectures are then trained on the training set and ranked according to their accuracy on the validation set. The ranking information of the candidate neural architecture is then used as feedback information to adjust the search strategy, enabling a set of new candidate neural architectures to be obtained. When the termination condition is reached, the search will be terminated to select the best neural architecture. The chosen neural architecture then conducts performance evaluation on the test set.

The early NAS approaches eventually made the automatically generated neural architecture a reality. In order to understand the reasons behind restricting the widespread use of early NAS, we will summarize the common characteristics existing in early NAS work from the perspective of a latecomer.

