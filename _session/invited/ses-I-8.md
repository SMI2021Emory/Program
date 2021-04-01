---
layout: session
ID: I-8
type: invited
order: 21
title: Bayesian Supervised and Unsupervised Image Processing and Analysis, with Applications to Radiogenomics and Diffusion Tensor Imaging
organizer:
    name: Rajarshi Guhaniyogi
    affil: University of California, Santa Cruz 
    email:  rguhaniy@ucsc.edu
chair:
    name: Jaroslaw (Jarek) Harezlak, Professor
    affil: Department of Epidemiology and Biostatistics, School of Public Health, Indiana Univeersity, Bloomington
    email:  harezlak@iu.edu
speakers:
    - id: 1
      name: John Kornak, Professor in Residence, Head of Data Science Program
      affil: Department of Epidemiology and Biostatistics, University of California San Francisco
      email:  john.kornak@ucsf.edu
      title: Bayesian image analysis in transformed spaces (BITS)­ and the BIFS/BIWS packages
      abstract:  'Bayesian image analysis can improve image quality by balancing a priori expectations of image characteristics with a model for the noise process. We will give a reformulation of the conventional image space Bayesian image analysis paradigm into Fourier and wavelet spaces. By specifying the Bayesian model in a transformed space, spatially correlated priors, that are relatively difficult to model and compute in conventional image space, can be efficiently modeled as a set of independent processes in an appropriately transformed space. The originally inter-correlated and high-dimensional problem in image space is thereby broken down into a series of (trivially parallelizable) independent one-dimensional problems. We will describe and show examples of the Bayesian image analysis in transformed space (BITS) modeling approach for both Fourier and wavelet space. In the process, we will showcase our Python package(s): BIFS/BIWS that can allow easy and fast implementation of BITS.'
    - id: 2
      name: Sharmistha Guha, Postdoctoral Associate
      affil: Department of Statistical Science, Duke University
      email: sg516@duke.edu
      title: Bayesian Regression with Undirected Network Predictors with an Application to Brain Connectome Data
      abstract: 'This article focuses on the relationship between a measure of creativity and the human brain network of subjects from a brain connectome dataset obtained using a diffusion weighted magnetic resonance imaging (DWI) procedure. We identify brain regions and interconnections between them that have a significant effect on the creativity. Brain networks are often expressed in terms of symmetric adjacency matrices, with row and column indices of the matrix representing the regions of interest (ROI), and a cell entry signifying the estimated number of fiber bundles connecting the corresponding row and column ROIs. Current statistical practices for regression analysis with the brain network as the predictor and the measure of creativity as the response typically vectorize the network predictor matrices prior to any analysis, thus failing to account for the important structural information in the network. This results in poor inferential and predictive performance. To answer the scientific questions above, this article develops a flexible Bayesian framework that avoids reshaping the network predictor matrix, draws inference on the brain ROIs and interconnections between ROIs significantly related to creativity and enables accurate prediction of creativity from a brain network. A novel class of network shrinkage priors for the coefficient corresponding to the network predictor is proposed to achieve these inferential goals simultaneously. The principled Bayesian framework allows precise characterization of the uncertainty in detecting an ROI as influential for creativity, as well as the quantification of uncertainty in prediction of creativity from a network predictor. Empirical results in simulation studies illustrate substantial inferential and predictive gains of the proposed framework in comparison with competitors. Our framework yields new insights into the relationship of brain regions with creativity, also providing the uncertainty associated with the scientific findings.'
    - id: 3
      name:  Shariq Mohammed, Postdoctoral Research Fellow
      affil:  Precision Health Scholar, University of Michigan Ann Arbor
      email: shariqm@umich.edu
      title: 'RADIOHEAD: Radiogenomic Analysis incorporating tumor heterogeneity in imaging through densities'
      abstract: Recent technological advancements have enabled detailed investigation of associations between the molecular architecture and morphological heterogeneity of tumors, through multi-source integration of radiological imaging and genomic (radiogenomic) data. We integrate and harness radiogenomic data in patients with lower grade gliomas (LGG), a type of brain cancer, in order to develop a formal regression framework called RADIOHEAD (RADIOgenomic analysis incorporating tumor HEterogeneity in imAging through Densities) for modelling association between them. Imaging data is represented through voxel intensity probability density functions of tumor sub-regions obtained from multimodal magnetic resonance imaging, and genomic data through molecular signatures in the form of pathway enrichment scores corresponding to their gene expression profiles. Employing a Riemannian-geometric framework for principal component analysis on the set of probability density functions, we map each probability density to a vector of principal component scores, which are then included as predictors in a Bayesian regression model with the pathway enrichment scores as the response. Variable selection compatible with the grouping structure amongst the predictors induced through the tumor sub-regions is carried out under a group spike-and-slab prior. A Bayesian false discovery rate mechanism is then used to infer statistically significant associations based on the posterior distribution of the regression coefficients. Our analyses reveal several pathways, relevant to LGG etiology (such as synaptic transmission, nerve impulse and neurotransmitter pathways), to have significant associations with the corresponding imaging-based predictors.  





---
