---
layout: session
ID: I-10
type: invited
order: 10
title: Complex response, dimension reduction and data integration with application on neuroimaging
organizer:
    name: Yize Zhao
    affil: Department of Biostatistics, Yale University 
    email: yz875@yale.edu
chair:
    name: Yize Zhao
    affil: Department of Biostatistics, Yale University
    email: yz875@yale.edu
speakers:
    - id: 1
      name: Xi Luo
      affil: Department of Biostatistics and Data Science, The University of Texas
      email: xi.Luo@uth.tmc.edu
      title: Covariate Assisted Principal Regression for Covariance Matrix Outcomes with an Application to fMRI
      abstract:  'Modeling variances in data has been an important topic in many fields, including in financial and neuroimaging analysis. We consider the problem of regressing covariance matrices on vector covariates, collected from each observational unit. The main aim of this paper is to uncover the variation in the covariance matrices across units that are explained by the covariates. This paper introduces Covariate Assisted Principal (CAP) regression, an optimization-based method for identifying the components predicted by (generalized) linear models of the covariates. We develop computationally efficient algorithms to jointly search the linear projections of the covariance matrices as well as the regression coefficients, and we establish the asymptotic properties. Using extensive simulation studies, our method shows higher accuracy and robustness in coefficient estimation than competing methods. Applied to a resting-state functional magnetic resonance imaging study, our approach identifies the human brain network changes associated with age and sex.'
    - id: 2
      name: Leo Duan
      affil: Department of Statistics, University of Florida
      email: li.duan@ufl.edu
      title: Bayesian Vector Autoregression using the Tree Rank Prior with an Application to fMRI Data Analysis
      abstract: 'When analyzing tensor-valued data such as images, the multi-scale factor models are particularly appealing, due to the adaptiveness to local geometry and intuitive interpretation. However, the reliance on the binary tree creates high complexity in the parameter space, making it difficult for model estimation and uncertainty quantification. In this talk, I will introduce a new generative distribution based on a simple matrix manipulation. I will show the sample matrix from this distribution automatically obeys a recursive partitioning structure, making it an appealing prior that simplifies the task of multi-scale analysis. The posterior enjoys nice properties such as linear independence and efficient computation via Hamiltonian Monte Carlo. I will demonstrate its immense potential in a multi-scale factor analysis on human brain connectivity.'
    - id: 3
      name:  Kristin Linn
      affil: Department of Biostatistics, Epidemiology and Informatics, University of Pennsylvania
      email: klinn@pennmedicine.upenn.edu
      title: Inter-modal Coupling for Multi-modal Image Analysis
      abstract: Local cortical coupling is a subject-specific measure of the spatially varying relationship between cortical thickness and sulcal depth. Although it is a promising first step towards understanding local covariance patterns between two image-derived measurements, a more general coupling framework that can accommodate multiple volumetric imaging modalities is warranted. We first introduce Inter-Modal Coupling (IMCo), an analogue of local coupling in volumetric space that can be used to produce subject-level, spatially varying feature maps derived from two volumetric imaging modalities. We then leverage IMCo to address partial volume effects when studying localized relationships between gray matter density and cerebral blood flow (CBF) among participants in the Philadelphia Neurodevelopmental Cohort. We also develop a generalized estimating equation approach to study spatial variation in multi-modal image relationships at the population level.
---
