---
layout: session
ID: I-9
type: invited
order: 9
title: Regularization methods in medical imaging
organizer:
    name: John Kornak
    affil: University of California, San Francisco
    email:   john.kornak@ucsf.edu
chair:
    name: John Kornak
    affil: University of California, San Francisco
    email: john.kornak@ucsf.edu
speakers:
    - id: 1
      name: Jaroslaw Harezlak, Professor in Residence, Head of Data Science Program
      affil: Indiana University, Bloomington
      email: harezlak@iu.edu
      title: Regularized regression for multi-modal brain imaging
      abstract:  'We address the problem of adaptive incorporation of multi-modal brain imagining data in the multiple linear regression setting. We assume the model of the form E[Y|X,Z] = X*beta + Z*b, where the response variable y corresponds to a neuropsychological outcome, X are the possible confounders, and Z are the explanatory variables (e.g. cortical thickness or area) for which the functional and structural connectivity information exists. The connectivity information is used to build the adaptive penalty terms in the regularized regression problem. The general idea of incorporating connectivity information in regularization approach via linear mixed model representation has been recently established in our prior work: ridgified Partially Empirical Eigenvectors for Regression (riPEER). Here, we incorporate multiple sources of information, e.g. functional connectivity network structure, and estimate the regression parameters with multiple penalty terms via a riPEER extension called msPEER (Multi-Source Partially Empirical Eigenvectors for Regression). We present an extensive simulation study testing various realistic scenarios and apply msPEER to data arising from the Human Connectome Project (HCP) study.'

    - id: 2
      name:  Fengqing (Zoe) Zhang
      affil: Drexel University
      email: fz53@drexel.edu
      title: Penalized multi-state models for examining multimodal imaging signatures of Alzheimer's disease.
      abstract: 'Identifying antemortem biomarkers for progression from mild cognitive impairment (MCI) to dementia of Alzheimer‘s type is crucial to detect areas particularly sensitive to neurodegeneration caused by Alzheimer’s disease (AD), in addition to potentially providing a strong diagnostic tool at early disease stages. Jointly modeling the multiple states including normal control, MCI, and dementia as well as the transition probability between them provides a new approach to unravel the mechanism underlying the clinical progression of AD with enhanced statistical power. To deal with a large number of imaging features, we incorporate penalization in multi-state Markov transition models to select predictive imaging signatures of AD. We demonstrate the performance of the proposed approach using MRI and metabolism FDG-PET imaging data from the ADNI project.'
    - id: 3
      name:  Yi Zhao
      affil: Indiana University‑Purdue University Indianapolis
      email: zhaoyi1026@gmail.com
      title: Multimodal Neuroimaging Data Integration and Pathway Analysis.
      abstract: With fast advancements in technologies, the collection of multiple types of measurements on a common set of subjects is becoming routine in science. Some notable examples include multi- modal neuroimaging studies for the simultaneous investigation of brain structure and function, and multi-omics studies for combining genetic and genomic information. Integrative analysis of multimodal data allows scientists to interrogate new mechanistic questions. However, the data collection and generation of integrative hypotheses is outpacing available methodology for joint analysis of multimodal measurements. In this article, we study high-dimensional multimodal data integration in the context of mediation analysis. We aim to understand the roles different data modalities play as possible mediators in the pathway between an exposure variable and an outcome. We propose a mediation model framework with two data types serving as separate sets of mediators, and develop a penalized optimization approach for parameter estimation. We study both the theoretical properties of the estimator through an asymptotic analysis, and its finite-sample performance through simulations. We illustrate our method with a multimodal brain pathway analysis having both structural and functional connectivities as mediators in the association between sex and language processing.

---
