---
title: ACML 2020 Tutorial - Towards Efficient Neural Architecture Search -- Challenges and Solutions
layout: default
excerpt: NAS Tutorial
permalink: /nas-tutorial-acml2020
---

| <a href="mailto:cxj273#gmail.com" target="_blank" style="text-align:center; display:block"><i class="fa fa-envelope ai-3x"></i></a> | <a href="{{ site.google_scholar_url }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-google ai-3x"></i></a> | <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" style="text-align:center; display:block"><i class="fa fa-linkedin ai-3x"></i></a> | <a href="https://www.rmit.edu.au/contact/staff-contacts/academic-staff/s/chang-associate-professor-xiaojun" target="_blank" style="text-align:center; display:block"><i class="fa fa-graduation-cap ai-3x"></i></a> |

<img class="profile-picture" src="{{site.url}}{{site.baseurl}}/images/profile-picture/profile_picture.jpg" />

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
[Dr Xiaojun Chang](https://www.xiaojun.ai/){:target="_blank"} is a Senior Lecturer at Vision & Lanugage Group, Department of Data Science and AI, Faculty of Information Technology, Monash University Clayton Campus, Australia. Dr Chang is an ARC Discovery Early Career Researcher Award (DECRA) Fellow between 2019-2021 (awarded in 2018).

Before joining Monash, he was a Postdoc Research Associate in School of Computer Science, Carnegie Mellon University, working with Prof. Alex Hauptmann. He has focused his research on exploring multiple signals (visual, acoustic, textual) for automatic content analysis in unconstrained or surveillence videos. His team has won multiple prizes from international grand challenges which hosted competitive teams from MIT, University of Maryland, Facebook AI Research (FAIR) and Baidu VIS, and aim to advance visual understanding using deep learning. For example, he won the first place in the TrecVID 2019 - Activity Extended Video (ActEV) challenge, which was held by National Institute of Standards and Technology, US.

### References
[1] Pengzhen Ren, Yun Xiao, <b>Xiaojun Chang</b>, Po-Yao Huang, Zhihui Li, Xiaojiang Chen, Xin Wang. A Comprehensive Survey of Neural Architecture Search: Challenges and Solutions. CoRR abs/2006.02903 (2020).

[2] Miao Zhang, Huiqi Li, Shirui Pan, <b>Xiaojun Chang</b>, Zongyuan Ge, and Steven Su. One-Shot Neural Architecture Search: Maximising Diversity to Overcome Catastrophic Forgetting. IEEE Trans. Pattern Anal. Mach. Intell. (T-PAMI), 2020.

[3] Changlin Li, Jiefeng Peng, Liuchun Yuan, Guangrun Wang, Xiaodan Liang, Liang Lin, <b>Xiaojun Chang</b>. Neural Architecture Search by Block-wisely Distilling Architecture Knowledge. CVPR 2020.

[4] Xuelian Cheng, Yiran Zhong, Mehrtash Harandi, Yuchao Dai, <b>Xiaojun Chang</b>, Hongdong Li, Tom Drummond, and Zongyuan Ge. Hierarchical Neural Architecture Search for Deep Stereo Matching. NeurIPS 2020.

[5] Miao Zhang, Huiqi Li, Shirui Pan, <b>Xiaojun Chang</b>, Zongyuan Ge and Steven Su. Differentiable Neural Architecture Search in Equivalent Space with Exploration Enhancement. NeurIPS 2020.

[6] Miao Zhang, Huiqi Li, Shirui Pan, <b>Xiaojun Chang</b>, and Steven Su. Overcoming Multi-Model Forgetting in One-Shot NAS with Diversity Maximization. CVPR 2020.

[7] Ahmed, K., & Torresani, L. (2018). Maskconnect: Connectivity learning by gradient descent. In Proceedings of the European Conference on Computer Vision (ECCV) (pp. 349-365).

[8] Ren, S., He, K., Girshick, R., & Sun, J. (2015). Faster r-cnn: Towards real-time object detection with region proposal networks. In Advances in neural information processing systems (pp. 91-99).

[9] Liu, W., Anguelov, D., Erhan, D., Szegedy, C., Reed, S., Fu, C. Y., & Berg, A. C. (2016, October). Ssd: Single shot multibox detector. In European conference on computer vision (pp. 21-37). Springer, Cham.

[10] Lin, T. Y., Goyal, P., Girshick, R., He, K., & DollÃąr, P. (2017). Focal loss for dense object detection. In Proceedings of the IEEE international conference on computer vision (pp. 2980-2988).

[11] Zoph, B., & Le, Q. V. (2016). Neural architecture search with reinforcement learning. arXiv preprint arXiv:1611.01578.

[12] Baker, B., Gupta, O., Naik, N., & Raskar, R. (2016). Designing neural network architectures using reinforcement learning. arXiv preprint arXiv:1611.02167.

[13] Dalal, N., & Triggs, B. (2005, June). Histograms of oriented gradients for human detection. In 2005 IEEE computer society conference on computer vision and pattern recognition (CVPR’05) (Vol. 1, pp. 886-893). IEEE.

[14] Lowe, D. G. (1999, September). Object recognition from local scale-invariant features. In Proceedings of the seventh IEEE international conference on computer vision (Vol. 2, pp. 1150-1157). Ieee.

[15] Real, E., Moore, S., Selle, A., Saxena, S., Suematsu, Y. L., Tan, J., ... & Kurakin, A. (2017, August). Large-scale evolution of image classifiers. In Proceedings of the 34th International Conference on Machine Learning-Volume 70 (pp. 2902-2911). JMLR. org.

[16] Xie, L., & Yuille, A. (2017). Genetic cnn. In Proceedings of the IEEE international conference on computer vision (pp. 1379-1388).

[17] Liu, H., Simonyan, K., & Yang, Y. (2018). Darts: Differentiable architecture search. arXiv preprint arXiv:1806.09055.

[18] Shu, Y., Wang, W., & Cai, S. (2019). Understanding Architectures Learnt by Cell-based Neural Architecture Search. arXiv preprint arXiv:1909.09569.

[19] Pham, H., Guan, M. Y., Zoph, B., Le, Q. V., & Dean, J. (2018). Efficient neural architecture search via parameter sharing. arXiv preprint arXiv:1802.03268.

[20] Baker, B., Gupta, O., Raskar, R., & Naik, N. (2017). Accelerating neural architecture search using performance prediction. arXiv preprint arXiv:1705.10823.

[21] Li, C., Peng, J., Yuan, L., Wang, G., Liang, X., Lin, L., & Chang, X. (2019). Blockwisely Supervised Neural Architecture Search with Knowledge Distillation. arXiv preprint arXiv:1911.13053.

[22] Bender, G. (2019). Understanding and simplifying one-shot architecture search.

[23] Brock, A., Lim, T., Ritchie, J. M., & Weston, N. (2017). Smash: one-shot model architecture search through hypernetworks. arXiv preprint arXiv:1708.05344.

[24] Sciuto, C., Yu, K., Jaggi, M., Musat, C., & Salzmann, M. (2019). Evaluating the search phase of neural architecture search. arXiv preprint arXiv:1902.08142.

[25] Zhang, M., Li, H., Pan, S., Chang, X., & Su, S. Overcoming Multi-Model Forgetting in One-Shot NAS with Diversity Maximization.

[26] Elsken, T., Metzen, J. H., & Hutter, F. (2018). Neural architecture search: A survey. arXiv preprint arXiv:1808.05377.

[27] Wistuba, M., Rawat, A., & Pedapati, T. (2019). A survey on neural architecture search. arXiv preprint arXiv:1905.01392.

[28] Tan, M., Chen, B., Pang, R., Vasudevan, V., Sandler, M., Howard, A., & Le, Q. V. (2019). Mnasnet: Platform-aware neural architecture search for mobile. In Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (pp. 2820-2828).

[29] He, K., Zhang, X., Ren, S., & Sun, J. (2016). Deep residual learning for image recognition. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 770-778).

[30] Szegedy, C., Liu, W., Jia, Y., Sermanet, P., Reed, S., Anguelov, D., ... & Rabinovich, A. (2015). Going deeper with convolutions. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 1-9).

[31] Zoph, B., Vasudevan, V., Shlens, J., & Le, Q. V. (2018). Learning transferable architectures for scalable image recognition. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 8697-8710).

[32] Zhong, Z., Yan, J., Wu, W., Shao, J., & Liu, C. L. (2018). Practical block-wise neural network architecture generation. In Proceedings of the IEEE conference on computer vision and pattern recognition (pp. 2423-2432).

[33] Liu, H., Simonyan, K., Vinyals, O., Fernando, C., & Kavukcuoglu, K. (2017). Hierarchical representations for efficient architecture search. arXiv preprint arXiv:1711.00436.

[34] Dong, J. D., Cheng, A. C., Juan, D. C., Wei, W., & Sun, M. (2018). Dpp-net: Device-aware progressive search for pareto-optimal neural architectures. In Proceedings of the European Conference on Computer Vision (ECCV) (pp. 517-531).
