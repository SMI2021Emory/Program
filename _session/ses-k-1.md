---
layout: default
ID: K-1
type: keynote
order: 7
title: Keynote Speakers
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
      name: Tom Nichols
      affil: Professor of Neuroimaging Statistics, Nuffield Department of Population Health, University of Oxford
      email: 
      title: Statistical Challenges and Opportunities in Population Neuroimaging
      abstract:  
      photolink: https://scholarblogs.emory.edu/smi2021/files/2019/10/tomnichols-300x300.png 
---



  <h2>
    <a href="{{ page.url | prepend: site.relative_url }}">
      {{ page.title }}
    </a>
  </h2>



  {% for speaker in page.speakers %}
  
  ![Photo]({{speaker.photolink}})
  
  <b>{{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  {% if speaker.email %}
  Email: {{speaker.email}} <br/> 
  {% endif %}
  <b>Title</b>: {{speaker.title}} <br/>
  <b>Abstract</b>: {{speaker.abstract}} <br/>
  {% endfor %}

