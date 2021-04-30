---
layout: session
ID: I-3
type: invited
order: 11
title: Recent Advances and New Directions in Neuroimaging Statistics
organizer:
    name: Carolyn Lou
    affil: > 
        University of Pennsylvania
    email: louc@pennmedicine.upenn.edu
chair:
    name: Carolyn Lou
    affil: > 
        University of Pennsylvania
    email: louc@pennmedicine.upenn.edu
speakers:
    - id: 1
      name:  Ani Eloyan
      affil: Brown University
      email: ani_eloyan@brown.edu
      title: Analysis of structural imaging data in cancer
      abstract: Cancer patients routinely undergo radiological evaluations when images of various modalities including computed tomography, positron emission tomography, and magnetic resonance images are collected for diagnosis and for evaluation of disease progression. Tumor characteristics, often referred to as measures of "tumor heterogeneity", can be computed using these clinical images and used as predictors of disease progression and patient survival. Several approaches to quantifying tumor heterogeneity have been proposed including simple intensity histogram-based measures, metrics attempting to quantify average distance from a homogeneous surface, and texture analysis-based methods. I will present a statistical framework for estimating tumor heterogeneity using clustering methods taking into account the topology of the tumors. The proposed approach incorporates the spatial structure of the tumor image using neighborhood summary measures. In addition, I will describe a principal manifold estimation approach for estimating the surface of cancer tumors using a smooth surface.
    - id: 2
      name: Amanda Mejia
      affil: Indiana University
      email: afmejia@iu.edu
      title: Leveraging shared population and spatial information for accurate estimation of subject-level brain networks
      abstract: Accurate, reliable fMRI-based measures of subject-level brain organization and connectivity are needed to advance fMRI-based research. Such insights would allow researchers to deepen understanding of disease, disorders, development and aging; to build imaging biomarkers; and to impact clinical care. A common approach used to estimate spatial functional brain organization and functional connectivity is independent component analysis (ICA). Unfortunately, the low signal-to-noise ratio of fMRI data makes accurate ICA estimation challenging. The existence of big fMRI datasets provides an opportunity to establish computationally advantageous empirical prior distributions for use in Bayesian models. Additionally, recent advances in spatial and Bayesian statistics now make it possible to leverage information shared across the brain. Spatial template ICA leverages spatial and population information to perform ICA reliably in individual subjects.  Through simulations and a reliability study employing the Human Connectome Project, we find that this framework has high estimation efficiency and power. We also present an application to a study of the effects of psilocybin (a prodrug compound found in mushrooms) to thalamic organization and connectivity.  Spatial template ICA is implemented in the R package templateICAr.
    - id: 3
      name: Emily Hector
      affil: North Carolina State University
      email: ehector@ncsu.edu
      title: Integrative fused mean structure learning with application to image-on-scalar regression
      abstract: Motivated by image-on-scalar regression with data aggregated across multiple sites, we consider a setting in which multiple independent studies each collect multiple dependent vector outcomes, with potential mean model parameter homogeneity between studies and outcome vectors. To determine the validity of jointly analyzing these data sources, we must learn which of these data sources share mean model parameters. We propose a new model fusion approach that delivers improved flexibility, statistical performance and computational speed over existing methods. Our proposed approach specifies a quadratic inference function within each data source and fuses mean model parameter vectors in their entirety based on a new formulation of a pairwise fusion penalty. We also propose an asymptotically equivalent weighted oracle meta-estimator that is more computationally efficient and privacy preserving. Simulations and application to amplitude of low frequency fluctuations data from the ABIDE neuroimaging consortium highlight the flexibility of the proposed approach.

---
