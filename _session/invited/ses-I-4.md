---
layout: session
ID: I-4
type: invited
order: 6
title: Recent advances in statistical methods for complex neuroimaging data
organizer:
    name:  Fengqing (Zoe) Zhang, Assistant Professor
    affil: > 
        Drexel University        
    email:  fz53@drexel.edu
chair:
    name:  Jiangtao Gou, Assistant Professor
    affil: >
        Villanova University        
    email: jiangtao.gou@villanova.edu
speakers:
    - id: 1
      name: Todd Ogden, Professor 
      affil: Columbia University
      email: to166@cumc.columbia.edu
      title: Constrained functional additive models for interaction effects between a treatment and functional covariates
      abstract: A primary goal of precision medicine is to make efficient use of data gathered at the time a patient presents for treatment, including imaging and other high-dimensional data, to select the optimal treatment for each patient.  We present a functional additive regression model, uniquely constrained to represent the effect of the interaction between a categorical treatment variable and a potentially large number of pretreatment functional covariates on a response variable, while allowing the marginal effects of the covariates to remain unspecified.  This method simultaneously selects functional/scalar treatment effect modifiers that exhibit possibly nonlinear interactions with the treatment indicator and that are relevant for making optimal treatment decisions.  We present theoretical properties of the proposed method and demonstrate its performance on both simulated and real data.
    - id: 2
      name: Nicole Lazar, Professor
      affil: Penn State University
      email:  nfl5182@psu.edu
      title: Topological Data Analysis for the Study of Brain Networks
      abstract: The study of brain networks and brain connectivity has increased in prominence in recent years.  In this talk, I will describe the use of topological data analysis (TDA) for brain networks.  In contrast to more traditional modes of analysis, TDA focuses on the topological features of a data set, and hence offers new insight into the brain network structure and characteristics.  The effectiveness of the approach will be demonstrated on both simulated and real data.
    - id: 3
      name: Haochang Shou, Assistant Professor,
      affil: University of Pennsylvania
      email: hshou@pennmedicine.upenn.edu
      title: Correcting Site Differences in the Covariance Structures of Neuroimaging Data
      abstract: With the increasing needs for big data analytics in medical imaging, pooling and integrating data from multi-site studies has become critical. Yet site differences attributed to various sources including differences in scanner manufacturers, acquisition and preprocessing protocols are known to exist and might have substantial impact towards the analytic results. Recently, batch-effect corrections methods such as ComBat (Johnson et al. 2007; Fortin et al., 2017) have been successfully adapted to remove scanner and site differences in neuroimaging data in many large-scale studies. However, the existing methods have mostly been focusing on correcting the mean shifts and scale differences for individual dimension across sites. However, we demonstrate that the remaining site differences after applying the existing harmonization techniques could hinder the performance of multivariate pattern analysis (MVPA). This poses a concern in validities of multivariate testing as well as analyses for functional connectivity where the focus is on estimating the dependency structures between regions. We propose CovBat, a novel approach that extends ComBat and utilizes covariance decomposition to remove the unwanted spatially-dependent site deviations in the covariance structures. Further developments have been focusing on preserving the biologically-relevant variations by accounting for related covariates effects in the covariance for functional connectivity analysis. We will demonstrate the performance of the methods using data from ADNI and ABCD studies. 

---
