---
title : Poster and Opening Mixer
layout: default
order : 4
---

<h1 style="color: #120659;"> {{page.title}} </h1>


<h3> Poster Presenters: </h3>

  {% for speaker in site.data.posters %}
  <p> 
  <b>{{speaker.id}}. {{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  {% if speaker.email %}
  Email: {{speaker.email}} <br/> 
  {% endif %}
  <p> <b>Title</b>: {{speaker.title}} <br/>
  <b> Abstract</b>: {{speaker.abstract}} </p>
  {% endfor %}

