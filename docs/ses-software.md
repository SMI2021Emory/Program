---
title : Software Sessions
layout: default
order : 3
---

{% assign sorted_sessions = site.session | sort:"order" %}
{% for session in sorted_sessions %}
  {% if session.type == "software" %}
  <h2 style="color: #120659;">  
      {{ session.title }}
  </h2>
  
  The video recording of this talk can be viewed <a href="https://www.youtube.com/watch?v=sdRT92s-rFo&list=PLwENUD1LkzXLXYGi5zItDMJLIxDF01WVw&index=3" style="color: blue">here</a>.

<p>
  <b>Organizer</b>: {{session.organizer.name}} <br/> 
   {{session.organizer.affil}} <br/> 
   {% if session.organizer.email %}
   Email: {{session.organizer.email}} <br/> 
   {% endif %}
  </p>
  
  <p>
  <b>Chair</b>: {{session.chair.name}}<br/> 
  {{session.chair.affil}} <br/> 
  {% if session.chair.email %}
  Email: {{session.chair.email}}<br/> 
  {% endif %}
  </p>


<h3 style="color: #120659;">Speakers: </h3>

  {% for speaker in session.speakers %}
  <p> 
  <b>{{speaker.id}}. {{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  {% if speaker.email %}
  Email: {{speaker.email}} <br/> 
  <b>Time: {{speaker.speakertime}}</b> <br/>
  {% endif %}
  <p> <b>Title</b>: {{speaker.title}} <br/>
  <b> Abstract</b>: {{speaker.abstract}} </p>
  {% endfor %}


  <!-- <p>{{ session.content | markdownify }}</p> -->
  {% endif %}
{% endfor %}

<!-- # {{page.title}}

### Neuroconductor: An R Platform for Medical Imaging Analysis
 
John Muschelli, Johns Hopkins University <br/>

**Abstract**<br/>
Neuroconductor (https://neuroconductor.org) is an open-source platform for rapid testing and dissemination of reproducible computational imaging software. The goals of the project are to: 1) provide a centralized repository of R software dedicated to image analysis, 2) disseminate software updates quickly, 3) train a large, diverse community of scientists using detailed tutorials and short courses, 4) increase software quality via automatic and manual quality controls, and 5) promote reproducibility of image data analysis. <br/>

We provide a description of the purpose of Neuroconductor, highlight packages in this framework, and some imaging analysis examples with real data sets.

### Efficient and accessible Machine Learning with rtemis
  
Stathis D. Gennatas, University of California, San Francisco
Efstathios.Gennatas@ucsf.edu <br/>
  
**Abstract**<br/>
The increasing volume and variety of research and clinical biomedical data generated daily is driving up demand for sophisticated quantitative data analysis. rtemis is a comprehensive, open source, machine learning (ML) platform written in R, which grew out of the need to analyze large neuroimaging and cognitive data. It offers a homogenized input/output interface for unsupervised and supervised learning algorithms using a modern object-oriented class system, along with support for powerful static and interactive graphics. It aims to make advanced machine learning analyses highly efficient and accessible to both the expert and novice user alike. It provides low- and high-level functions that replace a very large number of lines of code while allowing control of all parameters of the data analysis pipeline. It offers seamless support for a comprehensive list of learning algorithms implemented in other R packages along with a growing array of novel methods developed on the platform (The Additive Tree, the Hybrid Tree, Conditional Interpretable SuperLearner, Expert-Augmented Machine Learning, and others).<br/>
The rtemis project aims to promote open science and reproducibility. Increasing the efficiency of data analysis pipelines, makes code more compact, easier to share and comprehend, and easier to replicate. Major ongoing research on the rtemis platform includes novel procedures for joint optimization of structured and unstructured data and extension of Expert-Augmented Machine Learning to imaging. Documentation and educational material are available on the project website (https://rtemis.netlify.com).


### HINT – A Matlab toolbox for hierarchical covariate-adjusted independent component analysis of fMRI data
 
Joshua Lukemire, Emory University
 
**Abstract**<br/>
We introduce a Matlab toolbox, HINT (Hierarchical INdependent component analysis Toolbox), that provides a hierarchical covariate-adjusted ICA (hc-ICA) for modeling and testing covariate effects and generates model-based estimates of brain networks on both the population- and individual-level. HINT provides a user-friendly Matlab GUI that allows users to easily load images, specify covariate effects, monitor model estimation via an EM algorithm, specify hypothesis tests, and visualize results. HINT also has a command line interface which allows users to conveniently run and reproduce the analysis with a script. We provide a walkthrough of the toolbox features and a demonstration on synthetic data.
 
### Modeling and Visualization of Connectivity in EEG

Hernando Ombao, KAUST <br/>
  
### User-friendly MATLAB GUIs for Bayesian Multi-Subject Modeling of fMRI Data

Marina Vannucci
 
**Abstract**<br/>
We first introduce BVAR-connect, a variational inference approach to a Bayesian multi-subjectvector autoregressive (VAR) model for inference on effective brain connectivity based on resting statefunctional MRI data. The modeling framework uses a Bayesian variable selection approach that flexibly integrates multi-modal data into the prior construction. The variational inference approach we develop allows scalability of the methods and results in the ability to estimate subject- and group-level brain connectivity networks over whole-brain parcellations of the data. Next, we describe NPBayes-fMRI, a unified, probabilistically coherent non-parametric Bayesian framework for the analysis of task-related fMRI data from multi-subject experiments. The modeling approach is based on a spatio-temporal linear regression model that specifically accounts for the between-subjects heterogeneity in neuronal activity via a spatially informed multi-subject non-parametric variable selection prior. A characteristic feature of the approach is that it results in a clustering of the subjects into subgroups characterized by similar brain responses, while simultaneously producing group-level as well as subject-level activation maps. -->
 





