---
layout: session
ID: I-13
type: invited
order: 14
title: New statistical learning methods for imaging data analysis
organizer:
    name:  Jian Kang
    affil:  University of Michigan
    email:  jiankang@umich.edu 
chair:
    name: Shuo Chen
    affil: University of Maryland
    email: ShuoChen@som.umaryland.edu 
speakers:
    - id: 1
      name: Yize Zhao
      affil: Yale University
      email:  yize.zhao@yale.edu 
      title:  Imaging Genetics Analysis under Brain Connectivity with Application on Human Connectome Project
      abstract:  'With the availability of large-scale brain imaging and genetics data, brain imaging genetics, which studies the relationship between genetic variations and brain imaging phenotypes, is becoming an emerging and rapidly growing research field. Among different imaging quantitative traits, brain connectivity/network is the one plays an essential role to shape physiological and pathological behaviors as well as brain functional or structural composition. However, there are still limited works investigate the impact of genetic variants on brain connectivity and the existing ones typically broke down the contingency matrix via vectorization, ignoring the natural network structure. In this work, we developed a biologically interpretable network response regression under a proposed Bayesian hierarchical shrinkage prior. Our model incorporated the LD information within SNPs as well as the population brain network to better understand which and how genotypes impact the individual level brain connectivity. We also develop an efficient EM algorithm which scales up our method to analyze the whole brain network. We applied our method to Human Connectome Project (HCP).'
    - id: 2
      name:  Annie Qu
      affil: University of California, Irvine
      email: aqu2@uci.edu
      title: Correlation Tensor Decomposition and Its Application in Spatial Imaging Data
      abstract: 'In this paper, motivated by the multimodal optical imaging data in a breast cancer study, we propose a new correlation tensor learning approach to analyze spatial-correlated imaging data. Specifically, we construct a higher-order correlation tensor which effectively represents the spatial information and captures the pixel-wise correlation structure. In addition, we propose a new semi-symmetric tensor decomposition to model spatial correlations, which enables us to identify spatial correlation structures associated with disease, and thus improves the diagnostic power. We also establish the theoretical properties for estimation consistency and classification consistency incorporating spatial correlation and develop scalable computational algorithm. We illustrate the performance of the proposed method in both simulation studies and the application to optical breast cancer imaging data. The numerical results indicate that the proposed method outperforms other competing methods including the Convolutional Neural Network (CNN). This is joint work with Yujia Deng and Xiwei Tang.'
    - id: 3
      name:  Jian Kang
      affil: University of Michigan
      email: jiankang@umich.edu 
      title:  Bayesian Inferences in EEG-Based Brain-Computer Interface via the Split-and-Merge Gaussian Process
      abstract: A brain-computer interface (BCI) refers to a system that uses brain activity to control or communicate with technology.  In particular, BCIs can help people with disabilities use technology for communication. The fundamental statistical problem in BCI is classification. A common design for an electroencephalogram (EEG) BCI relies on classification of the P300 event-related potential (ERP), which is a response elicited by the rare occurrence of target stimuli among common non-target stimuli. Many machine learning methods have constructed P300 ERP-based classifiers, but few provide insights on the underlying mechanism of the neural activity. In this work, we propose a new Bayesian generative method to model the conditional distribution of the EEG signals given our EEG-BCI design, from which the predictive probability of brain signals can be derived. Our method focuses on detecting spatial-temporal differences where the EEG signals have strong predictive powers, providing an understanding of the neural activity in response to external stimuli. Extensive simulation studies and analysis of real participants show the advantages of the proposed method compared to previous methods.

---
