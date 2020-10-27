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

### Part II -- Optimization Strategy
Regarding the characteristics and challenges of early NAS, in this part, we will summarize the existing NAS research work with reference to the following four aspects:

(1) Modular search space. Corresponds to the global search space, the modular search space treats the neural architecture as a stack of multiple different types of modules. Therefore, the search task is simplified from the original global search to only one or more modules of different types.

(2) Continuous search strategy. Corresponds to the discrete search strategy, the continuous search strategy continuously relaxes the structural parameters of the neural architecture so that they can be gradient optimized like network parameters.

(3) Neural architecture recycling. Corresponding to the search from scratch, neural architecture recycling takes the existing artificially designed high-performance neural architecture as a starting point, and uses the NAS method to perform network transformations on them to improve their performance.

(4) Incomplete training. Corresponding to fully training, incomplete training aims to speed up the relative performance ranking of candidate architectures by making full use of the shared structure between candidate architectures or performance prediction, thereby avoiding resource consumption caused by complete training of all candidate architectures.

### Part III -- Performance Comparison
In this part, we will classify and compare the performance of existing NAS based on mainstream search methods. These search methods primarily include the following: reinforcement learning (RL), evolutionary algorithm (EA), gradient optimization (GO), random search (RS) and sequential model-based optimization (SMBO). We intend to obtain their similarities and differences from these summaries. The situation is not as simple as it might appear. In fact, it is relatively difficult to compare NAS performance, because NAS lacks certain baselines. In addition, the preprocessing, hyperparameters, search space, trick, etc. differ between different types of NAS, which exacerbates the difficulty of NAS performance comparison.

We will compare and summarize the popular NAS method with mainstream, artificially designed networks in multiple dimensions in terms of both performance and parameter amount. It is however worth noting that, the performance gains obtained using NAS are limited compared to those achieved using manually designed networks.

### Part IV -- Future Directions
The emergence of NAS is exciting, as it is expected to end the tedious trial and error process of manual neural architecture design. Moreover, it is also hoped that it can design a network structure that is completely different from the artificial network, thereby breaking through the existing human mindset. Artificially designed networks have made breakthroughs in many fields, including image recognition, machine translation, semantic segmentation, object detection, and video understanding and so on. Although the NASrelated research has been quite rich, compared with the rapid development of artificial neural architecture design in various fields, NAS is still in the preliminary research stage. The current NAS is primarily focused on improving image classification accuracy, compressing the time required to search for neural architecture, and making it as light and easy to promote as possible. In this process, a proper baseline is crucial, as this helps to avoid NAS search strategy research being masked by various powerful augmenting technologies, regularization, and search space design tricks. In addition, the search strategies currently used by NAS are relatively concentrated, especially GO based on supernets, and there are many theoretical deficiencies in the related research. Therefore, improving the related research background is of great benefit to the development of NAS.

### Prerequisites
We do not require the audiences to have strong background knowledge on neural architecture search. However, we expect the audience already understand some basic concepts and terminologies on artificial intelligence, computer vision, and machine learning.

### Presenters
Dr Xiaojun Chang is a Senior Lecturer at Vision & Lanugage Group, Department of Data Science and AI, Faculty of Information Technology, Monash University Clayton Campus, Australia. Dr Chang is an ARC Discovery Early Career Researcher Award (DECRA) Fellow between 2019-2021 (awarded in 2018).

Before joining Monash, he was a Postdoc Research Associate in School of Computer Science, Carnegie Mellon University, working with Prof. Alex Hauptmann. He has focused his research on exploring multiple signals (visual, acoustic, textual) for automatic content analysis in unconstrained or surveillence videos. His team has won multiple prizes from international grand challenges which hosted competitive teams from MIT, University of Maryland, Facebook AI Research (FAIR) and Baidu VIS, and aim to advance visual understanding using deep learning. For example, he won the first place in the TrecVID 2019 - Activity Extended Video (ActEV) challenge, which was held by National Institute of Standards and Technology, US.

### References
[1] Pengzhen Ren, Yun Xiao, Xiaojun Chang, Po-Yao Huang, Zhihui Li, Xiaojiang Chen, Xin Wang. A Comprehensive Survey of Neural Architecture Search: Challenges and Solutions. CoRR abs/2006.02903 (2020).
