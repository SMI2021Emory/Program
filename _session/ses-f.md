---
layout: default
ID: 
type: founder
order: 2
title: Founders talk
organizer:
    name: 
    affil: 
    email: 
chair:
    name: Tingting Zhang
    affil: University of Pittsburgh
    email: tiz67@pitt.edu
speakers:
    - id: 1
      name: Timothy Johnson
      affil: University of Michigan
      email: 
      title: A Bayesian semi-parametric model for functional near-infrared spectroscopy data
      abstract: 'Functional near-infrared spectroscopy (fNIRS) is a relatively new neuroimaging technique. It is a low cost, portable, and non-invasive method to monitor brain activity. Similar to fMRI, it measures changes in the level of blood oxygen in the brain. Its time resolution is much finer than fMRI, however its spatial resolution is much courser—similar to EEG or MEG. fNIRS is finding widespread use on young children whom cannot remain still in the MRI magnet and it can be used in situations where fMRI is contraindicated—such as with patients whom have cochlear implants. In this talk, I propose a fully Bayesian semi-parametric model to analyze fNIRS data. The hemodynamic response function is modeled with the canonical HRF. The model error and the auto-regressive process vary with time and are modeled in the dynamic linear model framework. The low frequency drift is modeled non-parameterically with a variable B-spline model (both locations and number of knots are allowed to vary). Although motion is not as big an issue as in fMRI, it can still cause huge inferential bias and poor statistical properties if not handled appropriately. The variable B-spline model not only models the low frequency drift, but will regress out motion artifacts as well. Most methods require motion to be removed prior to any statistical analysis except one, which I refer to as the AR-IRLS model. Via simulation studies, I show that this Bayesian model easily handles motion artifacts and results in better statistical properties than the AR-IRLS model. I then show its performance on real data.'

      photolink: https://scholarblogs.emory.edu/smi2021/files/2021/02/JohnsonTim-e1614022250691-300x300.jpg   
---



  <h2 style="color: #120659;">
    <a href="{{ page.url | prepend: site.relative_url }}">
      {{ page.title }}
    </a>
  </h2>
  
  <p>
  <b>Chair</b>: Tingting Zhang<br/> 
  University of Pittsburgh <br/> 
  Email: tiz67@pitt.edu<br/> 
  </p>

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

