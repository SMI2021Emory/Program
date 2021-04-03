---
layout: session
ID: I-7
type: invited
order: 20
title: Recent advances in brain network statistics   
organizer:
    name:   Shuo Chen
    affil: University of Maryland
    email: shuochen@som.umaryland.edu  
chair:
    name:  Qiong Wu
    affil:  University of Maryland
    email: qwu1221@terpmail.umd.edu
speakers:
    - id: 1
      name:  Jesus Arroyo
      affil: Johns Hopkins University
      email: jesus.arroyo@jhu.edu
      title: Inference for multiple heterogeneous networks with a common invariant subspace
      abstract: The development of models for multiple heterogeneous network data is of critical importance both in statistical network theory and across multiple application domains, including neuroscience. Although single-graph inference is well-studied, multiple graph inference is largely unexplored, in part because of the challenges inherent in appropriately modeling graph differences and yet retaining sufficient model simplicity to render estimation feasible. The common subspace independent-edge (COSIE) multiple random graph model addresses this gap, by describing a heterogeneous collection of networks with a shared latent structure on the vertices but potentially different connectivity patterns for each graph. The COSIE model is both flexible to account for important graph differences and tractable to allow for accurate spectral inference. The model can be deployed for a number of subsequent network inference tasks, including dimensionality reduction, classification, hypothesis testing, and community detection. Performance is demonstrated on a dataset of connectomes, showing an accurate classification of brain scans by patients and a meaningful determination of heterogeneity across different subjects.
    - id: 2
      name: Gang Chen
      affil: NIMH
      email: gangchen@mail.nih.gov
      title: Improving reproducibility in network modeling
      abstract: 'With the popular approach of massively univariate analysis in neuroimaging, one builds as many models as the number of elements, leading to a major contributor to the reproducibility crisis due to three intrinsic problems: 1) modeling inefficiency, 2) artificial dichotomization, and 3) researcher degrees of freedom. We propose a Bayesian multilevel framework that incorporates all elements through global calibration in one integrative model. Statistical inferences at each element are thus achieved from the overall posterior distribution through Markov Chain Monte Carlo simulations. In addition, our framework incorporates multiplicity as an integral component of the modeling structure, not as a separate correction step. By turning multiplicity from an annoying penalty into a strength, we aim to achieve six goals: 1) improve model efficiency, 2) gain a higher predictive accuracy, 3) control the errors of incorrect magnitude and incorrect sign instead of conventional false positives and false negatives, 4) validate each model relative to its competing candidates, 5) reduce the reliance on and the sensitivity to the choice of data space, and 6) promote full results reporting. Our modeling framework reverberates with recent proposals to abandon the dichotomization of statistical evidence (“significant” vs. “non-significant”), to improve the interpretability of research findings, as well as to encourage reporting the full gamut of results (not only “significant” ones), thereby enhancing research transparency and reproducibility.'
    - id: 3
      name:  Shuo Chen
      affil:  University of Maryland, School of Medicine 
      email: shuochen@som.umaryland.edu 
      title: l_0 shrinkage in graph space for brain network inference
      abstract: We consider group-level statistical inference for networks, where the outcome variables of each subject are multivariate edges in an adjacency matrix. We assume the nodes of adjacency matrices are identical across all subjects and the goal is to identify and statistically test whether edges in some subnetworks that are associated with the covariates of interest. We propose a group level network statistical framework to extract the subgraphs where edges are likely to be related to the covariate via $l_0$ norm regularization and perform statistical tests on the detected subgraphs by graph combinatorics. Theoretical properties of the novel objective function and network-level inference are provided. We apply the proposed method to a brain connectomic study to identify the subnetworks of brain-connectome that are associated with brain diseases. In addition, we perform extensive simulation studies. The results demonstrate the proposed method outperform existing multivariate statistical methods by simultaneously improve false positive and false negative discovery rates and significantly increase replicability.
---
