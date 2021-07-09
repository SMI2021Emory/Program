---
layout: session
ID: I-12
type: invited
order: 22
title: Functional and Spatial Techniques in Neuroimaging Data 
youtubelink: https://www.youtube.com/watch?v=79XIyGnthXk&list=PLwENUD1LkzXLXYGi5zItDMJLIxDF01WVw&index=22
organizer:
    name:  Linglong Kong
    affil:  University of Alberta
    email: lkong@ualberta.ca
chair:
    name: Jian Kang
    affil: University of Michigan
    email: jiankang@umich.edu
speakers:
    - id: 1
      name: Michelle F. Miranda
      affil: University of Victoria
      email: michellemiranda@uvic.ca
      title: Composite-hybrid basis approach incorporating residual connectivity in task fMRI data
      abstract:  'Task-based functional magnetic resonance imaging (fMRI) studies are a powerful tool to understand human sensory, cognitive, and emotional processes. The fMRI measurement consist of an indirect and non-invasive measure of brain activity based on the Blood Oxygen Level Dependent (BOLD) contrast. A critical challenge is to account for the dependencies from the complex structure of the brain. In this talk, I propose an adaptive composite-hybrid basis approach to model task fMRI data. The proposed basis approach tackles the high-dimensionality inherent to the brain data while simultaneously accounting for nearby and distant spatial correlation in a multilevel basis procedure. The first level accounts for whitin-ROI spatial correlation by selecting a sparse set of bases for each ROI. The second level considers between-ROIs correlation and obtains a set of basis functions that represents the entire brain spatial structure. The third level of the approach models time dependencies in the BOLD time series by projecting the time course into a wavelet space and then  assuming a long memory process that accounts for differences in each wavelet decomposition level.  Moreover, residual connectivity between ROIs is incorporated into the estimation procedure and can provide further insights into fMRI tasks. The spatial strategy gives us a sparse representation of the brain improving many folds in computational speed and effectively providing full Bayesian inference at the voxel or ROI level. '
    - id: 2
      name:  Jingyi Zheng
      affil:  Auburn University
      email: jzz0121@auburn.edu
      title: Time-frequency Spectral Analysis of Scalp EEG signals using Empirical Mode Decomposition
      abstract: 'Electroencephalography (EEG) is an electrophysiological monitoring method to record electrical activity of the brain from different electrodes placed on scalp. In this talk, we propose an effective data-driven processing pipeline to first clean, decompose the scalp EEG signals, and perform time-frequency analysis using Hilbert-Huang transform, and further build machine learning classifiers. Specifically, we propose to decompose a EEG signal into a set of Intrinsic Mode Functions (IMFs) using a data-driven method named Empirical Mode Decomposition (EMD). For each IMF, we obtain the instantaneous frequency and amplitude through Hilbert transform. Then we propose a new metric to measure the frequency component of each IMF and further select the IMF to represent certain brain wave. We also propose a metric to measure the averaged amplitude of certain brain wave. Using the proposed metrics, we can test some cognitive hypothesis, as well as build machine learning classifiers. Specifically, we first train a between task classifier using Random Forest to successfully classify four tasks with 99.12% accuracy in average, and further build within task classifiers to classify body/eye movements for each task with at least 94.47% accuracy.'
    - id: 3
      name:  Adam Ciarleglio
      affil: George Washington University
      email: aciarleglio@email.gwu.edu
      title:  Multiple imputation in functional regression with applications to EEG data in a depression study
      abstract: Missing data are a common problem in biomedical research.  Valid approaches for addressing this problem have been proposed and are regularly implemented in applications where the data are exclusively scalar-valued.  With advances in technology and data storage, biomedical studies now frequently collect both scalar and functional data, both of which may be subject to missingness.  However, little work has been done to deal with missing functional data.  We propose extensions of multiple imputation and Rubin’s Rules for pooling estimates derived from multiply imputed data sets that accommodate both scalar and functional data. We present results from a simulation study showing the performance of our proposed approach with respect to fidelity to the observed data and estimation of the parameters of interest.  We also present results from applying our proposed approach in the context of fitting a function-on-scalar regression model relating characteristics derived from electroencephalography to depression status (major depressive disorder vs. healthy control).
    - id: 4
      name:  Guanqun Cao
      affil: Auburn University
      email: gzc0009@auburn.edu 
      title:  Estimation of the Mean Function of Functional Data via Deep Neural Networks
      abstract: In this work, we propose a deep neural networks based method to perform nonparametric regression for functional data.  The proposed estimators are based on sparsely connected deep neural networks with ReLU activation function. We provide the convergence rate of the proposed deep neural networks estimator  in terms of the empirical norm.  We discuss how to properly select  of the architecture parameters by cross-validation.  Through Monte Carlo simulation studies we examine the finite-sample performance of the proposed method. Finally, the proposed method is applied to analyze positron emission tomography images of patients with Alzheimer disease obtained from the Alzheimer Disease Neuroimaging Initiative database.
---
