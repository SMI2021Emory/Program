---
id: I-1
title: Statistical methods for neuroimaging studies of Alzheimer’s Disease
organizer:
    name: Dana Tudorascu, PhD
    affil: > 
        University of Pittsburgh
        Department of Medicine, Psychiatry and Biostatistics
    email: dlt30@pitt.edu
chair:
    name: John Kornak, PhD
    affil: > 
        University of California, SF
        Department of Epidemiology and Biostatistics
        University of California, San Francisco
        San Francisco, CA 94158-2549
    email: john.kornak@ucsf.edu
speaker:
    - id: 1
      name: Ciprian Crainiceanu
      affil: Johns Hopkins University, Department of Biostatistics
      email: ccraini1@jhu.edu
      title: Longitudinal Image Analysis and Inference
      abstract: We propose massive univariate generalized linear mixed effects models for studies that collect images at multiple visit. Joint inference for fixed effects is conducted using bootstrap of study participants while for random effects we use leave-one-in bootstrap. For conducting inference and sample size calculation we propose to use the upstrap, which samples with replacement either more or fewer samples than the original sample size.
    - id: 2
      name: Dana Tudorascu
      affil: University of Pittsburgh, Department of Medicine, Psychiatry and Biostatistics.
      email: dlt30@pitt.edu
      title: Methods for MRI and PET neuroimaging data harmonization across different scanners in Alzheimer Disease.
      abstract: Positron Emission Tomography (PET) and Structural Magnetic Resonance Imaging (MRI) are two imaging modalities that are frequently used in studies of Alzheimer’s Disease (AD).  [11C]Pittsburgh Compound B (PiB) PET standardized uptake value ratio (SUVR), play a crucial role in studying the progression of AD in the elderly, autosomal dominant AD mutation carriers and Down Syndrome populations. Harmonization of these multimodal imaging studies collected at multiple sites presents a challenging problem. The focus of this work was to investigate an intensity normalization method, Removal of Artificial Voxel Effect by Linear regression (RAVEL) (Fortin et al., 2016), followed by a data harmonization technique, ComBat (Fortin et al., 2018). Effects on cortical thickness, MR-based quantification of [11C]PiB SUVR and a neuraradiological study of accuracy of AD related ROI segmentations, were evaluated. We found that RAVEL/ ComBat combination was most effective at MRI harmonization. Large differences observed in effect sizes suggest that combining data from different sites/scanners should be properly addressed.
    - id: 3
      name: Joanne Beer
      affil: University of Pennsylvania, Department of Biostatistics, Epidemiology and Informatics. 
      email: joanne.beer@pennmedicine.upenn.edu
      title: Extensions of ComBat for harmonization of multi-scanner neuroimaging data in an Alzheimer’s Disease Neuroimaging Initiative dataset
      abstract: While aggregation of neuroimaging datasets from multiple sites and scanners presents opportunities for larger sample sizes and increased statistical power, it also presents challenges due to systematic scanner effects. In this talk we present several recent extensions of ComBat (Combatting Batch Effects when Combining Batches), a harmonization method originally developed for genomics and later adapted to cross-sectional neuroimaging data. Specifically, we discuss ComBat extended to linear mixed effects models (longitudinal ComBat), generalized additive (mixed) models (ComBatGA(M)M), and harmonization of covariance (CovBat). Using structural MRI data from 663 participants in the Alzheimer’s Disease Neuroimaging Initiative (ADNI) study, we demonstrate the presence of scanner-related effects on the means, variances, and covariance of cortical thickness measures across brain atlas regions. We discuss situations where ComBat increases statistical power, helps control type I error rate, and yields better classification and prediction performance than unharmonized data.
---
