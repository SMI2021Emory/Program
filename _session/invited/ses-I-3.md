---
layout: session
ID: I-3
type: invited
order: 3
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
      abstract: > 
            'Cancer patients routinely undergo radiological evaluations when images of various modalities including computed tomography, positron emission tomography, and magnetic resonance images are collected for diagnosis and for evaluation of disease progression. Tumor characteristics, often referred to as measures of "tumor heterogeneity", can be computed using these clinical images and used as predictors of disease progression and patient survival. Several approaches to quantifying tumor heterogeneity have been proposed including simple intensity histogram-based measures, metrics attempting to quantify average distance from a homogeneous surface, and texture analysis-based methods. I will present a statistical framework for estimating tumor heterogeneity using clustering methods taking into account the topology of the tumors. The proposed approach incorporates the spatial structure of the tumor image using neighborhood summary measures. In addition, I will describe a principal manifold estimation approach for estimating the surface of cancer tumors using a smooth surface.'
    - id: 2
      name: Amanda Mejia
      affil: Indiana University
      email: afmejia@iu.edu
      title: Leveraging shared population and spatial information for accurate estimation of subject-level brain networks
      abstract: > 
            'Accurate, reliable fMRI-based measures of functional brain organization and connectivity at the subject level are greatly needed to advance fMRI-based research and translation to clinical care.  Such individual-level insights would allow researchers to deepen understanding of disease, disorders, development and aging, to build imaging-based biomarkers for disease classification, and to impact clinical care.  A common approach used to estimate spatial functional brain organization and functional connectivity is independent component analysis (ICA), wherein independent components (ICs) are spatial maps of the brain that represent functionally coherent regions.  Unfortunately, the low signal-to-noise ratio of fMRI data makes accurate estimation of ICs and their functional connectivity (FC) challenging.  The existence of big fMRI datasets provides an opportunity to establish computationally advantageous empirical prior distributions for use in Bayesian models.  Additionally, recent advances in spatial and Bayesian statistics now make it possible to efficiently and effectively pool information shared across the cortical surface and other grey matter regions, leading to much more accurate estimation over models that implicitly or explicitly assume spatial independence.  We combine these two approaches–pooling over subjects and space–to obtain accurate estimates of subject-level brain networks based on independent component analysis (ICA). Spatial template ICA is a hierarchical Bayesian ICA framework for single-subject brain network organization that uses empirical population priors or "templates", as well as spatial priors on subject effects.  The population priors are spatially varying, providing more shrinkage toward the population in areas of the brain where subjects are similar and more flexibility in areas where they tend to differ.  Spatial template ICA provides a statistically principled alternative to ad-hoc approaches like dual regression, while retaining its primary benefits: subject-level component estimates are matched to existing group-level IC's, and it is applicable to new subjects not included in the original group ICA. Additionally, standard template ICA (without spatial priors) is very fast to estimate.  In contrast to dual regression, template ICA can also estimate subject-specific components representing additional brain networks or sources of noise, thereby avoiding contamination of the components of interest.  Through simulation studies and a reliability study based on data from the Human Connectome Project, we find that the use of empirical population priors substantially improves estimation efficiency, and the use of spatial priors further enhances efficiency and power.  We also present an application of the proposed methods to a study of the effects of psilocybin (a prodrug compound found in mushrooms) to organization and connectivity of the thalamus. The proposed methods are implemented in the R package templateICAr.'

    - id: 3
      name: Manjari Narayan
      affil: Stanford University
      email: manjarin@stanford.edu
      title: Operating Characteristics of Network Centrality with applications to Network Neuroscience
      abstract: 
---
