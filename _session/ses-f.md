---
layout: default
ID: 
type: founder
order: 1
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
      affil: Johns Hopkins University, Department of Biostatistics
      email: 
      title: Bayesian Nonparametric Analysis of Dual-Resolution fMRI for Presurgical Planning
      abstract:  
      photolink: https://scholarblogs.emory.edu/smi2021/files/2021/02/JohnsonTim-e1614022250691-300x300.jpg   
---



  <h2>
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
  {% endfor %}

