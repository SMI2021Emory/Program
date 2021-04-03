---
layout: session
ID: I-10
type: invited
order: 15
title: Complex response, dimension reduction and data integration with application on neuroimaging
organizer:
    name: Yize Zhao
    affil:  Yale University 
    email: yz875@yale.edu
chair:
    name: Yize Zhao
    affil: Yale University
    email: yz875@yale.edu
speakers:
    - id: 1
      name: Xi Luo
      affil: The University of Texas
      email: xi.luo@uth.tmc.edu
      title: Covariate Assisted Principal Regression for Covariance Matrix Outcomes with an Application to fMRI
      abstract:  'Modeling variances in data has been an important topic in many fields, including in financial and neuroimaging analysis. We consider the problem of regressing covariance matrices on vector covariates, collected from each observational unit. The main aim of this paper is to uncover the variation in the covariance matrices across units that are explained by the covariates. This paper introduces Covariate Assisted Principal (CAP) regression, an optimization-based method for identifying the components predicted by (generalized) linear models of the covariates. We develop computationally efficient algorithms to jointly search the linear projections of the covariance matrices as well as the regression coefficients, and we establish the asymptotic properties. Using extensive simulation studies, our method shows higher accuracy and robustness in coefficient estimation than competing methods. Applied to a resting-state functional magnetic resonance imaging study, our approach identifies the human brain network changes associated with age and sex.'
    - id: 2
      name: Leo Duan
      affil: University of Florida
      email: li.duan@ufl.edu
      title: Bayesian Vector Autoregression using the Tree Rank Prior with an Application to fMRI Data Analysis
      abstract: Vector autoregression is very popular for analyzing the multivariate time series. Besides good predictive performance, it enjoys nice interpretation in the Granger-causality graph --- the past values of some variables are helpful for predicting the others. In the high dimensional setting with p variables, one often relies on the matrix-norm/matrix-rank based regularization to induce sparsity; however, this tends to create too many disconnected graph components that are difficult to interpret. To solve this problem, we propose a new type of low-rankness based on the graph topology --- we define the "tree rank" as the  number of spanning trees needed to cover the graph. Each spanning tree is a minimalist subgraph with (p-1) edges but connects p nodes. As the result, having the regression coefficients on a few spanning trees leads to both high sparsity and high connectivity. To allow efficient computation and uncertainty quantification on the estimates, we develop a novel graph-based continuous shrinkage prior, that exploits a continuous relaxation for the spanning trees. This prior, that we call "Tree Rank Prior", avoids the costly combinatorial search in the graph estimation and enjoys the gradient-based Hamiltonian Monte Carlo algorithm for its posterior estimation. We show that this model enjoys appealing theoretical properties, such as the mild stability conditions, posterior consistency, as well as useful information retrieval even under model misspecification. The model is applied to find the Granger causality graph in the functional magnetic resonance imaging data.
    - id: 3
      name:  Kristin Linn
      affil: University of Pennsylvania
      email: klinn@pennmedicine.upenn.edu
      title: Inter-modal Coupling for Multi-modal Image Analysis
      abstract: Local cortical coupling is a subject-specific measure of the spatially varying relationship between cortical thickness and sulcal depth. Although it is a promising first step towards understanding local covariance patterns between two image-derived measurements, a more general coupling framework that can accommodate multiple volumetric imaging modalities is warranted. We first introduce Inter-Modal Coupling (IMCo), an analogue of local coupling in volumetric space that can be used to produce subject-level, spatially varying feature maps derived from two volumetric imaging modalities. We then leverage IMCo to address partial volume effects when studying localized relationships between gray matter density and cerebral blood flow (CBF) among participants in the Philadelphia Neurodevelopmental Cohort. We also develop a generalized estimating equation approach to study spatial variation in multi-modal image relationships at the population level.
---
