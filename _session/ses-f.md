---
layout: default
ID: 
type: founder
order: 2
title: Founder's talk
organizer:
    name: 
    affil: 
    email: 
chair:
    name: 
    affil: 
    email: 
speakers:
    - id: 1
      name: Timothy Johnson
      affil: University of Michigan
      email: 
      title: Bayesian Nonparametric Analysis of Dual-Resolution fMRI for Presurgical Planning
      abstract: "There is growing interest amongst neuroradiologists and neurosurgeons in using functional magnetic resonance imaging (fMRI) to map functionally relevant brain regions to aid in presurgical planning.  This application requires a high degree of spatial accuracy.  However, standard fMRI does not have the spatial resolution required and high spatial resolution fMRI is too noisy for this application. Our idea is to leverage the advantage of standard resolution fMRI (high signal-to-noise ratio) with the advantage of high-resolution fMRI (refined spatial resolution). We develop a new Bayesian nonparametric model to leverage the advantages of both. Working with the unsmoothed z-statistic images from both resolutions, we place a Gaussian process prior to the mean intensity function and use ideas similar to the Gaussian predictive process to infer the mean intensity. We also develop an efficient computational algorithm to integrate these two sources of data. Simulation studies show our method performs better than alternative methods that use only one source of data alone.  Finally, we illustrate our method on real, presurgical data. 
      <p>
      Neuroradiologists and neurosurgeons may opt to use functional magnetic resonance imaging (fMRI) to map functionally relevant brain regions and plan out surgical access routes noninvasively. This application requires a high degree of spatial accuracy, but the fMRI signal-to-noise ratio (SNR) decreases as spatial resolution increases. In practice, fMRI scans can be collected at multiple spatial resolutions,  and it is of interest to make more accurate inference on brain activity by combining data with different resolutions. To this end, we develop a new Bayesian model to leverage both better spatial precision in high resolution fMRI and higher SNR in standard resolution fMRI. We assign a Gaussian process prior to the mean intensity function and develop an efficient, scalable posterior computation algorithm to integrate both sources of data. We draw posterior samples using an algorithm analogous to Riemann manifold Hamiltonian Monte Carlo in an expanded parameter space. We illustrate our method in analysis of presurgical fMRI data, and show in simulation our method infers the mean intensity more accurately than alternatives that use either the high or standard resolution fMRI data alone.
      </p>

      Co-authors:   Andrew Whiteman,  Jian Kang, Andreas J Bartsch"
      photolink: https://scholarblogs.emory.edu/smi2021/files/2021/02/JohnsonTim-e1614022250691-300x300.jpg   
---



  <h2 style="color: #120659;">
    <a href="{{ page.url | prepend: site.relative_url }}">
      {{ page.title }}
    </a>
  </h2>



  {% for speaker in page.speakers %}
  ![Photo]({{speaker.photolink}})
  <p> 
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  {% if speaker.email %}
  Email: {{speaker.email}} <br/> 
  {% endif %}
  <b>Title</b>: {{speaker.title}} <br/>
  <b>Abstract</b>:<br/> {{speaker.abstract}} <br/>
  {% endfor %}

