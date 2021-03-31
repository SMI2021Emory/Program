---
layout: default
ID: K-2
type: keynote
order: 1
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
      name: Vince Calhoun
      affil: Director, Tri-institutional Center for Translational Research in Neuroimaging and Data Science
      email: 
      title: 
      abstract:  
      photolink: https://scholarblogs.emory.edu/smi2021/files/2019/11/VinceCalhoun.jpg
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

