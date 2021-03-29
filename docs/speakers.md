---
title : Speakers
layout: default
order : 1
---

{% assign sorted_sessions = site.session | sort:"order" %}

<!-- Founder's talk -->

{% for session in sorted_sessions %}
  {% if session.type == "founder" %}
  <h2>
    <a href="{{ session.url | prepend: site.relative_url }}">
      {{ session.title }}
    </a>
  </h2>

  {% for speaker in session.speakers %}

  ![Photo]({{speaker.photolink}})
  
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  <b>Title</b>: <a href="{{ session.url | prepend: site.relative_url }}"> {{ speaker.title }} </a><br/>
  {% endfor %}
  {% endif %}
{% endfor %}

<!-- Keynote talk -->

{% for session in sorted_sessions %}
  {% if session.type == "keynote" %}
  <h2>
    <a href="{{ session.url | prepend: site.relative_url }}">
      {{ session.title }}
    </a>
  </h2>

  {% for speaker in session.speakers %}
  
  ![Photo]({{speaker.photolink}})
  
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  <b>Title</b>: <a href="{{ session.url | prepend: site.relative_url }}">{{speaker.title}}</a> <br/>
  {% endfor %}
  {% endif %}
{% endfor %}


<!-- Short course -->

<!-- Software -->

## Statistical Software for Imaging Analysis

Efstathios D. Gennatas, Stanford University
“Efficient and accessible Machine Learning with rtemis”

Joshua Lukemire, Emory University
“HINT – A Matlab toolbox for hierarchical covariate-adjusted independent component analysis of fMRI data”

John Muschelli, Johns Hopkins Bloomberg School of Public Health
“Neuroconductor: An R Platform for Medical Imaging Analysis”

Hernando Ombao, King Abdullah University of Science and Technology
“Modeling and Visualization of Connectivity in EEG”

Marina Vannucci, Rice University
“User-friendly MATLAB GUIs for Bayesian Multi-Subject Modeling of fMRI Data”

<!-- Invited -->

## Speakers in Invited Oral Sessions

{% for session in sorted_sessions %}
  {% if session.type == "invited" %}
  {% for speaker in session.speakers %}   
  <b>{{speaker.name}}</b>, {{speaker.affil}} <br/> 
  <a href="{{ session.url | prepend: site.relative_url }}"> {{speaker.title}} </a><br/>
  {% endfor %}
  {% endif %}
{% endfor %}