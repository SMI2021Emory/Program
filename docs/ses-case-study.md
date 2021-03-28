---
title : Case-study Sessions
layout: default
order : 3
---

{% assign sorted_sessions = site.session | sort:"order" %}
{% for session in sorted_sessions %}
  {% if session.type == "case_study" %}
  <h2>
    <a href="{{ session.url | prepend: site.relative_url }}">
      Session {{ session.ID }}: {{ session.title }}
    </a>
  </h2>

  <p>
  <b>Organizer</b>: {{session.organizer.name}} <br/> 
   {{session.organizer.affil}} <br/> 
   Email: {{session.organizer.email}} <br/> 
  </p>
  
  <p>
  <b>Chair</b>: {{session.chair.name}}<br/> 
  {{session.chair.affil}} <br/> 
  Email: {{session.chair.email}}<br/> 
  </p>

<h3> Speakers: </h3>

  {% for speaker in session.speakers %}
  <p> 
  <b>{{speaker.id}}. {{speaker.name}}</b><br/>
    {{speaker.affil}} <br/> 
  Email: {{speaker.email}} <br/> 
  <p> <b>Title</b>: {{speaker.title}} <br/>
  <b> Abstract</b>: {{speaker.abstract}} </p>
  {% endfor %}


  <!-- <p>{{ session.content | markdownify }}</p> -->
  {% endif %}
{% endfor %}