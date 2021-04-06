---
layout: session
ID: I-2
type: invited
order: 8
title: Flexible Bayesian Approaches for Imaging Analysis
organizer:
    name: Suprateek Kundu
    affil: Emory University        
    email: suprateek.kundu@emory.edu
chair:
    name: Suprateek Kundu
    affil: Emory University
    email: suprateek.kundu@emory.edu
speakers:
    - id: 1
      name: Michele Guindani
      affil: University of California, Irvine
      email: michele.guindani@UCI.edu
      title: Bayesian Time-Varying Tensor Vector Autoregressive Models for Dynamic  Effective Connectivity
      abstract: Recent developments in functional magnetic resonance imaging (fMRI) investigate how  some brain regions directly influence the activity of other regions of the brain  dynamically throughout the course of an  experiment, i.e. the so-called dynamic effective connectivity. Time-varying vector autoregressive (TV-VAR) models have been  employed to draw inferences for this purpose,  but they are very computationally intensive, since  the  number  of  parameters  to  be  estimated  increases quadratically  with  the  number of  time-series. In this talk, we propose a computationally efficient time-varying Bayesian VAR approach for  modeling  high-dimensional  time  series. The proposed framework employs a tensor decomposition for the VAR coefficient matrices at different lags.  Dynamically varying connectivity patterns are captured by assuming that at any given time the VAR coefficient matrices are  obtained as a mixture of only an active subset of components in the tensor decomposition. Latent binary time-series select the active components at each time via a convenient Ising prior specification. Sparsity-inducing priors are employed to allow for  global-local shrinkage of the coefficients, to determine automatically the rank of the tensor decomposition and to guide the selection of the lags of the auto-regression. The proposed prior structure encourages sparsity in the tensor structure and allows to ascertain model complexity through the posterior distribution. We show the performances of our model formulation via simulation studies and data from a real fMRI study involving a book reading experiment.
    - id: 2
      name: Marina Vannucci
      affil: Rice University
      email:  marina@rice.edu
      title: Bayesian Inference for Stationary Points in Gaussian Process Regression Models with Applications to ERP Analysis
      abstract: Stationary points embedded in the derivatives are often critical for a model to be interpretable and may be considered as key  features of interest in many applications. We propose a semiparametric Bayesian model to efficiently infer the locations of stationary points  of a nonparametric function, while treating the function itself as a  nuisance parameter. We use Gaussian processes as a flexible prior for  the underlying function and impose derivative constraints to control  the function's shape via conditioning. We illustrate the proposed  methods using simulations and then apply the method to the estimation  of event-related potentials (ERP) derived from electroencephalography  (EEG) signals. We show how the proposed method automatically  identifies characteristic components and their latencies at the  individual level, avoiding the excessive averaging across subjects  which is routinely done in the field to obtain smooth curves. By  applying this approach to EEG data collected from younger and older  adults during a speech perception task, we are able to demonstrate how  the time course of speech perception processes change with age.
    - id: 3
      name: Jeff Morris
      affil: University of Pennsylvania
      email: jeffrey.morris@pennmedicine.upenn.edu
      title: Connectivity Regression
      abstract: Assessing heterogeneity of multivariate associations across covariates is an important problem in many areas of modern science, including in neuroscience to discover factors explaining intersubject variability in functional connectivity networks.  In this work, we present general methodological framework to regress subject-specific networks on a set of covariates that produces multiplicity-adjusted hypothesis tests for which covariates affect the networks, as well as statistical measures indicating which network edges are driving these differences.  Our strategy involves projecting a subject-specific empirical correlation matrix into the Fisher correlation space using a matrix logarithm transform, which ensures positive-semidefiniteness and justifies Gaussian modeling.  Using a Gaussian multivariate regression framework in this space with cutting-edge sparsity priors, we regress the networks on predictors while discovering and accounting for second-order dependence across network edges which we show leads to greater efficiency and power for statistical inference using the principles of Seemingly Unrelated Regression.  We apply our approach to analyze functional connectivity networks of 1003 healthy young patients taken from the Human Connectome Project (HCP), finding subject-specific connectivity is associated with their post central gyrus area, precuneus area, and language processing capabilities.  Overall, our framework serves as a promising tool for solving problems in functional connectivity and addresses a growing need for performing inference on observations with complex structure.
---
